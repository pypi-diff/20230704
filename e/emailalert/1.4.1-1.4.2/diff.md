# Comparing `tmp/emailalert-1.4.1.tar.gz` & `tmp/emailalert-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.1.tar", last modified: Tue Jul  4 04:53:17 2023, max compression
+gzip compressed data, was "emailalert-1.4.2.tar", last modified: Tue Jul  4 05:18:52 2023, max compression
```

## Comparing `emailalert-1.4.1.tar` & `emailalert-1.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.961551 emailalert-1.4.1/
--rw-rw-rw-   0        0        0      178 2023-07-04 04:53:17.959388 emailalert-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.917005 emailalert-1.4.1/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-04 04:53:17.000000 emailalert-1.4.1/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 04:53:17.952032 emailalert-1.4.1/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.4.1/sck/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-07-04 04:51:57.000000 emailalert-1.4.1/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-07-04 04:53:17.963049 emailalert-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-07-04 04:52:51.000000 emailalert-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.720605 emailalert-1.4.2/
+-rw-rw-rw-   0        0        0      178 2023-07-04 05:18:52.717355 emailalert-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.621991 emailalert-1.4.2/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-04 05:18:52.000000 emailalert-1.4.2/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 05:18:52.697830 emailalert-1.4.2/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.4.2/sck/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-07-04 05:14:01.000000 emailalert-1.4.2/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 05:18:52.721621 emailalert-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-04 05:18:44.000000 emailalert-1.4.2/setup.py
```

### Comparing `emailalert-1.4.1/README.md` & `emailalert-1.4.2/README.md`

 * *Files identical despite different names*

