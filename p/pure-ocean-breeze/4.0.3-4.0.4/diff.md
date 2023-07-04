# Comparing `tmp/pure_ocean_breeze-4.0.3.tar.gz` & `tmp/pure_ocean_breeze-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.3.tar", last modified: Tue Jul  4 01:25:31 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.4.tar", last modified: Tue Jul  4 07:38:53 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.3.tar` & `pure_ocean_breeze-4.0.4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.883294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   266936 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267121 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.632640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.636640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:38:53.628640 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 07:38:53.000000 pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:38:53.640640 pure_ocean_breeze-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 07:38:44.000000 pure_ocean_breeze-4.0.4/setup.py
```

### Comparing `pure_ocean_breeze-4.0.3/LICENSE` & `pure_ocean_breeze-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/PKG-INFO` & `pure_ocean_breeze-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.3
+Version: 4.0.4
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.3/README.md` & `pure_ocean_breeze-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-03 20:59:40"
-__version__ = "4.0.3"
+__updated__ = "2023-07-04 09:39:33"
+__version__ = "4.0.4"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-03 21:16:22"
+__updated__ = "2023-07-04 15:30:48"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -28,14 +28,16 @@
 from plotly.tools import FigureFactory as FF
 import pyfinance.ols as po
 from texttable import Texttable
 from xpinyin import Pinyin
 import tradetime as tt
 import cufflinks as cf
 import deprecation
+import duckdb
+import concurrent
 from mpire import WorkerPool
 from scipy.optimize import minimize
 from pure_ocean_breeze import __version__
 
 cf.set_config_file(offline=True)
 from typing import Callable, Union, Dict, List, Tuple
 from pure_ocean_breeze.data.read_data import (
@@ -1355,15 +1357,15 @@
                     corrs3 = corrs.iloc[60:90, :].reset_index(drop=True)
                     corrs = pd.concat([corrs1, corrs2, corrs3], axis=1).fillna('')
             else:
                 olds = [df] + olds
                 corrs = show_corrs(olds, old_orders, method=method)
         else:
             corrs = show_corrs(olds, old_orders, method=method)
-    return corrs
+    return corrs.sort_index()
 
 
 @do_on_dfs
 def remove_unavailable(df: pd.DataFrame) -> pd.DataFrame:
     """对日频或月频因子值，剔除st股、不正常交易的股票和上市不足60天的股票
 
     Parameters
@@ -6566,34 +6568,31 @@
         """
         return self.factor.copy()
 
     def select_one_calculate(
         self,
         date: pd.Timestamp,
         func: Callable,
+        fields: str='*',
         resample_frequency: str = None,
         opens_in: bool = 0,
         highs_in: bool = 0,
         lows_in: bool = 0,
-        moneys_in: bool = 0,
+        amounts_in: bool = 0,
         merge_them: bool = 0,
     ) -> None:
         the_func = partial(func)
         if not isinstance(date, int):
             date = int(datetime.datetime.strftime(date, "%Y%m%d"))
+        parquet_name=homeplace.tick_by_tick_data+ str(date)[:4]+ "-"+ str(date)[4:6]+ "-"+ str(date)[6:]+ ".parquet"
+        if resample_frequency is not None:
+            fields='date,code,price,amount'
         # 开始计算因子值
-        df = pd.read_parquet(
-            homeplace.tick_by_tick_data
-            + str(date)[:4]
-            + "-"
-            + str(date)[4:6]
-            + "-"
-            + str(date)[6:]
-            + ".parquet"
-        )
+        cursor=duckdb.connect()
+        df=cursor.execute(f"select {fields} from '{parquet_name}';").arrow().to_pandas()
         date = df.date.iloc[0]
         date0 = pd.Timestamp(year=date.year, month=date.month, day=date.day)
         age_here = self.age.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
         age_here = age_here.where(age_here > 180, np.nan).dropna()
         state_here = self.state.loc[pd.Timestamp(pd.Timestamp(df.date.iloc[0]).date())]
         state_here = state_here.where(state_here > 0, np.nan).dropna()
         df = df[df.code.isin(age_here.index)]
@@ -6654,33 +6653,33 @@
                 ) + lows.fillna(0)
                 self.lows = lows
                 names.append("low")
             else:
                 self.low = None
 
             names.append("close")
