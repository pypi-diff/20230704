# Comparing `tmp/universal_framework_vk-0.23.tar.gz` & `tmp/universal_framework_vk-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_framework_vk-0.23.tar", last modified: Tue Jul  4 04:23:53 2023, max compression
+gzip compressed data, was "universal_framework_vk-0.3.tar", last modified: Tue Jul  4 04:29:06 2023, max compression
```

## Comparing `universal_framework_vk-0.23.tar` & `universal_framework_vk-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/universal_framework_vk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:06.402218 universal_framework_vk-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 04:28:56.000000 universal_framework_vk-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 04:29:06.402218 universal_framework_vk-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:28:56.000000 universal_framework_vk-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:29:06.402218 universal_framework_vk-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-04 04:28:56.000000 universal_framework_vk-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:29:06.402218 universal_framework_vk-0.3/universal_framework_vk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 04:29:06.000000 universal_framework_vk-0.3/universal_framework_vk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 04:29:06.000000 universal_framework_vk-0.3/universal_framework_vk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:29:06.000000 universal_framework_vk-0.3/universal_framework_vk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:29:06.000000 universal_framework_vk-0.3/universal_framework_vk.egg-info/top_level.txt
```

### Comparing `universal_framework_vk-0.23/setup.py` & `universal_framework_vk-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='universal_framework_vk',
-    version='0.23',
+    version='0.3',
     packages=find_packages(),
     description='universal framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Viral Killer',
     author_email='jules3313@gmail.com',
     license='MIT',
+    python_requires='>=3.10.0',
     install_requires=[
         # List of your package dependencies
         # For example: 'numpy>=1.18.1'
     ],
 )
```

