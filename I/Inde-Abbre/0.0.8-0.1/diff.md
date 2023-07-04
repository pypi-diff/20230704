# Comparing `tmp/Inde_Abbre-0.0.8.tar.gz` & `tmp/Inde_Abbre-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Inde_Abbre-0.0.8.tar", last modified: Mon Jan 16 17:12:00 2023, max compression
+gzip compressed data, was "Inde_Abbre-0.1.tar", last modified: Mon Jan 16 15:53:12 2023, max compression
```

## Comparing `Inde_Abbre-0.0.8.tar` & `Inde_Abbre-0.1.tar`

### file list

```diff
@@ -1,35 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:12:00.791992 Inde_Abbre-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:12:00.787992 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-16 17:12:00.000000 Inde_Abbre-0.0.8/Inde_Abbre.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-01-16 17:12:00.791992 Inde_Abbre-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:12:00.791992 Inde_Abbre-0.0.8/cf_remote/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/aramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/cloud_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    16911 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/cf_remote/web.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 17:12:00.791992 Inde_Abbre-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:12:00.791992 Inde_Abbre-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-16 17:11:51.000000 Inde_Abbre-0.0.8/tests/test_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:53:12.627823 Inde_Abbre-0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:53:12.627823 Inde_Abbre-0.1/Inde_Abbre/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-16 15:53:03.000000 Inde_Abbre-0.1/Inde_Abbre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:53:12.627823 Inde_Abbre-0.1/Inde_Abbre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-16 15:53:12.000000 Inde_Abbre-0.1/Inde_Abbre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-16 15:53:12.000000 Inde_Abbre-0.1/Inde_Abbre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 15:53:12.000000 Inde_Abbre-0.1/Inde_Abbre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-16 15:53:12.000000 Inde_Abbre-0.1/Inde_Abbre.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-01-16 15:53:03.000000 Inde_Abbre-0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-16 15:53:12.627823 Inde_Abbre-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 15:53:12.627823 Inde_Abbre-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-16 15:53:03.000000 Inde_Abbre-0.1/setup.py
```

### Comparing `Inde_Abbre-0.0.8/cf_remote/main.py` & `Inde_Abbre-0.1/Inde_Abbre/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pandas as pd
 import json
 
-df = pd.read_csv("cf-remote/List_of_Abbrevations_Main.csv")
+df = pd.read_csv("E:\\Inde_Abbre\\List_of_Abbrevations_Main.csv")
 
 
 # you can simply use the dataframe (df) to read the columns and covert them as a dict and save it as a jSON file
 # below is the part
 abb_dict = {}
 for i, j in df.iterrows():
     abb_dict[j['Unnamed: 0']] = j['List of Abbreviations ']
@@ -21,7 +21,13 @@
     """The passing argument should be given in string characters within quotes """
     with open("output.json",) as jfile:
         loaded_dict = json.load(jfile)
         arr1=arr.upper().strip()
         for i,j in loaded_dict.items():
             if i==arr1:
                 print(j)
+
+
+
+
+
+
```

