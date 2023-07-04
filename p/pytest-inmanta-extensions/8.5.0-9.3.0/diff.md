# Comparing `tmp/pytest-inmanta-extensions-8.5.0.tar.gz` & `tmp/pytest-inmanta-extensions-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-extensions-8.5.0.tar", last modified: Tue Jul  4 12:54:48 2023, max compression
+gzip compressed data, was "pytest-inmanta-extensions-9.3.0.tar", last modified: Tue Jul  4 11:30:21 2023, max compression
```

## Comparing `pytest-inmanta-extensions-8.5.0.tar` & `pytest-inmanta-extensions-9.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.124203 pytest-inmanta-extensions-8.5.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 12:54:48.124203 pytest-inmanta-extensions-8.5.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/README.md
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-07-04 12:54:48.125203 pytest-inmanta-extensions-8.5.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.121203 pytest-inmanta-extensions-8.5.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.122203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    70075 2023-07-04 12:54:22.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/conftest.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.123203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.121203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.123203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.key
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-07-04 12:54:22.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/server.crt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-07-04 12:54:22.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/server.open.key
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.123203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-07-04 12:54:22.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/common.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.123203 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/simple_project/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/simple_project/main.cf
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/simple_project/project.yml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-07-04 12:50:50.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/plugin.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25613 2023-07-04 12:54:22.000000 pytest-inmanta-extensions-8.5.0/src/inmanta_tests/utils.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 12:54:48.124203 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-07-04 12:54:48.000000 pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      199 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      467 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/README.md
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       59 2023-07-04 11:30:21.852827 pytest-inmanta-extensions-9.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2481 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.849827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    70339 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.848827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6223 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2069 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3243 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1237 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1679 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.850827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      980 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      212 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/main.cf
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      185 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/simple_project/project.yml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      685 2023-07-04 11:27:43.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25613 2023-07-04 11:29:55.000000 pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-07-04 11:30:21.851827 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1287 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      882 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       55 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      122 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       14 2023-07-04 11:30:21.000000 pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/top_level.txt
```

### Comparing `pytest-inmanta-extensions-8.5.0/PKG-INFO` & `pytest-inmanta-extensions-9.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.5.0
+Version: 9.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.5.0/setup.py` & `pytest-inmanta-extensions-9.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Contact: code@inmanta.com
 """
 from os import path
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.5.0"
+version = "9.3.0"
 
 requires = [
     "asyncpg",
     "click",
     f"inmanta-core~={version}.dev",
     "pip2pi",
     "pyformance",
```

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/__init__.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/conftest.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1069,15 +1069,15 @@
             pkg_resources.working_set = self.working_set
             self._using_venv = True
 
 
 class SnippetCompilationTest(KeepOnFail):
     def setUpClass(self):
         self.libs = tempfile.mkdtemp()
-        self.repo = "https://github.com/inmanta/"
+        self.repo: str = "https://github.com/inmanta/"
         self.env = tempfile.mkdtemp()
         self.venv = ReentrantVirtualEnv(env_path=self.env)
         config.Config.load_config()
         self.keep_shared = False
         self.project = None
 
     def tearDownClass(self):
@@ -1113,14 +1113,15 @@
         add_to_module_path: Optional[List[str]] = None,
         python_package_sources: Optional[List[str]] = None,
         project_requires: Optional[List[InmantaModuleRequirement]] = None,
         python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
         relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
         strict_deps_check: Optional[bool] = None,
+        use_pip_config_file: Optional[bool] = False,
     ) -> Project:
         """
         Sets up the project to compile a snippet of inmanta DSL. Activates the compiler environment (and patches
         env.process_env).
 
         :param install_project: Install the project and all its modules. This is required to be able to compile the model.
         :param install_v2_modules: Indicates which V2 modules should be installed in the compiler venv
