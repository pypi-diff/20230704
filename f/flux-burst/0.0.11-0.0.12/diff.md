# Comparing `tmp/flux-burst-0.0.11.tar.gz` & `tmp/flux-burst-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.11.tar", last modified: Mon Jul  3 07:22:13 2023, max compression
+gzip compressed data, was "flux-burst-0.0.12.tar", last modified: Tue Jul  4 01:36:56 2023, max compression
```

## Comparing `flux-burst-0.0.11.tar` & `flux-burst-0.0.12.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.11/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.11/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.11/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.11/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-03 07:22:13.278146 flux-burst-0.0.11/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.11/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.11/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7109 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7534 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/handles.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/kubernetes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6537 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.11/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.11/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.11/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.11/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.11/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-03 07:22:00.000000 flux-burst-0.0.11/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.11/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-03 07:22:13.278146 flux-burst-0.0.11/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.11/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.12/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.12/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.12/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.12/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-04 01:36:56.450937 flux-burst-0.0.12/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.12/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.446937 flux-burst-0.0.12/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-04 01:36:56.000000 flux-burst-0.0.12/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.12/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.446937 flux-burst-0.0.12/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.12/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7534 2023-07-03 07:21:31.000000 flux-burst-0.0.12/fluxburst/handles.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8931 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.12/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.12/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.12/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.12/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.12/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.12/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.12/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.12/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-04 01:36:56.450937 flux-burst-0.0.12/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.12/setup.py
```

### Comparing `flux-burst-0.0.11/LICENSE` & `flux-burst-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/NOTICE` & `flux-burst-0.0.12/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/PKG-INFO` & `flux-burst-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.11
+Version: 0.0.12
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.11 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.12 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.11/README.md` & `flux-burst-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/flux_burst.egg-info/PKG-INFO` & `flux-burst-0.0.12/flux_burst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.11
+Version: 0.0.12
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.11 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.12 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.11/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.12/flux_burst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/client.py` & `flux-burst-0.0.12/fluxburst/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,28 +14,31 @@
 
 
 class FluxBurst:
     """
     Flux Burst Client
     """
 
-    def __init__(self, handle=None, mock=False):
+    def __init__(self, handle=None, mock=False, validate=True):
         """
         Create a new burst client.
 
         Selectors: Process the current queue and add flags/filter jobs for plugins.
         Plugins: take jobs that need bursting, and burst some subset.
         A filter can (on the simplest terms) just look for a job flagged as
         burstable. For more complex cases, it can perform it's own logic and
-        flag some subset as burstable instead.
+        flag some subset as burstable instead. Validation is always done for
+        the top level module, howevert the validate boolean here determines
+        if the plugin should run its own validation function.
         """
         self.reset_selector()
         self.reset_plugins()
         self.flux = handles.FluxMock(handle) if mock else handles.FluxHandle(handle)
         self.set_ordering(sorting.in_order)
+        self.validate = validate
 
     @property
     def choices(self):
         return "|".join(list(self.plugins))
 
     def load(self, name, dataclass, **kwargs):
         """
@@ -50,15 +53,21 @@
 
         # Validate the plugin, first plugin module then loaded class
         self.validate_module(name)
         plugin = burstable_plugins[name].init(dataclass)
 
         # We set the name attribute so it's always matched to the module
         plugin.name = name
-        self.validate_plugin(plugin)
+        self.check_plugin_integrity(plugin)
+
+        # If the plugin does it's own validation, do here
+        if not self.validate_plugin(plugin):
+            logger.warning(f"Plugin {name} did not validate and cannot be added.")
+            return
+
         self.plugins[name] = plugin
 
     def validate_module(self, name):
         """
         Validate the structure of the module.
 
         We currently just require the init function to import and return the class
@@ -68,14 +77,23 @@
                 f"Plugin {name} is missing required init attribute to return BurstPlugin class."
             )
 
     def validate_plugin(self, plugin):
         """
         Validate a plugin, and if valid, load into module.
         """
+        # This should return a boolean for valid or not
+        if hasattr(plugin, "validate") and self.validate:
+            return plugin.validate()
+        return True
+
+    def check_plugin_integrity(self, plugin):
+        """
+        Validate a plugin, and if valid, load into module.
+        """
         required_attributes = ["schedule", "run", "_param_dataclass", "set_params"]
         for required in required_attributes:
             if not hasattr(plugin, required):
                 raise ValueError(
                     f"Plugin {plugin.name} is not valid, missing attribute or function {required}"
                 )
 
