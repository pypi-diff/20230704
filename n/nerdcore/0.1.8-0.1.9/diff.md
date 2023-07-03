# Comparing `tmp/nerdcore-0.1.8.tar.gz` & `tmp/nerdcore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.1.8.tar", last modified: Mon Jul  3 23:34:57 2023, max compression
+gzip compressed data, was "nerdcore-0.1.9.tar", last modified: Mon Jul  3 23:39:41 2023, max compression
```

## Comparing `nerdcore-0.1.8.tar` & `nerdcore-0.1.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.120223 nerdcore-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-03 23:34:40.000000 nerdcore-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 23:34:57.120223 nerdcore-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 23:34:40.000000 nerdcore-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.112223 nerdcore-0.1.8/nerdcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.112223 nerdcore-0.1.8/nerdcore/abilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/abilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/abilities/gpt_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.112223 nerdcore-0.1.8/nerdcore/base_entitiies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/base_entitiies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/base_entitiies/command_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/base_entitiies/deployment_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.112223 nerdcore-0.1.8/nerdcore/base_entitiies/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/base_entitiies/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/base_entitiies/utils/cli_runnable_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/list.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/make.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/toggle-light-mode.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/commands/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/config/env_class.py
--rw-rw-rw-   0 root         (0) root         (0)     8372 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/config/nerd_config_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/config/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/config/yaml_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/defs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/help/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/help/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/help/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/help/help.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/ncdefs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/stor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/stor/defaults/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/.default-gitignore
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/.env.default
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/DEFAULT-README.md
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/DefaultDeployment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/context-file.txt
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/nerd-config-defaults.yaml
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/defaults/nerd-manifest.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/stor/entity_examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/entity_examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/entity_examples/example-command.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/entity_examples/example-deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/stor/snippets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/snippets/banner.txt
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/snippets/header-comment.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/stor/snippets/header-comment.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.116223 nerdcore-0.1.8/nerdcore/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.120223 nerdcore-0.1.8/nerdcore/utils/env/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/env/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/env/environment_checks.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/env/get_env_prop_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/env/update_env_class.py
--rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/ncdefs_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.120223 nerdcore-0.1.8/nerdcore/utils/nerd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/find_entity.py
--rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/generate_nerd_configs.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/get_config_name.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/parse_nerd_args.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/run_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     6970 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd/theme_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.120223 nerdcore-0.1.8/nerdcore/utils/nerd_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd_config/load_nerd_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd_config/nerd_config_validations.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-03 23:34:40.000000 nerdcore-0.1.8/nerdcore/utils/nerd_config/update_nerd_config_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.112223 nerdcore-0.1.8/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 23:34:57.000000 nerdcore-0.1.8/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:34:57.120223 nerdcore-0.1.8/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-07-03 23:34:40.000000 nerdcore-0.1.8/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3607 2023-07-03 23:34:40.000000 nerdcore-0.1.8/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 23:34:57.120223 nerdcore-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-07-03 23:34:40.000000 nerdcore-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-03 23:39:25.000000 nerdcore-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 23:39:41.302154 nerdcore-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 23:39:25.000000 nerdcore-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.294154 nerdcore-0.1.9/nerdcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.294154 nerdcore-0.1.9/nerdcore/abilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/abilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/abilities/gpt_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.294154 nerdcore-0.1.9/nerdcore/base_entitiies/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/base_entitiies/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/base_entitiies/command_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/base_entitiies/deployment_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/base_entitiies/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/base_entitiies/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/base_entitiies/utils/cli_runnable_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/make.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/toggle-light-mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/commands/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/config/env_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/config/nerd_config_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/config/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/config/yaml_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/defs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/help/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/help/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/help/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/help/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/ncdefs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/stor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/stor/defaults/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/.default-gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/.env.default
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/DEFAULT-README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1149 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/DefaultDeployment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/context-file.txt
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/nerd-config-defaults.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/defaults/nerd-manifest.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/stor/entity_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/entity_examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/entity_examples/example-command.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/entity_examples/example-deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/stor/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/snippets/banner.txt
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/snippets/header-comment.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/stor/snippets/header-comment.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.298154 nerdcore-0.1.9/nerdcore/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/nerdcore/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/nerdcore/utils/env/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/env/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/env/environment_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/env/get_env_prop_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/env/update_env_class.py
+-rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/ncdefs_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/nerdcore/utils/nerd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/find_entity.py
+-rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/generate_nerd_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/get_config_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/parse_nerd_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/run_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     6978 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd/theme_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/nerdcore/utils/nerd_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd_config/load_nerd_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd_config/nerd_config_validations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-03 23:39:25.000000 nerdcore-0.1.9/nerdcore/utils/nerd_config/update_nerd_config_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.294154 nerdcore-0.1.9/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 23:39:41.000000 nerdcore-0.1.9/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 23:39:41.302154 nerdcore-0.1.9/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2911 2023-07-03 23:39:25.000000 nerdcore-0.1.9/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2023-07-03 23:39:25.000000 nerdcore-0.1.9/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 23:39:41.302154 nerdcore-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-07-03 23:39:25.000000 nerdcore-0.1.9/setup.py
```

### Comparing `nerdcore-0.1.8/PKG-INFO` & `nerdcore-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.1.8/nerdcore/abilities/gpt_client.py` & `nerdcore-0.1.9/nerdcore/abilities/gpt_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 import openai
 import tiktoken
 
