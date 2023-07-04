# Comparing `tmp/configdict-2.7.0-py3-none-any.whl.zip` & `tmp/configdict-2.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 31720 bytes, number of entries: 9
+Zip file size: 32179 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    63756 b- defN 23-Jun-12 15:33 configdict/configdict.py
+-rw-rw-r--  2.0 unx    65970 b- defN 23-Jul-04 12:25 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-Jun-12 15:35 configdict-2.7.0.dist-info/RECORD
-9 files, 92268 bytes uncompressed, 30434 bytes compressed:  67.0%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/RECORD
+9 files, 94482 bytes uncompressed, 30893 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.7.0.dist-info/LICENSE.md
+Filename: configdict-2.8.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.7.0.dist-info/METADATA
+Filename: configdict-2.8.0.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.7.0.dist-info/WHEEL
+Filename: configdict-2.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.7.0.dist-info/top_level.txt
+Filename: configdict-2.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.7.0.dist-info/RECORD
+Filename: configdict-2.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -252,23 +252,40 @@
 def _asRstLinkKey(key: str) -> str:
     return key.replace(".", "_").replace(" ", "").lower()
 
 def _asYaml(d: dict[str, Any],
             doc: dict[str, str],
             default: dict[str, Any],
             validator: dict[str, Any] = None,
-            sortKeys=False
+            keys: list[str] = None,
+            advancedPrefix = '.'
             ) -> str:
     lines = []
 
-    items = list(d.items())
-    if sortKeys:
-        items.sort(key=lambda pair: pair[0])
+    # detect if keys have advanced keys and they are all at the end
+
+    if keys:
+        items = [(k, d[k]) for k in keys]
+    else:
+        items = list(d.items())
+
+    firstAdvanced = next((i for i, item in enumerate(items) if item[0].startswith(advancedPrefix)), None)
+    if firstAdvanced is not None and all(k.startswith(advancedPrefix) for k, v in items[firstAdvanced:]):
+        addAdvancedSeparator = True
+    else:
+        addAdvancedSeparator = False
 
     for key, value in items:
+        if addAdvancedSeparator and key.startswith(advancedPrefix):
+            addAdvancedSeparator = False
+            lines.append("\n"
+                         "#####################################################\n"
+                         "#                 Advanced Keys                     #\n"
+                         "#####################################################\n")
+
         choices = validator.get(f"{key}::choices")
         valuerange = validator.get(f"{key}::range")
         valuetype = validator.get(f"{key}::type")
         valuetypestr = type(value).__name__ if valuetype is None else _typeName(valuetype)
         comment = _yamlComment(doc=doc.get(key), default=default.get(key),
                                choices=choices, valuerange=valuerange,
                                valuetype=valuetypestr)
@@ -303,14 +320,24 @@
             else:
                 _(f'<td style="text-align:left">{cell}</td>')
         _("</tr>")
     _("</tbody></table>")
     return "".join(parts)
 
 
+def _checkDocs(docs: dict[str, str], keys: set[str]) -> bool:
+    ok = True
+    for key in docs.keys():
+        if key not in keys:
+            likely = _bestMatches(key, keys, limit=16, minpercent=60)
+            logger.warning(f"Key {key} not defined. Did you mean {likely}?. \nPossible keys: {keys}")
+            ok = False
+    return ok
+
+
 def _checkValidator(validatordict: dict, defaultdict: dict) -> dict:
     """
     Checks the validity of the validator itself, and makes any needed
     postprocessing on the validator
 
     Args:
         validatordict: the validator dict
@@ -510,25 +537,30 @@
     def __init__(self,
                  default: dict[str, Any] = None,
                  validator: dict[str, Any] = None,
                  docs: dict[str, str] = None,
                  callback: Callable[[str, Any], None] = None,
                  precallback=None,
                  autoload=True,
-                 strict=True) -> None:
+                 strict=True,
+                 advancedPrefix='.') -> None:
 
         self.default = default if default else {}
         self._validator = _checkValidator(validator, default) if validator else {}
         self._docs = docs if docs else {}
         self._allowedkeys = set(default.keys()) if default else set()
         self._precallback = precallback
         self._callback = callback
         self._building = False
         self._normalizedKeys: dict[str, str] = {}
         self._bypass = False
+        self._advancedPrefix = advancedPrefix
+
+        if docs:
+            _checkDocs(docs, self._allowedkeys)
 
         if self.default:
             if autoload:
                 self.load()
             if not strict:
                 self._normalizedKeys = {normalizeKey(k): k for k in self.default.keys()}
 
@@ -674,26 +706,28 @@
     def __getitem__(self, key: str):
         if (value := dict.get(self, key, _UNKNOWN)) is not _UNKNOWN:
             return value
 
         if self._normalizedKeys and (key2 := self._normalizedKeys.get(normalizeKey(key))):
             return dict.__getitem__(self, key2)
 
-        raise KeyError(f"key '{key}' not known. Possible keys: {sorted(self.keys())}")
+        nearest = self._bestMatches(key, limit=8)
+        raise KeyError(f"key '{key}' not known. Did you mean {nearest}?\n"
+                       f"Possible keys: {sorted(self.keys())}")
 
     def __setitem__(self, key: str, value) -> None:
         if self._bypass:
             dict.__setitem__(key, value)
             return
 
         if key not in self._allowedkeys:
             if self._normalizedKeys and (normkey := self._normalizedKeys.get(normalizeKey(key))):
                 key = normkey
             else:
-                mostlikely = _bestMatches(key, list(self._allowedkeys), 16, minpercent=60)
+                mostlikely = self._bestMatches(key=key, limit=8)
                 msg = f"Unknown key {key}. Did you mean {', '.join(mostlikely)}?"
                 raise KeyError(msg)
 
         oldvalue = self.get(key)
         if oldvalue is not None and oldvalue == value:
             return
         if self._validator:
@@ -706,14 +740,17 @@
                 value = newvalue
 
         super().__setitem__(key, value)
 
         if self._callback is not None:
             self._callback(key, value)
 
+    def _bestMatches(self, key: str, limit=16, minpercent=60):
+        return _bestMatches(key, list(self._allowedkeys), limit=limit, minpercent=minpercent)
+
     def load(self) -> None:
         """
         Update any undefined key in self with the default value
 
         Example
         ~~~~~~~
 
