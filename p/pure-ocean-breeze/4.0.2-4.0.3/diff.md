# Comparing `tmp/pure_ocean_breeze-4.0.2.tar.gz` & `tmp/pure_ocean_breeze-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.2.tar", last modified: Sun Jul  2 17:30:46 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.3.tar", last modified: Tue Jul  4 01:25:31 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.2.tar` & `pure_ocean_breeze-4.0.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.238962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   263550 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.242962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.246962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:30:46.238962 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 17:30:46.000000 pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:30:46.250962 pure_ocean_breeze-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-02 17:30:36.000000 pure_ocean_breeze-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.883294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66656 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   266936 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.891294 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.895295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:25:31.887294 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 01:25:31.000000 pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:25:31.899295 pure_ocean_breeze-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 01:25:20.000000 pure_ocean_breeze-4.0.3/setup.py
```

### Comparing `pure_ocean_breeze-4.0.2/LICENSE` & `pure_ocean_breeze-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/PKG-INFO` & `pure_ocean_breeze-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.2
+Version: 4.0.3
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
@@ -17,15 +17,15 @@
 # pure_ocean_breeze 
 #### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
 * v4.0.0 — 2023.06.28
-> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据&全新的因子成果数据库来啦！
 
 * v3.0.0 — 2022.08.16
 
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
```

### Comparing `pure_ocean_breeze-4.0.2/README.md` & `pure_ocean_breeze-4.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pure_ocean_breeze 
 #### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
 * v4.0.0 — 2023.06.28
-> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据&全新的因子成果数据库来啦！
 
 * v3.0.0 — 2022.08.16
 
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
```

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-03 01:29:04"
-__version__ = "4.0.2"
+__updated__ = "2023-07-03 20:59:40"
+__version__ = "4.0.3"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/read_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-__updated__ = "2023-06-21 14:48:09"
+__updated__ = "2023-07-04 09:13:50"
 
 import os
 import numpy as np
 import pandas as pd
 import datetime
-from typing import Union, Dict, Tuple
+import deprecation
+from typing import Any, Union, Dict, Tuple
 from loguru import logger
 
+from pure_ocean_breeze import __version__
 from pure_ocean_breeze.state.states import STATES
 from pure_ocean_breeze.state.homeplace import HomePlace
 from pure_ocean_breeze.state.decorators import *
 from pure_ocean_breeze.data.database import ClickHouseClient, Questdb
 
 try:
     homeplace = HomePlace()
@@ -168,82 +170,82 @@
 
     if not unadjust:
         if path:
             return pd.read_parquet(homeplace.daily_data_file + path)
         elif open:
             opens = pd.read_parquet(
                 homeplace.daily_data_file + "opens.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = opens
         elif close:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = closes
         elif high:
             highs = pd.read_parquet(
                 homeplace.daily_data_file + "highs.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = highs
         elif low:
             lows = pd.read_parquet(
                 homeplace.daily_data_file + "lows.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = lows
         elif vwap:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "vwaps.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1,start=start)
+                * read_daily(state=1, start=start)
             )
         elif tr:
             trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet").replace(
                 0, np.nan
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = trs
         elif sharenum:
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             df = sharenums
         elif total_sharenum:
             df = pd.read_parquet(homeplace.daily_data_file + "total_sharenums.parquet")
         elif amount:
             volumes = pd.read_parquet(
                 homeplace.daily_data_file + "amounts.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = volumes
         elif money:
             df = pd.read_parquet(
                 homeplace.factor_data_file + "日频数据-每日成交额/每日成交额.parquet"
             )
         elif age:
             age = pd.read_parquet(homeplace.daily_data_file + "ages.parquet")
             df = age
         elif flow_cap:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             flow_cap = closes * sharenums
             df = flow_cap
         elif total_cap:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             sharenums = pd.read_parquet(
                 homeplace.daily_data_file + "total_sharenums.parquet"
             )
             flow_cap = closes * sharenums
             df = flow_cap
         elif adjfactor:
             # df=pd.read_parquet(homeplace.daily_data_file+'adjfactors.parquet')
             df = (
                 read_daily(close=1, start=start)
-                * read_daily(state=1,start=start)
+                * read_daily(state=1, start=start)
                 / read_daily(close=1, start=start, unadjust=1)
-                * read_daily(state=1,start=start)
+                * read_daily(state=1, start=start)
             )
         elif st:
             st = pd.read_parquet(homeplace.daily_data_file + "sts.parquet")
             df = st
         elif state:
             state = pd.read_parquet(homeplace.daily_data_file + "states.parquet")
             state = state.where(state == 1, np.nan)
@@ -274,54 +276,54 @@
             df = df.rolling(20, min_periods=10).std()
         elif swing:
             df = (
                 read_daily(high=1, start=start) - read_daily(low=1, start=start)
             ) / read_daily(close=1, start=start)
         elif pb:
             df = pd.read_parquet(homeplace.daily_data_file + "pb.parquet") * read_daily(
-                state=1,start=start
+                state=1, start=start
             )
         elif pe:
             df = pd.read_parquet(homeplace.daily_data_file + "pe.parquet") * read_daily(
-                state=1,start=start
+                state=1, start=start
             )
         elif pettm:
-            df = pd.read_parquet(homeplace.daily_data_file + "pettm.parquet") * read_daily(
-                state=1,start=start
-            )
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "pettm.parquet"
+            ) * read_daily(state=1, start=start)
         elif iret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "idiosyncratic_ret.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif ivol:
             df = read_daily(iret=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif illiquidity:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "illiquidity.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif swindustry_ret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "股票对应申万一级行业每日收益率.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif zxindustry_ret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "股票对应中信一级行业每日收益率.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif stop_up:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "stop_ups.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1,start=start)
+                * read_daily(state=1, start=start)
             )
         elif stop_down:
             df = (
                 pd.read_parquet(homeplace.daily_data_file + "stop_downs.parquet")
                 * read_daily(adjfactor=1, start=start)
-                * read_daily(state=1,start=start)
+                * read_daily(state=1, start=start)
             )
         elif zxindustry_dummy_code:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量代码版.parquet")
         elif zxindustry_dummy_name:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量名称版.parquet")
         elif swindustry_dummy:
             df = pd.read_parquet(homeplace.daily_data_file + "申万行业2021版哑变量.parquet")
@@ -345,43 +347,43 @@
             )
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     else:
         if open:
             opens = pd.read_parquet(
                 homeplace.daily_data_file + "opens_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = opens
         elif close:
             closes = pd.read_parquet(
                 homeplace.daily_data_file + "closes_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = closes
         elif high:
             highs = pd.read_parquet(
                 homeplace.daily_data_file + "highs_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = highs
         elif low:
             lows = pd.read_parquet(
                 homeplace.daily_data_file + "lows_unadj.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
             df = lows
         elif vwap:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "vwaps.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif stop_up:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "stop_ups.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         elif stop_down:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "stop_downs.parquet"
-            ) * read_daily(state=1,start=start)
+            ) * read_daily(state=1, start=start)
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     if "date" not in df.columns:
         df = df[df.index >= pd.Timestamp(str(start))]
     return df.dropna(how="all")
 
 
@@ -751,14 +753,20 @@
         df = industry_dummy[["date", "code", w]]
         df = df.pivot(index="date", columns="code", values=w)
         df = df.replace(0, np.nan)
         ress[w] = df
     return ress
 
 
+@deprecation.deprecated(
+    deprecated_in="4.0",
+    removed_in="5.0",
+    current_version=__version__,
+    details="由于因子成果数据库升级，3.x版本的因子成果读取函数将下线",
+)
 def database_read_final_factors(
     name: str = None,
     order: int = None,
     freq: str = "月",
     output: bool = 0,
     new: bool = 0,
 ) -> Tuple[pd.DataFrame, str]:
@@ -873,14 +881,20 @@
             df.to_csv(fac_name)
             logger.success(f"截至{final_date}的因子值已保存")
         return df, fac_name
     else:
         return df, ""
 
 
+@deprecation.deprecated(
+    deprecated_in="4.0",
+    removed_in="5.0",
+    current_version=__version__,
+    details="由于因子成果数据库升级，3.x版本的因子成果读取函数将下线",
+)
 def database_read_primary_factors(name: str, name2: str = None) -> pd.DataFrame:
     """根据因子名字，读取初级因子的因子值
 
     Parameters
     ----------
     name : str, optional
         因子的名字, by default None
@@ -896,7 +910,81 @@
     if name2 is None:
         name = name + "/" + name + "_初级.parquet"
     else:
         name = name + "/" + name + "_初级_" + name2 + ".parquet"
     df = pd.read_parquet(homeplace.factor_data_file + name)
     df = df[sorted(list(df.columns))]
     return df
+
+
+class FactorDone(object):
+    def __init__(
+        self,
+        order: str,
+        name: str = None,
+        place: str = None,
+        son_name: str = None,
+        freq: str = "月",
+    ) -> None:
+        self.homeplace = HomePlace()
+        self.order = order
+        self.freq = freq
+        self.qdb = Questdb()
+        try:
+            self.factor_infos = self.qdb.get_data(
+                f"select * from factor_infos where order='{self.order}' and freq='{self.freq}'"
+            )
+        except Exception:
+            self.factor_infos = pd.DataFrame()
+        self.name = name
+        self.place = place
+        self.son_name = son_name
+        if (self.place is None) or (self.name is None):
+            final_line = self.qdb.get_data(
+                f"select * from factor_infos where order='{self.order}' and freq='{self.freq}'"
+            )
+            self.name = final_line.name.iloc[0]
+            self.place = final_line.place.iloc[0]
+        if son_name is None:
+            self.file = f"因子{self.order}_{self.name}_{self.freq}_{self.place}.parquet"
+            self.son_factors = {}
+            if self.factor_infos.shape[0] > 0:
+                for row in self.factor_infos.dropna().itertuples():
+                    self.son_factors[row.son_name] = FactorDone(
+                        order=row.order,
+                        name=row.name,
+                        place=row.place,
+                        son_name=row.son_name,
+                        freq=row.freq,
+                    )
+        else:
+            self.file = f"因子{self.order}_{self.name}_{self.son_name}_{self.freq}_{self.place}.parquet"
+
+
+    def __call__(self, son_name: str = None) -> Union[pd.DataFrame, dict]:
+        if son_name is None:
+            return pd.read_parquet(self.homeplace.final_factor_file + self.file)
+        else:
+            return self.son_factors[son_name]()
+
+    def save_factor(self, factor: pd.DataFrame):
+        try:
+            son_info = self.qdb.get_data(
+                f"select * from factor_infos where order='{self.order}' and son_name='{self.son_name}' and freq='{self.freq}'"
+            )
+        except Exception:
+            logger.warning(f"本次为第一次写入{self.name}_{self.son_name}因子")
+            son_info = pd.DataFrame()
+        if son_info.shape[0] == 0:
+            self.qdb.write_via_df(
+                pd.DataFrame(
+                    {
+                        "order": [self.order],
+                        "name": [self.name],
+                        "place": [self.place],
+                        "son_name": [self.son_name],
+                        "freq": [self.freq],
+                    }
+                ),
+                "factor_infos",
+            )
+        factor.to_parquet(self.homeplace.final_factor_file + self.file)
```

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/labor/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-02 02:33:46"
+__updated__ = "2023-07-03 21:16:22"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -42,14 +42,15 @@
     read_daily,
     read_market,
     get_industry_dummies,
     read_swindustry_prices,
     read_zxindustry_prices,
     database_read_final_factors,
     read_index_single,