@@ -87,30 +105,46 @@
 
     def reset_plugins(self):
         self.plugins = collections.OrderedDict()
 
     def reset_selector(self):
         self._job_selector = selectors.is_burstable
 
-    def run_burst(self):
+    def run_burst(self, request_burst=False, nodes=None, tasks=None):
         """
         A full run burst includes:
 
         1. Selecting jobs using the client filter(s)
         2. In the order of plugins desired, schedule jobs
         3. Return back lookup of scheduled (by plugin)
+
+        If request_burst with nodes and tasks are required, each plugin
+        will simply request creation for the size/tasks needed.
         """
         # TODO what to do with unmatched jobs?
         unmatched = self.process_queue()
 
         # When we get here, run the bursts
         for _, plugin in self.iter_plugins():
-            plugin.run()
+            plugin.run(request_burst=request_burst, nodes=nodes, tasks=tasks)
         return unmatched
 
+    def request_burst(self, name, nodes, tasks):
+        """
+        Request burst is a direct handle to get a plugin and request a burst.
+
+        In this case, we do not create MiniClusters to launch jobs to, but instead
+        create a connected cluster anticipating receiving jobs.
+        """
+        plugin = self.plugins.get(name)
+        if not plugin:
+            logger.warning(f"Plugin {plugin} is not known.")
+            return
+        return plugin.run(request_burst=True, nodes=nodes, tasks=tasks)
+
     def set_ordering(self, func):
         """
         Set a custom function that knows how to yield names, plugins.
         """
         self._iter_func = func
 
     def iter_plugins(self):
```

### Comparing `flux-burst-0.0.11/fluxburst/defaults.py` & `flux-burst-0.0.12/fluxburst/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/handles.py` & `flux-burst-0.0.12/fluxburst/handles.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/kubernetes/cluster.py` & `flux-burst-0.0.12/fluxburst/kubernetes/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     Limits should be slightly below actual pod resources. The curve cert and broker config
     are required, since we need this external cluster to connect to ours!
     """
     flags = flags or "-ompi=openmpi@5 -c 1 -o cpu-affinity=per-task"
     image = image or "ghcr.io/flux-framework/flux-restful-api"
     container = {"image": image, "command": command, "resources": {}}
 
+    # Are we bursting?
+    doing_burst = lead_port and lead_size and lead_jobname
     if cpu_limit is None and memory_limit is None:
         del container["resources"]
     elif cpu_limit is not None or memory_limit is not None:
         container["resources"] = {"limits": {}, "requests": {}}
     if cpu_limit is not None:
         container["resources"]["limits"]["cpu"] = cpu_limit
         container["resources"]["requests"]["cpu"] = cpu_limit
@@ -70,40 +72,43 @@
         "name": name,
         "interactive": False,
         "logging": {"zeromq": zeromq, "quiet": quiet, "strict": strict},
         "flux": {
             "option_flags": flags,
             "connect_timeout": "5s",
             "log_level": log_level,
-            # Providing the lead broker and port points back to the parent
-            "bursting": {
-                "lead_broker": {
-                    "address": lead_host,
-                    "port": int(lead_port),
-                    "name": lead_jobname,
-                    "size": int(lead_size),
-                },
-                "clusters": [{"size": size, "name": name}],
-            },
         },
     }
 
+    # Are we bursting?
+    # Providing the lead broker and port points back to the parent
+    if doing_burst:
+        mc["flux"]["bursting"] = {
+            "lead_broker": {
+                "address": lead_host,
+                "port": int(lead_port),
+                "name": lead_jobname,
+                "size": int(lead_size),
+            },
+            "clusters": [{"size": size, "name": name}],
+        }
+
     if tasks is not None:
         mc["tasks"] = tasks
 
     # This is text directly in config
-    if curve_cert:
+    if doing_burst and curve_cert:
         mc["flux"]["curve_cert"] = curve_cert
 
     # A provided secret will take precedence
-    if curve_cert_secret_name:
+    if doing_burst and curve_cert_secret_name:
         mc["flux"]["curve_cert_secret"] = curve_cert_secret_name
 
     # This is just the secret name
-    if munge_secret_name:
+    if doing_burst and munge_secret_name:
         mc["flux"]["munge_secret"] = munge_secret_name
     if broker_toml:
         mc["flux"]["broker_config"] = broker_toml
 
     # eg., this would require strace "strace,-e,network,-tt"
     if wrap is not None:
         mc["flux"]["wrap"] = wrap
@@ -125,15 +130,15 @@
     """
     Ensure we are provided with the installation yaml and it exists!
     """
     # flux operator yaml default is current from main
     if not flux_operator_yaml:
         flux_operator_yaml = utils.get_tmpfile(prefix="flux-operator") + ".yaml"
         r = requests.get(defaults.flux_operator_yaml, allow_redirects=True)
-        utils.write_file(r.content, flux_operator_yaml)
+        utils.write_file(r.text, flux_operator_yaml)
 
     # Ensure it really really exists
     flux_operator_yaml = os.path.abspath(flux_operator_yaml)
     if not os.path.exists(flux_operator_yaml):
         raise ValueError(f"{flux_operator_yaml} does not exist.")
     return flux_operator_yaml
```

### Comparing `flux-burst-0.0.11/fluxburst/kubernetes/plugins.py` & `flux-burst-0.0.12/fluxburst/kubernetes/plugins.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 
 
 class KubernetesBurstPlugin(BurstPlugin):
     """
     An additional wrapper to the plugin that adds support for the Flux Operator
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.clusters = {}
-
     def ensure_namespace(self, kubectl):
         """
         Use the instantiated kubectl to ensure the cluster namespace exists.
         """
         try:
             kubectl.create_namespace(
                 kubernetes_client.V1Namespace(
@@ -37,14 +33,46 @@
                 )
             )
         except Exception:
             logger.warning(
                 f"🥵️ Issue creating namespace {self.params.namespace}, assuming already exists."
             )
 