-from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.defs import TOKEN_UNCERTAINTY_BUFFER
 from nerdcore.defs import import_env_class
+from nerdcore.utils.nerd.theme_functions import print_t
 
 ENV = import_env_class()
 
 # Set up OpenAI client with API key
 ENV = ENV()
 openai.api_key = ENV.OPENAI_API_KEY
```

### Comparing `nerdcore-0.1.8/nerdcore/base_entitiies/deployment_class.py` & `nerdcore-0.1.9/nerdcore/base_entitiies/deployment_class.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from typing import Dict, Any, List
 
 from nerdcore.base_entitiies.utils.cli_runnable_class import CliRunnable
+from nerdcore.defs import import_nerd_config_class
 from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.utils.nerd_config.load_nerd_config import load_nerd_config
-from nerdcore.defs import import_nerd_config_class
 
 NerdConfig = import_nerd_config_class()
 
 
 class Deployment(CliRunnable):
     named_arg_keys = ['config']
     config: str = None
```

### Comparing `nerdcore-0.1.8/nerdcore/base_entitiies/utils/cli_runnable_class.py` & `nerdcore-0.1.9/nerdcore/base_entitiies/utils/cli_runnable_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/commands/list-processes.py` & `nerdcore-0.1.9/nerdcore/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/commands/list.py` & `nerdcore-0.1.9/nerdcore/commands/list.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from nerdcore.ncdefs import NC_COMMANDS_PATH, NC_DEPLOYMENTS_PATH
 from nerdcore.base_entitiies.command_class import Command
-from nerdcore.utils.nerd.theme_functions import print_tree
 from nerdcore.defs import COMMANDS_PATH, DEPLOYMENTS_PATH
+from nerdcore.ncdefs import NC_COMMANDS_PATH, NC_DEPLOYMENTS_PATH
+from nerdcore.utils.nerd.theme_functions import print_tree
 
 
 class List(Command):
     named_arg_keys = ['all']
     all: bool = False
 
     def run(self):
```

### Comparing `nerdcore-0.1.8/nerdcore/commands/make.py` & `nerdcore-0.1.9/nerdcore/commands/make.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 
-from nerdcore.ncdefs import NC_EXAMPLE_COMMAND_PATH, NC_EXAMPLE_DEPLOYMENT_PATH
 from nerdcore.base_entitiies.command_class import Command
 from nerdcore.defs import COMMANDS_PATH, DEPLOYMENTS_PATH
+from nerdcore.ncdefs import NC_EXAMPLE_COMMAND_PATH, NC_EXAMPLE_DEPLOYMENT_PATH
 
 
 class Make(Command):
     # Specify args that are required (must be initialized as None)
     required_arg_keys = ['entity_type', 'entity_name']
 
     # Specify unnamed args (passed without --name) (define in passing order)
```

### Comparing `nerdcore-0.1.8/nerdcore/commands/toggle-light-mode.py` & `nerdcore-0.1.9/nerdcore/commands/toggle-light-mode.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from nerdcore.base_entitiies.command_class import Command
-from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.defs import THEME_CONFIG_PATH, nl
+from nerdcore.utils.nerd.theme_functions import print_t
 
 
 class ToggleLightMode(Command):
 
     def run(self):
 
         with open(THEME_CONFIG_PATH, "r+") as file:
