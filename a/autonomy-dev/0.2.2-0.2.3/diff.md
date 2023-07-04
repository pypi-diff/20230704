# Comparing `tmp/autonomy_dev-0.2.2.tar.gz` & `tmp/autonomy_dev-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.2.2.tar", max compression
+gzip compressed data, was "autonomy_dev-0.2.3.tar", max compression
```

## Comparing `autonomy_dev-0.2.2.tar` & `autonomy_dev-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      578 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/LICENSE
--rw-r--r--   0        0        0      913 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/__init__.py
--rw-r--r--   0        0        0     2569 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     3456 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     1890 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0      962 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/fsm.py
--rw-r--r--   0        0        0     2144 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     5195 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/repo.py
--rw-r--r--   0        0        0     3400 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/scaffold.py
--rw-r--r--   0        0        0     1450 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/test.py
--rw-r--r--   0        0        0      515 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/constants.py
--rw-r--r--   0        0        0     1482 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/block_explorer.py
--rw-r--r--   0        0        0     5617 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract.py
--rw-r--r--   0        0        0     2914 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_functions.py
--rw-r--r--   0        0        0     2238 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_scafolder.py
--rw-r--r--   0        0        0     6086 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_templates.py
--rw-r--r--   0        0        0     1493 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/function.py
--rw-r--r--   0        0        0      525 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/param_type.py
--rw-r--r--   0        0        0     1392 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/utils.py
--rw-r--r--   0        0        0     1534 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/variable.py
--rw-r--r--   0        0        0     1158 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/contracts/header.py
--rw-r--r--   0        0        0      173 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      642 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      532 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/repo/templates/python/readme.py
--rw-r--r--   0        0        0     2027 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/fmt.py
--rw-r--r--   0        0        0     4084 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/fsm/fsm.py
--rw-r--r--   0        0        0      464 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/lint.py
--rw-r--r--   0        0        0     2153 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/local_fork.py
--rw-r--r--   0        0        0      470 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/test.py
--rw-r--r--   0        0        0     2542 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/utils.py
--rw-r--r--   0        0        0     2635 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      296 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1634 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_augmenter.py
--rw-r--r--   0        0        0     1084 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_cli.py
--rw-r--r--   0        0        0     2459 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_contracts.py
--rw-r--r--   0        0        0     3626 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_fsm.py
--rw-r--r--   0        0        0     1562 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_local_fork.py
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 autonomy_dev-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/LICENSE
+-rw-r--r--   0        0        0      913 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3456 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     1890 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     1372 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/fsm.py
+-rw-r--r--   0        0        0     2144 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     5195 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0     3400 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/constants.py
+-rw-r--r--   0        0        0     1482 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/block_explorer.py
+-rw-r--r--   0        0        0     5617 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/contract.py
+-rw-r--r--   0        0        0     2914 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/contract_functions.py
+-rw-r--r--   0        0        0     2238 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/contract_scafolder.py
+-rw-r--r--   0        0        0     6086 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/contract_templates.py
+-rw-r--r--   0        0        0     1493 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/function.py
+-rw-r--r--   0        0        0      525 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/param_type.py
+-rw-r--r--   0        0        0     1392 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/utils.py
+-rw-r--r--   0        0        0     1534 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/contracts/variable.py
+-rw-r--r--   0        0        0     1158 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/data/contracts/header.py
+-rw-r--r--   0        0        0      173 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      642 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2027 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/fmt.py
+-rw-r--r--   0        0        0     3090 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/fsm/chain.py
+-rw-r--r--   0        0        0     8406 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/fsm/fsm.py
+-rw-r--r--   0        0        0      464 2023-07-04 00:29:47.105924 autonomy_dev-0.2.3/auto_dev/lint.py
+-rw-r--r--   0        0        0     2153 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/auto_dev/local_fork.py
+-rw-r--r--   0        0        0      470 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/auto_dev/test.py
+-rw-r--r--   0        0        0     2542 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/auto_dev/utils.py
+-rw-r--r--   0        0        0     2635 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1084 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2459 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/test_contracts.py
+-rw-r--r--   0        0        0     5241 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/test_fsm.py
+-rw-r--r--   0        0        0     1562 2023-07-04 00:29:47.109923 autonomy_dev-0.2.3/tests/test_local_fork.py
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 autonomy_dev-0.2.3/PKG-INFO
```

### Comparing `autonomy_dev-0.2.2/LICENSE` & `autonomy_dev-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/README.md` & `autonomy_dev-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/base.py` & `autonomy_dev-0.2.3/auto_dev/base.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/cli_executor.py` & `autonomy_dev-0.2.3/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/augment.py` & `autonomy_dev-0.2.3/auto_dev/commands/augment.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/fmt.py` & `autonomy_dev-0.2.3/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/fsm.py` & `autonomy_dev-0.2.3/auto_dev/commands/fsm.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,22 +21,31 @@
     """
     Implement fsm tooling
     """
 
 
 @fsm.command()
 @click.argument("fsm-spec", type=click.File("r", encoding=DEFAULT_ENCODING))
