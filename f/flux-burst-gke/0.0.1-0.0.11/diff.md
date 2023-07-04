# Comparing `tmp/flux-burst-gke-0.0.1.tar.gz` & `tmp/flux-burst-gke-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-gke-0.0.1.tar", last modified: Sat Jul  1 07:04:00 2023, max compression
+gzip compressed data, was "flux-burst-gke-0.0.11.tar", last modified: Tue Jul  4 01:34:41 2023, max compression
```

## Comparing `flux-burst-gke-0.0.1.tar` & `flux-burst-gke-0.0.11.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-24 19:35:42.000000 flux-burst-gke-0.0.1/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-24 19:35:39.000000 flux-burst-gke-0.0.1/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-23 23:45:36.000000 flux-burst-gke-0.0.1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-24 19:35:45.000000 flux-burst-gke-0.0.1/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1837 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1019 2023-07-01 07:03:06.000000 flux-burst-gke-0.0.1/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1837 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/fluxburst_gke/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-25 03:11:54.000000 flux-burst-gke-0.0.1/fluxburst_gke/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5590 2023-07-01 07:03:06.000000 flux-burst-gke-0.0.1/fluxburst_gke/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1130 2023-07-01 07:03:34.000000 flux-burst-gke-0.0.1/fluxburst_gke/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 23:28:22.000000 flux-burst-gke-0.0.1/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-24 19:36:42.000000 flux-burst-gke-0.0.1/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:34:41.339541 flux-burst-gke-0.0.11/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-24 19:35:42.000000 flux-burst-gke-0.0.11/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-24 19:35:39.000000 flux-burst-gke-0.0.11/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-23 23:45:36.000000 flux-burst-gke-0.0.11/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-24 19:35:45.000000 flux-burst-gke-0.0.11/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-07-04 01:34:41.339541 flux-burst-gke-0.0.11/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1156 2023-07-04 01:34:38.000000 flux-burst-gke-0.0.11/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:34:41.339541 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-07-04 01:34:41.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2023-07-04 01:34:41.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-04 01:34:41.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-07-04 01:34:41.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-07-04 01:34:41.000000 flux-burst-gke-0.0.11/flux_burst_gke.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:34:41.339541 flux-burst-gke-0.0.11/fluxburst_gke/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-25 03:11:54.000000 flux-burst-gke-0.0.11/fluxburst_gke/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6165 2023-07-04 01:34:38.000000 flux-burst-gke-0.0.11/fluxburst_gke/plugin.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1131 2023-07-04 01:34:38.000000 flux-burst-gke-0.0.11/fluxburst_gke/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 23:28:22.000000 flux-burst-gke-0.0.11/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-07-04 01:34:41.339541 flux-burst-gke-0.0.11/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-24 19:36:42.000000 flux-burst-gke-0.0.11/setup.py
```

### Comparing `flux-burst-gke-0.0.1/LICENSE` & `flux-burst-gke-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.1/NOTICE` & `flux-burst-gke-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.1/PKG-INFO` & `flux-burst-gke-0.0.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-gke
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and GKE
 Home-page: https://github.com/converged-computing/flux-burst-gke
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
@@ -26,14 +26,15 @@
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
 Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
 
 ![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
 
+For a mock example (a burst without a local cluster, but just to test the ability to create the bursted cluster) see [example](example).
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.1/README.md` & `flux-burst-gke-0.0.11/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
 Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
 
 ![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
 
+For a mock example (a burst without a local cluster, but just to test the ability to create the bursted cluster) see [example](example).
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.1/flux_burst_gke.egg-info/PKG-INFO` & `flux-burst-gke-0.0.11/flux_burst_gke.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-gke
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and GKE
 Home-page: https://github.com/converged-computing/flux-burst-gke
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
@@ -26,14 +26,15 @@
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
 Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
 
 ![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
 
+For a mock example (a burst without a local cluster, but just to test the ability to create the bursted cluster) see [example](example).
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.1/fluxburst_gke/__init__.py` & `flux-burst-gke-0.0.11/fluxburst_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.1/fluxburst_gke/plugin.py` & `flux-burst-gke-0.0.11/fluxburst_gke/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,22 +22,25 @@
     It should be possible to read this in from yaml, or the
     environment (or both).
     """
 
     # Google Cloud Project
     project: str
 
+    # An isolated burst brings up an independent cluster
+    isolated_burst: Optional[bool] = False
+
     # Lead broker service hostname or ip address
-    lead_host: str
+    lead_host: Optional[str] = None
 
     # Lead broker service port (e.g, 30093)
-    lead_port: str
+    lead_port: Optional[str] = None
 
     # Lead broker size
-    lead_size: int
+    lead_size: Optional[str] = None
 
     # Custom broker toml template for bursted cluster
     broker_toml: Optional[str] = None
 
     # Name of a secret to be made in the same namespace
     munge_secret_name: Optional[str] = "munge-key"
 
@@ -78,28 +81,38 @@
     wrap: Optional[str] = None
 
 
 class FluxBurstGKE(bases.KubernetesBurstPlugin):
     # Set our custom dataclass, otherwise empty
     _param_dataclass = BurstParameters
 
-    def schedule(self, job):
+    def validate(self):
         """
-        Given a burstable job, determine if we can schedule it.
+        Validate ensures that required conditions are met.
 
-        This function should also consider logic for deciding if/when to
-        assign clusters, but run should actually create/destroy.
+        This should return True/False to indicate if valid or not, and
+        print meaninging error messages for the user
         """
         # We cannot run any jobs without Google Application Credentials
         if "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ:
             logger.warning(
                 "GOOGLE_APPLICATION_CREDENTIALS not found in environment, cannot schedule to GKE."
             )
             return False
 
+        # Shared validation functions from kubernetes
+        return super(FluxBurstGKE, self).validate()
+
+    def schedule(self, job):
+        """
+        Given a burstable job, determine if we can schedule it.
+
+        This function should also consider logic for deciding if/when to
+        assign clusters, but run should actually create/destroy.
+        """
         # TODO determine if we can match some resource spec to another,
         # We likely want this class to be able to generate a lookup of
         # instances / spec about them.
 
         # For now, we just accept anything, and add to our jobs and return true
         if job["id"] in self.jobs:
             logger.debug(f"{job['id']} is already scheduled")
@@ -110,23 +123,26 @@
         return True
 
     def cleanup(self, name=None):
         """
         Cleanup (delete) one or more clusters
         """
         if name and name not in self.clusters:
-            raise ValueError(f"{name} is not a known cluster.")
-        clusters = self.clusters if not name else {"name": self.clusters["name"]}
-        for cluster_name, _ in clusters.items():
+            logger.warning(f"{name} is not a known cluster.")
+        clusters = list(self.clusters) if not name else [name]
+        for cluster_name in clusters:
             logger.info(f"Cleaning up {cluster_name}")
             cli = GKECluster(
                 project=self.params.project,
                 name=cluster_name,
             )
-            cli.delete_cluster()
+            try:
+                cli.delete_cluster()
+            except Exception:
+                logger.warning(f"Issue deleting {cluster_name}")
 
         # Update known clusters
         updated = {}
         for name in self.clusters:
             if name not in clusters:
                 updated[name] = self.clusters[name]
         self.clusters = updated
```

### Comparing `flux-burst-gke-0.0.1/fluxburst_gke/version.py` & `flux-burst-gke-0.0.11/fluxburst_gke/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.1"
+__version__ = "0.0.11"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-gke"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-gke"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and GKE"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-gke-0.0.1/setup.py` & `flux-burst-gke-0.0.11/setup.py`

 * *Files identical despite different names*

