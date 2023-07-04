# Comparing `tmp/kubescaler-0.0.13.tar.gz` & `tmp/kubescaler-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubescaler-0.0.13.tar", last modified: Sat Jul  1 07:06:24 2023, max compression
+gzip compressed data, was "kubescaler-0.0.14.tar", last modified: Tue Jul  4 01:31:26 2023, max compression
```

## Comparing `kubescaler-0.0.13.tar` & `kubescaler-0.0.14.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.13/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.13/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.13/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.13/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-01 07:06:24.801142 kubescaler-0.0.13/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.13/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.797141 kubescaler-0.0.13/kubescaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/decorators.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6104 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/scaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:18.000000 kubescaler-0.0.13/kubescaler/scaler/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/scaler/aws/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/ami.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    24799 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/scaler/aws/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/scaler/aws/template.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1321 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/scaler/aws/token.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.13/kubescaler/scaler/google.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.13/kubescaler/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.13/kubescaler/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-07-01 07:06:21.000000 kubescaler-0.0.13/kubescaler/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:06:24.801142 kubescaler-0.0.13/kubescaler.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      747 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.13/kubescaler.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      230 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-07-01 07:06:24.000000 kubescaler-0.0.13/kubescaler.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.13/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-07-01 07:06:24.801142 kubescaler-0.0.13/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3584 2023-06-25 05:02:18.000000 kubescaler-0.0.13/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.150070 kubescaler-0.0.14/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.14/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.14/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.14/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.14/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-04 01:31:26.150070 kubescaler-0.0.14/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.14/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.146069 kubescaler-0.0.14/kubescaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/decorators.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6104 2023-07-01 07:06:21.000000 kubescaler-0.0.14/kubescaler/logger.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.150070 kubescaler-0.0.14/kubescaler/scaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:18.000000 kubescaler-0.0.14/kubescaler/scaler/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.150070 kubescaler-0.0.14/kubescaler/scaler/aws/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/scaler/aws/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/scaler/aws/ami.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    24678 2023-07-04 01:31:22.000000 kubescaler-0.0.14/kubescaler/scaler/aws/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/scaler/aws/template.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1321 2023-07-01 07:06:21.000000 kubescaler-0.0.14/kubescaler/scaler/aws/token.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.14/kubescaler/scaler/google.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.150070 kubescaler-0.0.14/kubescaler/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.14/kubescaler/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.14/kubescaler/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-07-04 01:31:22.000000 kubescaler-0.0.14/kubescaler/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:31:26.150070 kubescaler-0.0.14/kubescaler.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-07-04 01:31:25.000000 kubescaler-0.0.14/kubescaler.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      747 2023-07-04 01:31:26.000000 kubescaler-0.0.14/kubescaler.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-04 01:31:25.000000 kubescaler-0.0.14/kubescaler.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.14/kubescaler.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      230 2023-07-04 01:31:25.000000 kubescaler-0.0.14/kubescaler.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-07-04 01:31:25.000000 kubescaler-0.0.14/kubescaler.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.14/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-07-04 01:31:26.150070 kubescaler-0.0.14/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3584 2023-06-25 05:02:18.000000 kubescaler-0.0.14/setup.py
```

### Comparing `kubescaler-0.0.13/LICENSE` & `kubescaler-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/NOTICE` & `kubescaler-0.0.14/NOTICE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/PKG-INFO` & `kubescaler-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.13
+Version: 0.0.14
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.13 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.14 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `kubescaler-0.0.13/README.md` & `kubescaler-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/cluster.py` & `kubescaler-0.0.14/kubescaler/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/decorators.py` & `kubescaler-0.0.14/kubescaler/decorators.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/defaults.py` & `kubescaler-0.0.14/kubescaler/defaults.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/logger.py` & `kubescaler-0.0.14/kubescaler/logger.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/scaler/aws/ami.py` & `kubescaler-0.0.14/kubescaler/scaler/aws/ami.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/scaler/aws/cluster.py` & `kubescaler-0.0.14/kubescaler/scaler/aws/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 try:
     import boto3
 except ImportError:
     sys.exit("Please pip install kubescaler[aws]")
 
 from kubernetes import client as k8s
-from kubernetes import config
 from kubernetes import utils as k8sutils
 
 import kubescaler.utils as utils
 from kubescaler.cluster import Cluster
 from kubescaler.decorators import retry, timed
 from kubescaler.logger import logger
 
@@ -71,15 +70,15 @@
 
         # Here we define cluster name from name
         self.cluster_name = self.name
         self.tags = self.tags or {}
         if not isinstance(self.tags, dict):
             raise ValueError("Tags must be key value pairs (dict)")
 
-        # kube config file
+        # kube config file (this is no longer used)
         self.kube_config_file = kube_config_file or "kubeconfig-aws.yaml"
         self.image_ami = get_latest_ami(self.region, self.kubernetes_version)
         self.machine_type = self.machine_type or "m5.large"
         self.configuration = None
         self._kubectl = None
 
         # Client connections
@@ -239,24 +238,20 @@
 
         After this, kubectl --kubeconfig=./kubeconfig.yaml get nodes
         will (or I should say "should") work!
         """
         # Easier to write to file and then apply!
         auth_config = auth_config_data % self.node_instance_role
         utils.write_file(auth_config, self.auth_config_file)
+        kubectl = self.get_k8s_client()
 
-        # We can likely do it this way in the future (will open issue)
-        config.load_kube_config(self.kube_config_file)
-        koobcli = k8s.ApiClient()
-
-        # If the cluster was already created, this would raise an error
         try:
-            k8sutils.create_from_yaml(koobcli, self.auth_config_file)
-        except Exception:
-            pass
+            k8sutils.create_from_yaml(kubectl.api_client, self.auth_config_file)
+        except Exception as e:
+            print(f"😭️ Kubectl create from yaml returns in error: {e}")
 
     def ensure_kube_config(self):
         """
         Ensure the kubernetes kubectl config file exists
 
         Since this might change, let's always just write it again.
         We require the user to install awscli so the aws executable
@@ -607,15 +602,15 @@
         logger.info("⏳️ Cluster deletion started! Waiting...")
         waiter = self.eks.get_waiter("cluster_deleted")
         waiter.wait(name=self.cluster_name)
 
         # Delete the VPC stack and we are done!
         logger.info("🥅️ Deleting VPC and associated assets...")
         self.delete_vpc_stack()
-        self.delete_worker_stack()
+        self.delete_workers_stack()
         logger.info("⭐️ Done!")
 
     @property
     def data(self):
         """
         Combine class data into json object to save
         """
```