-def from_file(fsm_spec: str):
+@click.option("--in-type", type=click.Choice(["mermaid", "fsm-spec"], case_sensitive=False))
+@click.option("--output", type=click.Choice(["mermaid", "fsm-spec"], case_sensitive=False))
+def from_file(fsm_spec: str, in_type: str, output: str):
     """We template from a file."""
     # we need perform the following steps:
     # 1. load the yaml file
     # 2. validate the yaml file using the open-autonomy fsm tooling
     # 3. perform the generation command
     # 4. write the generated files to disk
     # 5. perform the cleanup commands
     # 5a. clean the tests
     # 5b. clean the payloads
     # 6. perform updates of the generated files
 
-    fsm = FsmSpec.from_yaml(fsm_spec)
+    if in_type == "mermaid":
+        _fsm_spec = fsm_spec.read()
+        fsm = FsmSpec.from_mermaid(_fsm_spec)
+    else:
+        fsm = FsmSpec.from_yaml(fsm_spec)
 
-    print(fsm.to_mermaid())
+    if output == "mermaid":
+        print(fsm.to_mermaid())
+    else:
+        print(fsm.to_string())
```

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/lint.py` & `autonomy_dev-0.2.3/auto_dev/commands/lint.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/repo.py` & `autonomy_dev-0.2.3/auto_dev/commands/repo.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/scaffold.py` & `autonomy_dev-0.2.3/auto_dev/commands/scaffold.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/commands/test.py` & `autonomy_dev-0.2.3/auto_dev/commands/test.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/constants.py` & `autonomy_dev-0.2.3/auto_dev/constants.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/block_explorer.py` & `autonomy_dev-0.2.3/auto_dev/contracts/block_explorer.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/contract.py` & `autonomy_dev-0.2.3/auto_dev/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/contract_functions.py` & `autonomy_dev-0.2.3/auto_dev/contracts/contract_functions.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/contract_scafolder.py` & `autonomy_dev-0.2.3/auto_dev/contracts/contract_scafolder.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/contract_templates.py` & `autonomy_dev-0.2.3/auto_dev/contracts/contract_templates.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/function.py` & `autonomy_dev-0.2.3/auto_dev/contracts/function.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/param_type.py` & `autonomy_dev-0.2.3/auto_dev/contracts/param_type.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/utils.py` & `autonomy_dev-0.2.3/auto_dev/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/contracts/variable.py` & `autonomy_dev-0.2.3/auto_dev/contracts/variable.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/data/contracts/header.py` & `autonomy_dev-0.2.3/auto_dev/data/contracts/header.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/data/pylama.ini` & `autonomy_dev-0.2.3/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/data/repo/templates/python/readme.py` & `autonomy_dev-0.2.3/auto_dev/data/repo/templates/python/readme.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/fmt.py` & `autonomy_dev-0.2.3/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/local_fork.py` & `autonomy_dev-0.2.3/auto_dev/local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/auto_dev/utils.py` & `autonomy_dev-0.2.3/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/pyproject.toml` & `autonomy_dev-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.2.2"
+version = "0.2.3"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `autonomy_dev-0.2.2/tests/test_augmenter.py` & `autonomy_dev-0.2.3/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/tests/test_cli.py` & `autonomy_dev-0.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/tests/test_contracts.py` & `autonomy_dev-0.2.3/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/tests/test_local_fork.py` & `autonomy_dev-0.2.3/tests/test_local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.2/PKG-INFO` & `autonomy_dev-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<=3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