@@ -967,57 +1004,70 @@
         """
         return value if value is not None else self.get(key, default)
 
     def asYaml(self, sortKeys=False) -> str:
         """
         Returns this dict as yaml str, with comments, defaults, etc.
         """
-        return _asYaml(self, doc=self._docs, validator=self._validator,
-                       default=self.default, sortKeys=sortKeys)
+        if sortKeys:
+            keys = self._sortedKeys()
+        else:
+            keys = list(self.keys())
+            keys.sort(key=lambda key: int(key.startswith(self._advancedPrefix)))
+            return _asYaml(self, doc=self._docs, validator=self._validator,
+                       default=self.default, keys=keys)
 
     def __enter__(self):
         self._building = True
         return self
 
     def __exit__(self, *args, **kws):
         self._building = False
         self.load()
 
-    def edit(self, waitOnModified=True) -> None:
+    def edit(self, waitOnModified=True, sortKeys=False) -> None:
         configfile = tempfile.mktemp(suffix=".yaml")
         header = _editHeaderWatch if waitOnModified else _editHeaderPopup
-        self._saveAsYaml(configfile, header=header)
+        self._saveAsYaml(configfile, header=header, sortKeys=sortKeys)
         _openInEditor(configfile)
         if waitOnModified:
             try:
                 _waitOnFileModified(configfile)
             except KeyboardInterrupt:
                 logger.debug("Editing aborted")
                 return
         else:
             _waitForClick(title=self.name)
         self.load(configfile)
 
-    def _saveAsYaml(self, path: str, header: str = '', sortKeys=False) -> None:
+    def _saveAsYaml(self, path: str, header: str = '', sortKeys=False, separateAdvancedKeys=True) -> None:
         yamlstr = self.asYaml(sortKeys=sortKeys)
         folder = os.path.split(path)[0]
         os.makedirs(folder, exist_ok=True)
         with open(path, "w") as f:
             if header:
                 f.write(header)
                 f.write("\n")
             f.write(yamlstr)
         if not os.path.exists(path):
             raise RuntimeError(f"Could not save config to file '{path}', file not found")
-    
+
+    @cache
+    def _sortedKeys(self) -> list[str]:
+        keys = list(self.keys())
+        keys.sort()
+        keys.sort(key=lambda k: int(k.startswith(self._advancedPrefix)))
+        return keys
+
     def _repr_html_(self) -> str:
         parts = [f'<div><h4>{type(self).__name__}</h4>']
         parts.append("<br>")
         rows = []
-        for k in self.keys():
+        keys = self._sortedKeys()
+        for k in keys:
             v = self[k]
             rows.append((k, str(v), self._infoStr(k), self.getDoc(k)))
         table = _htmlTable(rows, headers=('Key', 'Value', 'Type', 'Descr'), maxwidths=[0, 0, 150, 400],
                            rowstyles=('strong', 'code', None, None))
         parts.append(table)
         parts.append("</div>")
         return "".join(parts)
@@ -1180,15 +1230,16 @@
                  docs: dict[str, str] = None,
                  precallback:Callable[[ConfigDict, str, Any, Any], Any]=None,
                  persistent=False,
                  load=True,
                  fmt='yaml',
                  sortKeys=False,
                  description='',
-                 strict=True) -> None:
+                 strict=True,
+                 advancedPrefix='.') -> None:
 
         self._name = ''
         self._base = ''
         self._persistent = persistent
         self._configPath = None
         self._callbacks = []
         self._loaded = False
@@ -1214,15 +1265,16 @@
 
         self.fmt = fmt
         super().__init__(default=default,
                          validator=validator,
                          docs=docs,
                          callback=self._mycallback,
                          precallback=precallback,
-                         autoload=False)
+                         autoload=False,
+                         advancedPrefix=advancedPrefix)
         self.sortKeys = sortKeys
 
         if default is not None:
             self._updateWithDefault()
             if load:
                 self.load()
 
@@ -1508,15 +1560,16 @@
 
     def _repr_html_(self) -> str:
         parts = [f'<div><h4>{type(self).__name__}: <strong>{self.name}</strong></h4>']
         if self.persistent:
             parts.append(f'persistent (<code>"{self.getPath()}"</code>)')
         parts.append("<br>")
         rows = []
-        for k in self.keys():
+        keys = self._sortedKeys()
+        for k in keys:
             v = self[k]
             descr = self.getDoc(k)
             if v == self.default[k]:
                 strv = str(v)
             else:
                 strv = f'<i><b>{v}</b></i>'
             rows.append((k, strv, self._infoStr(k), descr))
@@ -1570,15 +1623,15 @@
         """
         if not self._name:
             return ''
         if not self._configPath:
             self._configPath = configPathFromName(self._name, self.fmt)
         return self._configPath
 
