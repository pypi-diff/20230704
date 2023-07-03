# Comparing `tmp/plantilla-0.1.0.6.tar.gz` & `tmp/plantilla-0.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantilla-0.1.0.6.tar", last modified: Mon Oct 31 21:04:42 2022, max compression
+gzip compressed data, was "plantilla-0.1.0.7.tar", last modified: Mon Jul  3 22:51:32 2023, max compression
```

## Comparing `plantilla-0.1.0.6.tar` & `plantilla-0.1.0.7.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.375900 plantilla-0.1.0.6/
--rw-rw-rw-   0        0        0       25 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0       58 2022-10-31 21:04:42.375900 plantilla-0.1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.358901 plantilla-0.1.0.6/__pycache__/
--rw-rw-rw-   0        0        0     1444 2022-03-08 20:10:56.000000 plantilla-0.1.0.6/__pycache__/setup.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.363901 plantilla-0.1.0.6/_old/
--rw-rw-rw-   0        0        0     8632 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/_old/Plantilla pyfile.ipynb
--rw-rw-rw-   0        0        0     2019 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/_old/plantilla-0.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     1716 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/_old/plantilla-0.0.1.tar.gz
--rw-rw-rw-   0        0        0     1148 2022-03-11 18:45:05.000000 plantilla-0.1.0.6/_old/plantilla.do
--rw-rw-rw-   0        0        0     3440 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/_old/plantilla.py
--rw-rw-rw-   0        0        0      125 2022-03-08 13:22:32.000000 plantilla-0.1.0.6/_old/prueba stata.do
--rw-rw-rw-   0        0        0      104 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/old_setup.cfg
--rw-rw-rw-   0        0        0      708 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/old_setup.py
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.364901 plantilla-0.1.0.6/plantilla/
--rw-rw-rw-   0        0        0    15676 2022-10-31 21:04:17.000000 plantilla-0.1.0.6/plantilla/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.373902 plantilla-0.1.0.6/plantilla/__pycache__/
--rw-rw-rw-   0        0        0     7161 2022-03-08 20:11:57.000000 plantilla-0.1.0.6/plantilla/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.374902 plantilla-0.1.0.6/plantilla/styles/
--rw-rw-rw-   0        0        0     1940 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/plantilla/styles/mecon.mplstyle
-drwxrwxrwx   0        0        0        0 2022-10-31 21:04:42.372900 plantilla-0.1.0.6/plantilla.egg-info/
--rw-rw-rw-   0        0        0       58 2022-10-31 21:04:42.000000 plantilla-0.1.0.6/plantilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2022-10-31 21:04:42.000000 plantilla-0.1.0.6/plantilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 21:04:42.000000 plantilla-0.1.0.6/plantilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-10-31 21:04:42.000000 plantilla-0.1.0.6/plantilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-31 21:04:42.000000 plantilla-0.1.0.6/plantilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2022-02-16 15:08:29.000000 plantilla-0.1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-31 21:04:42.375900 plantilla-0.1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1280 2022-10-31 21:04:26.000000 plantilla-0.1.0.6/setup.py
--rw-rw-rw-   0        0        0      253 2022-03-08 13:27:02.000000 plantilla-0.1.0.6/subir a pip.md
--rw-rw-rw-   0        0        0      189 2022-03-18 15:35:57.000000 plantilla-0.1.0.6/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.114809 plantilla-0.1.0.7/
+-rw-rw-rw-   0        0        0       25 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0       58 2023-07-03 22:51:32.113809 plantilla-0.1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.039654 plantilla-0.1.0.7/__pycache__/
+-rw-rw-rw-   0        0        0     2479 2023-07-03 22:51:27.000000 plantilla-0.1.0.7/__pycache__/setup.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1444 2022-03-08 20:10:56.000000 plantilla-0.1.0.7/__pycache__/setup.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.054766 plantilla-0.1.0.7/_old/
+-rw-rw-rw-   0        0        0     8632 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/_old/Plantilla pyfile.ipynb
+-rw-rw-rw-   0        0        0     2019 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/_old/plantilla-0.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     1716 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/_old/plantilla-0.0.1.tar.gz
+-rw-rw-rw-   0        0        0     1148 2022-03-11 18:45:05.000000 plantilla-0.1.0.7/_old/plantilla.do
+-rw-rw-rw-   0        0        0     3440 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/_old/plantilla.py
+-rw-rw-rw-   0        0        0      125 2022-03-08 13:22:32.000000 plantilla-0.1.0.7/_old/prueba stata.do
+-rw-rw-rw-   0        0        0      104 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/old_setup.cfg
+-rw-rw-rw-   0        0        0      708 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/old_setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.063766 plantilla-0.1.0.7/plantilla/
+-rw-rw-rw-   0        0        0    15579 2023-07-03 22:50:42.000000 plantilla-0.1.0.7/plantilla/__init__.py
+-rw-rw-rw-   0        0        0    15675 2022-10-31 20:59:38.000000 plantilla-0.1.0.7/plantilla/__init__.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.109804 plantilla-0.1.0.7/plantilla/__pycache__/
+-rw-rw-rw-   0        0        0     7161 2022-03-08 20:11:57.000000 plantilla-0.1.0.7/plantilla/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.111806 plantilla-0.1.0.7/plantilla/styles/
+-rw-rw-rw-   0        0        0     1940 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/plantilla/styles/mecon.mplstyle
+drwxrwxrwx   0        0        0        0 2023-07-03 22:51:32.106804 plantilla-0.1.0.7/plantilla.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-07-03 22:51:31.000000 plantilla-0.1.0.7/plantilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-07-03 22:51:31.000000 plantilla-0.1.0.7/plantilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 22:51:31.000000 plantilla-0.1.0.7/plantilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-03 22:51:31.000000 plantilla-0.1.0.7/plantilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 22:51:31.000000 plantilla-0.1.0.7/plantilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2022-02-16 15:08:29.000000 plantilla-0.1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 22:51:32.114809 plantilla-0.1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2023-07-03 22:50:54.000000 plantilla-0.1.0.7/setup.py
+-rw-rw-rw-   0        0        0     1280 2022-10-31 21:00:11.000000 plantilla-0.1.0.7/setup.py.bak
+-rw-rw-rw-   0        0        0      253 2022-03-08 13:27:02.000000 plantilla-0.1.0.7/subir a pip.md
+-rw-rw-rw-   0        0        0      189 2022-03-18 15:35:57.000000 plantilla-0.1.0.7/test.py
```

### Comparing `plantilla-0.1.0.6/__pycache__/setup.cpython-39.pyc` & `plantilla-0.1.0.7/__pycache__/setup.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/_old/Plantilla pyfile.ipynb` & `plantilla-0.1.0.7/_old/Plantilla pyfile.ipynb`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/_old/plantilla-0.0.1-py3-none-any.whl` & `plantilla-0.1.0.7/_old/plantilla-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/_old/plantilla-0.0.1.tar.gz` & `plantilla-0.1.0.7/_old/plantilla-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/_old/plantilla.do` & `plantilla-0.1.0.7/_old/plantilla.do`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/_old/plantilla.py` & `plantilla-0.1.0.7/_old/plantilla.py`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/old_setup.py` & `plantilla-0.1.0.7/old_setup.py`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/plantilla/__init__.py` & `plantilla-0.1.0.7/plantilla/__init__.py.bak`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         # global path_figures  
         # global path_maps	  
         # global path_tables	  
         # global path_programas
 
         
         path_datain	   = path_user + r'\data\data_in'
-        path_dataout   = path_user + fr'\data\data_out\{subproyecto}'
+        path_dataout   = path_user + r'\data\data_out\{subproyecto}'
         path_scripts   = path_user + fr'\scripts\{subproyecto}'
         path_figures   = path_user + fr'\outputs\figures\{subproyecto}'
         path_maps	   = path_user + fr'\outputs\maps\{subproyecto}'
         path_tables	   = path_user + fr'\outputs\tables\{subproyecto}'
         path_programas = path_user + r'"C:\Users\Administrador\Documents\MECON\0. Varios\scripts\Programas"'
```

### Comparing `plantilla-0.1.0.6/plantilla/__pycache__/__init__.cpython-39.pyc` & `plantilla-0.1.0.7/plantilla/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/plantilla/styles/mecon.mplstyle` & `plantilla-0.1.0.7/plantilla/styles/mecon.mplstyle`

 * *Files identical despite different names*

### Comparing `plantilla-0.1.0.6/setup.py` & `plantilla-0.1.0.7/setup.py.bak`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class PostInstallMoveFile(install):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         atexit.register(install_styles)
 
 
-__version__ = '0.1.0.6'
+__version__ = '0.1.0.5'
 
 setup(
     name='plantilla',
     package_data={
         'styles': [
             "mecon.mplstyle"
         ]
```

