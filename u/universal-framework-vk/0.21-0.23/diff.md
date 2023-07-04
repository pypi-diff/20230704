# Comparing `tmp/universal_framework_vk-0.21.tar.gz` & `tmp/universal_framework_vk-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_framework_vk-0.21.tar", last modified: Tue Jul  4 04:04:20 2023, max compression
+gzip compressed data, was "universal_framework_vk-0.23.tar", last modified: Tue Jul  4 04:23:53 2023, max compression
```

## Comparing `universal_framework_vk-0.21.tar` & `universal_framework_vk-0.23.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/universal_framework_vk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 04:23:42.000000 universal_framework_vk-0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:23:53.736681 universal_framework_vk-0.23/universal_framework_vk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:23:53.000000 universal_framework_vk-0.23/universal_framework_vk.egg-info/top_level.txt
```

### Comparing `universal_framework_vk-0.21/setup.py` & `universal_framework_vk-0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='universal_framework_vk',
-    version='0.21',
+    version='0.23',
     packages=find_packages(),
     description='universal framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Viral Killer',
     author_email='jules3313@gmail.com',
     license='MIT',
```

