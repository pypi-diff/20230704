# Comparing `tmp/unearth-0.9.1.tar.gz` & `tmp/unearth-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unearth-0.9.1.tar", last modified: Mon May 15 07:34:57 2023, max compression
+gzip compressed data, was "unearth-0.9.2.tar", last modified: Tue Jul  4 02:02:53 2023, max compression
```

## Comparing `unearth-0.9.1.tar` & `unearth-0.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1059 2023-05-15 07:34:42.539511 unearth-0.9.1/LICENSE
--rw-r--r--   0        0        0     2885 2023-05-15 07:34:42.539511 unearth-0.9.1/README.md
--rw-r--r--   0        0        0     1919 2023-05-15 07:34:42.539511 unearth-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      616 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/__init__.py
--rw-r--r--   0        0        0     5993 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/__main__.py
--rw-r--r--   0        0        0    13606 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/auth.py
--rw-r--r--   0        0        0     7912 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/collector.py
--rw-r--r--   0        0        0      970 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/errors.py
--rw-r--r--   0        0        0    10775 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/evaluator.py
--rw-r--r--   0        0        0    15178 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/finder.py
--rw-r--r--   0        0        0     5538 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/link.py
--rw-r--r--   0        0        0     5406 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/pep425tags.py
--rw-r--r--   0        0        0    11520 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/preparer.py
--rw-r--r--   0        0        0        0 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/py.typed
--rw-r--r--   0        0        0     6687 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/session.py
--rw-r--r--   0        0        0     6405 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/utils.py
--rw-r--r--   0        0        0      258 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/__init__.py
--rw-r--r--   0        0        0     8415 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/base.py
--rw-r--r--   0        0        0     2589 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/bazaar.py
--rw-r--r--   0        0        0     4813 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/git.py
--rw-r--r--   0        0        0     2006 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/hg.py
--rw-r--r--   0        0        0     6238 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/svn.py
--rw-r--r--   0        0        0      132 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2581 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2173 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/app.py
--rw-r--r--   0        0        0    96588 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/files/click-8.1.3-py3-none-any.whl
--rw-r--r--   0        0        0   133101 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
--rw-r--r--   0        0        0      816 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/findlinks/index.html
--rw-r--r--   0        0        0     1860 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/black.html
--rw-r--r--   0        0        0      876 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/click.html
--rw-r--r--   0        0        0      461 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/first.html
--rw-r--r--   0        0        0      964 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/pipenv.html
--rw-r--r--   0        0        0     2345 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/black.json
--rw-r--r--   0        0        0     1081 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/click.json
--rw-r--r--   0        0        0      521 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/first.json
--rw-r--r--   0        0        0     1178 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/pipenv.json
--rw-r--r--   0        0        0     2628 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_collector.py
--rw-r--r--   0        0        0     8267 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_evaluator.py
--rw-r--r--   0        0        0     6341 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_finder.py
--rw-r--r--   0        0        0     4044 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_link.py
--rw-r--r--   0        0        0     3380 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_session.py
--rw-r--r--   0        0        0      558 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_utils.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 unearth-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-04 02:02:38.374191 unearth-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2885 2023-07-04 02:02:38.374191 unearth-0.9.2/README.md
+-rw-r--r--   0        0        0     1919 2023-07-04 02:02:38.374191 unearth-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-07-04 02:02:38.374191 unearth-0.9.2/src/unearth/__init__.py
+-rw-r--r--   0        0        0     5993 2023-07-04 02:02:38.374191 unearth-0.9.2/src/unearth/__main__.py
+-rw-r--r--   0        0        0    13606 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/auth.py
+-rw-r--r--   0        0        0     7965 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/collector.py
+-rw-r--r--   0        0        0      970 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/errors.py
+-rw-r--r--   0        0        0    10775 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/evaluator.py
+-rw-r--r--   0        0        0    15178 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/finder.py
+-rw-r--r--   0        0        0     5526 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/link.py
+-rw-r--r--   0        0        0     5406 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/pep425tags.py
+-rw-r--r--   0        0        0    11520 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/preparer.py
+-rw-r--r--   0        0        0        0 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/py.typed
+-rw-r--r--   0        0        0     6687 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/session.py
+-rw-r--r--   0        0        0     6405 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/utils.py
+-rw-r--r--   0        0        0      258 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/__init__.py
+-rw-r--r--   0        0        0     8415 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/base.py
+-rw-r--r--   0        0        0     2589 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/bazaar.py
+-rw-r--r--   0        0        0     4813 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/git.py
+-rw-r--r--   0        0        0     2006 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/hg.py
+-rw-r--r--   0        0        0     6238 2023-07-04 02:02:38.378192 unearth-0.9.2/src/unearth/vcs/svn.py
+-rw-r--r--   0        0        0      132 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2581 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2173 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/app.py
+-rw-r--r--   0        0        0    96588 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/files/click-8.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0   133101 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0      816 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/findlinks/index.html
+-rw-r--r--   0        0        0     1860 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/black.html
+-rw-r--r--   0        0        0      876 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/click.html
+-rw-r--r--   0        0        0      461 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/first.html
+-rw-r--r--   0        0        0      964 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/index/pipenv.html
+-rw-r--r--   0        0        0     2345 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/black.json
+-rw-r--r--   0        0        0     1081 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/click.json
+-rw-r--r--   0        0        0      521 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/first.json
+-rw-r--r--   0        0        0     1178 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/fixtures/json/pipenv.json
+-rw-r--r--   0        0        0     2628 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_collector.py
+-rw-r--r--   0        0        0     8267 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_evaluator.py
+-rw-r--r--   0        0        0     6341 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_finder.py
+-rw-r--r--   0        0        0     4044 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_link.py
+-rw-r--r--   0        0        0     3380 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_session.py
+-rw-r--r--   0        0        0      558 2023-07-04 02:02:38.378192 unearth-0.9.2/tests/test_utils.py
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 unearth-0.9.2/PKG-INFO
```

### Comparing `unearth-0.9.1/LICENSE` & `unearth-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/README.md` & `unearth-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/pyproject.toml` & `unearth-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.9.1"
+version = "0.9.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/unearth"
 Documentation = "https://unearth.readthedocs.io"