+    FactorDone,
 )
 from pure_ocean_breeze.state.homeplace import HomePlace
 
 try:
     homeplace = HomePlace()
 except Exception:
     print("您暂未初始化，功能将受限")
@@ -997,72 +998,80 @@
     df = df * dummy_df
     return df
 
 
 def show_corr(
     fac1: pd.DataFrame,
     fac2: pd.DataFrame,
-    method: str = "spearman",
+    method: str = "pearson",
     plt_plot: bool = 1,
     show_series: bool = 0,
+    old_way: bool = 0,
 ) -> float:
     """展示两个因子的截面相关性
 
     Parameters
     ----------
     fac1 : pd.DataFrame
         因子1
     fac2 : pd.DataFrame
         因子2
     method : str, optional
-        计算相关系数的方法, by default "spearman"
+        计算相关系数的方法, by default "pearson"
     plt_plot : bool, optional
         是否画出相关系数的时序变化图, by default 1
     show_series : bool, optional
         返回相关性的序列，而非均值
+    old_way : bool, optional
+        使用3.x版本的方式求相关系数
 
     Returns
     -------
     `float`
         平均截面相关系数
     """
-    if method == "spearman":
-        corr = show_x_with_func(fac1, fac2, lambda x: x.rank().corr().iloc[0, 1])
+    if old_way:
+        if method == "spearman":
+            corr = show_x_with_func(fac1, fac2, lambda x: x.rank().corr().iloc[0, 1])
+        else:
+            corr = show_x_with_func(
+                fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1]
+            )
     else:
