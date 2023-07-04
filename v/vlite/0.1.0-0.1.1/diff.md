# Comparing `tmp/vlite-0.1.0.tar.gz` & `tmp/vlite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.0.tar", last modified: Tue Jul  4 07:55:56 2023, max compression
+gzip compressed data, was "vlite-0.1.1.tar", last modified: Tue Jul  4 08:03:21 2023, max compression
```

## Comparing `vlite-0.1.0.tar` & `vlite-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 07:55:56.268347 vlite-0.1.0/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 07:55:56.268125 vlite-0.1.0/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.0/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 07:55:56.268390 vlite-0.1.0/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      431 2023-07-04 07:55:13.000000 vlite-0.1.0/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 07:55:56.267933 vlite-0.1.0/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 07:55:56.000000 vlite-0.1.0/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      162 2023-07-04 07:55:56.000000 vlite-0.1.0/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 07:55:56.000000 vlite-0.1.0/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       53 2023-07-04 07:55:56.000000 vlite-0.1.0/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 07:55:56.000000 vlite-0.1.0/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:03:21.479279 vlite-0.1.1/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:03:21.479128 vlite-0.1.1/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.1/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 08:03:21.479321 vlite-0.1.1/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 08:03:00.000000 vlite-0.1.1/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:03:21.478943 vlite-0.1.1/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      162 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/top_level.txt
```

