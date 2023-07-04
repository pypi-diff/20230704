# Comparing `tmp/vlite-0.1.2.tar.gz` & `tmp/vlite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.2.tar", last modified: Tue Jul  4 08:28:02 2023, max compression
+gzip compressed data, was "vlite-0.1.4.tar", last modified: Tue Jul  4 15:15:50 2023, max compression
```

## Comparing `vlite-0.1.2.tar` & `vlite-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:28:02.399430 vlite-0.1.2/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:28:02.399227 vlite-0.1.2/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.2/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 08:28:02.399516 vlite-0.1.2/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 08:27:55.000000 vlite-0.1.2/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 08:28:02.399015 vlite-0.1.2/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      162 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 08:28:02.000000 vlite-0.1.2/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.779893 vlite-0.1.4/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 15:15:50.779743 vlite-0.1.4/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)        8 2023-06-26 16:58:01.000000 vlite-0.1.4/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-04 15:15:50.779951 vlite-0.1.4/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-04 15:15:30.000000 vlite-0.1.4/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.778784 vlite-0.1.4/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.4/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     2626 2023-07-04 15:11:01.000000 vlite-0.1.4/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     2611 2023-07-04 15:11:23.000000 vlite-0.1.4/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3041 2023-07-04 15:13:56.000000 vlite-0.1.4/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-04 15:15:50.779545 vlite-0.1.4/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      224 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2023-07-04 15:15:50.000000 vlite-0.1.4/vlite.egg-info/top_level.txt
```

