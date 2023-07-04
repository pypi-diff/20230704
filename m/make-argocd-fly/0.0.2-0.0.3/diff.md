# Comparing `tmp/make_argocd_fly-0.0.2.tar.gz` & `tmp/make_argocd_fly-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.2.tar", last modified: Tue Jul  4 19:09:44 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.3.tar", last modified: Tue Jul  4 20:49:29 2023, max compression
```

## Comparing `make_argocd_fly-0.0.2.tar` & `make_argocd_fly-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.2/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.2/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      263 2023-07-04 09:12:34.000000 make_argocd_fly-0.0.2/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.2/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.2/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.2/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5016 2023-07-04 19:07:55.000000 make_argocd_fly-0.0.2/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4245 2023-07-04 11:06:06.000000 make_argocd_fly-0.0.2/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      876 2023-07-04 11:05:47.000000 make_argocd_fly-0.0.2/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      614 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-04 19:09:44.000000 make_argocd_fly-0.0.2/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      692 2023-07-04 19:09:37.000000 make_argocd_fly-0.0.2/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.2/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-04 19:09:44.433123 make_argocd_fly-0.0.2/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.3/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.3/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      990 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      639 2023-07-04 19:17:22.000000 make_argocd_fly-0.0.3/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.3/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.3/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.3/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.3/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.3/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.3/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      990 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      692 2023-07-04 20:48:54.000000 make_argocd_fly-0.0.3/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.3/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/setup.cfg
```

### Comparing `make_argocd_fly-0.0.2/LICENSE` & `make_argocd_fly-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.2/make_argocd_fly/config.py` & `make_argocd_fly-0.0.3/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.2/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.3/make_argocd_fly/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,20 +31,22 @@
   for app in apps:
     yml_children = viewer.get_child(app.name).get_files_children('.yml$')
     j2_children = viewer.get_child(app.name).get_files_children('.j2$')
     log.debug('app: {}, yml files: {}, j2_files: {}'.format(app.name, [child.element_rel_path for child in yml_children], [child.element_rel_path for child in j2_children]))
 
     for yml_child in yml_children:
       dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
-      writer.write_file(dir_rel_path, yml_child.name, yml_child.content)
+      for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
+        writer.update_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
 
     for j2_child in j2_children:
       dir_rel_path = extract_dir_rel_path(j2_child.element_rel_path)
       template = environment.get_template(j2_child.element_rel_path)
-      writer.write_file(dir_rel_path, j2_child.name[:-3], template.render(config.vars))
+      for resource_kind, resource_name, resource_yml in multi_resource_parser(template.render(config.vars)):
+        writer.update_resource(dir_rel_path, resource_kind, resource_name, resource_yml)
 
 def step_2(viewer: ResourceViewer, writer: ResourceWriter, config: Config) -> None:
   # step 2: run kustomize
   apps = [app for app in viewer.get_dirs_children(depth=1)]
   for env in config.envs:
     for app in apps:
       env_child = app.get_child(env)
@@ -54,37 +56,37 @@
           dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
           process = subprocess.Popen(['kubectl', 'kustomize',
                                       os.path.join(viewer.root_element_abs_path, dir_rel_path)],
                                       stdout=subprocess.PIPE,stderr=subprocess.PIPE,
                                       universal_newlines=True)
           stdout, stderr = process.communicate()
 
-          for resource_kind, _, resource_yml in multi_resource_parser(stdout):
-            writer.update_resource(os.path.join(env, app.name), resource_yml)
+          for resource_kind, resource_name, resource_yml in multi_resource_parser(stdout):
+            writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
           log.debug(stdout)
       else:
         yml_child = app.get_child('kustomization.yml')
         if yml_child:
           dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
           process = subprocess.Popen(['kubectl', 'kustomize',
                                       os.path.join(viewer.root_element_abs_path, dir_rel_path)],
                                       stdout=subprocess.PIPE,stderr=subprocess.PIPE,
                                       universal_newlines=True)
           stdout, _ = process.communicate()
 
-          for resource_kind, _, resource_yml in multi_resource_parser(stdout):
-            writer.update_resource(os.path.join(env, app.name), resource_yml)
+          for resource_kind, resource_name, resource_yml in multi_resource_parser(stdout):
+            writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
           log.debug(stdout)
         else:
           yml_children = app.get_files_children('.yml$')
 
           for yml_child in yml_children:
             dir_rel_path = extract_dir_rel_path(yml_child.element_rel_path)
