# Comparing `tmp/embeddings_visualizer-0.0.2.tar.gz` & `tmp/embeddings_visualizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_visualizer-0.0.2.tar", max compression
+gzip compressed data, was "embeddings_visualizer-0.0.3.tar", max compression
```

## Comparing `embeddings_visualizer-0.0.2.tar` & `embeddings_visualizer-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1425 2023-07-03 19:11:42.483758 embeddings_visualizer-0.0.2/README.md
--rw-r--r--   0        0        0     2423 2023-07-03 19:11:42.483758 embeddings_visualizer-0.0.2/embeddings_visualizer/main.py
--rw-r--r--   0        0        0      679 2023-07-03 19:11:42.487758 embeddings_visualizer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-04 17:14:30.081307 embeddings_visualizer-0.0.3/README.md
+-rw-r--r--   0        0        0     2423 2023-07-04 17:14:30.081307 embeddings_visualizer-0.0.3/embeddings_visualizer/main.py
+-rw-r--r--   0        0        0      686 2023-07-04 17:14:30.081307 embeddings_visualizer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.3/PKG-INFO
```

### Comparing `embeddings_visualizer-0.0.2/README.md` & `embeddings_visualizer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.2/embeddings_visualizer/main.py` & `embeddings_visualizer-0.0.3/embeddings_visualizer/main.py`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.2/pyproject.toml` & `embeddings_visualizer-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "embeddings-visualizer"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["markus <datamastery87@gmail.com>"]
 readme = "README.md"
 packages = [{include = "embeddings_visualizer"}]
 
 [tool.poetry.scripts]
 ev = "embeddings_visualizer.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9.0, !=3.9.7"
-streamlit = "^1.24.0"
-typer = "^0.9.0"
-numpy = "^1.25.0"
-pandas = "^2.0.3"
-openai = "^0.27.8"
+streamlit = ">=1.20.0"
+typer = ">=0.7.0"
+numpy = ">=1.20.0"
+pandas = ">=2.0.0"
+openai = ">=0.27.0"
 python-dotenv = "^1.0.0"
-scikit-learn = "^1.3.0"
-plotly = "^5.15.0"
-matplotlib = "^3.7.1"
-langchain = "^0.0.222"
+scikit-learn = "^1.2.0"
+plotly = ">=5.0.0"
+matplotlib = ">=3.6.0"
+langchain = ">=0.0.200"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [build-system]
```

### Comparing `embeddings_visualizer-0.0.2/PKG-INFO` & `embeddings_visualizer-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: embeddings-visualizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: markus
 Author-email: datamastery87@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.0.222,<0.0.223)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.25.0,<2.0.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: plotly (>=5.15.0,<6.0.0)
+Requires-Dist: langchain (>=0.0.200)
+Requires-Dist: matplotlib (>=3.6.0)
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: openai (>=0.27.0)
+Requires-Dist: pandas (>=2.0.0)
+Requires-Dist: plotly (>=5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
-Requires-Dist: streamlit (>=1.24.0,<2.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: streamlit (>=1.20.0)
+Requires-Dist: typer (>=0.7.0)
 Description-Content-Type: text/markdown
 
 # Embeddings Visualizer
 
 `Embeddings Visualizer` is a Python package that provides tools for visualizing text embeddings generated from the OpenAI API. The package uses Streamlit for creating interactive visualization dashboards, and can be executed within a local Python environment or deployed to a web server.
 
 ## Initialization
```

