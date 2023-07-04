# Comparing `tmp/embeddings_visualizer-0.0.8.tar.gz` & `tmp/embeddings_visualizer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_visualizer-0.0.8.tar", max compression
+gzip compressed data, was "embeddings_visualizer-0.0.9.tar", max compression
```

## Comparing `embeddings_visualizer-0.0.8.tar` & `embeddings_visualizer-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1425 2023-07-04 18:05:15.850598 embeddings_visualizer-0.0.8/README.md
--rw-r--r--   0        0        0     3207 2023-07-04 18:05:15.850598 embeddings_visualizer-0.0.8/embeddings_visualizer/app.py
--rw-r--r--   0        0        0     3235 2023-07-04 18:05:15.850598 embeddings_visualizer-0.0.8/embeddings_visualizer/embeddings.ipynb
--rw-r--r--   0        0        0     2335 2023-07-04 18:05:15.850598 embeddings_visualizer-0.0.8/embeddings_visualizer/main.py
--rw-r--r--   0        0        0     2778 2023-07-04 18:05:15.850598 embeddings_visualizer-0.0.8/embeddings_visualizer/questions.csv
--rw-r--r--   0        0        0      686 2023-07-04 18:05:15.854598 embeddings_visualizer-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/README.md
+-rw-r--r--   0        0        0     3268 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/embeddings_visualizer/app.py
+-rw-r--r--   0        0        0     3235 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/embeddings_visualizer/embeddings.ipynb
+-rw-r--r--   0        0        0     2292 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/embeddings_visualizer/main.py
+-rw-r--r--   0        0        0     2778 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/embeddings_visualizer/questions.csv
+-rw-r--r--   0        0        0      686 2023-07-04 18:14:32.303229 embeddings_visualizer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.9/PKG-INFO
```

### Comparing `embeddings_visualizer-0.0.8/README.md` & `embeddings_visualizer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.8/embeddings_visualizer/app.py` & `embeddings_visualizer-0.0.9/embeddings_visualizer/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 import plotly.express as px
 import plotly.graph_objects as go
 import streamlit as st
 from dotenv import find_dotenv, load_dotenv
 from langchain.embeddings import OpenAIEmbeddings
 from openai.embeddings_utils import get_embeddings
 from sklearn.decomposition import PCA
+import openai
 
 load_dotenv(find_dotenv())
 
+openai.api_key = os.environ["OPENAI_API_KEY"]
+
 st.set_page_config(layout="wide")
 
 st.title("Text Embeddings Visualization")
 
 uploaded_file = st.file_uploader("Choose a file")
 if uploaded_file:
     delimiter = st.text_input("Enter the delimiter", ";")
```

### Comparing `embeddings_visualizer-0.0.8/embeddings_visualizer/embeddings.ipynb` & `embeddings_visualizer-0.0.9/embeddings_visualizer/embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.8/embeddings_visualizer/main.py` & `embeddings_visualizer-0.0.9/embeddings_visualizer/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from enum import Enum
 
 import typer
-from dotenv import find_dotenv, load_dotenv
 
 app = typer.Typer()
 
 
 class Provider(str, Enum):
     OPENAI = "openai"
     AZURE = "azure"
 
+
 def is_valid_provider(value: str) -> str:
     if value not in Provider:
         raise typer.BadParameter("Provider should be either 'openai' or 'azure'.")
     return value
 
 
 @app.command()
```

### Comparing `embeddings_visualizer-0.0.8/embeddings_visualizer/questions.csv` & `embeddings_visualizer-0.0.9/embeddings_visualizer/questions.csv`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.8/pyproject.toml` & `embeddings_visualizer-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embeddings-visualizer"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["markus <datamastery87@gmail.com>"]
 readme = "README.md"
 packages = [{include = "embeddings_visualizer"}]
 
 [tool.poetry.scripts]
 ev = "embeddings_visualizer.main:app"
```

### Comparing `embeddings_visualizer-0.0.8/PKG-INFO` & `embeddings_visualizer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-visualizer
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: markus
 Author-email: datamastery87@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

