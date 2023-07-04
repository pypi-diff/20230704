# Comparing `tmp/make_argocd_fly-0.0.1.tar.gz` & `tmp/make_argocd_fly-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.1.tar", last modified: Tue Jul  4 12:31:18 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.2.tar", last modified: Tue Jul  4 19:09:44 2023, max compression
```

## Comparing `make_argocd_fly-0.0.1.tar` & `make_argocd_fly-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 12:31:18.033131 make_argocd_fly-0.0.1/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.1/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.1/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 12:31:18.033131 make_argocd_fly-0.0.1/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      263 2023-07-04 09:12:34.000000 make_argocd_fly-0.0.1/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 12:31:18.023131 make_argocd_fly-0.0.1/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.1/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.1/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.1/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5110 2023-07-04 11:21:06.000000 make_argocd_fly-0.0.1/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4245 2023-07-04 11:06:06.000000 make_argocd_fly-0.0.1/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      876 2023-07-04 11:05:47.000000 make_argocd_fly-0.0.1/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 12:31:18.033131 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-04 12:31:18.000000 make_argocd_fly-0.0.1/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      692 2023-07-04 12:30:14.000000 make_argocd_fly-0.0.1/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.1/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-04 12:31:18.033131 make_argocd_fly-0.0.1/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.2/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.2/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      263 2023-07-04 09:12:34.000000 make_argocd_fly-0.0.2/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.2/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.2/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.2/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5016 2023-07-04 19:07:55.000000 make_argocd_fly-0.0.2/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4245 2023-07-04 11:06:06.000000 make_argocd_fly-0.0.2/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      876 2023-07-04 11:05:47.000000 make_argocd_fly-0.0.2/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      692 2023-07-04 19:09:37.000000 make_argocd_fly-0.0.2/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.2/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/setup.cfg
```

### Comparing `make_argocd_fly-0.0.1/LICENSE` & `make_argocd_fly-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.1/PKG-INFO` & `make_argocd_fly-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make_argocd_fly
-Version: 0.0.1
+Version: 0.0.2
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `make_argocd_fly-0.0.1/make_argocd_fly/config.py` & `make_argocd_fly-0.0.2/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.1/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.2/make_argocd_fly/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,26 @@
                                       universal_newlines=True)
           stdout, stderr = process.communicate()
 
           for resource_kind, _, resource_yml in multi_resource_parser(stdout):
             writer.update_resource(os.path.join(env, app.name), resource_yml)
           log.debug(stdout)
       else:
-        base_child= app.get_child('base')
-        if base_child:
-          yml_child = base_child.get_child('kustomization.yml')
-          if yml_child:
-            dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
-            process = subprocess.Popen(['kubectl', 'kustomize',
-                                        os.path.join(viewer.root_element_abs_path, dir_rel_path)],
-                                        stdout=subprocess.PIPE,stderr=subprocess.PIPE,
-                                        universal_newlines=True)
-            stdout, _ = process.communicate()
+        yml_child = app.get_child('kustomization.yml')
+        if yml_child:
+          dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
+          process = subprocess.Popen(['kubectl', 'kustomize',
+                                      os.path.join(viewer.root_element_abs_path, dir_rel_path)],
+                                      stdout=subprocess.PIPE,stderr=subprocess.PIPE,
+                                      universal_newlines=True)
+          stdout, _ = process.communicate()
 
-            for resource_kind, _, resource_yml in multi_resource_parser(stdout):
-              writer.update_resource(os.path.join(env, app.name), resource_yml)
-            log.debug(stdout)
+          for resource_kind, _, resource_yml in multi_resource_parser(stdout):
+            writer.update_resource(os.path.join(env, app.name), resource_yml)
+          log.debug(stdout)
         else:
           yml_children = app.get_files_children('.yml$')
 
           for yml_child in yml_children:
             dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
             resource_kind, _ = resource_parser(yml_child.content)
             writer.write_file(os.path.join(env, app.name), resource_kind + '.yml', yml_child.content)
```

### Comparing `make_argocd_fly-0.0.1/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.2/make_argocd_fly/resource.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.1/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.2/make_argocd_fly/utils.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.1/make_argocd_fly.egg-info/PKG-INFO` & `make_argocd_fly-0.0.2/make_argocd_fly.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-argocd-fly
-Version: 0.0.1
+Version: 0.0.2
 Summary: A project to generate ArgoCD application resources
 Author-email: Andrei Lapin <karandash8@gmail.com>
 License: GPLv3+
 Keywords: argocd,kustomize,jinja2
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `make_argocd_fly-0.0.1/pyproject.toml` & `make_argocd_fly-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
```