```

### Comparing `unearth-0.9.1/src/unearth/__init__.py` & `unearth-0.9.2/src/unearth/__init__.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/__main__.py` & `unearth-0.9.2/src/unearth/__main__.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/auth.py` & `unearth-0.9.2/src/unearth/auth.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/collector.py` & `unearth-0.9.2/src/unearth/collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,20 @@
     for anchor in parser.anchors:
         href = anchor.get("href")
         if href is None:
             continue
         url = parse.urljoin(base_url, href)
         requires_python = anchor.get("data-requires-python")
         yank_reason = anchor.get("data-yanked")
-        data_dist_info_metadata = anchor.get("data-dist-info-metadata")
+        metadata_hash = anchor.get(
+            "data-core-metadata", anchor.get("data-dist-info-metadata")
+        )
         dist_info_metadata: bool | dict[str, str] | None = None
-        if data_dist_info_metadata:
-            hash_name, has_hash, hash_value = data_dist_info_metadata.partition("=")
+        if metadata_hash:
+            hash_name, has_hash, hash_value = metadata_hash.partition("=")
             if has_hash:
                 dist_info_metadata = {hash_name: hash_value}
             else:
                 dist_info_metadata = True
         yield Link(
             url,
             base_url,
@@ -86,15 +88,15 @@
         url = file.get("url")
         if not url:
             continue
         url = parse.urljoin(base_url, url)
         requires_python: str | None = file.get("requires-python")
         yank_reason: str | None = file.get("yanked") or None
         dist_info_metadata: bool | dict[str, str] | None = file.get(
-            "data-dist-info-metadata"
+            "core-metadata", file.get("data-dist-info-metadata")
         )
         hashes: dict[str, str] | None = file.get("hashes")
         yield Link(
             url,
             base_url,
             yank_reason=yank_reason,
             requires_python=requires_python,
```

### Comparing `unearth-0.9.1/src/unearth/errors.py` & `unearth-0.9.2/src/unearth/errors.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/evaluator.py` & `unearth-0.9.2/src/unearth/evaluator.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/finder.py` & `unearth-0.9.2/src/unearth/finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/link.py` & `unearth-0.9.2/src/unearth/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     def filename(self) -> str:
         return os.path.basename(unquote(self.parsed.path))
 
     @property
     def dist_info_link(self) -> Link | None:
         return (
             type(self)(f"{self.url_without_fragment}.metadata", self.comes_from)
-            if self.dist_info_metadata is not None
+            if self.dist_info_metadata
             else None
         )
 
     @property
     def is_wheel(self) -> bool:
         return self.filename.endswith(".whl")
```

### Comparing `unearth-0.9.1/src/unearth/pep425tags.py` & `unearth-0.9.2/src/unearth/pep425tags.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/preparer.py` & `unearth-0.9.2/src/unearth/preparer.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/session.py` & `unearth-0.9.2/src/unearth/session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/utils.py` & `unearth-0.9.2/src/unearth/utils.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/vcs/base.py` & `unearth-0.9.2/src/unearth/vcs/base.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/vcs/bazaar.py` & `unearth-0.9.2/src/unearth/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/vcs/git.py` & `unearth-0.9.2/src/unearth/vcs/git.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/vcs/hg.py` & `unearth-0.9.2/src/unearth/vcs/hg.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/src/unearth/vcs/svn.py` & `unearth-0.9.2/src/unearth/vcs/svn.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/conftest.py` & `unearth-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/app.py` & `unearth-0.9.2/tests/fixtures/app.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/files/click-8.1.3-py3-none-any.whl` & `unearth-0.9.2/tests/fixtures/files/click-8.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl` & `unearth-0.9.2/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/findlinks/index.html` & `unearth-0.9.2/tests/fixtures/findlinks/index.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/index/black.html` & `unearth-0.9.2/tests/fixtures/index/black.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/index/click.html` & `unearth-0.9.2/tests/fixtures/index/click.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/index/pipenv.html` & `unearth-0.9.2/tests/fixtures/index/pipenv.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/json/black.json` & `unearth-0.9.2/tests/fixtures/json/black.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/json/click.json` & `unearth-0.9.2/tests/fixtures/json/click.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/json/first.json` & `unearth-0.9.2/tests/fixtures/json/first.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/fixtures/json/pipenv.json` & `unearth-0.9.2/tests/fixtures/json/pipenv.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_collector.py` & `unearth-0.9.2/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_evaluator.py` & `unearth-0.9.2/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_finder.py` & `unearth-0.9.2/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_link.py` & `unearth-0.9.2/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_session.py` & `unearth-0.9.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/tests/test_utils.py` & `unearth-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.1/PKG-INFO` & `unearth-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unearth
-Version: 0.9.1
+Version: 0.9.2
 Summary: A utility to fetch and download python packages
 License: MIT
 Author-email: Frost Ming <me@frostming.com>
 Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