-        corr = show_x_with_func(fac1, fac2, lambda x: x.corr(method=method).iloc[0, 1])
+        corr = fac1.corrwith(fac2, axis=1, method=method)
     if show_series:
         return corr
     else:
         if plt_plot:
             corr.plot(rot=60)
             plt.show()
         return corr.mean()
 
 
 def show_corrs(
     factors: List[pd.DataFrame],
     factor_names: List[str] = None,
     print_bool: bool = True,
     show_percent: bool = True,
-    method: str = "spearman",
+    method: str = "pearson",
 ) -> pd.DataFrame:
     """展示很多因子两两之间的截面相关性
 
     Parameters
     ----------
     factors : List[pd.DataFrame]
         所有因子构成的列表, by default None
     factor_names : List[str], optional
         上述因子依次的名字, by default None
     print_bool : bool, optional
         是否打印出两两之间相关系数的表格, by default True
     show_percent : bool, optional
         是否以百分数的形式展示, by default True
     method : str, optional
-        计算相关系数的方法, by default "spearman"
+        计算相关系数的方法, by default "pearson"
 
     Returns
     -------
     `pd.DataFrame`
         两两之间相关系数的表格
     """
     corrs = []
@@ -1219,70 +1228,141 @@
     y = pure_fallmount(y)
     xs = [pure_fallmount(i) for i in xs]
     return (y - xs)()
 
 
 @do_on_dfs
 def show_corrs_with_old(
-    df: pd.DataFrame = None, method: str = "spearman", only_new: bool = 1
+    df: pd.DataFrame = None,
+    method: str = "pearson",
+    only_new: bool = 1,
+    with_son_factors: bool = 1,
+    freq: str = "M",
+    old_database: bool = 0,
 ) -> pd.DataFrame:
     """计算新因子和已有因子的相关系数
 
     Parameters
     ----------
     df : pd.DataFrame, optional
         新因子, by default None
     method : str, optional
-        求相关系数的方法, by default 'spearman'
+        求相关系数的方法, by default 'pearson'
     only_new : bool, optional
         仅计算新因子与旧因子之间的相关系数, by default 1
+    with_son_factors : bool, optional
+        计算新因子与数据库中各个细分因子的相关系数, by default 1
+    freq : str, optional
+        读取因子数据的频率, by default 'M'
+    old_database : bool, optional
+        使用3.x版本的数据库, by default 0
+
 
     Returns
     -------
     pd.DataFrame
         相关系数矩阵
     """
     if df is not None:
-        df0 = df.resample("M").last()
+        df0 = df.resample(freq).last()
         if df.shape[0] / df0.shape[0] > 2:
             daily = 1
         else:
             daily = 0
