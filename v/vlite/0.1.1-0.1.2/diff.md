# Comparing `tmp/vlite-0.1.1.tar.gz` & `tmp/vlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.1.tar", last modified: Tue Jul  4 08:03:21 2023, max compression
+gzip compressed data, was "vlite-0.1.2.tar", last modified: Tue Jul  4 08:28:02 2023, max compression
```

## Comparing `vlite-0.1.1.tar` & `vlite-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:03:21.479279 vlite-0.1.1/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:03:21.479128 vlite-0.1.1/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.1/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 08:03:21.479321 vlite-0.1.1/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 08:03:00.000000 vlite-0.1.1/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:03:21.478943 vlite-0.1.1/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      162 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:03:21.000000 vlite-0.1.1/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:28:02.399430 vlite-0.1.2/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:28:02.399227 vlite-0.1.2/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.2/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 08:28:02.399516 vlite-0.1.2/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 08:27:55.000000 vlite-0.1.2/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:28:02.399015 vlite-0.1.2/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      162 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/top_level.txt
```

