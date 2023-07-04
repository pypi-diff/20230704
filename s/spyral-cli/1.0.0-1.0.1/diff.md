# Comparing `tmp/spyral_cli-1.0.0.tar.gz` & `tmp/spyral_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-1.0.0.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.1.tar", max compression
```

## Comparing `spyral_cli-1.0.0.tar` & `spyral_cli-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      691 2023-07-04 07:49:38.767133 spyral_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.0/src/spyral/__init__.py
--rw-r--r--   0        0        0     5497 2023-07-04 07:49:32.356053 spyral_cli-1.0.0/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-04 15:44:41.867588 spyral_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.1/src/spyral/__init__.py
+-rw-r--r--   0        0        0     5630 2023-07-04 15:44:41.867734 spyral_cli-1.0.1/src/spyral/cli.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.1/PKG-INFO
```

### Comparing `spyral_cli-1.0.0/pyproject.toml` & `spyral_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spyral-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Paul Gessinger <hello@paulgessinger.com>"]
 license = "MIT"
 packages = [
   { include = "spyral", from = "src" },
 ]
```

### Comparing `spyral_cli-1.0.0/src/spyral/cli.py` & `spyral_cli-1.0.1/src/spyral/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     interval: float
 
     max_rss: float = 0
     max_vms: float = 0
 
     terminate: bool = False
 
+    exception = None
+
     def __init__(
         self,
         command: List[str],
         output: IO[str],
         interval: float = 0.5,
         live: Optional[rich.live.Live] = None,
     ):
@@ -84,14 +86,17 @@
                             ),
                         )
                     )
 
                 time.sleep(self.interval)
         except (psutil.NoSuchProcess, psutil.AccessDenied):
             return
+        except Exception as e:
+            self.exception = e
+            raise e
 
 
 @app.command()
 def run(
     cmd: List[str],
     interval: float = typer.Option(0.5, "--interval", "-i"),
     output: Path = typer.Option("spyral.csv", "--output", "-o"),
@@ -108,15 +113,16 @@
         t = threading.Thread(target=mon.run, args=(p,))
         t.start()
 
         try:
             while p.status() in (psutil.STATUS_RUNNING, psutil.STATUS_SLEEPING):
                 for line in iter(p.stdout.readline, b""):
                     if not t.is_alive():
-                        raise RuntimeError("Monitoring thread has died")
+                        print("Monitoring thread has died")
+                        raise t.exception
                     live.console.out(line.decode("utf-8"), highlight=False, end="")
         except KeyboardInterrupt:
             mon.terminate = True
             t.join()
             p.kill()
             raise
```

### Comparing `spyral_cli-1.0.0/PKG-INFO` & `spyral_cli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

