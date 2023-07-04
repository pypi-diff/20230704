# Comparing `tmp/cachefunc-0.2.5.tar.gz` & `tmp/cachefunc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachefunc-0.2.5.tar", max compression
+gzip compressed data, was "cachefunc-0.2.6.tar", max compression
```

## Comparing `cachefunc-0.2.5.tar` & `cachefunc-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1734 2023-07-02 14:10:32.741223 cachefunc-0.2.5/README.md
--rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.5/cachefunc/__init__.py
--rw-r--r--   0        0        0     1680 2023-07-02 13:49:54.101540 cachefunc-0.2.5/cachefunc/cache/base.py
--rw-r--r--   0        0        0      865 2023-07-02 13:50:55.496357 cachefunc-0.2.5/cachefunc/cache/dict_cache.py
--rw-r--r--   0        0        0      545 2023-07-02 13:50:48.773435 cachefunc-0.2.5/cachefunc/cache/redis_cache.py
--rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.5/cachefunc/log.py
--rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.5/cachefunc/main.py
--rw-r--r--   0        0        0      394 2023-07-02 14:08:34.340523 cachefunc-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 cachefunc-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1734 2023-07-02 14:10:32.741223 cachefunc-0.2.6/README.md
+-rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.6/cachefunc/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-02 13:49:54.101540 cachefunc-0.2.6/cachefunc/cache/base.py
+-rw-r--r--   0        0        0      865 2023-07-02 13:50:55.496357 cachefunc-0.2.6/cachefunc/cache/dict_cache.py
+-rw-r--r--   0        0        0      545 2023-07-02 13:50:48.773435 cachefunc-0.2.6/cachefunc/cache/redis_cache.py
+-rw-r--r--   0        0        0      204 2023-07-04 15:46:59.802802 cachefunc-0.2.6/cachefunc/log.py
+-rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.6/cachefunc/main.py
+-rw-r--r--   0        0        0      394 2023-07-04 15:55:16.681247 cachefunc-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 cachefunc-0.2.6/PKG-INFO
```

### Comparing `cachefunc-0.2.5/README.md` & `cachefunc-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.5/cachefunc/cache/base.py` & `cachefunc-0.2.6/cachefunc/cache/base.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.5/cachefunc/cache/dict_cache.py` & `cachefunc-0.2.6/cachefunc/cache/dict_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.5/cachefunc/cache/redis_cache.py` & `cachefunc-0.2.6/cachefunc/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.5/cachefunc/main.py` & `cachefunc-0.2.6/cachefunc/main.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.5/PKG-INFO` & `cachefunc-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachefunc
-Version: 0.2.5
+Version: 0.2.6
 Summary: Caching functions and coroutines result with decorators
 Home-page: https://github.com/ma-petrov/cachefunc
 License: MIT
 Author: Petrov Mikhail
 Author-email: petrov.ma@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

