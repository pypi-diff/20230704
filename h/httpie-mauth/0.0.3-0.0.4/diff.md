# Comparing `tmp/httpie_mauth-0.0.3.tar.gz` & `tmp/httpie_mauth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie_mauth-0.0.3.tar", max compression
+gzip compressed data, was "httpie_mauth-0.0.4.tar", max compression
```

## Comparing `httpie_mauth-0.0.3.tar` & `httpie_mauth-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1062 2023-06-28 22:11:14.519859 httpie_mauth-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      858 2023-06-28 22:11:14.519859 httpie_mauth-0.0.3/README.md
--rw-r--r--   0        0        0      974 2023-06-28 22:11:14.519859 httpie_mauth-0.0.3/httpie_mauth.py
--rw-r--r--   0        0        0      884 2023-06-30 19:02:42.360258 httpie_mauth-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 httpie_mauth-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      858 2023-06-28 22:11:14.519859 httpie_mauth-0.0.4/README.md
+-rw-r--r--   0        0        0      974 2023-06-28 22:11:14.519859 httpie_mauth-0.0.4/httpie_mauth.py
+-rw-r--r--   0        0        0      879 2023-07-04 03:13:32.337808 httpie_mauth-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 httpie_mauth-0.0.4/PKG-INFO
```

### Comparing `httpie_mauth-0.0.3/README.md` & `httpie_mauth-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `httpie_mauth-0.0.3/httpie_mauth.py` & `httpie_mauth-0.0.4/httpie_mauth.py`

 * *Files identical despite different names*

### Comparing `httpie_mauth-0.0.3/pyproject.toml` & `httpie_mauth-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "httpie-mauth"
-version = "0.0.3"
+version = "0.0.4"
 description = "MAuth plugin for HTTPie"
-authors = ["Mason Gup <mason.gup@3ds.com>"]
+authors = ["Mason Gup <masongup@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "httpie_mauth.py"}]
-repository = "https://github.com/masongup-mdsol/httpie-mauth"
+repository = "https://github.com/masongup/httpie-mauth"
 classifiers = [
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Internet :: WWW/HTTP',
```

### Comparing `httpie_mauth-0.0.3/PKG-INFO` & `httpie_mauth-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpie-mauth
-Version: 0.0.3
+Version: 0.0.4
 Summary: MAuth plugin for HTTPie
-Home-page: https://github.com/masongup-mdsol/httpie-mauth
+Home-page: https://github.com/masongup/httpie-mauth
 License: MIT
 Author: Mason Gup
-Author-email: mason.gup@3ds.com
+Author-email: masongup@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: httpie (>=3.0.0,<4.0.0)
 Requires-Dist: mauth-client (>=1.2.1,<2.0.0)
-Project-URL: Repository, https://github.com/masongup-mdsol/httpie-mauth
+Project-URL: Repository, https://github.com/masongup/httpie-mauth
 Description-Content-Type: text/markdown
 
 # HTTPie mauth
 
 This is a plugin for the [HTTPie](https://github.com/jakubroztocil/httpie)
 command line request library that allows it to send mauth-authenticated requests.
```