```

### Comparing `nerdcore-0.1.8/nerdcore/config/env_class.py` & `nerdcore-0.1.9/nerdcore/config/env_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/config/nerd_config_class.py` & `nerdcore-0.1.9/nerdcore/config/nerd_config_class.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import dataclasses
 import os
 import re
 from dataclasses import dataclass
 
 from nerdcore.config.yaml_helpers import get_nerd_config_defaults
-from nerdcore.utils.nerd.theme_functions import print_t
-from nerdcore.utils.nerd_config.nerd_config_validations import is_prompt_key
 from nerdcore.defs import NERDS_PATH
 from nerdcore.defs import import_env_class
+from nerdcore.utils.nerd.theme_functions import print_t
+from nerdcore.utils.nerd_config.nerd_config_validations import is_prompt_key
 
 ENV = import_env_class()
 
 
 def insert_cop_file_contents(value: str) -> str:
     matches = re.findall(r'{cop:(.*?)}', value)
     for match in matches:
```

### Comparing `nerdcore-0.1.8/nerdcore/config/theme.py` & `nerdcore-0.1.9/nerdcore/config/theme.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/config/yaml_helpers.py` & `nerdcore-0.1.9/nerdcore/config/yaml_helpers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import yaml
 from ruamel.yaml import YAML
 
-from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.defs import NERD_CONFIG_DEFAULTS_PATH
+from nerdcore.utils.nerd.theme_functions import print_t
 
 
 def read_yaml_file(file_path, ruamel=False):
     try:
         with open(file_path, 'r') as file:
             if ruamel:
                 ruamel_yaml = get_ruamel_yaml()
```

### Comparing `nerdcore-0.1.8/nerdcore/defs.py` & `nerdcore-0.1.9/nerdcore/defs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/help/commands/list-processes.py` & `nerdcore-0.1.9/nerdcore/help/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/help/help.py` & `nerdcore-0.1.9/nerdcore/help/help.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
-from nerdcore.utils.nerd.theme_functions import print_banner, print_table, print_t, apply_t
 from nerdcore.defs import nl2, nl
+from nerdcore.utils.nerd.theme_functions import print_banner, print_table, print_t, apply_t
 
 
 def run_default_help(nerd_args: argparse.Namespace = None):
 
     # Nerd CLI Banner
     print_banner()
```

### Comparing `nerdcore-0.1.8/nerdcore/ncdefs.py` & `nerdcore-0.1.9/nerdcore/ncdefs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
+
 from pkg_resources import resource_filename
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 """  CORE PATHS
 
 This is a framework-level PATH definitions file.
 It is separate from defs.py for usage in nerd-new, when there is no project ROOT_PATH.
 It is also used anywhere else a framework-level path is needed.
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  """
@@ -34,14 +35,15 @@
 # HELP
 NC_HELP_PATH = resource_filename('nerdcore', "help")
 
 # STOR CORE
 NC_STOR_PATH = resource_filename('nerdcore', "stor")
 NC_STOR_TEMP_PATH = os.path.join(NC_STOR_PATH, "temp")
 NC_STOR_NERD_PATH = os.path.join(NC_STOR_PATH, "nerd")
+NC_STOR_SNIPPETS_PATH = os.path.join(NC_STOR_PATH, 'snippets')
 NC_STOR_DEFAULTS_PATH = os.path.join(NC_STOR_PATH, "defaults")
 
 # DEFAULTS
 NC_ENV_DEFAULT_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, ".env.default")
 NC_NERD_MANIFEST_DEFAULT_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, "nerd-manifest.yaml")
 NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, "nerd-config-defaults.yaml")
 NC_CONTEXT_FILE_EXAMPLE_PATH = os.path.join(NC_STOR_DEFAULTS_PATH, 'context-file.txt')
```

### Comparing `nerdcore-0.1.8/nerdcore/stor/defaults/.env.default` & `nerdcore-0.1.9/nerdcore/stor/defaults/.env.default`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/stor/defaults/DefaultDeployment.py` & `nerdcore-0.1.9/nerdcore/stor/defaults/DefaultDeployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from typing import Dict, Any, List
 
+from nerdcore.tasks.process_file import process_file
+
 from nerdcore.base_entitiies.deployment_class import Deployment
 from nerdcore.utils.nerd.theme_functions import print_t
-from nerdcore.tasks.process_file import process_file
-from nerdcore.tasks.summarize_context import summarize_context_file
 
 
 class Default(Deployment):
     required_config_keys = ['WORK_PATH', 'MAIN_PROMPT', 'OUTPUT_EXT']
 
     def __init__(self, nerd_args: argparse.Namespace, named_args: Dict[str, Any], unnamed_args: List[str]):
         super().__init__(nerd_args, named_args, unnamed_args)
```

