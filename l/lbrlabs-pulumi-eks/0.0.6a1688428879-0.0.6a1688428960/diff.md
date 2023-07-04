# Comparing `tmp/lbrlabs_pulumi_eks-0.0.6a1688428879.tar.gz` & `tmp/lbrlabs_pulumi_eks-0.0.6a1688428960.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_eks-0.0.6a1688428879.tar", last modified: Tue Jul  4 00:08:17 2023, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_eks-0.0.6a1688428960.tar", last modified: Tue Jul  4 00:09:54 2023, max compression
```

## Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879.tar` & `lbrlabs_pulumi_eks-0.0.6a1688428960.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/attached_node_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/iam_role_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/iam_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:08:17.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-04 00:08:16.000000 lbrlabs_pulumi_eks-0.0.6a1688428879/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/attached_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/iam_role_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/iam_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:09:54.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-04 00:09:53.000000 lbrlabs_pulumi_eks-0.0.6a1688428960/setup.py
```

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/PKG-INFO` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs_pulumi_eks
-Version: 0.0.6a1688428879
+Name: lbrlabs-pulumi-eks
+Version: 0.0.6a1688428960
 Summary: A batteries included EKS cluster following best practices.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-lbrlabs-eks
 Description: # Pulumi LBr Labs EKS 
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a "batteries included" cluster ready for you to attach your EKS nodes to.
```

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/README.md` & `lbrlabs_pulumi_eks-0.0.6a1688428960/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/__init__.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/_utilities.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/attached_node_group.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/attached_node_group.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/cluster.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/iam_role_mapping.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/iam_role_mapping.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/iam_service_account_role.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/iam_service_account_role.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks/provider.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/PKG-INFO` & `lbrlabs_pulumi_eks-0.0.6a1688428960/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lbrlabs-pulumi-eks
-Version: 0.0.6a1688428879
+Name: lbrlabs_pulumi_eks
+Version: 0.0.6a1688428960
 Summary: A batteries included EKS cluster following best practices.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-lbrlabs-eks
 Description: # Pulumi LBr Labs EKS 
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a "batteries included" cluster ready for you to attach your EKS nodes to.
```

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/lbrlabs_pulumi_eks.egg-info/SOURCES.txt` & `lbrlabs_pulumi_eks-0.0.6a1688428960/lbrlabs_pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.0.6a1688428879/setup.py` & `lbrlabs_pulumi_eks-0.0.6a1688428960/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.6a1688428879"
-PLUGIN_VERSION = "0.0.6-alpha.1688428879+b8903b53"
+VERSION = "0.0.6a1688428960"
+PLUGIN_VERSION = "0.0.6-alpha.1688428960+c8d1cfc8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'lbrlabs-eks', PLUGIN_VERSION, '--server', 'github://api.github.com/lbrlabs'])
         except OSError as error:
```

