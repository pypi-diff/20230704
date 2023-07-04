# Comparing `tmp/flux-burst-eks-0.0.0.tar.gz` & `tmp/flux-burst-eks-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-eks-0.0.0.tar", last modified: Sat Jul  1 06:50:00 2023, max compression
+gzip compressed data, was "flux-burst-eks-0.0.1.tar", last modified: Tue Jul  4 01:33:45 2023, max compression
```

## Comparing `flux-burst-eks-0.0.0.tar` & `flux-burst-eks-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:50:00.728804 flux-burst-eks-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.0/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.0/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-29 20:12:24.000000 flux-burst-eks-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1836 2023-07-01 06:50:00.728804 flux-burst-eks-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1018 2023-07-01 06:49:32.000000 flux-burst-eks-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:50:00.728804 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1836 2023-07-01 06:50:00.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2023-07-01 06:50:00.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 06:50:00.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 06:49:36.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-07-01 06:50:00.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-07-01 06:50:00.000000 flux-burst-eks-0.0.0/flux_burst_eks.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:50:00.728804 flux-burst-eks-0.0.0/fluxburst_eks/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-29 20:30:18.000000 flux-burst-eks-0.0.0/fluxburst_eks/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5874 2023-07-01 06:49:32.000000 flux-burst-eks-0.0.0/fluxburst_eks/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1130 2023-06-29 20:28:21.000000 flux-burst-eks-0.0.0/fluxburst_eks/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-07-01 06:50:00.728804 flux-burst-eks-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-29 20:12:24.000000 flux-burst-eks-0.0.0/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:33:45.142119 flux-burst-eks-0.0.1/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.1/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.1/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-29 20:12:24.000000 flux-burst-eks-0.0.1/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.1/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1836 2023-07-04 01:33:45.142119 flux-burst-eks-0.0.1/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1018 2023-07-01 06:49:32.000000 flux-burst-eks-0.0.1/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:33:45.142119 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1836 2023-07-04 01:33:45.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2023-07-04 01:33:45.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-04 01:33:45.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 06:49:36.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-07-04 01:33:45.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-07-04 01:33:45.000000 flux-burst-eks-0.0.1/flux_burst_eks.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:33:45.142119 flux-burst-eks-0.0.1/fluxburst_eks/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-29 20:30:18.000000 flux-burst-eks-0.0.1/fluxburst_eks/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6518 2023-07-04 01:33:38.000000 flux-burst-eks-0.0.1/fluxburst_eks/plugin.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1130 2023-07-04 01:33:38.000000 flux-burst-eks-0.0.1/fluxburst_eks/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-29 20:09:52.000000 flux-burst-eks-0.0.1/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-07-04 01:33:45.142119 flux-burst-eks-0.0.1/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-29 20:12:24.000000 flux-burst-eks-0.0.1/setup.py
```

### Comparing `flux-burst-eks-0.0.0/LICENSE` & `flux-burst-eks-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-eks-0.0.0/NOTICE` & `flux-burst-eks-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-eks-0.0.0/PKG-INFO` & `flux-burst-eks-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-eks
-Version: 0.0.0
+Version: 0.0.1
 Summary: A bursting plugin for Flux and EKS
 Home-page: https://github.com/converged-computing/flux-burst-eks
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-eks-0.0.0/README.md` & `flux-burst-eks-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-eks-0.0.0/flux_burst_eks.egg-info/PKG-INFO` & `flux-burst-eks-0.0.1/flux_burst_eks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-eks
-Version: 0.0.0
+Version: 0.0.1
 Summary: A bursting plugin for Flux and EKS
 Home-page: https://github.com/converged-computing/flux-burst-eks
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-eks-0.0.0/fluxburst_eks/__init__.py` & `flux-burst-eks-0.0.1/fluxburst_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-eks-0.0.0/fluxburst_eks/plugin.py` & `flux-burst-eks-0.0.1/fluxburst_eks/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,28 +19,32 @@
     """
     Custom parameters for Flux Operator bursting.
 
     It should be possible to read this in from yaml, or the
     environment (or both).
     """
 
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
 
     # Require credentials from the environment
-    creds_from_environ: Optional[bool] = False
+    # This default to true because (I think) it's more common
+    creds_from_environ: Optional[bool] = True
 
     # Name of a secret to be made in the same namespace
     munge_secret_name: Optional[str] = "munge-key"
 
     # Path to munge.key file (local) to use to create config map
     # If this is owned by root, likely won't be readable
     munge_key: Optional[str] = "/etc/munge/munge.key"
@@ -78,28 +82,38 @@
     wrap: Optional[str] = None
 
 
 class FluxBurstEKS(bases.KubernetesBurstPlugin):
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
         # We cannot run any jobs without credentials
         if self.params.creds_from_environ and not self.check_creds():
             logger.warning(
                 "AWS credentials not found in environment, cannot schedule to EKS."
             )
             return False
 
+        # Shared validation functions from kubernetes
+        return super(FluxBurstEKS, self).validate()
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
@@ -120,19 +134,22 @@
                 )
                 return False
         return True
 
     def cleanup(self, name=None):
         """
         Cleanup (delete) one or more clusters
+
+        We are lenient in case that a cluster was created before, and
+        there isn't a record in self.clusters.
         """
         if name and name not in self.clusters:
-            raise ValueError(f"{name} is not a known cluster.")
-        clusters = self.clusters if not name else {"name": self.clusters["name"]}
-        for cluster_name, _ in clusters.items():
+            logger.warning(f"{name} is not a known cluster.")
+        clusters = list(self.clusters) if not name else [name]
+        for cluster_name in clusters:
             logger.info(f"Cleaning up {cluster_name}")
             cli = EKSCluster(name=cluster_name)
             cli.delete_cluster()
 
         # Update known clusters
         updated = {}
         for name in self.clusters:
@@ -164,14 +181,14 @@
             max_nodes=max_size,
         )
 
         # Create the cluster (this times it)
         try:
             self.clusters[cluster_name] = cli.create_cluster()
         # We still need to register the cluster exists
-        except Exception:
+        except Exception as exc:
             self.clusters[cluster_name] = True
-            print("🥵️ Issue creating cluster, assuming already exists.")
+            print(f"🥵️ Issue creating cluster, already exists?: {exc}")
 
         # Create a client from it
         logger.info(f"📦️ The cluster has {cli.node_count} nodes!")
         return cli
```

### Comparing `flux-burst-eks-0.0.0/fluxburst_eks/version.py` & `flux-burst-eks-0.0.1/fluxburst_eks/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-eks"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-eks"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and EKS"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-eks-0.0.0/setup.py` & `flux-burst-eks-0.0.1/setup.py`

 * *Files identical despite different names*