### Comparing `nerdcore-0.1.8/nerdcore/stor/defaults/nerd-config-defaults.yaml` & `nerdcore-0.1.9/nerdcore/stor/defaults/nerd-config-defaults.yaml`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/stor/defaults/nerd-manifest.yaml` & `nerdcore-0.1.9/nerdcore/stor/defaults/nerd-manifest.yaml`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/stor/entity_examples/example-command.py` & `nerdcore-0.1.9/nerdcore/stor/entity_examples/example-command.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/utils/env/get_env_prop_type.py` & `nerdcore-0.1.9/nerdcore/utils/env/get_env_prop_type.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/utils/env/update_env_class.py` & `nerdcore-0.1.9/nerdcore/utils/env/update_env_class.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 
 from dotenv import dotenv_values
 
+from nerdcore.defs import ENV_CLASS_PATH, ROOT_PATH, nl
 from nerdcore.ncdefs import NC_ENV_DEFAULT_PATH
 from nerdcore.utils.env.get_env_prop_type import get_env_prop_type
-from nerdcore.defs import ENV_CLASS_PATH, ROOT_PATH, nl
 
 ENV_DEFINITION_TEMPLATE = "    {var_name}: {var_type} = os.getenv('{var_name}')"
 ENV_DEFINITION_TEMPLATE_DEFAULT = "    {var_name}: {var_type} = os.getenv('{var_name}', '{default}')"
 
 
 def update_env_class():
     """
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/ncdefs_utils.py` & `nerdcore-0.1.9/nerdcore/utils/ncdefs_utils.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/find_entity.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/find_entity.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import Generator, List, Tuple
 
+from nerdcore.defs import nl, nl2, COMMANDS_PATH, DEPLOYMENTS_PATH
 from nerdcore.ncdefs import NC_COMMANDS_PATH, NC_HELP_PATH
 from nerdcore.utils.ncdefs_utils import levenshtein_distance
 from nerdcore.utils.nerd.theme_functions import print_t, input_t
-from nerdcore.defs import nl, nl2, COMMANDS_PATH, DEPLOYMENTS_PATH
 
 entity_paths = {
     'command': [COMMANDS_PATH, NC_COMMANDS_PATH],
     'deployment': [DEPLOYMENTS_PATH],
     'help': [NC_HELP_PATH],
 }
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/generate_nerd_configs.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/generate_nerd_configs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import time
 
 from nerdcore.config.yaml_helpers import read_yaml_file, write_yaml_file
-from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.defs import NERDS_PATH, NERD_MANIFEST_PATH
 from nerdcore.defs import import_nerd_config_class
+from nerdcore.utils.nerd.theme_functions import print_t
 
 NerdConfig = import_nerd_config_class()
 
 
 def generate_nerd_configs():
 
     os.makedirs(os.path.join(NERDS_PATH), exist_ok=True)
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/get_config_name.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/get_config_name.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 import pathlib
 from typing import List, Tuple
 
-from nerdcore.utils.nerd.theme_functions import print_t, input_t
 from nerdcore.defs import NERDS_PATH
+from nerdcore.utils.nerd.theme_functions import print_t, input_t
 
 
 def list_configs() -> List[str]:
     """ List all nerd configs.
     :return: A list of config names """
     file_paths = glob.glob(os.path.join(NERDS_PATH, '*.yaml'))
     return [os.path.splitext(os.path.basename(file))[0] for file in file_paths]
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/parse_nerd_args.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/parse_nerd_args.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/run_entities.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/run_entities.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd/theme_functions.py` & `nerdcore-0.1.9/nerdcore/utils/nerd/theme_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import re
 import sys
 import textwrap
 from math import floor
 
 from termcolor import colored, COLORS
 
-from nerdcore.ncdefs import NC_STOR_NERD_PATH, VERSION
 from nerdcore.defs import import_env_class, nl
+from nerdcore.ncdefs import VERSION, NC_STOR_SNIPPETS_PATH
 
 ENV = import_env_class()
 ENV = ENV()
 text_themes = ENV.text_themes
 light_mode_enabled = ENV.light_mode_enabled
 max_terminal_width = ENV.max_terminal_width
 keywords = ENV.keywords
@@ -96,15 +96,15 @@
 
 
 def strip_color_and_bold_codes(s):
     return re.sub(r'\x1b\[[0-9;]*m', '', s)
 
 
 def print_banner():
-    with open(os.path.join(NC_STOR_NERD_PATH, 'banner.txt'), 'r') as f:
+    with open(os.path.join(NC_STOR_SNIPPETS_PATH, 'banner.txt'), 'r') as f:
         art = f.read()
     print_t(art.replace('vX.X.X', f'v{VERSION}') + nl, 'light_yellow')
 
 
 def print_table(table, title=None, sub_indent='   ', min_col_width=10):
     terminal_width = min(os.get_terminal_size().columns, max_terminal_width)
     terminal_width -= len(sub_indent)
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd_config/load_nerd_config.py` & `nerdcore-0.1.9/nerdcore/utils/nerd_config/load_nerd_config.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
+from nerdcore.defs import import_nerd_config_class
 from nerdcore.ncdefs import NC_STOR_TEMP_PATH
 from nerdcore.utils.nerd.get_config_name import get_config_name
 from nerdcore.utils.nerd.theme_functions import print_t, input_t, apply_t
-from nerdcore.defs import import_nerd_config_class
 
 NerdConfig = import_nerd_config_class()
 
 
 def set_loaded_config(given_config_name: str) -> None:
     loaded_config_path = os.path.join(NC_STOR_TEMP_PATH, "loaded-config-name.txt")
     with open(loaded_config_path, 'w') as file:
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd_config/nerd_config_validations.py` & `nerdcore-0.1.9/nerdcore/utils/nerd_config/nerd_config_validations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from typing import List
 
-from nerdcore.utils.nerd.theme_functions import input_t, print_t
 from nerdcore.defs import ROOT_PATH
+from nerdcore.utils.nerd.theme_functions import input_t, print_t
 
 valid_values = {
     'temp': [0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1],
     'model': [3, 4]
 }
```

### Comparing `nerdcore-0.1.8/nerdcore/utils/nerd_config/update_nerd_config_class.py` & `nerdcore-0.1.9/nerdcore/utils/nerd_config/update_nerd_config_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.1.9/nerdcore.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.1.8/nerdcore.egg-info/SOURCES.txt` & `nerdcore-0.1.9/nerdcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerdcore-0.1.8/scripts/nerd` & `nerdcore-0.1.9/scripts/nerd`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 import os
 import subprocess
 import sys
 import traceback
 
+from nerdcore.defs import nl, PYTHON_COMMAND
 from nerdcore.utils.env.environment_checks import nerd_env_checks
 from nerdcore.utils.env.update_env_class import update_env_class
 from nerdcore.utils.nerd.find_entity import find_entity
 from nerdcore.utils.nerd.generate_nerd_configs import generate_nerd_configs
 from nerdcore.utils.nerd.parse_nerd_args import parse_nerd_args
 from nerdcore.utils.nerd.run_entities import run_deployment, run_command
 from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.utils.nerd_config.update_nerd_config_class import update_nerd_config_class
-from nerdcore.defs import nl, PYTHON_COMMAND
-
 
 # Some basic environment checks
 nerd_env_checks()
 
 # Regenerate "magic" config/env stuff
 update_env_class()
 update_nerd_config_class()
```

### Comparing `nerdcore-0.1.8/scripts/nerd-new` & `nerdcore-0.1.9/scripts/nerd-new`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 import shutil
 import sys
 
 from termcolor import colored
 
 from nerdcore.ncdefs import (NC_ENV_DEFAULT_PATH, NC_NERD_MANIFEST_DEFAULT_PATH, NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH,
-                             NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH, NC_DEFAULT_DEPLOYMENT_PATH,
+                             NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH,
+                             NC_DEFAULT_DEPLOYMENT_PATH,
                              NC_GITIGNORE_DEFAULT_PATH, NC_README_DEFAULT_PATH, NC_CONTEXT_FILE_EXAMPLE_PATH)
 
 top_level_dirs = [
     'abilities',
     'deployments',
     'commands',
     'config',
```

### Comparing `nerdcore-0.1.8/setup.py` & `nerdcore-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.1.8',
+    version='0.1.9',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

