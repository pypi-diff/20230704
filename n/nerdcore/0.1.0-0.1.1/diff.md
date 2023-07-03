# Comparing `tmp/nerdcore-0.1.0.tar.gz` & `tmp/nerdcore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.1.0.tar", last modified: Mon Jul  3 22:31:58 2023, max compression
+gzip compressed data, was "nerdcore-0.1.1.tar", last modified: Mon Jul  3 22:36:01 2023, max compression
```

## Comparing `nerdcore-0.1.0.tar` & `nerdcore-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.529066 nerdcore-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:31:58.529066 nerdcore-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:31:38.000000 nerdcore-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.513066 nerdcore-0.1.0/nerdcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.517066 nerdcore-0.1.0/nerdcore/abilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/abilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/abilities/gpt_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.517066 nerdcore-0.1.0/nerdcore/base_entitiies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/base_entitiies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/base_entitiies/command_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/base_entitiies/deployment_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.521066 nerdcore-0.1.0/nerdcore/base_entitiies/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/base_entitiies/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/base_entitiies/utils/cli_runnable_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.521066 nerdcore-0.1.0/nerdcore/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/list.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/make.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/toggle-light-mode.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/commands/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/config/env_class.py
--rw-rw-rw-   0 root         (0) root         (0)     8372 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/config/nerd_config_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/config/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/config/yaml_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/defs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/help/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/help/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/help/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/help/help.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/ncdefs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.525066 nerdcore-0.1.0/nerdcore/utils/env/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/env/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/env/environment_checks.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/env/get_env_prop_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/env/update_env_class.py
--rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/ncdefs_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.529066 nerdcore-0.1.0/nerdcore/utils/nerd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/find_entity.py
--rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/generate_nerd_configs.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/get_config_name.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/parse_nerd_args.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/run_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     6970 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd/theme_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.529066 nerdcore-0.1.0/nerdcore/utils/nerd_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd_config/load_nerd_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd_config/nerd_config_validations.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-03 22:31:38.000000 nerdcore-0.1.0/nerdcore/utils/nerd_config/update_nerd_config_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.513066 nerdcore-0.1.0/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1756 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 22:31:58.000000 nerdcore-0.1.0/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:31:58.529066 nerdcore-0.1.0/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 22:31:38.000000 nerdcore-0.1.0/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 22:31:38.000000 nerdcore-0.1.0/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:31:58.529066 nerdcore-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 22:31:38.000000 nerdcore-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.464989 nerdcore-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:36:01.464989 nerdcore-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:35:46.000000 nerdcore-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.452989 nerdcore-0.1.1/nerdcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.456989 nerdcore-0.1.1/nerdcore/abilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/abilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/abilities/gpt_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.456989 nerdcore-0.1.1/nerdcore/base_entitiies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/base_entitiies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/base_entitiies/command_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/base_entitiies/deployment_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.456989 nerdcore-0.1.1/nerdcore/base_entitiies/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/base_entitiies/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/base_entitiies/utils/cli_runnable_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.456989 nerdcore-0.1.1/nerdcore/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/make.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/toggle-light-mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/commands/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/config/env_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/config/nerd_config_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/config/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/config/yaml_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/defs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/help/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/help/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/help/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/help/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/ncdefs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/utils/env/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/env/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/env/environment_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/env/get_env_prop_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/env/update_env_class.py
+-rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/ncdefs_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.460989 nerdcore-0.1.1/nerdcore/utils/nerd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/find_entity.py
+-rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/generate_nerd_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/get_config_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/parse_nerd_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/run_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     6970 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd/theme_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.464989 nerdcore-0.1.1/nerdcore/utils/nerd_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd_config/load_nerd_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd_config/nerd_config_validations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-03 22:35:46.000000 nerdcore-0.1.1/nerdcore/utils/nerd_config/update_nerd_config_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.456989 nerdcore-0.1.1/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 22:36:01.000000 nerdcore-0.1.1/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:36:01.464989 nerdcore-0.1.1/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 22:35:46.000000 nerdcore-0.1.1/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 22:35:46.000000 nerdcore-0.1.1/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:36:01.464989 nerdcore-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 22:35:46.000000 nerdcore-0.1.1/setup.py
```

### Comparing `nerdcore-0.1.0/PKG-INFO` & `nerdcore-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.1.0/nerdcore/abilities/gpt_client.py` & `nerdcore-0.1.1/nerdcore/abilities/gpt_client.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/base_entitiies/deployment_class.py` & `nerdcore-0.1.1/nerdcore/base_entitiies/deployment_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/base_entitiies/utils/cli_runnable_class.py` & `nerdcore-0.1.1/nerdcore/base_entitiies/utils/cli_runnable_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/commands/list-processes.py` & `nerdcore-0.1.1/nerdcore/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/commands/list.py` & `nerdcore-0.1.1/nerdcore/commands/list.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/commands/make.py` & `nerdcore-0.1.1/nerdcore/commands/make.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/commands/toggle-light-mode.py` & `nerdcore-0.1.1/nerdcore/commands/toggle-light-mode.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/config/env_class.py` & `nerdcore-0.1.1/nerdcore/config/env_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/config/nerd_config_class.py` & `nerdcore-0.1.1/nerdcore/config/nerd_config_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/config/theme.py` & `nerdcore-0.1.1/nerdcore/config/theme.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/config/yaml_helpers.py` & `nerdcore-0.1.1/nerdcore/config/yaml_helpers.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/defs.py` & `nerdcore-0.1.1/nerdcore/defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 THEME_CONFIG_PATH = os.path.join(FRAMEWORK_CONFIG_PATH, 'theme.py')
 # ENV CLASS
 ENV_CLASS_PATH = os.path.join(FRAMEWORK_CONFIG_PATH, "env_class.py")
 # NERD CONFIG CLASS
 NERD_CONFIG_CLASS_PATH = os.path.join(FRAMEWORK_CONFIG_PATH, "nerd_config_class.py")
 
 # STOR