### Comparing `kubescaler-0.0.13/kubescaler/scaler/aws/template.py` & `kubescaler-0.0.14/kubescaler/scaler/aws/template.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/scaler/aws/token.py` & `kubescaler-0.0.14/kubescaler/scaler/aws/token.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/scaler/google.py` & `kubescaler-0.0.14/kubescaler/scaler/google.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/utils/fileio.py` & `kubescaler-0.0.14/kubescaler/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/utils/misc.py` & `kubescaler-0.0.14/kubescaler/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/utils/terminal.py` & `kubescaler-0.0.14/kubescaler/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/kubescaler/version.py` & `kubescaler-0.0.14/kubescaler/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.13"
+__version__ = "0.0.14"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "kubescaler"
 PACKAGE_URL = "https://github.com/converged-computing/kubescaler"
 KEYWORDS = "Kubernetes, elasticity, scaling, EKS, GKE"
 DESCRIPTION = "Helper classes for scaling Kubernetes clusters"
 LICENSE = "LICENSE"
```

### Comparing `kubescaler-0.0.13/kubescaler.egg-info/PKG-INFO` & `kubescaler-0.0.14/kubescaler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.13
+Version: 0.0.14
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.13 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.14 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `kubescaler-0.0.13/kubescaler.egg-info/SOURCES.txt` & `kubescaler-0.0.14/kubescaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.13/setup.py` & `kubescaler-0.0.14/setup.py`

 * *Files identical despite different names*

