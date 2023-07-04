# Comparing `tmp/ovk_grapher-0.0.tar.gz` & `tmp/ovk_grapher-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovk_grapher-0.0.tar", last modified: Tue Jul  4 16:04:30 2023, max compression
+gzip compressed data, was "ovk_grapher-0.1.tar", last modified: Tue Jul  4 16:19:56 2023, max compression
```

## Comparing `ovk_grapher-0.0.tar` & `ovk_grapher-0.1.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:04:30.453398 ovk_grapher-0.0/
--rw-r--r--   0 vankermotis   (501) staff       (20)      113 2023-07-04 16:04:30.453520 ovk_grapher-0.0/PKG-INFO
-drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:04:30.451260 ovk_grapher-0.0/ovk_grapher/
--rw-rw-r--   0 vankermotis   (501) staff       (20)     4648 2018-06-20 04:16:08.000000 ovk_grapher-0.0/ovk_grapher/Binomialdistribution.py
--rw-rw-r--   0 vankermotis   (501) staff       (20)     3631 2018-06-20 04:16:08.000000 ovk_grapher-0.0/ovk_grapher/Gaussiandistribution.py
--rw-rw-r--   0 vankermotis   (501) staff       (20)      932 2018-06-20 04:16:08.000000 ovk_grapher-0.0/ovk_grapher/Generaldistribution.py
--rw-rw-r--   0 vankermotis   (501) staff       (20)       86 2018-06-20 04:16:08.000000 ovk_grapher-0.0/ovk_grapher/__init__.py
-drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:04:30.453163 ovk_grapher-0.0/ovk_grapher.egg-info/
--rw-r--r--   0 vankermotis   (501) staff       (20)      113 2023-07-04 16:04:30.000000 ovk_grapher-0.0/ovk_grapher.egg-info/PKG-INFO
--rw-r--r--   0 vankermotis   (501) staff       (20)      323 2023-07-04 16:04:30.000000 ovk_grapher-0.0/ovk_grapher.egg-info/SOURCES.txt
--rw-r--r--   0 vankermotis   (501) staff       (20)        1 2023-07-04 16:04:30.000000 ovk_grapher-0.0/ovk_grapher.egg-info/dependency_links.txt
--rw-r--r--   0 vankermotis   (501) staff       (20)        1 2023-07-04 16:04:30.000000 ovk_grapher-0.0/ovk_grapher.egg-info/not-zip-safe
--rw-r--r--   0 vankermotis   (501) staff       (20)       12 2023-07-04 16:04:30.000000 ovk_grapher-0.0/ovk_grapher.egg-info/top_level.txt
--rw-rw-r--   0 vankermotis   (501) staff       (20)       38 2023-07-04 16:04:30.453977 ovk_grapher-0.0/setup.cfg
--rw-rw-r--   0 vankermotis   (501) staff       (20)      211 2023-07-04 16:00:07.000000 ovk_grapher-0.0/setup.py
+drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:19:56.122466 ovk_grapher-0.1/
+-rw-r--r--   0 vankermotis   (501) staff       (20)      113 2023-07-04 16:19:56.122656 ovk_grapher-0.1/PKG-INFO
+drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:19:56.118557 ovk_grapher-0.1/ovk_grapher/
+-rw-rw-r--   0 vankermotis   (501) staff       (20)       34 2023-07-04 16:12:56.000000 ovk_grapher-0.1/ovk_grapher/__init__.py
+-rw-r--r--   0 vankermotis   (501) staff       (20)      145 2023-07-04 16:12:18.000000 ovk_grapher-0.1/ovk_grapher/grapher.py
+drwxr-xr-x   0 vankermotis   (501) staff       (20)        0 2023-07-04 16:19:56.122025 ovk_grapher-0.1/ovk_grapher.egg-info/
+-rw-r--r--   0 vankermotis   (501) staff       (20)      113 2023-07-04 16:19:56.000000 ovk_grapher-0.1/ovk_grapher.egg-info/PKG-INFO
+-rw-r--r--   0 vankermotis   (501) staff       (20)      239 2023-07-04 16:19:56.000000 ovk_grapher-0.1/ovk_grapher.egg-info/SOURCES.txt
+-rw-r--r--   0 vankermotis   (501) staff       (20)        1 2023-07-04 16:19:56.000000 ovk_grapher-0.1/ovk_grapher.egg-info/dependency_links.txt
+-rw-r--r--   0 vankermotis   (501) staff       (20)        1 2023-07-04 16:04:30.000000 ovk_grapher-0.1/ovk_grapher.egg-info/not-zip-safe
+-rw-r--r--   0 vankermotis   (501) staff       (20)       12 2023-07-04 16:19:56.000000 ovk_grapher-0.1/ovk_grapher.egg-info/top_level.txt
+-rw-rw-r--   0 vankermotis   (501) staff       (20)       38 2023-07-04 16:19:56.123414 ovk_grapher-0.1/setup.cfg
+-rw-rw-r--   0 vankermotis   (501) staff       (20)      212 2023-07-04 16:15:46.000000 ovk_grapher-0.1/setup.py
```

