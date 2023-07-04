# Comparing `tmp/embeddings_visualizer-0.0.1.tar.gz` & `tmp/embeddings_visualizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_visualizer-0.0.1.tar", max compression
+gzip compressed data, was "embeddings_visualizer-0.0.2.tar", max compression
```

## Comparing `embeddings_visualizer-0.0.1.tar` & `embeddings_visualizer-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2423 2023-07-03 17:53:41.990372 embeddings_visualizer-0.0.1/embeddings_visualizer/main.py
--rw-r--r--   0        0        0      710 2023-07-03 18:19:58.307943 embeddings_visualizer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1425 2023-07-03 18:01:35.457861 embeddings_visualizer-0.0.1/README.md
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-03 19:11:42.483758 embeddings_visualizer-0.0.2/README.md
+-rw-r--r--   0        0        0     2423 2023-07-03 19:11:42.483758 embeddings_visualizer-0.0.2/embeddings_visualizer/main.py
+-rw-r--r--   0        0        0      679 2023-07-03 19:11:42.487758 embeddings_visualizer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.2/PKG-INFO
```

### Comparing `embeddings_visualizer-0.0.1/embeddings_visualizer/main.py` & `embeddings_visualizer-0.0.2/embeddings_visualizer/main.py`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.1/pyproject.toml` & `embeddings_visualizer-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[tool.poetry]
-name = "embeddings-visualizer"
-version = "0.0.1"
-description = ""
-authors = ["markus <datamastery87@gmail.com>"]
-readme = "README.md"
-packages = [{include = "embeddings_visualizer"}]
-
-[tool.poetry.scripts]
-ev = "embeddings_visualizer.main:app"
-
-[tool.poetry.dependencies]
-python = "^3.9.0, !=3.9.7"
-streamlit = "^1.24.0"
-typer = "^0.9.0"
-numpy = "^1.25.0"
-pandas = "^2.0.3"
-openai = "^0.27.8"
-python-dotenv = "^1.0.0"
-scikit-learn = "^1.3.0"
-plotly = "^5.15.0"
-matplotlib = "^3.7.1"
-langchain = "^0.0.222"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-isort = "^5.12.0"
-
-[build-system]
-requires = ["poetry-core"]
+[tool.poetry]
+name = "embeddings-visualizer"
+version = "0.0.2"
+description = ""
+authors = ["markus <datamastery87@gmail.com>"]
+readme = "README.md"
+packages = [{include = "embeddings_visualizer"}]
+
+[tool.poetry.scripts]
+ev = "embeddings_visualizer.main:app"
+
+[tool.poetry.dependencies]
+python = "^3.9.0, !=3.9.7"
+streamlit = "^1.24.0"
+typer = "^0.9.0"
+numpy = "^1.25.0"
+pandas = "^2.0.3"
+openai = "^0.27.8"
+python-dotenv = "^1.0.0"
+scikit-learn = "^1.3.0"
+plotly = "^5.15.0"
+matplotlib = "^3.7.1"
+langchain = "^0.0.222"
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+
+[build-system]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `embeddings_visualizer-0.0.1/README.md` & `embeddings_visualizer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.1/PKG-INFO` & `embeddings_visualizer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-visualizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: markus
 Author-email: datamastery87@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

