# Comparing `tmp/xboto-1.1.0.tar.gz` & `tmp/xboto-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xboto-1.1.0.tar", max compression
+gzip compressed data, was "xboto-1.1.1.tar", max compression
```

## Comparing `xboto-1.1.0.tar` & `xboto-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-04-15 14:14:27.837397 xboto-1.1.0/LICENSE
--rw-r--r--   0        0        0     2552 2023-04-15 14:14:27.837397 xboto-1.1.0/README.md
--rw-r--r--   0        0        0     1952 2023-04-15 14:14:27.841398 xboto-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/__init__.py
--rw-r--r--   0        0        0     7913 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/client.py
--rw-r--r--   0        0        0    41378 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/dependencies.py
--rw-r--r--   0        0        0     1868 2023-04-15 14:14:27.841398 xboto-1.1.0/xboto/resource.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 xboto-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-03 21:57:46.670415 xboto-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2552 2023-07-03 21:57:46.670415 xboto-1.1.1/README.md
+-rw-r--r--   0        0        0     1952 2023-07-03 21:57:46.670415 xboto-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-03 21:57:46.674415 xboto-1.1.1/xboto/__init__.py
+-rw-r--r--   0        0        0     7913 2023-07-03 21:57:46.674415 xboto-1.1.1/xboto/client.py
+-rw-r--r--   0        0        0    41523 2023-07-03 21:57:46.674415 xboto-1.1.1/xboto/dependencies.py
+-rw-r--r--   0        0        0     1868 2023-07-03 21:57:46.674415 xboto-1.1.1/xboto/resource.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 xboto-1.1.1/PKG-INFO
```

### Comparing `xboto-1.1.0/LICENSE` & `xboto-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xboto-1.1.0/README.md` & `xboto-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xboto-1.1.0/pyproject.toml` & `xboto-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xboto"
-version = "1.1.0"
+version = "1.1.1"
 description = "Easy lazy dependency injection for boto3 clients/resources."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xboto"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xboto"
 keywords = ["boto", "boto client", "boto resource", "inject", "lazy", "dependency", "dependency injection", "aws"]
 classifiers = [
```

### Comparing `xboto-1.1.0/xboto/client.py` & `xboto-1.1.1/xboto/client.py`

 * *Files identical despite different names*

### Comparing `xboto-1.1.0/xboto/dependencies.py` & `xboto-1.1.1/xboto/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,18 @@
         # Normalize name...
         # Client/Resources names never use `_`, they use a `-` instead.
         # Replace any `_` with a `-`
         # (allows one to still get it via attributes, vs having to pass a str into a/the method)
         boto_name = boto_name.replace("_", "-")
         boto_name = boto_name.lower()
 
+        if boto_name.endswith("-"):
+            # Remove ending underscore (ie: for the `lambda_` name).
+            boto_name = boto_name[:-1]
+
         if dep_cls := _dependency_classes[boto_kind].get(boto_name):
             return dep_cls
 
         # We are creating a new type/class lazily based on the required boto resource/client...
         cls_name = f'{boto_name.capitalize()}{boto_kind.capitalize()}'
         dep_cls: Any = type(cls_name, (cls,), {}, boto_name=boto_name, boto_kind=boto_kind)
```

### Comparing `xboto-1.1.0/xboto/resource.py` & `xboto-1.1.1/xboto/resource.py`

 * *Files identical despite different names*

### Comparing `xboto-1.1.0/PKG-INFO` & `xboto-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xboto
-Version: 1.1.0
+Version: 1.1.1
 Summary: Easy lazy dependency injection for boto3 clients/resources.
 Home-page: https://github.com/xyngular/py-xboto
 Keywords: boto,boto client,boto resource,inject,lazy,dependency,dependency injection,aws
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

