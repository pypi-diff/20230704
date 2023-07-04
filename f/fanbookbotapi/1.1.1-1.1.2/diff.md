# Comparing `tmp/fanbookbotapi-1.1.1.tar.gz` & `tmp/fanbookbotapi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fanbookbotapi-1.1.1.tar", last modified: Tue Jul  4 05:57:13 2023, max compression
+gzip compressed data, was "fanbookbotapi-1.1.2.tar", last modified: Tue Jul  4 06:11:06 2023, max compression
```

## Comparing `fanbookbotapi-1.1.1.tar` & `fanbookbotapi-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:57:13.617651 fanbookbotapi-1.1.1/
--rw-rw-rw-   0        0        0      168 2023-07-04 05:57:13.605653 fanbookbotapi-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-04 05:53:08.000000 fanbookbotapi-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 05:57:13.417024 fanbookbotapi-1.1.1/fanbookbotapi/
--rw-rw-rw-   0        0        0       42 2023-05-17 08:23:41.000000 fanbookbotapi-1.1.1/fanbookbotapi/__init__.py
--rw-rw-rw-   0        0        0      778 2023-05-17 07:56:23.000000 fanbookbotapi-1.1.1/fanbookbotapi/fanbookbotapi.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:57:13.592656 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/
--rw-rw-rw-   0        0        0      168 2023-07-04 05:57:12.000000 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-04 05:57:12.000000 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:57:12.000000 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 05:57:12.000000 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-04 05:57:12.000000 fanbookbotapi-1.1.1/fanbookbotapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 05:57:13.618651 fanbookbotapi-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      308 2023-07-04 05:51:23.000000 fanbookbotapi-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:06.249446 fanbookbotapi-1.1.2/
+-rw-rw-rw-   0        0        0      199 2023-07-04 06:11:06.245439 fanbookbotapi-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-04 05:53:08.000000 fanbookbotapi-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:06.167454 fanbookbotapi-1.1.2/fanbookbotapi/
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:23:41.000000 fanbookbotapi-1.1.2/fanbookbotapi/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-05-17 07:56:23.000000 fanbookbotapi-1.1.2/fanbookbotapi/fanbookbotapi.py
+drwxrwxrwx   0        0        0        0 2023-07-04 06:11:06.238441 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-07-04 06:11:05.000000 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-04 06:11:05.000000 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 06:11:05.000000 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 06:11:05.000000 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 06:11:05.000000 fanbookbotapi-1.1.2/fanbookbotapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:11:06.250445 fanbookbotapi-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      361 2023-07-04 06:10:49.000000 fanbookbotapi-1.1.2/setup.py
```

### Comparing `fanbookbotapi-1.1.1/fanbookbotapi/fanbookbotapi.py` & `fanbookbotapi-1.1.2/fanbookbotapi/fanbookbotapi.py`

 * *Files identical despite different names*

