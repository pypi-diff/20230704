# Comparing `tmp/autopack_tools-0.2.1.tar.gz` & `tmp/autopack_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.1.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.2.tar", max compression
```

## Comparing `autopack_tools-0.2.1.tar` & `autopack_tools-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.1/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.1/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.1/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.1/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.1/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-06-30 20:09:47.859652 autopack_tools-0.2.1/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-06-30 20:09:47.833824 autopack_tools-0.2.1/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.1/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-06-30 20:09:48.256517 autopack_tools-0.2.1/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-02 21:30:44.097116 autopack_tools-0.2.1/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-06-30 20:09:47.867664 autopack_tools-0.2.1/autopack/pack.py
--rw-r--r--   0        0        0      636 2023-06-30 20:05:59.914181 autopack_tools-0.2.1/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.1/autopack/search.py
--rw-r--r--   0        0        0     2773 2023-07-02 22:58:29.476822 autopack_tools-0.2.1/autopack/selection.py
--rw-r--r--   0        0        0     4450 2023-07-02 21:30:44.111776 autopack_tools-0.2.1/autopack/utils.py
--rw-r--r--   0        0        0      910 2023-07-02 22:58:35.269800 autopack_tools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.2/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.2/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.2/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.2/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.2/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.2/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.2/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.2/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-04 00:57:01.539973 autopack_tools-0.2.2/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.2/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.2/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.2/autopack/search.py
+-rw-r--r--   0        0        0     2608 2023-07-04 00:57:01.095471 autopack_tools-0.2.2/autopack/selection.py
+-rw-r--r--   0        0        0     4405 2023-07-04 00:57:01.553490 autopack_tools-0.2.2/autopack/utils.py
+-rw-r--r--   0        0        0      910 2023-07-04 00:56:03.603405 autopack_tools-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.2/PKG-INFO
```

### Comparing `autopack_tools-0.2.1/LICENSE` & `autopack_tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/README.md` & `autopack_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/api.py` & `autopack_tools-0.2.2/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/cli.py` & `autopack_tools-0.2.2/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/get_pack.py` & `autopack_tools-0.2.2/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/installation.py` & `autopack_tools-0.2.2/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/pack.py` & `autopack_tools-0.2.2/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.1/autopack/pack_response.py` & `autopack_tools-0.2.2/autopack/pack_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,11 +17,13 @@
     name: str
     dependencies: list[str]
     source: str
     run_args: dict[str, Any]
     init_args: dict[str, Any]
 
     def pack_path(self) -> str:
-        return f"{self.author}_{self.repo}_{self.name}".replace("-", "_")
+        return f"{self.author}_{self.repo}_{self.name}".replace("-", "_").replace(
+            " ", "_"
+        )
 
     def repo_url(self) -> str:
         return f"https://github.com/{self.author}/{self.repo}.git"
```

### Comparing `autopack_tools-0.2.1/autopack/selection.py` & `autopack_tools-0.2.2/autopack/selection.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,24 +48,22 @@
                 "name": pack.name,
                 "description": pack.description,
                 "arguments": pack.run_args,
             }
         )
 
     tools_string = json.dumps(pack_summaries)
-    prompt = TOOL_SELECTION_PROMPT.format(user_input=task_description, tools_string=tools_string)
+    prompt = TOOL_SELECTION_PROMPT.format(
+        user_input=task_description, tools_string=tools_string
+    )
 
     pseudo_ids = ask_llm(prompt, llm)
 
     selected_packs = []
     for pseudo_id in pseudo_ids:
-        # Sometimes they'll give an array like [{'tool_id': 1234}]. Try to accommodate that.
-        if type(pseudo_id) == dict:
-            pseudo_id = pseudo_id.get("tool_id")
-
         # Get the proper pack_id from the pseudo_id
         proper_id = packs_by_pseudo_id[pseudo_id]
         selected_packs.append(proper_id)
 
     return selected_packs
```

### Comparing `autopack_tools-0.2.1/autopack/utils.py` & `autopack_tools-0.2.2/autopack/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,27 +57,26 @@
     metadata_file = os.path.join(metadata_dir, "pack_metadata.json")
 
     with open(metadata_file, "w+") as f:
         json.dump(data, f)
 
 
 def find_module(pack_data: PackResponse) -> ModuleType:
+    autopack_dir = find_or_create_autopack_dir()
     module_path = pack_data.module_path
+    pack_module_path = os.path.join(autopack_dir, pack_data.pack_path())
+
+    sys.path.insert(0, autopack_dir)
+    sys.path.insert(0, pack_module_path)
 
-    # Just in case they already have it in their path for whatever reason
     try:
         return importlib.import_module(module_path)
-    except:
-        autopack_dir = find_or_create_autopack_dir()
-        sys.path.insert(0, autopack_dir)
-
-        try:
-            return importlib.import_module(pack_data.pack_path() + "." + module_path)
-        finally:
-            sys.path.remove(autopack_dir)
+    finally:
+        sys.path.remove(autopack_dir)
+        sys.path.remove(pack_module_path)
 
 
 def fetch_pack_object(pack_data: PackResponse, quiet=False) -> Pack:
     try:
         module = find_module(pack_data)
         if not module:
             message = (
```

### Comparing `autopack_tools-0.2.1/pyproject.toml` & `autopack_tools-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.1"
+version = "0.2.2"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.2.1/PKG-INFO` & `autopack_tools-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

