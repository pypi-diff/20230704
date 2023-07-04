# Comparing `tmp/pptx2md-1.4.0.tar.gz` & `tmp/pptx2md-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx2md-1.4.0.tar", max compression
+gzip compressed data, was "pptx2md-1.4.1.tar", max compression
```

## Comparing `pptx2md-1.4.0.tar` & `pptx2md-1.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3287 2023-03-16 15:51:00.353572 pptx2md-1.4.0/pptx2md/__init__.py
--rw-r--r--   0        0        0     4569 2023-07-01 23:59:27.523065 pptx2md-1.4.0/pptx2md/__main__.py
--rw-r--r--   0        0        0      809 2023-07-01 23:59:27.524066 pptx2md-1.4.0/pptx2md/global_var.py
--rw-r--r--   0        0        0     5609 2022-02-28 16:22:17.723400 pptx2md-1.4.0/pptx2md/outputter.py
--rw-r--r--   0        0        0     6721 2023-07-01 23:59:27.525152 pptx2md-1.4.0/pptx2md/parser.py
--rw-r--r--   0        0        0      846 2022-02-28 16:22:21.552969 pptx2md-1.4.0/pptx2md/tools.py
--rw-r--r--   0        0        0      602 2023-07-01 23:59:33.218348 pptx2md-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      797 2023-07-02 00:01:49.617844 pptx2md-1.4.0/setup.py
--rw-r--r--   0        0        0      724 2023-07-02 00:01:49.617844 pptx2md-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3408 2023-07-04 15:55:59.765409 pptx2md-1.4.1/pptx2md/__init__.py
+-rw-r--r--   0        0        0     4569 2023-07-01 23:59:27.523065 pptx2md-1.4.1/pptx2md/__main__.py
+-rw-r--r--   0        0        0      809 2023-07-01 23:59:27.524066 pptx2md-1.4.1/pptx2md/global_var.py
+-rw-r--r--   0        0        0     5609 2022-02-28 16:22:17.723400 pptx2md-1.4.1/pptx2md/outputter.py
+-rw-r--r--   0        0        0     6721 2023-07-01 23:59:27.525152 pptx2md-1.4.1/pptx2md/parser.py
+-rw-r--r--   0        0        0      846 2022-02-28 16:22:21.552969 pptx2md-1.4.1/pptx2md/tools.py
+-rw-r--r--   0        0        0      602 2023-07-04 15:56:19.973951 pptx2md-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      797 2023-07-04 15:56:24.880804 pptx2md-1.4.1/setup.py
+-rw-r--r--   0        0        0      724 2023-07-04 15:56:24.880804 pptx2md-1.4.1/PKG-INFO
```

### Comparing `pptx2md-1.4.0/pptx2md/__init__.py` & `pptx2md-1.4.1/pptx2md/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     disable_image: bool = False,  #  disable image extraction
     disable_wmf: bool = False,  # keep wmf formatted image untouched(avoid exceptions under linux)
     disable_color: bool = False,  # do not add color HTML tags
     disable_escaping: bool = False,  # do not attempt to escape special characters
     wiki: bool = False,  # generate output as wikitext(TiddlyWiki)
     mdk: bool = False,  # generate output as madoko markdown
     min_block_size: int = 15,  # the minimum character number of a text block to be converted
+    page: Union[int, None] = None # only convert the specified page 
 ):
 
     file_path = pptx_path
     g.file_prefix = "".join(os.path.basename(file_path).split(".")[:-1])
 
     if title == str:
         g.use_custom_title
@@ -90,14 +91,17 @@
         g.disable_color = False
 
     if disable_escaping:
         g.disable_escaping = True
     else:
         g.disable_escaping = False
 
+    if page is not None:
+        g.page = page
+
     if not os.path.exists(file_path):
         print(f"source file {file_path} not exist!")
         print(f"absolute path: {os.path.abspath(file_path)}")
         exit(0)
     prs = Presentation(file_path)
     if wiki:
         out = outputter.wiki_outputter(out_path)
```

### Comparing `pptx2md-1.4.0/pptx2md/__main__.py` & `pptx2md-1.4.1/pptx2md/__main__.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.4.0/pptx2md/global_var.py` & `pptx2md-1.4.1/pptx2md/global_var.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.4.0/pptx2md/outputter.py` & `pptx2md-1.4.1/pptx2md/outputter.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.4.0/pptx2md/parser.py` & `pptx2md-1.4.1/pptx2md/parser.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.4.0/pptx2md/tools.py` & `pptx2md-1.4.1/pptx2md/tools.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.4.0/pyproject.toml` & `pptx2md-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pptx2md"
-version = "1.4.0"
+version = "1.4.1"
 description = "This package converts pptx to markdown"
 repository = "https://github.com/ssine/pptx2md"
 authors = ["Liu Siyao <liu.siyao@qq.com>"]
 license = "MIT Licence"
 
 [tool.poetry.scripts]
 pptx2md = "pptx2md.__main__:main"
```

### Comparing `pptx2md-1.4.0/setup.py` & `pptx2md-1.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=6.0.0', 'python-pptx>=0.6.18', 'rapidfuzz>=0.10.0', 'tqdm>=4']
 
 entry_points = \
 {'console_scripts': ['pptx2md = pptx2md.__main__:main']}
 
 setup_kwargs = {
     'name': 'pptx2md',
-    'version': '1.4.0',
+    'version': '1.4.1',
     'description': 'This package converts pptx to markdown',
     'long_description': None,
     'author': 'Liu Siyao',
     'author_email': 'liu.siyao@qq.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ssine/pptx2md',
```

### Comparing `pptx2md-1.4.0/PKG-INFO` & `pptx2md-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx2md
-Version: 1.4.0
+Version: 1.4.1
 Summary: This package converts pptx to markdown
 Home-page: https://github.com/ssine/pptx2md
 License: MIT Licence
 Author: Liu Siyao
 Author-email: liu.siyao@qq.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
```