@@ -1131,23 +1132,26 @@
                                  file
         :param python_requires: The dependencies on Python packages providing v2 modules.
         :param install_mode: The install mode to configure in the project.yml file of the inmanta project. If None,
                              no install mode is set explicitly in the project.yml file.
         :param relation_precedence_policy: The relation precedence policy that should be stored in the project.yml file of the
                                            Inmanta project.
         :param strict_deps_check: True iff the returned project should have strict dependency checking enabled.
+        :param use_pip_config_file: True iff the pip config file should be used and no source is required for v2 to work
+                                    False if a package source is needed for v2 modules to work
         """
         self.setup_for_snippet_external(
             snippet,
             add_to_module_path,
             python_package_sources,
             project_requires,
             python_requires,
             install_mode,
             relation_precedence_rules,
+            use_pip_config_file,
         )
         return self._load_project(autostd, install_project, install_v2_modules, strict_deps_check=strict_deps_check)
 
     def _load_project(
         self,
         autostd: bool,
         install_project: bool,
@@ -1195,14 +1199,15 @@
         snippet: str,
         add_to_module_path: Optional[List[str]] = None,
         python_package_sources: Optional[List[str]] = None,
         project_requires: Optional[List[InmantaModuleRequirement]] = None,
         python_requires: Optional[List[Requirement]] = None,
         install_mode: Optional[InstallMode] = None,
         relation_precedence_rules: Optional[List[RelationPrecedenceRule]] = None,
+        use_pip_config_file: bool = False,
     ) -> None:
         add_to_module_path = add_to_module_path if add_to_module_path is not None else []
         python_package_sources = python_package_sources if python_package_sources is not None else []
         project_requires = project_requires if project_requires is not None else []
         python_requires = python_requires if python_requires is not None else []
         relation_precedence_rules = relation_precedence_rules if relation_precedence_rules else []
         with open(os.path.join(self.project_dir, "project.yml"), "w", encoding="utf-8") as cfg:
@@ -1212,31 +1217,30 @@
             modulepath: {self._get_modulepath_for_project_yml_file(add_to_module_path)}
             downloadpath: {self.libs}
             version: 1.0
             repo:
                 - {{type: git, url: {self.repo} }}
             """.rstrip()
             )
-            if python_package_sources:
-                cfg.write(
-                    "".join(
-                        f"""
-                - {{type: package, url: {source} }}
-                        """.rstrip()
-                        for source in python_package_sources
-                    )
-                )
+
             if relation_precedence_rules:
                 cfg.write("\n            relation_precedence_policy:\n")
                 cfg.write("\n".join(f"                - {rule}" for rule in relation_precedence_rules))
             if project_requires:
                 cfg.write("\n            requires:\n")
                 cfg.write("\n".join(f"                - {req}" for req in project_requires))
             if install_mode:
                 cfg.write(f"\n            install_mode: {install_mode.value}")
+            cfg.write(
+                f"""
+            pip:
+                use_config_file: {use_pip_config_file}
+                index_urls: [{", ".join(url for url in python_package_sources)}]
+            """
+            )
         with open(os.path.join(self.project_dir, "requirements.txt"), "w", encoding="utf-8") as fd:
             fd.write("\n".join(str(req) for req in python_requires))
         self.main = os.path.join(self.project_dir, "main.cf")
         with open(self.main, "w", encoding="utf-8") as x:
             x.write(snippet)
 
     def _get_modulepath_for_project_yml_file(self, add_to_module_path: List[str] = []) -> str:
```

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.chain` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.chain`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/ca/enduser-certs/server.key.open`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/server.crt` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.crt`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/data/server.open.key` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/data/server.open.key`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/db/common.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/db/common.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/plugin.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/inmanta_tests/utils.py` & `pytest-inmanta-extensions-9.3.0/src/inmanta_tests/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO` & `pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-extensions
-Version: 8.5.0
+Version: 9.3.0
 Summary: Inmanta tests package
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Keywords: pytest inmanta tests
```

### Comparing `pytest-inmanta-extensions-8.5.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt` & `pytest-inmanta-extensions-9.3.0/src/pytest_inmanta_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

