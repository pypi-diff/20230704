# Comparing `tmp/jupyter_cleaner-0.2.2.tar.gz` & `tmp/jupyter_cleaner-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_cleaner-0.2.2.tar", max compression
+gzip compressed data, was "jupyter_cleaner-0.2.3.tar", max compression
```

## Comparing `jupyter_cleaner-0.2.2.tar` & `jupyter_cleaner-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.2/jupyter_cleaner/__init__.py
--rw-r--r--   0        0        0    16637 2023-06-26 10:27:33.350629 jupyter_cleaner-0.2.2/jupyter_cleaner/jupyter_cleaner.py
--rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.2/LICENSE
--rw-r--r--   0        0        0     1985 2023-06-26 11:05:51.759642 jupyter_cleaner-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2175 2023-06-26 07:51:33.830990 jupyter_cleaner-0.2.2/README.md
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.3/jupyter_cleaner/__init__.py
+-rw-r--r--   0        0        0    16651 2023-07-04 12:00:55.012892 jupyter_cleaner-0.2.3/jupyter_cleaner/jupyter_cleaner.py
+-rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1676 2023-07-04 12:33:15.699775 jupyter_cleaner-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2175 2023-06-26 07:51:33.830990 jupyter_cleaner-0.2.3/README.md
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.3/PKG-INFO
```

### Comparing `jupyter_cleaner-0.2.2/jupyter_cleaner/jupyter_cleaner.py` & `jupyter_cleaner-0.2.3/jupyter_cleaner/jupyter_cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         with open(file) as f:
             original_data = json.load(f)
             if data == original_data:
                 continue
 
         with open(file, "w") as f:
-            json.dump(data, f, indent=indent_level)
+            f.write(json.dumps(data, indent=indent_level) + "\n")
         print(f"Reformatted {str(file)}")
 
 
 @lru_cache
 def find_project_root(
     srcs: Sequence[str], stdin_filename: Optional[str] = None
 ) -> Path:
```

### Comparing `jupyter_cleaner-0.2.2/LICENSE` & `jupyter_cleaner-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.2.2/README.md` & `jupyter_cleaner-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.2.2/PKG-INFO` & `jupyter_cleaner-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cleaner
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy git tracking of Jupyter lab files
 Home-page: https://github.com/Stoops-ML/jupyter-cleaner
 License: MIT
 Author: Daniel Stoops
 Author-email: danielstoops25@gmail.com
 Maintainer: Daniel Stoops
 Maintainer-email: danielstoops25@gmail.com
```

