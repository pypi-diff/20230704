# Comparing `tmp/holamundoplayergvs-0.0.1.tar.gz` & `tmp/holamundoplayergvs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holamundoplayergvs-0.0.1.tar", last modified: Tue Jul  4 13:22:31 2023, max compression
+gzip compressed data, was "holamundoplayergvs-0.1.2.tar", last modified: Tue Jul  4 03:57:31 2023, max compression
```

## Comparing `holamundoplayergvs-0.0.1.tar` & `holamundoplayergvs-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:22:31.882004 holamundoplayergvs-0.0.1/
--rw-rw-rw-   0        0        0    35821 2023-07-04 03:13:44.000000 holamundoplayergvs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      144 2023-07-04 13:22:31.881004 holamundoplayergvs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-07-04 03:15:33.000000 holamundoplayergvs-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 13:22:31.877004 holamundoplayergvs-0.0.1/holamundoplayergvs/
--rw-rw-rw-   0        0        0       57 2023-07-04 02:51:30.000000 holamundoplayergvs-0.0.1/holamundoplayergvs/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-04 02:46:52.000000 holamundoplayergvs-0.0.1/holamundoplayergvs/lala.py
--rw-rw-rw-   0        0        0      570 2023-07-04 02:59:02.000000 holamundoplayergvs-0.0.1/holamundoplayergvs/player.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:22:31.881004 holamundoplayergvs-0.0.1/holamundoplayergvs.egg-info/
--rw-rw-rw-   0        0        0      144 2023-07-04 13:22:31.000000 holamundoplayergvs-0.0.1/holamundoplayergvs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-04 13:22:31.000000 holamundoplayergvs-0.0.1/holamundoplayergvs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:22:31.000000 holamundoplayergvs-0.0.1/holamundoplayergvs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 13:22:31.000000 holamundoplayergvs-0.0.1/holamundoplayergvs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 13:22:31.882004 holamundoplayergvs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-07-04 13:12:13.000000 holamundoplayergvs-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:57:31.252389 holamundoplayergvs-0.1.2/
+-rw-rw-rw-   0        0        0    35821 2023-07-04 03:13:44.000000 holamundoplayergvs-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      144 2023-07-04 03:57:31.252389 holamundoplayergvs-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-07-04 03:15:33.000000 holamundoplayergvs-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 03:57:31.248389 holamundoplayergvs-0.1.2/holamundoplayergvs/
+-rw-rw-rw-   0        0        0       57 2023-07-04 02:51:30.000000 holamundoplayergvs-0.1.2/holamundoplayergvs/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-04 02:46:52.000000 holamundoplayergvs-0.1.2/holamundoplayergvs/lala.py
+-rw-rw-rw-   0        0        0      570 2023-07-04 02:59:02.000000 holamundoplayergvs-0.1.2/holamundoplayergvs/player.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:57:31.251389 holamundoplayergvs-0.1.2/holamundoplayergvs.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-07-04 03:57:31.000000 holamundoplayergvs-0.1.2/holamundoplayergvs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-04 03:57:31.000000 holamundoplayergvs-0.1.2/holamundoplayergvs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:57:31.000000 holamundoplayergvs-0.1.2/holamundoplayergvs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-04 03:57:31.000000 holamundoplayergvs-0.1.2/holamundoplayergvs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 03:57:31.252389 holamundoplayergvs-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      282 2023-07-04 03:54:02.000000 holamundoplayergvs-0.1.2/setup.py
```

### Comparing `holamundoplayergvs-0.0.1/LICENSE` & `holamundoplayergvs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `holamundoplayergvs-0.0.1/holamundoplayergvs/player.py` & `holamundoplayergvs-0.1.2/holamundoplayergvs/player.py`

 * *Files identical despite different names*