+    def validate(self):
+        """
+        Validate ensures that required conditions are met.
+
+        This should return True/False to indicate if the plugin is valid or not.
+        """
+        # If we aren't doing an isolated burst, we require host names, configs, etc.
+        if not self.params.isolated_burst:
+            # Lead host and port are required. A custom broker.toml can be provided,
+            # but we are having the operator create it for us
+            if (
+                not self.params.lead_port
+                or not self.params.lead_host
+                or not self.params.lead_size
+            ):
+                logger.warning(
+                    "Parameteres lead_host, lead_size, and lead_port must be defined when not doing an isolated_burst."
+                )
+                return False
+
+            print(
+                f"Broker lead will be accessible on {self.params.lead_host}:{self.params.lead_port}"
+            )
+
+            # We also need to have the munge key and curve cert
+            if self.params.munge_key and not os.path.exists(self.params.munge_key):
+                logger.warning(
+                    f"Provided munge key {self.params.munge_key} does not exist."
+                )
+                return False
+        return True
+
     def check_configs(self):
         """
         Ensure we have required config files.
         """
         message = "does not exist or you don't have permissions to see it"
         if not os.path.exists(self.params.munge_key):
             raise ValueError(f"Provided munge key {self.params.munge_key} {message}.")
@@ -60,46 +88,68 @@
             k8sutils.create_from_yaml(kubectl.api_client, flux_operator_yaml)
             logger.info("Installed the operator.")
         except Exception as exc:
             logger.warning(
                 f"Issue installing the operator: {exc}, assuming already exists"
             )
 
-    def run(self):
+    def run(self, request_burst=False, nodes=None, tasks=None):
         """
         Given some set of scheduled jobs, run bursting.
+
+        If request_burst is True, a specific number of tasks and size
+        must be provided to request a cluster in advance (that jobs can
+        be run on).
         """
         # Exit early if no jobs to burst
         if not self.jobs:
             logger.info(f"Plugin {self.name} has no jobs to burst.")
             return
 
+        # If we have requested a burst, tasks and size are required
+        if request_burst and (not tasks or not nodes):
+            logger.warning("Burst requests require nodes and tasks.")
+            return
+
         # Ensure we have a flux operator yaml file, fosho, foyaml!
         foyaml = helpers.ensure_flux_operator_yaml(self.params.flux_operator_yaml)
 
         # lead host / port / size / are required in the dataclass
+        # But ONLY if this isnt' an isolated burst!
         # We check munge paths here, because could be permissions issue
-        self.check_configs()
+        if not self.params.isolated_burst:
+            self.check_configs()
 
+        # This call registers the name of the cluster to self.clusters
         cli = self.create_cluster()
         kubectl = cli.get_k8s_client()
 
         # Install the operator!
         self.install_flux_operator(kubectl, foyaml)
 
