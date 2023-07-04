# Comparing `tmp/napari-stl-exporter-0.1.4.tar.gz` & `tmp/napari-stl-exporter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stl-exporter-0.1.4.tar", last modified: Fri Jan 27 15:14:26 2023, max compression
+gzip compressed data, was "napari-stl-exporter-0.1.5.tar", last modified: Tue Jul  4 08:50:13 2023, max compression
```

## Comparing `napari-stl-exporter-0.1.4.tar` & `napari-stl-exporter-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.654085 napari-stl-exporter-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-01-27 15:14:26.654085 napari-stl-exporter-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-27 15:14:26.658085 napari-stl-exporter-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.642084 napari-stl-exporter-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.646084 napari-stl-exporter-0.1.4/src/napari_stl_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_image_to_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.650085 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_tests/test_writer_and_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.654085 napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)  1651055 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/Cylinder.tif
--rw-r--r--   0 runner    (1001) docker     (123)  1641918 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/Pyramid.tif
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  3041784 2023-01-27 15:14:07.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/pyramid.stl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:14:26.646084 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-27 15:14:26.000000 napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.502199 napari-stl-exporter-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-04 08:50:13.502199 napari-stl-exporter-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-04 08:50:13.502199 napari-stl-exporter-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.494199 napari-stl-exporter-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.494199 napari-stl-exporter-0.1.5/src/napari_stl_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_image_to_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.494199 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_tests/test_writer_and_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.498199 napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1651055 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/Cylinder.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  1641918 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/Pyramid.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  3041784 2023-07-04 08:49:58.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/pyramid.stl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:50:13.494199 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:50:13.000000 napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/top_level.txt
```

### Comparing `napari-stl-exporter-0.1.4/LICENSE` & `napari-stl-exporter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/PKG-INFO` & `napari-stl-exporter-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: napari-stl-exporter
-Version: 0.1.4
+Version: 0.1.5
 Summary: Exports label images to 3D-printable stl files.
 Home-page: https://github.com/jo-mueller/napari-stl-exporter.git
-Author: Johannes Müller
-Author-email: johannes_richard.mueller@tu-dresden.de
+Author: Johannes Soltwedel
+Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Project Site, https://github.com/jo-mueller/napari-stl-exporter
 Project-URL: Report Issues, https://github.com/jo-mueller/napari-stl-exporter/issues
 Project-URL: Documentation, https://pypi.org/project/napari-stl-exporter/
 Project-URL: User Support, https://github.com/jo-mueller/napari-stl-exporter/issues
 Project-URL: Twitter, https://twitter.com/jm_mightypirate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `napari-stl-exporter-0.1.4/README.md` & `napari-stl-exporter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/requirements.txt` & `napari-stl-exporter-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/setup.cfg` & `napari-stl-exporter-0.1.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = napari-stl-exporter
-version = 0.1.4
-author = Johannes Müller
-author_email = johannes_richard.mueller@tu-dresden.de
+version = 0.1.5
+author = Johannes Soltwedel
+author_email = johannes_richard.soltwedel@tu-dresden.de
 license = BSD-3-Clause
 description = Exports label images to 3D-printable stl files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jo-mueller/napari-stl-exporter.git
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -31,17 +31,17 @@
 packages = find:
 python_requires = >=3.7
 package_dir = 
 	=src
 install_requires = 
 	napari
 	scikit-image
-	vedo
+	vedo>=2023.4.6
 	npe2
-	numpy < 1.24.0
+	numpy
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 napari-stl-exporter =
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/_image_to_surface.py` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/_image_to_surface.py`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/_reader.py` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     path : str
 
     Returns
     -------
     SurfaceData
 
     """
-    mesh = vedo.io.load(path, unpack=True, force=False)
+    mesh = vedo.load(path, unpack=True, force=False)
     _mesh = [mesh.points(), np.asarray(mesh.faces())]
     return [tuple([_mesh, {}, 'surface'])]
```

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/_sample_data.py` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/_tests/test_writer_and_readers.py` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/_tests/test_writer_and_readers.py`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/_writer.py` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/napari.yaml` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/Cylinder.tif` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/Cylinder.tif`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/Pyramid.tif` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/Pyramid.tif`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter/sample_data/pyramid.stl` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter/sample_data/pyramid.stl`

 * *Files identical despite different names*

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/PKG-INFO` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: napari-stl-exporter
-Version: 0.1.4
+Version: 0.1.5
 Summary: Exports label images to 3D-printable stl files.
 Home-page: https://github.com/jo-mueller/napari-stl-exporter.git
-Author: Johannes Müller
-Author-email: johannes_richard.mueller@tu-dresden.de
+Author: Johannes Soltwedel
+Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Project Site, https://github.com/jo-mueller/napari-stl-exporter
 Project-URL: Report Issues, https://github.com/jo-mueller/napari-stl-exporter/issues
 Project-URL: Documentation, https://pypi.org/project/napari-stl-exporter/
 Project-URL: User Support, https://github.com/jo-mueller/napari-stl-exporter/issues
 Project-URL: Twitter, https://twitter.com/jm_mightypirate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `napari-stl-exporter-0.1.4/src/napari_stl_exporter.egg-info/SOURCES.txt` & `napari-stl-exporter-0.1.5/src/napari_stl_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