-    def edit(self, waitOnModified=True) -> None:
+    def edit(self, waitOnModified=True, sortKeys=False) -> None:
         """
         Edit this config by opening it in an external application.
 
         The format used is *yaml*. This is independent of the format used for
         persistence. The application used is the user's default application
         for the .yaml format and can be configured at the os level. In macos
         we use ``open``, in linux ``xdg-open`` and in windows ``start``, which
@@ -1593,18 +1646,19 @@
             waitOnModified: if True, the transaction is accepted whenever the
                 file being edited is saved. Otherwise a message box is created
                 which needs to be clicked in order to confirm the transaction.
                 Just exiting the application will not cancel the edit job since
                 many applications which have a server mode or unique instance
                 mode might in fact exit right away from the perspective of the
                 subprocess which launched them
+            sortKeys: if True, keys appear in sorted order
         """
         header = _editHeaderWatch if waitOnModified else _editHeaderPopup
         configfile = tempfile.mktemp(suffix=".yaml")
-        self._saveAsYaml(configfile, header=header)
+        self._saveAsYaml(configfile, header=header, sortKeys=sortKeys)
         assert os.path.exists(configfile)
         _openInEditor(configfile)
         if waitOnModified:
             try:
                 _notify(f"Config Edit: {self.name}", "Modify the values as needed. Save the file to accept the changes "
                         f"or press ctrl-c at the python prompt to cancel (path: {configfile})")
                 _waitOnFileModified(configfile)
```

## Comparing `configdict-2.7.0.dist-info/LICENSE.md` & `configdict-2.8.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.7.0.dist-info/METADATA` & `configdict-2.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.7.0
+Version: 2.8.0
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

## Comparing `configdict-2.7.0.dist-info/RECORD` & `configdict-2.8.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 configdict/__init__.py,sha256=CI6gyI6isoSmOxiaMKQ1zJMLWzFYn6bOTnUcJtMAMRQ,25
-configdict/configdict.py,sha256=mZAF2AOJuxiKZG1DPSOizqlCCpe3Er2g8UJRIR0f3lA,63756
+configdict/configdict.py,sha256=xUyyTXx-pvaXOHy8kJbifKJ6DdboIjr3MxBgwV39urs,65970
 configdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 configdict/__pycache__/configdict.cpython-38.pyc,sha256=pmenTOMg3mEukCVKrOf7lNx1TTPjNga5bTXY_VRnSFU,22699
-configdict-2.7.0.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
-configdict-2.7.0.dist-info/METADATA,sha256=ArtjTXavlHB_r6gaApjmaXY7iJguBXDjkQ7jBthHmlg,3883
-configdict-2.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-configdict-2.7.0.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
-configdict-2.7.0.dist-info/RECORD,,
+configdict-2.8.0.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
+configdict-2.8.0.dist-info/METADATA,sha256=VCu8EkqwUl24Uz7Yb_E9jrwGW5N3E_ROlze24gC75l8,3883
+configdict-2.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+configdict-2.8.0.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
+configdict-2.8.0.dist-info/RECORD,,
```

