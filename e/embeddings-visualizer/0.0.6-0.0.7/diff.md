# Comparing `tmp/embeddings_visualizer-0.0.6.tar.gz` & `tmp/embeddings_visualizer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_visualizer-0.0.6.tar", max compression
+gzip compressed data, was "embeddings_visualizer-0.0.7.tar", max compression
```

## Comparing `embeddings_visualizer-0.0.6.tar` & `embeddings_visualizer-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1425 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/README.md
--rw-r--r--   0        0        0     3207 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/embeddings_visualizer/app.py
--rw-r--r--   0        0        0     3235 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/embeddings_visualizer/embeddings.ipynb
--rw-r--r--   0        0        0     2546 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/embeddings_visualizer/main.py
--rw-r--r--   0        0        0     2778 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/embeddings_visualizer/questions.csv
--rw-r--r--   0        0        0      686 2023-07-04 17:35:41.696328 embeddings_visualizer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-04 17:55:30.482554 embeddings_visualizer-0.0.7/README.md
+-rw-r--r--   0        0        0     3207 2023-07-04 17:55:30.482554 embeddings_visualizer-0.0.7/embeddings_visualizer/app.py
+-rw-r--r--   0        0        0     3235 2023-07-04 17:55:30.482554 embeddings_visualizer-0.0.7/embeddings_visualizer/embeddings.ipynb
+-rw-r--r--   0        0        0     2673 2023-07-04 17:55:30.482554 embeddings_visualizer-0.0.7/embeddings_visualizer/main.py
+-rw-r--r--   0        0        0     2778 2023-07-04 17:55:30.482554 embeddings_visualizer-0.0.7/embeddings_visualizer/questions.csv
+-rw-r--r--   0        0        0      686 2023-07-04 17:55:30.486554 embeddings_visualizer-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.7/PKG-INFO
```

### Comparing `embeddings_visualizer-0.0.6/README.md` & `embeddings_visualizer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.6/embeddings_visualizer/app.py` & `embeddings_visualizer-0.0.7/embeddings_visualizer/app.py`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.6/embeddings_visualizer/embeddings.ipynb` & `embeddings_visualizer-0.0.7/embeddings_visualizer/embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.6/embeddings_visualizer/main.py` & `embeddings_visualizer-0.0.7/embeddings_visualizer/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
 @app.command()
 def start_app():
     """
     Start the app
     """
     load_dotenv(find_dotenv())
+
+    # Debug line: print out the current environment variables
+    typer.echo(f"Current environment variables: {os.environ}")
+
     if "OPENAI_API_KEY" not in os.environ or not os.environ["OPENAI_API_KEY"]:
         typer.echo("Error: No OPENAI_API_KEY found.")
         raise typer.Exit(code=1)
     else:
         subprocess.call(["streamlit", "run", "app.py"])
```

### Comparing `embeddings_visualizer-0.0.6/embeddings_visualizer/questions.csv` & `embeddings_visualizer-0.0.7/embeddings_visualizer/questions.csv`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.6/pyproject.toml` & `embeddings_visualizer-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embeddings-visualizer"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["markus <datamastery87@gmail.com>"]
 readme = "README.md"
 packages = [{include = "embeddings_visualizer"}]
 
 [tool.poetry.scripts]
 ev = "embeddings_visualizer.main:app"
```

### Comparing `embeddings_visualizer-0.0.6/PKG-INFO` & `embeddings_visualizer-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-visualizer
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: markus
 Author-email: datamastery87@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

