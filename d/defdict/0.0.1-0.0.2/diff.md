# Comparing `tmp/defdict-0.0.1.tar.gz` & `tmp/defdict-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defdict-0.0.1.tar", last modified: Mon Jul  3 04:32:05 2023, max compression
+gzip compressed data, was "defdict-0.0.2.tar", last modified: Mon Jul  3 23:17:07 2023, max compression
```

## Comparing `defdict-0.0.1.tar` & `defdict-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 04:32:05.826337 defdict-0.0.1/
--rw-rw-rw-   0        0        0      341 2023-07-03 04:32:05.826337 defdict-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 04:32:05.826337 defdict-0.0.1/defdict/
--rw-rw-rw-   0        0        0    12243 2023-07-03 02:24:52.000000 defdict-0.0.1/defdict/DataFormat.py
--rw-rw-rw-   0        0        0    27850 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/DefDict.py
--rw-rw-rw-   0        0        0     4090 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/MapRule.py
--rw-rw-rw-   0        0        0     1981 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/SpaceDefinition.py
--rw-rw-rw-   0        0        0      400 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/SpeedTest.py
--rw-rw-rw-   0        0        0     6151 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/StdConversion.py
--rw-rw-rw-   0        0        0     2426 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/StdDefinitions.py
--rw-rw-rw-   0        0        0     3133 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/StdUnit.py
--rw-rw-rw-   0        0        0     2181 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/Tmat.py
--rw-rw-rw-   0        0        0    15323 2023-07-03 02:24:52.000000 defdict-0.0.1/defdict/UnitType.py
--rw-rw-rw-   0        0        0      321 2023-07-03 03:50:01.000000 defdict-0.0.1/defdict/__init__.py
--rw-rw-rw-   0        0        0       79 2023-07-03 04:32:05.827337 defdict-0.0.1/defdict/_static_version.py
--rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 defdict-0.0.1/defdict/_version.py
--rw-rw-rw-   0        0        0      165 2023-07-03 02:55:19.000000 defdict-0.0.1/defdict/system_keys.py
-drwxrwxrwx   0        0        0        0 2023-07-03 04:32:05.825337 defdict-0.0.1/defdict.egg-info/
--rw-rw-rw-   0        0        0      341 2023-07-03 04:32:05.000000 defdict-0.0.1/defdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-03 04:32:05.000000 defdict-0.0.1/defdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 04:32:05.000000 defdict-0.0.1/defdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-03 04:32:05.000000 defdict-0.0.1/defdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 04:32:05.000000 defdict-0.0.1/defdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 04:32:05.826337 defdict-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-03 04:31:55.000000 defdict-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.120406 defdict-0.0.2/
+-rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 defdict-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-07-03 23:17:07.120406 defdict-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.121406 defdict-0.0.2/defdict/
+-rw-rw-rw-   0        0        0    12243 2023-07-03 02:24:52.000000 defdict-0.0.2/defdict/DataFormat.py
+-rw-rw-rw-   0        0        0    27850 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/DefDict.py
+-rw-rw-rw-   0        0        0     4090 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/MapRule.py
+-rw-rw-rw-   0        0        0     1981 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/SpaceDefinition.py
+-rw-rw-rw-   0        0        0      400 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/SpeedTest.py
+-rw-rw-rw-   0        0        0     6151 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdConversion.py
+-rw-rw-rw-   0        0        0     2426 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdDefinitions.py
+-rw-rw-rw-   0        0        0     3133 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/StdUnit.py
+-rw-rw-rw-   0        0        0     2181 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/Tmat.py
+-rw-rw-rw-   0        0        0    15323 2023-07-03 02:24:52.000000 defdict-0.0.2/defdict/UnitType.py
+-rw-rw-rw-   0        0        0      331 2023-07-03 04:40:06.000000 defdict-0.0.2/defdict/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-07-03 23:17:07.121406 defdict-0.0.2/defdict/_static_version.py
+-rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 defdict-0.0.2/defdict/_version.py
+-rw-rw-rw-   0        0        0      165 2023-07-03 02:55:19.000000 defdict-0.0.2/defdict/system_keys.py
+drwxrwxrwx   0        0        0        0 2023-07-03 23:17:07.120406 defdict-0.0.2/defdict.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 23:17:07.000000 defdict-0.0.2/defdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       28 2023-07-03 02:55:19.000000 defdict-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 23:17:07.121406 defdict-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1690 2023-07-03 23:16:53.000000 defdict-0.0.2/setup.py
```

### Comparing `defdict-0.0.1/defdict/DataFormat.py` & `defdict-0.0.2/defdict/DataFormat.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/DefDict.py` & `defdict-0.0.2/defdict/DefDict.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/MapRule.py` & `defdict-0.0.2/defdict/MapRule.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/SpaceDefinition.py` & `defdict-0.0.2/defdict/SpaceDefinition.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/StdConversion.py` & `defdict-0.0.2/defdict/StdConversion.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/StdDefinitions.py` & `defdict-0.0.2/defdict/StdDefinitions.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/StdUnit.py` & `defdict-0.0.2/defdict/StdUnit.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/Tmat.py` & `defdict-0.0.2/defdict/Tmat.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/UnitType.py` & `defdict-0.0.2/defdict/UnitType.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/defdict/_version.py` & `defdict-0.0.2/defdict/_version.py`

 * *Files identical despite different names*

### Comparing `defdict-0.0.1/setup.py` & `defdict-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='defdict',
-    version='0.0.1',
+    version='0.0.2',
     cmdclass=cmdclass,
     description=get_metadata('description'),
+    url=get_metadata("url"),
     author=get_metadata('author'),
     license='LGPLv3',
     packages=find_packages(include=['defdict', 'defdict.*']),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Robot Framework',
```

