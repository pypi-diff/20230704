# Comparing `tmp/nombres-0.0.tar.gz` & `tmp/Nombres-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nombres-0.0.tar", last modified: Tue Jul  4 18:16:23 2023, max compression
+gzip compressed data, was "Nombres-1.2.tar", last modified: Thu May 25 07:12:29 2023, max compression
```

## Comparing `nombres-0.0.tar` & `Nombres-1.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-04 18:16:23.556537 nombres-0.0/
--rw-r--r--   0 macbook    (501) staff       (20)      241 2023-07-04 18:16:23.556201 nombres-0.0/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-07-04 18:16:23.555737 nombres-0.0/nombres.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)      241 2023-07-04 18:16:23.000000 nombres-0.0/nombres.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      162 2023-07-04 18:16:23.000000 nombres-0.0/nombres.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-04 18:16:23.000000 nombres-0.0/nombres.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)        7 2023-07-04 18:16:23.000000 nombres-0.0/nombres.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-07-04 18:16:23.000000 nombres-0.0/nombres.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-07-04 18:16:23.556640 nombres-0.0/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      908 2023-07-04 18:15:29.000000 nombres-0.0/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-05-25 07:12:29.062087 Nombres-1.2/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-05-25 07:12:29.059020 Nombres-1.2/Nombres.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)      225 2023-05-25 07:12:29.000000 Nombres-1.2/Nombres.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      192 2023-05-25 07:12:29.000000 Nombres-1.2/Nombres.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-05-25 07:12:29.000000 Nombres-1.2/Nombres.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        7 2023-05-25 07:12:29.000000 Nombres-1.2/Nombres.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        5 2023-05-25 07:12:29.000000 Nombres-1.2/Nombres.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      225 2023-05-25 07:12:29.061753 Nombres-1.2/PKG-INFO
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-05-25 07:12:29.060439 Nombres-1.2/base/
+-rw-r--r--   0 macbook    (501) staff       (20)       64 2023-05-25 07:07:08.000000 Nombres-1.2/base/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      954 2023-05-25 06:54:51.000000 Nombres-1.2/base/main.py
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-05-25 07:12:29.062179 Nombres-1.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      892 2023-05-25 07:12:27.000000 Nombres-1.2/setup.py
```

### Comparing `nombres-0.0/setup.py` & `Nombres-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0'
-PACKAGE_NAME = 'nombres' #Debe coincidir con el nombre de la carpeta 
+VERSION = '1.2'
+PACKAGE_NAME = 'Nombres' #Debe coincidir con el nombre de la carpeta
 AUTHOR = 'ItzelFranco' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'itzel_fd1@tesch.edu.mx' #Modificar con vuestros datos
 URL = 'https://github.com/itzelfd98' #Modificar con vuestros datos
 
 LICENSE = 'GNU GPL' #Tipo de licencia
-DESCRIPTION = 'Library to obtain names of Spanish men and women as well as surnames'
+DESCRIPTION = 'Muestra 100 nombres de hombre y 10 nombres de mujer '
+
+
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
     'pandas'
 ]
 
 setup(
@@ -24,8 +26,8 @@
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
     include_package_data=True
-)
+)
```

