# Comparing `tmp/enigmacrypt-0.0.6.tar.gz` & `tmp/enigmacrypt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmacrypt-0.0.6.tar", last modified: Mon Jul  3 20:51:16 2023, max compression
+gzip compressed data, was "enigmacrypt-0.0.7.tar", last modified: Mon Jul  3 21:32:42 2023, max compression
```

## Comparing `enigmacrypt-0.0.6.tar` & `enigmacrypt-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:51:16.177455 enigmacrypt-0.0.6/
--rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:16.000000 enigmacrypt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2530 2023-07-03 20:51:16.173466 enigmacrypt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:16.000000 enigmacrypt-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 20:51:16.170476 enigmacrypt-0.0.6/enigmacrypt.egg-info/
--rw-rw-rw-   0        0        0     2530 2023-07-03 20:51:15.000000 enigmacrypt-0.0.6/enigmacrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-03 20:51:15.000000 enigmacrypt-0.0.6/enigmacrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:51:15.000000 enigmacrypt-0.0.6/enigmacrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-03 20:51:15.000000 enigmacrypt-0.0.6/enigmacrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:51:15.000000 enigmacrypt-0.0.6/enigmacrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 20:51:16.178452 enigmacrypt-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-07-03 20:51:14.000000 enigmacrypt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:32:42.866859 enigmacrypt-0.0.7/
+-rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:16.000000 enigmacrypt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2530 2023-07-03 21:32:42.864863 enigmacrypt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:16.000000 enigmacrypt-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 21:32:42.788069 enigmacrypt-0.0.7/enigmacrypt/
+-rw-rw-rw-   0        0        0      144 2023-07-03 21:32:41.000000 enigmacrypt-0.0.7/enigmacrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:32:42.857882 enigmacrypt-0.0.7/enigmacrypt.egg-info/
+-rw-rw-rw-   0        0        0     2530 2023-07-03 21:32:42.000000 enigmacrypt-0.0.7/enigmacrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-07-03 21:32:42.000000 enigmacrypt-0.0.7/enigmacrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 21:32:42.000000 enigmacrypt-0.0.7/enigmacrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-03 21:32:42.000000 enigmacrypt-0.0.7/enigmacrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 21:32:42.000000 enigmacrypt-0.0.7/enigmacrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 21:32:42.866859 enigmacrypt-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-07-03 21:32:41.000000 enigmacrypt-0.0.7/setup.py
```

### Comparing `enigmacrypt-0.0.6/LICENSE` & `enigmacrypt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.6/PKG-INFO` & `enigmacrypt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Platform: UNKNOWN
```

### Comparing `enigmacrypt-0.0.6/README.md` & `enigmacrypt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.6/enigmacrypt.egg-info/PKG-INFO` & `enigmacrypt-0.0.7/enigmacrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Platform: UNKNOWN
```

### Comparing `enigmacrypt-0.0.6/setup.py` & `enigmacrypt-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Encoding and decoding strings using keys'
 
 # Setting up
 setup(
     name="enigmacrypt",
     version=VERSION,
     author="WooksCode (Wojciech Karwowski)",
```

