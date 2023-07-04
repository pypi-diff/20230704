# Comparing `tmp/ptarcade-0.1.3.tar.gz` & `tmp/ptarcade-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.3.tar", max compression
+gzip compressed data, was "ptarcade-0.1.4.tar", max compression
```

## Comparing `ptarcade-0.1.3.tar` & `ptarcade-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-06-30 22:17:44.000000 ptarcade-0.1.3/LICENSE
--rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.3/README.md
--rw-r--r--   0        0        0     3313 2023-07-02 17:53:09.136777 ptarcade-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      555 2023-07-02 01:53:08.893492 ptarcade-0.1.3/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-30 21:13:04.270655 ptarcade-0.1.3/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4994 2023-07-02 16:09:59.530041 ptarcade-0.1.3/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-07-02 03:08:58.531872 ptarcade-0.1.3/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6885 2023-06-30 21:13:19.488677 ptarcade-0.1.3/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    11542 2023-07-02 16:09:59.530041 ptarcade-0.1.3/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    18088 2023-06-30 21:26:10.379417 ptarcade-0.1.3/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-02 18:28:45.209694 ptarcade-0.1.4/LICENSE
+-rw-r--r--   0        0        0      673 2023-07-02 18:28:45.209694 ptarcade-0.1.4/README.md
+-rw-r--r--   0        0        0     3313 2023-07-04 17:31:28.939748 ptarcade-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4994 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30151 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6885 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    12031 2023-07-04 17:30:58.493116 ptarcade-0.1.4/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    18088 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.4/PKG-INFO
```

### Comparing `ptarcade-0.1.3/LICENSE` & `ptarcade-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/README.md` & `ptarcade-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/pyproject.toml` & `ptarcade-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.3"
+version = "0.1.4"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
```

### Comparing `ptarcade-0.1.3/src/ptarcade/__init__.py` & `ptarcade-0.1.4/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/chains_utils.py` & `ptarcade-0.1.4/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/data/default_config.py` & `ptarcade-0.1.4/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.4/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.4/src/ptarcade/fast_interpolate.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/input_handler.py` & `ptarcade-0.1.4/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/models_utils.py` & `ptarcade-0.1.4/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/plot_utils.py` & `ptarcade-0.1.4/src/ptarcade/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/pta_importer.py` & `ptarcade-0.1.4/src/ptarcade/pta_importer.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/src/ptarcade/sampler.py` & `ptarcade-0.1.4/src/ptarcade/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,21 +287,29 @@
         warnings.filterwarnings(
             "ignore",
             category=RuntimeWarning,
             message="divide by zero encountered in log",
             module="enterprise.signals.parameter",
             lineno=62,
         )
-        sampler.sample(
-            x0,
-            N_samples,
-            SCAMweight=inputs["config"].scam_weight,
-            AMweight=inputs["config"].am_weight,
-            DEweight=inputs["config"].de_weight,
-        )
+        try:
+            sampler.sample(
+                x0,
+                N_samples,
+                SCAMweight=inputs["config"].scam_weight,
+                AMweight=inputs["config"].am_weight,
+                DEweight=inputs["config"].de_weight,
+            )
+        except RuntimeError as e:
+            err = ("There was an error while sampling. If this error involves autocorrelation time,\n"
+                  "a temporary fix is to increase the number of samples in the configuration file.\n"
+                  "We are actively working to upgrade the autocorrelation routines in our sampler.\n\n")
+            console.print("\n\n")
+            log.exception(err)
+            raise SystemExit from None
 
     console.print()
     console.print(Panel.fit("[bold green]Done sampling[/]", border_style="green"))
     console.print()
 
 
 def main():
```

### Comparing `ptarcade-0.1.3/src/ptarcade/signal_builder.py` & `ptarcade-0.1.4/src/ptarcade/signal_builder.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.3/PKG-INFO` & `ptarcade-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.3
+Version: 0.1.4
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
```

