# Comparing `tmp/embeddings_visualizer-0.0.4.tar.gz` & `tmp/embeddings_visualizer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embeddings_visualizer-0.0.4.tar", max compression
+gzip compressed data, was "embeddings_visualizer-0.0.5.tar", max compression
```

## Comparing `embeddings_visualizer-0.0.4.tar` & `embeddings_visualizer-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1425 2023-07-04 17:25:30.480961 embeddings_visualizer-0.0.4/README.md
--rw-r--r--   0        0        0     2576 2023-07-04 17:25:30.480961 embeddings_visualizer-0.0.4/embeddings_visualizer/main.py
--rw-r--r--   0        0        0      686 2023-07-04 17:25:30.484961 embeddings_visualizer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-04 17:30:13.453397 embeddings_visualizer-0.0.5/README.md
+-rw-r--r--   0        0        0     2546 2023-07-04 17:30:13.453397 embeddings_visualizer-0.0.5/embeddings_visualizer/main.py
+-rw-r--r--   0        0        0      686 2023-07-04 17:30:13.453397 embeddings_visualizer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 embeddings_visualizer-0.0.5/PKG-INFO
```

### Comparing `embeddings_visualizer-0.0.4/README.md` & `embeddings_visualizer-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `embeddings_visualizer-0.0.4/embeddings_visualizer/main.py` & `embeddings_visualizer-0.0.5/embeddings_visualizer/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 def is_valid_provider(value: str) -> str:
     if value not in Provider:
         raise typer.BadParameter("Provider should be either 'openai' or 'azure'.")
     return value
 
 
 @app.command()
-def init(provider: Provider = typer.Argument(..., callback=is_valid_provider)):
+def init(provider: Provider):
     """
     Initialize the application:
     - Create a .env file with API settings
     - Copy the app.py, embeddings.ipynb, and questions.csv files to the current directory
 
     The 'provider' argument should be either 'openai' or 'azure'.
     """
     # Part 1: Create .env
     if Path(".env").exists():
         typer.echo("Warning: .env file already exists.")
     else:
         with open(".env", "w") as f:
-            if provider == "openai":
+            if provider == Provider.OPENAI:
                 f.write("OPENAI_API_TYPE=openai\n")
                 f.write("OPENAI_API_KEY=\n")
-            elif provider == "azure":
+            elif provider == Provider.AZURE:
                 f.write("OPENAI_API_TYPE=azure\n")
                 f.write("OPENAI_API_BASE=https://<your-endpoint>.openai.azure.com/\n")
                 f.write("OPENAI_API_KEY=<your AzureOpenAI key>\n")
                 f.write("OPENAI_API_VERSION=2023-03-15-preview\n")
-        typer.echo(f".env file with {provider.upper()} API settings created.")
+        typer.echo(f".env file with {provider.value.upper()} API settings created.")
 
     # Part 2: Copy files
     current_dir = Path.cwd()
     for filename in ["app.py", "embeddings.ipynb", "questions.csv"]:
         source_file = Path(__file__).parent / filename
         target_file = current_dir / filename
         if not source_file.exists():
```

### Comparing `embeddings_visualizer-0.0.4/pyproject.toml` & `embeddings_visualizer-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embeddings-visualizer"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["markus <datamastery87@gmail.com>"]
 readme = "README.md"
 packages = [{include = "embeddings_visualizer"}]
 
 [tool.poetry.scripts]
 ev = "embeddings_visualizer.main:app"
```

### Comparing `embeddings_visualizer-0.0.4/PKG-INFO` & `embeddings_visualizer-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embeddings-visualizer
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: markus
 Author-email: datamastery87@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