-STOR_PATH = os.path.join(ROOT_PATH, "../stor")
+STOR_PATH = os.path.join(ROOT_PATH, "stor")
 # TEMP
 TEMP_PATH = os.path.join(STOR_PATH, "temp")
 
 # NERD TEMP CONFIG FILES
 NERDS_PATH = os.path.join(TEMP_PATH, 'nerds')
 
 """  'GLOBAL' HELPERS/VARIABLES
```

### Comparing `nerdcore-0.1.0/nerdcore/help/commands/list-processes.py` & `nerdcore-0.1.1/nerdcore/help/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/help/help.py` & `nerdcore-0.1.1/nerdcore/help/help.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/ncdefs.py` & `nerdcore-0.1.1/nerdcore/ncdefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import os
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 """  CORE PATHS
 
 This is a framework-level PATH definitions file.
 It is separate from defs.py for usage in nerd-new, when there is no project ROOT_PATH.
 It is also used anywhere else a framework-level path is needed.
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  """
 
 # NC PATH (root package)
 NC_PATH = os.path.dirname(__file__)
 
-# NC outer ROOT_PATH
-NC_ROOT_PATH = os.path.join(NC_PATH, "..")
-
 # CM DEPLOYMENTS
 NC_DEPLOYMENTS_PATH = os.path.join(NC_PATH, "deployments")
 # CM TASKS
 NC_TASKS_PATH = os.path.join(NC_PATH, "tasks")
 # CM ABILITIES
 NC_ABILITIES_PATH = os.path.join(NC_PATH, "abilities")
 # CM COMMANDS
@@ -33,15 +30,15 @@
 # THEME CONFIG
 NC_THEME_CONFIG_PATH = os.path.join(NC_CONFIG_PATH, 'theme.py')
 
 # HELP
 NC_HELP_PATH = os.path.join(NC_PATH, "help")
 
 # STOR CORE
-NC_STOR_PATH = os.path.join(NC_ROOT_PATH, "stor")
+NC_STOR_PATH = os.path.join(NC_PATH, "stor")
 NC_STOR_TEMP_PATH = os.path.join(NC_STOR_PATH, "temp")
 NC_STOR_NERD_PATH = os.path.join(NC_STOR_PATH, "nerd")
 NC_STOR_DEFAULTS_PATH = os.path.join(NC_STOR_PATH, "defaults")
 
 # DEFAULTS
 NC_ENV_DEFAULT_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, ".env.default")
 NC_NERD_MANIFEST_DEFAULT_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, "nerd-manifest.yaml")
```

### Comparing `nerdcore-0.1.0/nerdcore/utils/env/get_env_prop_type.py` & `nerdcore-0.1.1/nerdcore/utils/env/get_env_prop_type.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/env/update_env_class.py` & `nerdcore-0.1.1/nerdcore/utils/env/update_env_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/ncdefs_utils.py` & `nerdcore-0.1.1/nerdcore/utils/ncdefs_utils.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/find_entity.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/find_entity.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/generate_nerd_configs.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/generate_nerd_configs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/get_config_name.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/get_config_name.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/parse_nerd_args.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/parse_nerd_args.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/run_entities.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/run_entities.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd/theme_functions.py` & `nerdcore-0.1.1/nerdcore/utils/nerd/theme_functions.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd_config/load_nerd_config.py` & `nerdcore-0.1.1/nerdcore/utils/nerd_config/load_nerd_config.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd_config/nerd_config_validations.py` & `nerdcore-0.1.1/nerdcore/utils/nerd_config/nerd_config_validations.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore/utils/nerd_config/update_nerd_config_class.py` & `nerdcore-0.1.1/nerdcore/utils/nerd_config/update_nerd_config_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.1.1/nerdcore.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.1.0/nerdcore.egg-info/SOURCES.txt` & `nerdcore-0.1.1/nerdcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/scripts/nerd` & `nerdcore-0.1.1/scripts/nerd`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/scripts/nerd-new` & `nerdcore-0.1.1/scripts/nerd-new`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.0/setup.py` & `nerdcore-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.1.0',
+    version='0.1.1',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

