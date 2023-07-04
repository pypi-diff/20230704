# Comparing `tmp/microviewer-1.6.0.tar.gz` & `tmp/microviewer-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.6.0.tar", last modified: Tue Jul  4 04:37:14 2023, max compression
+gzip compressed data, was "microviewer-1.6.1.tar", last modified: Tue Jul  4 05:00:02 2023, max compression
```

## Comparing `microviewer-1.6.0.tar` & `microviewer-1.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.980559 microviewer-1.6.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 04:37:14.000000 microviewer-1.6.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3444 2023-07-04 04:37:14.000000 microviewer-1.6.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 04:37:14.980738 microviewer-1.6.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.965953 microviewer-1.6.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.0/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.0/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.979614 microviewer-1.6.0/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    43146 2023-07-04 04:21:10.000000 microviewer-1.6.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    36471 2023-07-04 04:35:18.000000 microviewer-1.6.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.0/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.0/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.968949 microviewer-1.6.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.980202 microviewer-1.6.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.0/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 04:37:14.981561 microviewer-1.6.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.466029 microviewer-1.6.1/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 05:00:02.000000 microviewer-1.6.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3504 2023-07-04 05:00:02.000000 microviewer-1.6.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.1/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:00:02.466215 microviewer-1.6.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.1/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.459872 microviewer-1.6.1/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.1/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.1/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.464903 microviewer-1.6.1/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    42859 2023-07-04 04:58:01.000000 microviewer-1.6.1/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.1/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    36471 2023-07-04 04:35:18.000000 microviewer-1.6.1/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.1/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.1/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.462864 microviewer-1.6.1/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.1/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.465664 microviewer-1.6.1/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.1/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.1/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.1/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.1/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 05:00:02.466892 microviewer-1.6.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.1/setup.py
```

### Comparing `microviewer-1.6.0/ChangeLog` & `microviewer-1.6.1/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+1.6.1
+-----
+
+* perf: faster color assignment and rendering
+
 1.6.0
 -----
 
 * feat: adds invert selection
 * docs: numpy format link
 * docs: add feature highlights
 * docs: update demo image
```

### Comparing `microviewer-1.6.0/LICENSE` & `microviewer-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/PKG-INFO` & `microviewer-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.0
+Version: 1.6.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.0/README.md` & `microviewer-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/__init__.py` & `microviewer-1.6.1/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/crackle.js` & `microviewer-1.6.1/microviewer/crackle.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/exact-active.png` & `microviewer-1.6.1/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/exact.png` & `microviewer-1.6.1/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/large-active.png` & `microviewer-1.6.1/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/large.png` & `microviewer-1.6.1/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/medium-active.png` & `microviewer-1.6.1/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/cursors/medium.png` & `microviewer-1.6.1/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/datacube.js` & `microviewer-1.6.1/microviewer/datacube.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -23,34 +23,15 @@
     }
 
     progress() {
         return this.channel.progress;
     }
 
     initializeColorAssignments(cube) {
-        let assignments = {};
-        let last;
-
-        if (cube.length) {
-            last = cube[0];
-            assignments[cube[0]] = 0;
-        }
-
-        for (let i = cube.length - 1; i >= 0; i--) {
-            if (cube[i] == last) {
-                continue;
-            }
-
-            assignments[cube[i]] = 0;
-            last = cube[i];
-        }
-
-        assignments[0] = 0;
-
-        this.assigned_colors = assignments;
+        this.assigned_colors = new Uint32Array(this.renumbering.length);
         this.shuffleColors();
     }
 
     shuffleColors() {
         let colors = this.colors;
         const num_colors = colors.length;
```

### Comparing `microviewer-1.6.0/microviewer/favicon.ico` & `microviewer-1.6.1/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/index.html` & `microviewer-1.6.1/microviewer/index.html`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.6.1/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer/libcrackle.wasm` & `microviewer-1.6.1/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.6.1/microviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.0
+Version: 1.6.1
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.0/microviewer.egg-info/SOURCES.txt` & `microviewer-1.6.1/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/microviewer_cli/cli.py` & `microviewer-1.6.1/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/seg-demo.png` & `microviewer-1.6.1/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.0/setup.cfg` & `microviewer-1.6.1/setup.cfg`

 * *Files identical despite different names*

