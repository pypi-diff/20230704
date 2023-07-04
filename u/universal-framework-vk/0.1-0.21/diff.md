# Comparing `tmp/universal_framework_vk-0.1.tar.gz` & `tmp/universal_framework_vk-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_framework_vk-0.1.tar", last modified: Tue Jul  4 03:46:30 2023, max compression
+gzip compressed data, was "universal_framework_vk-0.21.tar", last modified: Tue Jul  4 04:04:20 2023, max compression
```

## Comparing `universal_framework_vk-0.1.tar` & `universal_framework_vk-0.21.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 03:46:30.207353 universal_framework_vk-0.1/
--rw-rw-rw-   0        0        0       13 2023-07-04 03:44:57.000000 universal_framework_vk-0.1/LICENSE
--rw-rw-rw-   0        0        0      243 2023-07-04 03:46:30.207353 universal_framework_vk-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-07-04 03:44:57.000000 universal_framework_vk-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 03:46:30.207353 universal_framework_vk-0.1/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-07-04 03:44:57.000000 universal_framework_vk-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:46:30.207353 universal_framework_vk-0.1/universal_framework_vk.egg-info/
--rw-rw-rw-   0        0        0      243 2023-07-04 03:46:30.000000 universal_framework_vk-0.1/universal_framework_vk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-04 03:46:30.000000 universal_framework_vk-0.1/universal_framework_vk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 03:46:30.000000 universal_framework_vk-0.1/universal_framework_vk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 03:46:30.000000 universal_framework_vk-0.1/universal_framework_vk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 04:04:09.000000 universal_framework_vk-0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:04:20.483033 universal_framework_vk-0.21/universal_framework_vk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:04:20.000000 universal_framework_vk-0.21/universal_framework_vk.egg-info/top_level.txt
```

