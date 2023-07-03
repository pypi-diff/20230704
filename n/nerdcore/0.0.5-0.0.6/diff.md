# Comparing `tmp/nerdcore-0.0.5.tar.gz` & `tmp/nerdcore-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.0.5.tar", last modified: Mon Jul  3 22:14:53 2023, max compression
+gzip compressed data, was "nerdcore-0.0.6.tar", last modified: Mon Jul  3 22:23:43 2023, max compression
```

## Comparing `nerdcore-0.0.5.tar` & `nerdcore-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:14:53.089931 nerdcore-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:14:35.000000 nerdcore-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/nerdcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/defs.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-03 22:14:35.000000 nerdcore-0.0.5/nerdcore/ncdefs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 22:14:53.000000 nerdcore-0.0.5/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:14:53.089931 nerdcore-0.0.5/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 22:14:35.000000 nerdcore-0.0.5/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 22:14:35.000000 nerdcore-0.0.5/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:14:53.089931 nerdcore-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 22:14:35.000000 nerdcore-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:23:43.819666 nerdcore-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:23:27.000000 nerdcore-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/abilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/abilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/abilities/gpt_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/base_entitiies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/base_entitiies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/base_entitiies/command_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/base_entitiies/deployment_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/base_entitiies/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/base_entitiies/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/base_entitiies/utils/cli_runnable_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/make.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/toggle-light-mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/commands/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/config/env_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/config/nerd_config_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/config/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/config/yaml_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/defs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/help/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/help/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/help/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/help/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/ncdefs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/utils/env/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/env/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/env/environment_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/env/get_env_prop_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/env/update_env_class.py
+-rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/ncdefs_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/utils/nerd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/find_entity.py
+-rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/generate_nerd_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/get_config_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/parse_nerd_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/run_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     6970 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd/theme_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/nerdcore/utils/nerd_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd_config/load_nerd_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd_config/nerd_config_validations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-03 22:23:27.000000 nerdcore-0.0.6/nerdcore/utils/nerd_config/update_nerd_config_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.815666 nerdcore-0.0.6/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 22:23:43.000000 nerdcore-0.0.6/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:23:43.819666 nerdcore-0.0.6/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 22:23:27.000000 nerdcore-0.0.6/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 22:23:27.000000 nerdcore-0.0.6/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:23:43.819666 nerdcore-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 22:23:27.000000 nerdcore-0.0.6/setup.py
```

### Comparing `nerdcore-0.0.5/PKG-INFO` & `nerdcore-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.5/nerdcore/defs.py` & `nerdcore-0.0.6/nerdcore/defs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.5/nerdcore/ncdefs.py` & `nerdcore-0.0.6/nerdcore/ncdefs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.5/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.0.6/nerdcore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.5/scripts/nerd` & `nerdcore-0.0.6/scripts/nerd`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.5/scripts/nerd-new` & `nerdcore-0.0.6/scripts/nerd-new`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.5/setup.py` & `nerdcore-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.0.5',
+    version='0.0.6',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

