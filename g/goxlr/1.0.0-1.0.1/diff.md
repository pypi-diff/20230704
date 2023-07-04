# Comparing `tmp/goxlr-1.0.0.tar.gz` & `tmp/goxlr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.0.0.tar", last modified: Tue Jul  4 01:01:55 2023, max compression
+gzip compressed data, was "goxlr-1.0.1.tar", last modified: Tue Jul  4 01:05:06 2023, max compression
```

## Comparing `goxlr-1.0.0.tar` & `goxlr-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 01:01:55.914781 goxlr-1.0.0/
--rw-rw-rw-   0        0        0       52 2023-07-03 17:47:02.000000 goxlr-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      307 2023-07-04 01:01:55.915280 goxlr-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-07-03 17:42:34.000000 goxlr-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 01:01:55.911281 goxlr-1.0.0/goxlr/
--rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.0/goxlr/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.0/goxlr/error.py
--rw-rw-rw-   0        0        0    27170 2023-07-04 00:51:17.000000 goxlr-1.0.0/goxlr/goxlr.py
--rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.0/goxlr/types.py
--rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.0/goxlr/ws.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:01:55.914781 goxlr-1.0.0/goxlr.egg-info/
--rw-rw-rw-   0        0        0      307 2023-07-04 01:01:55.000000 goxlr-1.0.0/goxlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-04 01:01:55.000000 goxlr-1.0.0/goxlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 01:01:55.000000 goxlr-1.0.0/goxlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 01:01:55.000000 goxlr-1.0.0/goxlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 01:01:55.000000 goxlr-1.0.0/goxlr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 01:01:55.915780 goxlr-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      435 2023-07-04 00:59:12.000000 goxlr-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:05:06.940119 goxlr-1.0.1/
+-rw-rw-rw-   0        0        0       52 2023-07-03 17:47:02.000000 goxlr-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      405 2023-07-04 01:05:06.940617 goxlr-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-04 01:04:08.000000 goxlr-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 01:05:06.936617 goxlr-1.0.1/goxlr/
+-rw-rw-rw-   0        0        0       26 2023-07-03 21:36:56.000000 goxlr-1.0.1/goxlr/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-03 22:14:52.000000 goxlr-1.0.1/goxlr/error.py
+-rw-rw-rw-   0        0        0    27170 2023-07-04 00:51:17.000000 goxlr-1.0.1/goxlr/goxlr.py
+-rw-rw-rw-   0        0        0    11669 2023-07-04 00:56:11.000000 goxlr-1.0.1/goxlr/types.py
+-rw-rw-rw-   0        0        0     2171 2023-07-03 22:52:03.000000 goxlr-1.0.1/goxlr/ws.py
+drwxrwxrwx   0        0        0        0 2023-07-04 01:05:06.939617 goxlr-1.0.1/goxlr.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-07-04 01:05:06.000000 goxlr-1.0.1/goxlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-04 01:05:06.000000 goxlr-1.0.1/goxlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 01:05:06.000000 goxlr-1.0.1/goxlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-04 01:05:06.000000 goxlr-1.0.1/goxlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 01:05:06.000000 goxlr-1.0.1/goxlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 01:05:06.941118 goxlr-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      535 2023-07-04 01:04:10.000000 goxlr-1.0.1/setup.py
```

### Comparing `goxlr-1.0.0/goxlr/goxlr.py` & `goxlr-1.0.1/goxlr/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.0/goxlr/types.py` & `goxlr-1.0.1/goxlr/types.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.0.0/goxlr/ws.py` & `goxlr-1.0.1/goxlr/ws.py`

 * *Files identical despite different names*