+        # Are we requesting or running jobs?
+        if request_burst:
+            self.create_minicluster(kubectl, "sleep infinity", nodes, tasks)
+        else:
+            self.run_jobs(kubectl)
+
+    def run_jobs(self, kubectl):
+        """
+        Run jobs (creating MiniClusters), assuming that the burst has been done.
+        """
         # Create a MiniCluster for each job
         for _, job in self.jobs.items():
-            self.create_minicluster(kubectl, job)
+            command = " ".join(job["spec"]["tasks"][0]["command"])
+            self.create_minicluster(kubectl, command, job["nnodes"], job["ntasks"])
 
-    def create_minicluster(self, kubectl, job):
+    def create_minicluster(self, kubectl, command, nodes, tasks):
         """
         Create the MiniCluster
         """
-        command = " ".join(job["spec"]["tasks"][0]["command"])
-        logger.info(f"Preparing MiniCluster for {job['id']}: {command}")
+        logger.info(f"Preparing MiniCluster for {command}")
 
         # The plugin is assumed to be running from the lead broker
         # of the cluster it is bursting from, this we get info about it
         podname = socket.gethostname()
         hostname = podname.rsplit("-", 1)[0]
 
         # TODO: we are using defaults for now, but will update this to be likely
@@ -107,16 +157,16 @@
         minicluster, container = helpers.get_minicluster(
             command,
             name=self.params.name,
             memory_limit=self.params.memory_limit,
             cpu_limit=self.params.cpu_limit,
             namespace=self.params.namespace,
             broker_toml=self.params.broker_toml,
-            tasks=job["ntasks"],
-            size=job["nnodes"],
+            tasks=tasks,
+            size=nodes,
             image=self.params.image,
             wrap=self.params.wrap,
             log_level=self.params.log_level,
             flux_user=self.params.flux_user,
             lead_host=self.params.lead_host,
             lead_port=self.params.lead_port,
             munge_secret_name=self.params.munge_secret_name,
@@ -126,24 +176,30 @@
         )
         # Create the namespace
         self.ensure_namespace(kubectl)
 
         # Let's assume there could be bugs applying this differently
         crd_api = kubernetes_client.CustomObjectsApi(kubectl.api_client)
 
-        self.ensure_secrets(kubectl)
+        # These are not needed if we are doing an isolated burst
+        if not self.params.isolated_burst:
+            self.ensure_secrets(kubectl)
 
         # Create the MiniCluster! This also waits for it to be ready
         print(
             f"⭐️ Creating the minicluster {self.params.name} in {self.params.namespace}..."
         )
 
         # Make sure we provide the core_v1_api we've created
         operator = FluxMiniCluster(core_v1_api=kubectl)
-        return operator.create(**minicluster, container=container, crd_api=crd_api)
+        try:
+            return operator.create(**minicluster, container=container, crd_api=crd_api)
+        except Exception as e:
+            print(f"Issue creating cluster, does it already exist?: {e}")
+            return True
 
     def ensure_secrets(self, kubectl):
         """
         Ensure secrets (munge.key and curve.cert) are ready for a job
         """
         secrets = []
```

### Comparing `flux-burst-0.0.11/fluxburst/logger.py` & `flux-burst-0.0.12/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/plugins.py` & `flux-burst-0.0.12/fluxburst/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/utils/__init__.py` & `flux-burst-0.0.12/fluxburst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/utils/fileio.py` & `flux-burst-0.0.12/fluxburst/utils/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     if os.path.exists(destination) and force is True:
         os.remove(destination)
 
     shutil.copyfile(source, destination)
     return destination
 
 
-def write_file(filename, content, mode="w", exec=False):
+def write_file(content, filename, mode="w", exec=False):
     """
     Write content to a filename
     """
     with open(filename, mode) as filey:
         filey.writelines(content)
     if exec:
         st = os.stat(filename)
```

### Comparing `flux-burst-0.0.11/fluxburst/utils/misc.py` & `flux-burst-0.0.12/fluxburst/utils/misc.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/utils/terminal.py` & `flux-burst-0.0.12/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.11/fluxburst/version.py` & `flux-burst-0.0.12/fluxburst/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.11"
+__version__ = "0.0.12"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-0.0.11/setup.py` & `flux-burst-0.0.12/setup.py`

 * *Files identical despite different names*