-    nums = os.listdir(homeplace.final_factor_file)
-    nums = sorted(
-        set(
-            [
-                int(i.split("多因子")[1].split("_月")[0])
-                for i in nums
-                if i.endswith("月.parquet")
-            ]
+    if old_database:
+        nums = os.listdir(homeplace.final_factor_file)
+        nums = sorted(
+            set(
+                [
+                    int(i.split("多因子")[1].split("_月")[0])
+                    for i in nums
+                    if i.endswith("月.parquet")
+                ]
+            )
         )
-    )
-    olds = []
-    for i in nums:
-        try:
+        olds = []
+        for i in nums:
+            try:
+                if daily:
+                    old = database_read_final_factors(order=i)[0]
+                else:
+                    old = database_read_final_factors(order=i)[0].resample("M").last()
+                olds.append(old)
+            except Exception:
+                break
+        if df is not None:
+            if only_new:
+                corrs = [
+                    to_percent(show_corr(df, i, plt_plot=0, method=method))
+                    for i in olds
+                ]
+                corrs = pd.Series(corrs, index=[f"old{i}" for i in nums])
+                corrs = corrs.to_frame(f"{method}相关系数").T
+            else:
+                olds = [df] + olds
+                corrs = show_corrs(
+                    olds, ["new"] + [f"old{i}" for i in nums], method=method
+                )
+        else:
+            corrs = show_corrs(olds, [f"old{i}" for i in nums], method=method)
+    else:
+        qdb = Questdb()
+        if freq == "M":
+            factor_infos = qdb.get_data("select * from factor_infos where freq='月'")
+        else:
+            factor_infos = qdb.get_data("select * from factor_infos where freq='周'")
+        if not with_son_factors:
+            old_orders = list(set(factor_infos.order))
             if daily:
-                old = database_read_final_factors(order=i)[0]
+                olds = [FactorDone(order=i)() for i in old_orders]
             else:
-                old = database_read_final_factors(order=i)[0].resample("M").last()
-            olds.append(old)
-        except Exception:
-            break
-    if df is not None:
-        if only_new:
-            corrs = [
-                to_percent(show_corr(df, i, plt_plot=0, method=method)) for i in olds
+                olds = [FactorDone(order=i)().resample(freq).last() for i in old_orders]
+        else:
+            old_orders = [
+                i.order + i.son_name.replace("因子", "")
+                for i in factor_infos.dropna().itertuples()
             ]
-            corrs = pd.Series(corrs, index=[f"old{i}" for i in nums])
-            corrs = corrs.to_frame(f"{method}相关系数").T
+            if daily:
+                olds = [
+                    FactorDone(order=i.order)(i.son_name)
+                    for i in factor_infos.dropna().itertuples()
+                ]
+            else:
+                olds = [
+                    FactorDone(order=i.order)(i.son_name).resample(freq).last()
+                    for i in factor_infos.dropna().itertuples()
+                ]
+        if df is not None:
+            if only_new:
+                corrs = [
+                    to_percent(show_corr(df, i, plt_plot=0, method=method))
+                    for i in olds
+                ]
+                corrs = pd.Series(corrs, index=old_orders)
+                corrs = corrs.to_frame(f"{method}相关系数")
+                if corrs.shape[0] <= 30:
+                    ...
+                elif corrs.shape[0] <= 60:
+                    corrs = corrs.reset_index()
+                    corrs.columns = ["因子名称", "相关系数"]
+                    corrs1 = corrs.iloc[:30, :]
+                    corrs2 = corrs.iloc[30:, :].reset_index(drop=True)
+                    corrs = pd.concat([corrs1, corrs2], axis=1).fillna('')
+                elif corrs.shape[0] <= 90:
+                    corrs = corrs.reset_index()
+                    corrs.columns = ["因子名称", "相关系数"]
+                    corrs1 = corrs.iloc[:30, :]
+                    corrs2 = corrs.iloc[30:60, :].reset_index(drop=True)
+                    corrs3 = corrs.iloc[60:90, :].reset_index(drop=True)
+                    corrs = pd.concat([corrs1, corrs2, corrs3], axis=1).fillna('')
+            else:
+                olds = [df] + olds
+                corrs = show_corrs(olds, old_orders, method=method)
         else:
-            olds = [df] + olds
-            corrs = show_corrs(olds, ["new"] + [f"old{i}" for i in nums], method=method)
-    else:
-        corrs = show_corrs(olds, [f"old{i}" for i in nums], method=method)
+            corrs = show_corrs(olds, old_orders, method=method)
     return corrs
 
 
 @do_on_dfs
 def remove_unavailable(df: pd.DataFrame) -> pd.DataFrame:
     """对日频或月频因子值，剔除st股、不正常交易的股票和上市不足60天的股票
 
@@ -2911,15 +2991,14 @@
         在横截面上做标准化
         输入的df应为，列名是股票代码，索引是时间
         """
         df = df.T
         df = (df - df.mean()) / df.std()
         df = df.T
         return df
-    
 
 
 class pure_fallmount(pure_fall):
     """继承自父类，专为做因子截面标准化之后相加和因子剔除其他辅助因子的作用"""
 
     def __init__(self, monthly_factors):
         """输入月度因子值，以设定新的对象"""
@@ -3522,36 +3601,39 @@
                     func=func,
                     fields=fields,
                     chunksize=chunksize,
                     show_time=show_time,
                     many_days=many_days,
                     n_jobs=n_jobs,
                 )
-            if len(self.factor_new)>0:
+            if len(self.factor_new) > 0:
                 self.factor_new = pd.concat(self.factor_new)
                 # 拼接新的和旧的
                 self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
                 self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
-                new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
+                new_end_date = datetime.datetime.strftime(
+                    self.factor.index.max(), "%Y%m%d"
+                )
                 # 存入本地
                 self.factor.to_parquet(self.factor_file)
                 logger.info(f"截止到{new_end_date}的因子值计算完了")
                 # 删除存储在questdb的中途备份数据
                 try:
-                    self.factor_steps.do_order(f"drop table '{self.factor_file_pinyin}'")
+                    self.factor_steps.do_order(
+                        f"drop table '{self.factor_file_pinyin}'"
+                    )
                     logger.info("备份在questdb的表格已删除")
                 except Exception:
                     logger.warning("删除questdb中表格时，存在某个未知错误，请当心")
             else:
-                logger.warning('由于某种原因，更新的因子值计算失败，建议检查🤒')
+                logger.warning("由于某种原因，更新的因子值计算失败，建议检查🤒")
                 # 拼接新的和旧的
                 self.factor = pd.concat([self.factor_old]).sort_index()
                 self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
 
-
         else:
             self.factor = drop_duplicates_index(self.factor_old)
             # 存入本地
             self.factor.to_parquet(self.factor_file)
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             logger.info(f"当前截止到{new_end_date}的因子值已经是最新的了")
 
@@ -6694,15 +6776,15 @@
                         merge_them=merge_them,
                     )
                     self.factor_new.append(df)
             # 拼接新的和旧的
             if self.factor_old is not None:
                 self.factor = pd.concat([self.factor_old, self.factor_new]).sort_index()
             else:
