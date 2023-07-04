# Comparing `tmp/spyral_cli-1.0.3.tar.gz` & `tmp/spyral_cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.3.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.4.tar", max compression
```

## Comparing `spyral_cli-1.0.3.tar` & `spyral_cli-1.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-04 18:55:07.636875 spyral_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.3/src/spyral/__init__.py
--rw-r--r--   0        0        0     5725 2023-07-04 18:55:39.755060 spyral_cli-1.0.3/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-04 19:34:29.786440 spyral_cli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.4/src/spyral/__init__.py
+-rw-r--r--   0        0        0     5798 2023-07-04 19:34:21.402466 spyral_cli-1.0.4/src/spyral/cli.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.4/PKG-INFO
```

### Comparing `spyral_cli-1.0.3/pyproject.toml` & `spyral_cli-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.0.3/src/spyral/cli.py` & `spyral_cli-1.0.4/src/spyral/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                                 f"[{delta:8.2f}s] [rss: {rss/1e6:8.2f}M, max: {self.max_rss/1e6:8.2f}M] [vms: {vms/1e6:8.2f}M, max: {self.max_vms/1e6:8.2f}M]"
                             ),
                         )
                     )
 
                 time.sleep(self.interval)
         except (psutil.NoSuchProcess, psutil.AccessDenied):
+            print("Main process is gone, terminating monitoring thread")
             return
         except Exception as e:
             self.exception = e
             raise e
 
 
 @app.command()
```

### Comparing `spyral_cli-1.0.3/PKG-INFO` & `spyral_cli-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