-            resource_kind, _ = resource_parser(yml_child.content)
-            writer.write_file(os.path.join(env, app.name), resource_kind + '.yml', yml_child.content)
+            for resource_kind, resource_name, resource_yml in multi_resource_parser(yml_child.content):
+              writer.update_resource(os.path.join(env, app.name), resource_kind, resource_name, resource_yml)
 
 def main() -> None:
   parser = argparse.ArgumentParser(description='Render ArgoCD Applications.')
   parser.add_argument('--env', type=str, default=None, help='Environment to render')
   parser.add_argument('--app', type=str, default=None, help='Application to render')
   parser.add_argument('--root-dir', type=str, default=os.getcwd(), help='Root directory')
   parser.add_argument('--config-file', type=str, default=CONFIG_FILE, help='Configuration file')
@@ -96,12 +98,16 @@
   config = read_config(root_dir, args.config_file)
   if os.path.exists(config.config['tmp_dir']):
     shutil.rmtree(config.config['tmp_dir'])
 
   source_viewer = build_resource_viewer(config.config['source_dir'], args.app)
   tmp_writer = build_resource_writer(config.config['tmp_dir'], config.envs, args.env)
   step_1(source_viewer, tmp_writer, config)
+  tmp_writer.write_updates()
 
   tmp_viewer = build_resource_viewer(config.config['tmp_dir'], args.app)
   output_writer = build_resource_writer(config.config['output_dir'], config.envs, args.env)
   step_2(tmp_viewer, output_writer, config)
+  #TODO: clean only filtered apps/envs
+  if os.path.exists(config.config['output_dir']):
+    shutil.rmtree(config.config['output_dir'])
   output_writer.write_updates()
```

### Comparing `make_argocd_fly-0.0.2/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.3/make_argocd_fly/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,33 +76,31 @@
 
 class ResourceWriter:
   def __init__(self, output_dir_abs_path: str, envs: list, existing_resources: list = None) -> None:
     self.output_dir_abs_path = output_dir_abs_path
     self.envs = envs
     self.existing_resources = existing_resources
 
-  def update_resource(self, dir_rel_path: str, resource_yml: str) -> None:
-    resource_kind, resource_name = resource_parser(resource_yml)
-
+  def update_resource(self, dir_rel_path: str, resource_kind: str, resource_name: str, resource_yml: str) -> None:
     self.existing_resources[(dir_rel_path, resource_kind, resource_name)] = resource_yml
 
   def write_updates(self) -> None:
     for (dir_rel_path, resource_kind, _), resource_yml in self.existing_resources.items():
       self.write_file(dir_rel_path, resource_kind + '.yml', resource_yml)
 
   def write_file(self, dir_rel_path: str, filename: str, resource_yml: str) -> None:
     path = os.path.join(self.output_dir_abs_path, dir_rel_path)
     os.makedirs(path, exist_ok=True)
 
-    if not os.path.exists(os.path.join(path, filename)):
-      with open(os.path.join(path, filename), 'w') as f:
+    if not os.path.exists(os.path.join(path, filename.lower())):
+      with open(os.path.join(path, filename.lower()), 'w') as f:
         f.write(resource_yml)
         f.write('\n')
     else:
-      with open(os.path.join(path, filename), 'a') as f:
+      with open(os.path.join(path, filename.lower()), 'a') as f:
         f.write('---\n')
         f.write(resource_yml)
         f.write('\n')
 
 
 def build_resource_viewer(root_element_abs_path: str, filter: str = None) -> ResourceViewer:
   source_viewer = ResourceViewer(root_element_abs_path)
```

### Comparing `make_argocd_fly-0.0.2/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.3/make_argocd_fly/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 def extract_dir_rel_path(path: str) -> str:
   return os.path.normpath('/'.join(path.split('/')[:-1]))
 
 def resource_parser(resource_yml: str) -> tuple[str, str]:
   resource_kind = None
   resource_name = None
 
-  match = re.search('\nkind:(.*)', resource_yml)
+  match = re.search('kind:(.*)', resource_yml)
   if match and match.groups():
     resource_kind = match.group(1).strip()
 
   match = re.search('\n  name:(.*)', resource_yml)
   if match and match.groups():
     resource_name = match.group(1).strip()
 
   return (resource_kind, resource_name)
 
 def multi_resource_parser(multi_resource_yml: str) -> tuple[str, str, str]:
   for resource_yml in multi_resource_yml.split('---'):
     (resource_kind, resource_name) = resource_parser(resource_yml)
 
-    if resource_kind and resource_name:
+    if resource_kind:
       yield (resource_kind, resource_name, resource_yml.strip())
```

### Comparing `make_argocd_fly-0.0.2/pyproject.toml` & `make_argocd_fly-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
```

