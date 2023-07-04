# Comparing `tmp/napari-vedo-bridge-0.0.2.tar.gz` & `tmp/napari-vedo-bridge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-vedo-bridge-0.0.2.tar", last modified: Mon Jul  3 15:51:08 2023, max compression
+gzip compressed data, was "napari-vedo-bridge-0.0.3.tar", last modified: Tue Jul  4 07:24:39 2023, max compression
```

## Comparing `napari-vedo-bridge-0.0.2.tar` & `napari-vedo-bridge-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.376338 napari-vedo-bridge-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_cutter_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/vedo_extension.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 07:24:39.169400 napari-vedo-bridge-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_cutter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-04 07:24:22.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/vedo_extension.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:24:39.165400 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 07:24:39.000000 napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/top_level.txt
```

### Comparing `napari-vedo-bridge-0.0.2/LICENSE` & `napari-vedo-bridge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/PKG-INFO` & `napari-vedo-bridge-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-vedo-bridge
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transfer mesh data between napari and vedo for interactive processing
 Author: Johannes Soltwedel, Marco Musy
 Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
@@ -37,15 +37,15 @@
 To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
 
 To cut meshes you can use the following cutters:
 - `PlaneCutter`: cuts a mesh with a plane
 - `SphereCutter`: cuts a mesh with a sphere
 - `BoxCutter`: cuts a mesh with a box
 
-![](docs/imgs/screenshot_box_cutter.png)
+![](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/docs/imgs/screenshot_box_cutter.png)
 
 To send and get data into and from the plugin, you can:
 
 - Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
 - Load a mesh from file (click `Load mesh`)
 - Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
```

### Comparing `napari-vedo-bridge-0.0.2/README.md` & `napari-vedo-bridge-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
 
 To cut meshes you can use the following cutters:
 - `PlaneCutter`: cuts a mesh with a plane
 - `SphereCutter`: cuts a mesh with a sphere
 - `BoxCutter`: cuts a mesh with a box
 
-![](docs/imgs/screenshot_box_cutter.png)
+![](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/docs/imgs/screenshot_box_cutter.png)
 
 To send and get data into and from the plugin, you can:
 
 - Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
 - Load a mesh from file (click `Load mesh`)
 - Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
```

### Comparing `napari-vedo-bridge-0.0.2/pyproject.toml` & `napari-vedo-bridge-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/setup.cfg` & `napari-vedo-bridge-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_cutter_widget.py` & `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_cutter_widget.py`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/test_widget.py` & `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/vedo_extension.ui` & `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge/vedo_extension.ui`

 * *Files identical despite different names*

### Comparing `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/PKG-INFO` & `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-vedo-bridge
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transfer mesh data between napari and vedo for interactive processing
 Author: Johannes Soltwedel, Marco Musy
 Author-email: johannes_richard.soltwedel@tu-dresden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
@@ -37,15 +37,15 @@
 To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
 
 To cut meshes you can use the following cutters:
 - `PlaneCutter`: cuts a mesh with a plane
 - `SphereCutter`: cuts a mesh with a sphere
 - `BoxCutter`: cuts a mesh with a box
 
-![](docs/imgs/screenshot_box_cutter.png)
+![](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/docs/imgs/screenshot_box_cutter.png)
 
 To send and get data into and from the plugin, you can:
 
 - Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
 - Load a mesh from file (click `Load mesh`)
 - Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
```

### Comparing `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/SOURCES.txt` & `napari-vedo-bridge-0.0.3/src/napari_vedo_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