-            if moneys_in:
-                moneys = df.groupby(["code", "date"]).money.sum().reset_index()
-                moneys = moneys.pivot(index="date", columns="code", values="money")
-                moneys = moneys.resample(resample_frequency).sum().fillna(0)
-                self.moneys = moneys
-                names.append("money")
+            if amounts_in:
+                amounts = df.groupby(["code", "date"]).amount.sum().reset_index()
+                amounts = amounts.pivot(index="date", columns="code", values="amount")
+                amounts = amounts.resample(resample_frequency).sum().fillna(0)
+                self.amounts = amounts
+                names.append("amount")
             else:
-                self.moneys = None
+                self.amounts = None
 
             if merge_them:
                 self.data = merge_many(
                     [
                         i
                         for i in [
                             self.opens,
                             self.highs,
                             self.lows,
                             self.closes,
-                            self.moneys,
+                            self.amounts,
                         ]
                         if i is not None
                     ],
                     names,
                 )
 
         if self.groupby_code:
@@ -6711,15 +6710,15 @@
         self,
         func: Callable,
         n_jobs: int = 1,
         resample_frequency: str = None,
         opens_in: bool = 0,
         highs_in: bool = 0,
         lows_in: bool = 0,
-        moneys_in: bool = 0,
+        amounts_in: bool = 0,
         merge_them: bool = 0,
     ) -> None:
         """每次抽取chunksize天的截面上全部股票的分钟数据
         对每天的股票的数据计算因子值
 
         Parameters
         ----------
@@ -6736,47 +6735,44 @@
             可在循环计算的函数中使用`self.opens`来调用计算好的值，by default 0
         highs_in : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好最高价矩阵(index为时间,columns为股票代码,values为最高价)，
             可在循环计算的函数中使用`self.highs`来调用计算好的值，by default 0
         lows_in : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，提前计算好最低价矩阵(index为时间,columns为股票代码,values为最低价)，
             可在循环计算的函数中使用`self.lows`来调用计算好的值，by default 0
-        moneys_in : bool, optional
-            在resample_frequency不为None的情况下，可以使用此参数，提前计算好成交额矩阵(index为时间,columns为股票代码,values为成交额)，
-            可在循环计算的函数中使用`self.moneys`来调用计算好的值，by default 0
+        amounts_in : bool, optional
+            在resample_frequency不为None的情况下，可以使用此参数，提前计算好成交额矩阵(index为时间,columns为股票代码,values为成交量)，
+            可在循环计算的函数中使用`self.amounts`来调用计算好的值，by default 0
         merge_them : bool, optional
             在resample_frequency不为None的情况下，可以使用此参数，将计算好的因子值合并到一起，生成类似于分钟数据的sql形式，by default 0
         """
         if len(self.dates_new) > 0:
             if n_jobs > 1:
-                with WorkerPool(n_jobs=n_jobs) as pool:
-                    self.factor_new = pool.map(
+                with concurrent.futures.ThreadPoolExecutor(max_workers=n_jobs) as executor:
+                    self.factor_new=list(tqdm.auto.tqdm(executor.map(
                         lambda x: self.select_one_calculate(
                             date=x,
                             func=func,
                             resample_frequency=resample_frequency,
                             opens_in=opens_in,
                             highs_in=highs_in,
                             lows_in=lows_in,
-                            moneys_in=moneys_in,
+                            moneys_in=amounts_in,
                             merge_them=merge_them,
-                        ),
-                        self.dates_new,
-                        progress_bar=True,
-                    )
+                        ),self.dates_new),total=len(self.dates_new)))
             else:
                 for date in tqdm.auto.tqdm(self.dates_new, "您现在处于单核运算状态，建议仅在调试时使用单核"):
                     df = self.select_one_calculate(
                         date=date,
                         func=func,
                         resample_frequency=resample_frequency,
                         opens_in=opens_in,
                         highs_in=highs_in,
                         lows_in=lows_in,
-                        moneys_in=moneys_in,
+                        amounts_in=amounts_in,
                         merge_them=merge_them,
                     )
                     self.factor_new.append(df)
             # 拼接新的和旧的
             if self.factor_old is not None:
                 self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
             else:
```

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.3
+Version: 4.0.4
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.4/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.3/setup.py` & `pure_ocean_breeze-4.0.4/setup.py`

 * *Files identical despite different names*

