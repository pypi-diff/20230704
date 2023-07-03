# Comparing `tmp/NotionLab-1.1.3.tar.gz` & `tmp/NotionLab-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionLab-1.1.3.tar", last modified: Sat May 20 08:50:44 2023, max compression
+gzip compressed data, was "NotionLab-1.1.4.tar", last modified: Mon Jul  3 23:33:14 2023, max compression
```

## Comparing `NotionLab-1.1.3.tar` & `NotionLab-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-20 08:50:32.000000 NotionLab-1.1.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/NotionLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 08:50:44.063879 NotionLab-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 08:50:32.000000 NotionLab-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/notion_lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/notion_lab/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/HtmlCvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/MDCvt.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/html/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/html/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Code.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/List.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/TableRow.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Text.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/md/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/md/md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/database/DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:50:44.063879 NotionLab-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-20 08:50:32.000000 NotionLab-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.641253 NotionLab-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-03 23:33:02.000000 NotionLab-1.1.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.633252 NotionLab-1.1.4/NotionLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 23:33:14.000000 NotionLab-1.1.4/NotionLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-03 23:33:14.000000 NotionLab-1.1.4/NotionLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:33:14.000000 NotionLab-1.1.4/NotionLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 23:33:14.000000 NotionLab-1.1.4/NotionLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 23:33:14.000000 NotionLab-1.1.4/NotionLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 23:33:14.641253 NotionLab-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-03 23:33:02.000000 NotionLab-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.633252 NotionLab-1.1.4/notion_lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.633252 NotionLab-1.1.4/notion_lab/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/HtmlCvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/MDCvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.633252 NotionLab-1.1.4/notion_lab/converter/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.637253 NotionLab-1.1.4/notion_lab/converter/util/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.637253 NotionLab-1.1.4/notion_lab/converter/util/html/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/Code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/List.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/TableRow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/Toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/html/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.641253 NotionLab-1.1.4/notion_lab/converter/util/md/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/converter/util/md/md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:33:14.641253 NotionLab-1.1.4/notion_lab/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/database/DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 23:33:02.000000 NotionLab-1.1.4/notion_lab/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:33:14.641253 NotionLab-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 23:33:02.000000 NotionLab-1.1.4/setup.py
```

### Comparing `NotionLab-1.1.3/LICENSE` & `NotionLab-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/NotionLab.egg-info/PKG-INFO` & `NotionLab-1.1.4/NotionLab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionLab
-Version: 1.1.3
+Version: 1.1.4
 Summary: A kit for Notion based on Notion Python SDK.
 Home-page: https://github.com/ElaBosak233/NotionLab
 Author: ElaBosak233
 Author-email: ElaBosak233@gmail.com
 License: MIT Licence
 Keywords: notion,kit,parser,html,markdown,lab
 Platform: any
```

### Comparing `NotionLab-1.1.3/NotionLab.egg-info/SOURCES.txt` & `NotionLab-1.1.4/NotionLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/PKG-INFO` & `NotionLab-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionLab
-Version: 1.1.3
+Version: 1.1.4
 Summary: A kit for Notion based on Notion Python SDK.
 Home-page: https://github.com/ElaBosak233/NotionLab
 Author: ElaBosak233
 Author-email: ElaBosak233@gmail.com
 License: MIT Licence
 Keywords: notion,kit,parser,html,markdown,lab
 Platform: any
```

### Comparing `NotionLab-1.1.3/README.md` & `NotionLab-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/notion_lab/converter/Converter.py` & `NotionLab-1.1.4/notion_lab/converter/Converter.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/notion_lab/converter/HtmlCvt.py` & `NotionLab-1.1.4/notion_lab/converter/HtmlCvt.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,29 @@
     _table_row_parsed: bool = False
 
     def __init__(
             self,
             api_token: str,
             block_id: str,
             is_page: bool = False,
+            is_table: bool = False,
             has_column_header: bool = False
     ) -> None:
+        if not is_table:
+            # 前缀, 强制使用 UTF-8
+            self._html += textwrap.dedent("""
+            <head>
+                <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
+            </head>
+            """)
         super().__init__(api_token, block_id, is_page, has_column_header)
 
     def convert(
             self
     ) -> str:
-        # 前缀, 强制使用 UTF-8
-        self._html += '<meta http-equiv="Content-Type" content="text/html; charset=utf-8">'
         if self._title:
             self._html += f"<title>{self._title}</title>"
         for block in self._ctx:
             b_type = block["type"]
             b_ctx = block[f"{b_type.lower()}"]
             b_id = block["id"]
             if b_type != "bulleted_list_item" and self._bulleted_list_counter != 0:
```

### Comparing `NotionLab-1.1.3/notion_lab/converter/MDCvt.py` & `NotionLab-1.1.4/notion_lab/converter/MDCvt.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                 self._md += f"{self._numbered_list_counter}. {r}\n"
                 self._numbered_list_counter += 1
             elif b_type == "table":
                 r: str = HtmlCvt(
                     api_token=self._api_token,
                     block_id=b_id,
                     is_page=False,
+                    is_table=True,
                     has_column_header=b_ctx["has_column_header"]
                 ).convert()
                 self._md += f'<table>{r}</table>'
             elif b_type == "table_row":
                 self._md += TableRow(b_ctx).export()
             elif b_type == "toggle":
                 r: str = MDCvt(
```

### Comparing `NotionLab-1.1.3/notion_lab/converter/util/html/elements/TableRow.py` & `NotionLab-1.1.4/notion_lab/converter/util/html/elements/TableRow.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/notion_lab/converter/util/html/html.py` & `NotionLab-1.1.4/notion_lab/converter/util/html/html.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/notion_lab/converter/util/md/md.py` & `NotionLab-1.1.4/notion_lab/converter/util/md/md.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/notion_lab/database/DB.py` & `NotionLab-1.1.4/notion_lab/database/DB.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.3/setup.py` & `NotionLab-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="NotionLab",
-    version="1.1.3",
+    version="1.1.4",
     keywords=["notion", "kit", "parser", "html", "markdown", "lab"],
     description="A kit for Notion based on Notion Python SDK.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT Licence",
 
     url="https://github.com/ElaBosak233/NotionLab",
```