-                self.factor=self.factor_new.sort_index()
+                self.factor = self.factor_new.sort_index()
             self.factor = drop_duplicates_index(self.factor.dropna(how="all"))
             new_end_date = datetime.datetime.strftime(self.factor.index.max(), "%Y%m%d")
             # 存入本地
             self.factor.to_parquet(self.factor_file)
             logger.info(f"截止到{new_end_date}的因子值计算完了")
             # 删除存储在questdb的中途备份数据
             try:
```

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.2
+Version: 4.0.3
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
@@ -17,15 +17,15 @@
 # pure_ocean_breeze 
 #### **众人的因子框架**
 ##### 我们的口号是：量价因子才是最牛的！
 ***
 
 ### 全新大版本📢
 * v4.0.0 — 2023.06.28
-> 因子框架4.0版本来啦！逐笔数据&任意秒级数据来啦！
+> 因子框架4.0版本来啦！逐笔数据&任意秒级数据&全新的因子成果数据库来啦！
 
 * v3.0.0 — 2022.08.16
 
 >回测框架3.0版本来啦！ 模块拆分&说明文档来啦！[pure_ocean_breeze说明文档](https://chen-001.github.io/pure_ocean_breeze/)
 * v2.0.0 — 2022.07.12
 >回测框架2.0版本来啦！数据库&自动更新&最终因子库功能上线啦！
```

### Comparing `pure_ocean_breeze-4.0.2/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.3/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.2/setup.py` & `pure_ocean_breeze-4.0.3/setup.py`

 * *Files identical despite different names*

