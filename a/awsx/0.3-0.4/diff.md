# Comparing `tmp/awsx-0.3.tar.gz` & `tmp/awsx-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsx-0.3.tar", last modified: Tue Jul  4 01:16:14 2023, max compression
+gzip compressed data, was "awsx-0.4.tar", last modified: Tue Jul  4 13:45:17 2023, max compression
```

## Comparing `awsx-0.3.tar` & `awsx-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 01:16:14.143018 awsx-0.3/
--rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 01:16:14.142913 awsx-0.3/PKG-INFO
-drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 01:16:14.142786 awsx-0.3/awsx.egg-info/
--rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/PKG-INFO
--rw-r--r--   0 mini       (501) staff       (20)      186 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/SOURCES.txt
--rw-r--r--   0 mini       (501) staff       (20)        1 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/dependency_links.txt
--rw-r--r--   0 mini       (501) staff       (20)       41 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/entry_points.txt
--rw-r--r--   0 mini       (501) staff       (20)       12 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/requires.txt
--rw-r--r--   0 mini       (501) staff       (20)        5 2023-07-04 01:16:14.000000 awsx-0.3/awsx.egg-info/top_level.txt
--rw-r--r--   0 mini       (501) staff       (20)      446 2023-07-04 01:15:02.000000 awsx-0.3/main.py
--rw-r--r--   0 mini       (501) staff       (20)       38 2023-07-04 01:16:14.143045 awsx-0.3/setup.cfg
--rw-r--r--   0 mini       (501) staff       (20)      247 2023-07-04 01:16:09.000000 awsx-0.3/setup.py
+drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 13:45:17.521254 awsx-0.4/
+-rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 13:45:17.521148 awsx-0.4/PKG-INFO
+drwxr-xr-x   0 mini       (501) staff       (20)        0 2023-07-04 13:45:17.521025 awsx-0.4/awsx.egg-info/
+-rw-r--r--   0 mini       (501) staff       (20)       46 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/PKG-INFO
+-rw-r--r--   0 mini       (501) staff       (20)      186 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 mini       (501) staff       (20)        1 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 mini       (501) staff       (20)       41 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/entry_points.txt
+-rw-r--r--   0 mini       (501) staff       (20)       12 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/requires.txt
+-rw-r--r--   0 mini       (501) staff       (20)        5 2023-07-04 13:45:17.000000 awsx-0.4/awsx.egg-info/top_level.txt
+-rw-r--r--   0 mini       (501) staff       (20)      890 2023-07-04 13:44:27.000000 awsx-0.4/main.py
+-rw-r--r--   0 mini       (501) staff       (20)       38 2023-07-04 13:45:17.521282 awsx-0.4/setup.cfg
+-rw-r--r--   0 mini       (501) staff       (20)      247 2023-07-04 13:45:16.000000 awsx-0.4/setup.py
```

