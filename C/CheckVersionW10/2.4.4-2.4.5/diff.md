# Comparing `tmp/CheckVersionW10-2.4.4.tar.gz` & `tmp/CheckVersionW10-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheckVersionW10-2.4.4.tar", last modified: Mon Jul  3 18:22:45 2023, max compression
+gzip compressed data, was "CheckVersionW10-2.4.5.tar", last modified: Mon Jul  3 18:57:37 2023, max compression
```

## Comparing `CheckVersionW10-2.4.4.tar` & `CheckVersionW10-2.4.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 18:22:45.126905 CheckVersionW10-2.4.4/
-drwxrwxrwx   0        0        0        0 2023-07-03 18:22:45.112914 CheckVersionW10-2.4.4/CheckVersionW10/
--rw-rw-rw-   0        0        0      435 2023-07-03 18:22:14.000000 CheckVersionW10-2.4.4/CheckVersionW10/Funciones.py
--rw-rw-rw-   0        0        0       66 2023-06-29 18:43:56.000000 CheckVersionW10-2.4.4/CheckVersionW10/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 18:22:45.122906 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/
--rw-rw-rw-   0        0        0      758 2023-07-03 18:22:45.000000 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-03 18:22:45.000000 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 18:22:45.000000 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 18:22:45.000000 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-03 18:22:45.000000 CheckVersionW10-2.4.4/CheckVersionW10.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      758 2023-07-03 18:22:45.124908 CheckVersionW10-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-06-29 18:26:12.000000 CheckVersionW10-2.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 18:22:45.126905 CheckVersionW10-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-07-03 18:22:14.000000 CheckVersionW10-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:57:37.746577 CheckVersionW10-2.4.5/
+drwxrwxrwx   0        0        0        0 2023-07-03 18:57:37.737582 CheckVersionW10-2.4.5/CheckVersionW10/
+-rw-rw-rw-   0        0        0      432 2023-07-03 18:56:54.000000 CheckVersionW10-2.4.5/CheckVersionW10/Funciones.py
+-rw-rw-rw-   0        0        0       66 2023-06-29 18:43:56.000000 CheckVersionW10-2.4.5/CheckVersionW10/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:57:37.744588 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/
+-rw-rw-rw-   0        0        0      758 2023-07-03 18:57:37.000000 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-03 18:57:37.000000 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 18:57:37.000000 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 18:57:37.000000 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 18:57:37.000000 CheckVersionW10-2.4.5/CheckVersionW10.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      758 2023-07-03 18:57:37.746577 CheckVersionW10-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-06-29 18:26:12.000000 CheckVersionW10-2.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 18:57:37.746577 CheckVersionW10-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-07-03 18:57:31.000000 CheckVersionW10-2.4.5/setup.py
```

### Comparing `CheckVersionW10-2.4.4/CheckVersionW10.egg-info/PKG-INFO` & `CheckVersionW10-2.4.5/CheckVersionW10.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckVersionW10
-Version: 2.4.4
+Version: 2.4.5
 Summary: Librería para Validar Fecha de Librerias de Windows 10
 Home-page: https://github.com/AHernanandez1234/
 Author: Arturo Hernandez
 Author-email: ahernandez1980ene@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `CheckVersionW10-2.4.4/PKG-INFO` & `CheckVersionW10-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckVersionW10
-Version: 2.4.4
+Version: 2.4.5
 Summary: Librería para Validar Fecha de Librerias de Windows 10
 Home-page: https://github.com/AHernanandez1234/
 Author: Arturo Hernandez
 Author-email: ahernandez1980ene@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `CheckVersionW10-2.4.4/setup.py` & `CheckVersionW10-2.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.4.4' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '2.4.5' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'CheckVersionW10' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Arturo Hernandez' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'ahernandez1980ene@gmail.com' #Modificar con vuestros datos
 URL = 'https://github.com/AHernanandez1234/' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para Validar Fecha de Librerias de Windows 10' #Descripción corta
```

