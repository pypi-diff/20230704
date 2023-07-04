# Comparing `tmp/spyral_cli-1.0.1.tar.gz` & `tmp/spyral_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.1.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.2.tar", max compression
```

## Comparing `spyral_cli-1.0.1.tar` & `spyral_cli-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-04 15:44:41.867588 spyral_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.1/src/spyral/__init__.py
--rw-r--r--   0        0        0     5630 2023-07-04 15:44:41.867734 spyral_cli-1.0.1/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-04 18:22:37.700533 spyral_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.2/src/spyral/__init__.py
+-rw-r--r--   0        0        0     5632 2023-07-04 18:22:31.212400 spyral_cli-1.0.2/src/spyral/cli.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.2/PKG-INFO
```

### Comparing `spyral_cli-1.0.1/pyproject.toml` & `spyral_cli-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.0.1/src/spyral/cli.py` & `spyral_cli-1.0.2/src/spyral/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         t.start()
 
         try:
             while p.status() in (psutil.STATUS_RUNNING, psutil.STATUS_SLEEPING):
                 for line in iter(p.stdout.readline, b""):
                     if not t.is_alive():
                         print("Monitoring thread has died")
-                        raise t.exception
+                        raise mon.exception
                     live.console.out(line.decode("utf-8"), highlight=False, end="")
         except KeyboardInterrupt:
             mon.terminate = True
             t.join()
             p.kill()
             raise
```

### Comparing `spyral_cli-1.0.1/PKG-INFO` & `spyral_cli-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

