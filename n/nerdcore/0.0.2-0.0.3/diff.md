# Comparing `tmp/nerdcore-0.0.2.tar.gz` & `tmp/nerdcore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.0.2.tar", last modified: Mon Jul  3 21:24:17 2023, max compression
+gzip compressed data, was "nerdcore-0.0.3.tar", last modified: Mon Jul  3 21:55:00 2023, max compression
```

## Comparing `nerdcore-0.0.2.tar` & `nerdcore-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:24:17.730085 nerdcore-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 21:23:59.000000 nerdcore-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2905 2023-07-03 21:23:59.000000 nerdcore-0.0.2/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3586 2023-07-03 21:23:59.000000 nerdcore-0.0.2/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 21:24:17.730085 nerdcore-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 21:23:59.000000 nerdcore-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:55:00.005357 nerdcore-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:55:00.005357 nerdcore-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 21:54:40.000000 nerdcore-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:55:00.001357 nerdcore-0.0.3/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:54:59.000000 nerdcore-0.0.3/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:55:00.001357 nerdcore-0.0.3/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 21:54:40.000000 nerdcore-0.0.3/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 21:54:40.000000 nerdcore-0.0.3/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 21:55:00.005357 nerdcore-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 21:54:40.000000 nerdcore-0.0.3/setup.py
```

### Comparing `nerdcore-0.0.2/PKG-INFO` & `nerdcore-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.2/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.0.3/nerdcore.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.2/scripts/nerd` & `nerdcore-0.0.3/scripts/nerd`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nerdcore.utils.env.update_env_class import update_env_class
 from nerdcore.utils.nerd.find_entity import find_entity
 from nerdcore.utils.nerd.generate_nerd_configs import generate_nerd_configs
 from nerdcore.utils.nerd.parse_nerd_args import parse_nerd_args
 from nerdcore.utils.nerd.run_entities import run_deployment, run_command
 from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.utils.nerd_config.update_nerd_config_class import update_nerd_config_class
-from ..defs import nl, PYTHON_COMMAND
+from nerdcore.defs import nl, PYTHON_COMMAND
 
 
 # Some basic environment checks
 nerd_env_checks()
 
 # Regenerate "magic" config/env stuff
 update_env_class()
```

### Comparing `nerdcore-0.0.2/scripts/nerd-new` & `nerdcore-0.0.3/scripts/nerd-new`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 import os
 import shutil
 import sys
 
 from termcolor import colored
 
-from ..ncdefs import (NC_ENV_DEFAULT_PATH, NC_NERD_MANIFEST_DEFAULT_PATH, NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH,
-                      NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH, NC_DEFAULT_DEPLOYMENT_PATH,
-                      NC_GITIGNORE_DEFAULT_PATH, NC_README_DEFAULT_PATH, NC_CONTEXT_FILE_EXAMPLE_PATH)
+from nerdcore.ncdefs import (NC_ENV_DEFAULT_PATH, NC_NERD_MANIFEST_DEFAULT_PATH, NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH,
+                             NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH, NC_DEFAULT_DEPLOYMENT_PATH,
+                             NC_GITIGNORE_DEFAULT_PATH, NC_README_DEFAULT_PATH, NC_CONTEXT_FILE_EXAMPLE_PATH)
 
 top_level_dirs = [
     'abilities',
     'deployments',
     'commands',
     'config',
     'tasks',
```

### Comparing `nerdcore-0.0.2/setup.py` & `nerdcore-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.0.2',
+    version='0.0.3',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

