# Comparing `tmp/jsonjavascriptnotation-0.1.5-py3-none-any.whl.zip` & `tmp/jsonjavascriptnotation-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3428 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 22:08 jsonjavascriptnotation/__init__.py
--rw-r--r--  2.0 unx     2000 b- defN 23-Jul-02 22:18 jsonjavascriptnotation/json_wrapper.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-02 23:25 jsonjavascriptnotation-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1232 b- defN 23-Jul-02 23:25 jsonjavascriptnotation-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 23:25 jsonjavascriptnotation-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jul-02 23:25 jsonjavascriptnotation-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      644 b- defN 23-Jul-02 23:25 jsonjavascriptnotation-0.1.5.dist-info/RECORD
-7 files, 5056 bytes uncompressed, 2262 bytes compressed:  55.3%
+Zip file size: 3996 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 21:11 jsonjavascriptnotation/__init__.py
+-rw-r--r--  2.0 unx     2767 b- defN 23-Jul-03 22:47 jsonjavascriptnotation/json_wrapper.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-03 23:33 jsonjavascriptnotation-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2301 b- defN 23-Jul-03 23:33 jsonjavascriptnotation-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 23:33 jsonjavascriptnotation-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-03 23:33 jsonjavascriptnotation-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      644 b- defN 23-Jul-03 23:33 jsonjavascriptnotation-0.1.6.dist-info/RECORD
+7 files, 6892 bytes uncompressed, 2830 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jsonjavascriptnotation/__init__.py
 Comment: 
 
 Filename: jsonjavascriptnotation/json_wrapper.py
 Comment: 
 
-Filename: jsonjavascriptnotation-0.1.5.dist-info/LICENSE
+Filename: jsonjavascriptnotation-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: jsonjavascriptnotation-0.1.5.dist-info/METADATA
+Filename: jsonjavascriptnotation-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: jsonjavascriptnotation-0.1.5.dist-info/WHEEL
+Filename: jsonjavascriptnotation-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: jsonjavascriptnotation-0.1.5.dist-info/top_level.txt
+Filename: jsonjavascriptnotation-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonjavascriptnotation-0.1.5.dist-info/RECORD
+Filename: jsonjavascriptnotation-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonjavascriptnotation/json_wrapper.py

```diff
@@ -1,37 +1,60 @@
 class JsonWrapperException(Exception):
     pass
 
 
 class Wrapper:
 
     def __init__(self, collection=None):
+        self.__wrapper_normalized_names = {}
         if collection:
             self._static_load(self, collection)
 
     def __repr__(self):
         res = "{"
         for e in self.__dict__.items():
+            name = e[0]
+            if name == "_Wrapper__wrapper_normalized_names":
+                continue
             if len(res) > 1:
                 res += ', '
-            val = f'"{e[1]}"' if isinstance(e[1], str) else e[1]
-            res += f'"{e[0]}": {val}'
+            if isinstance(e[1], str):
+                val = f'"{e[1]}"'
+            elif isinstance(e[1], bool):
+                val = 'true' if e[1] else 'false'
+            else:
+                val = e[1]
+            if name in self.__wrapper_normalized_names.keys():
+                name = self.__wrapper_normalized_names[name]
+            res += f'"{name}": {val}'
         res += "}"
         return res
 
     @staticmethod
+    def _normalize(instance, name):
+        res = name
+        normalized = False
+        if res.find('$') > -1:
+            res = res.replace('$', '')
+            normalized = True
+        if res.find('-') > -1:
+            res = res.replace('-', '_')
+            normalized = True
+        if res.find('#') > -1:
+            res = res.replace('#', '')
+            normalized = True
+        if normalized:
+            instance.__wrapper_normalized_names.update({res: name})
+        return res
+
+    @staticmethod
     def _set_attribute(instance, name, value):
-        if name.find('$') > -1:
-            name = name.replace('$', '')
-        if name.find('-') > -1:
-            name = name.replace('-', '_')
-        if name.find('#') > -1:
-            name = name.replace('#', '')
-        if not hasattr(instance, name):
-            setattr(instance, name, value)
+        nname = Wrapper._normalize(instance, name)
+        if not hasattr(instance, nname):
+            setattr(instance, nname, value)
 
     @staticmethod
     def _static_load(instance, collection):
         if isinstance(collection, dict):
             for el in collection.items():
                 n, v = el[0], el[1]
                 if isinstance(v, dict):
```

## Comparing `jsonjavascriptnotation-0.1.5.dist-info/LICENSE` & `jsonjavascriptnotation-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

