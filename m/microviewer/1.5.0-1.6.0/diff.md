# Comparing `tmp/microviewer-1.5.0.tar.gz` & `tmp/microviewer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.5.0.tar", last modified: Mon Jul  3 19:25:41 2023, max compression
+gzip compressed data, was "microviewer-1.6.0.tar", last modified: Tue Jul  4 04:37:14 2023, max compression
```

## Comparing `microviewer-1.5.0.tar` & `microviewer-1.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758931 microviewer-1.5.0/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-03 19:25:41.000000 microviewer-1.5.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3317 2023-07-03 19:25:41.000000 microviewer-1.5.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.5.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.5.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-03 19:25:41.759113 microviewer-1.5.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1649 2023-06-28 21:32:21.000000 microviewer-1.5.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.754207 microviewer-1.5.0/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.5.0/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.5.0/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758033 microviewer-1.5.0/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.5.0/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    42723 2023-07-03 19:24:55.000000 microviewer-1.5.0/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.5.0/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    35771 2023-07-03 18:34:37.000000 microviewer-1.5.0/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.5.0/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.5.0/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.756336 microviewer-1.5.0/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     2663 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.5.0/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-03 19:25:41.000000 microviewer-1.5.0/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-03 19:25:41.758602 microviewer-1.5.0/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.5.0/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.5.0/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.5.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)   297931 2023-06-28 20:05:35.000000 microviewer-1.5.0/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-03 19:25:41.759784 microviewer-1.5.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.5.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.980559 microviewer-1.6.0/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 04:37:14.000000 microviewer-1.6.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3444 2023-07-04 04:37:14.000000 microviewer-1.6.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 04:37:14.980738 microviewer-1.6.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.0/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.965953 microviewer-1.6.0/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.0/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.0/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.979614 microviewer-1.6.0/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.0/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    43146 2023-07-04 04:21:10.000000 microviewer-1.6.0/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.0/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    36471 2023-07-04 04:35:18.000000 microviewer-1.6.0/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.0/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.0/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.968949 microviewer-1.6.0/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.0/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 04:37:14.000000 microviewer-1.6.0/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 04:37:14.980202 microviewer-1.6.0/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.0/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.0/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.0/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 04:37:14.981561 microviewer-1.6.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.0/setup.py
```

### Comparing `microviewer-1.5.0/ChangeLog` & `microviewer-1.6.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+1.6.0
+-----
+
+* feat: adds invert selection
+* docs: numpy format link
+* docs: add feature highlights
+* docs: update demo image
+
 1.5.0
 -----
 
 * fix: undo/redo seemingly working now
 * feat: add date to file names
 * feat: adjust canvas dimensions on axis rotation
 * feat: add controls info about ctrl+z and ctrl+shift+z (undo/redo)
```

### Comparing `microviewer-1.5.0/LICENSE` & `microviewer-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/PKG-INFO` & `microviewer-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.5.0
+Version: 1.6.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,23 @@
 uview labels.npy.gz --seg # view as segmentation
 ```
 
 ![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
 
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
+## Features
+
+- 3 axis visualization of 3D images.
+- Grayscale images with segmentation overlay.
+- Segmentation selection with brush tools.
+- Direct voxel painting.
+- Save segmentation as [.npy](https://numpy.org/neps/nep-0001-npy-format.html) or [.ckl](https://github.com/seung-lab/crackle), an advanced compresssion format.
+- Undo/Redo
+
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
```

### Comparing `microviewer-1.5.0/README.md` & `microviewer-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 uview labels.npy.gz --seg # view as segmentation
 ```
 
 ![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
 
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
+## Features
+
+- 3 axis visualization of 3D images.
+- Grayscale images with segmentation overlay.
+- Segmentation selection with brush tools.
+- Direct voxel painting.
+- Save segmentation as [.npy](https://numpy.org/neps/nep-0001-npy-format.html) or [.ckl](https://github.com/seung-lab/crackle), an advanced compresssion format.
+- Undo/Redo
+
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
```

### Comparing `microviewer-1.5.0/microviewer/__init__.py` & `microviewer-1.6.0/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/crackle.js` & `microviewer-1.6.0/microviewer/crackle.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/exact-active.png` & `microviewer-1.6.0/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/exact.png` & `microviewer-1.6.0/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/large-active.png` & `microviewer-1.6.0/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/large.png` & `microviewer-1.6.0/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/medium-active.png` & `microviewer-1.6.0/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/cursors/medium.png` & `microviewer-1.6.0/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/datacube.js` & `microviewer-1.6.0/microviewer/datacube.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -203,14 +203,32 @@
     selected() {
         let _this = this;
         return Object.keys(_this.segments)
             .filter((segid) => _this.segments[segid])
             .map((segid) => _this.renumbering[segid]);
     }
 
+    getInvertedSelection() {
+        let _this = this;
+        let new_selection = {};
+        for (let i = _this.renumbering.length - 1; i >= 0; i--) {
+            let segid = _this.renumbering[i];
+            if (segid === 0) {
+                continue;
+            } else if (!_this.segments[i]) {
+                new_selection[i] = true;
+            }
+        }
+        return new_selection;
+    }
+
+    invertSelection() {
+        this.segments = this.getInvertedSelection();
+    }
+
     get(x, y, z) {
         return this.renumbering[this.channel.get(x, y, z)];
     }
 
     getSegmentation() {
         return this.channel;
     }
```

### Comparing `microviewer-1.5.0/microviewer/favicon.ico` & `microviewer-1.6.0/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/index.html` & `microviewer-1.6.0/microviewer/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,23 @@
         background: #0d0d0d;
       }
 
       #infobar {
         margin-bottom: 10px;
       }
 
+      #brush-tools {
+        display: flex;
+        justify-content: left;
+      }
+
+      #invert-selection {
+        margin-left: 5px;
+      }
+
       #brush-size {
         height: 35px;
         
         display: flex;
         flex-direction: row;
         align-items: center;
         justify-content: space-around;
@@ -323,17 +332,20 @@
               return false;
             }
 
             return arr1.every( (v,i) => v === arr2[i] );
           }
         }
         
-        push () {
+        push (action) {
           let item = null;
-          if (elems.paintmode.prop("checked")) {
+          if (
+            (action === undefined && elems.paintmode.prop("checked"))
+            || (action === 'paint')
+          ) {
             let img2d = vol.getSegmentation().slice(AXIS, SLICE[AXIS], true);
             item = [ 'paint', [ img2d, AXIS, SLICE[AXIS] ] ];
           }
           else {
             item = [ 'select', [ structuredClone(vol.segments) ] ];
           }
 
@@ -745,14 +757,15 @@
             .split(",")
             .map((x) => BigInt(x))
             .forEach((segid) => vol.selectSegment(segid));
 
           elems.addsegs.val("");
           elems.addsegs.blur();
           vol.hover_id = null;
+          Undo.push('select');
           render(true);
         });
 
         elems.rtsidebar.on('wheel', function (e) {
           e.stopPropagation();
         });
       });
@@ -824,14 +837,17 @@
           BRUSH = Math.max(BRUSH - 1, 0);
           render(true);
         }
         else if (evt.keyCode === 'E'.charCodeAt(0)) {
           BRUSH = Math.min(BRUSH + 1, 3);
           render(true);
         }
+        else if (evt.keyCode === "I".charCodeAt(0)) {
+          invertSelection();
+        }
         else if (
           evt.keyCode === 'Z'.charCodeAt(0) && evt.ctrlKey
         ) {
           if (evt.shiftKey) {
             UNDO.redo();
           }
           else {
@@ -1177,14 +1193,19 @@
 
       function saveCrackle () {
         let d = new Date();
         let filename = `image-${d.getFullYear()}-${d.getMonth()}-${d.getDay()}.ckl`;
         vol.getSegmentation().saveCrackle(filename);
       }
 
+      function invertSelection () {
+        vol.invertSelection();
+        UNDO.push('select');
+        render(true);
+      }
     </script>
   </head>
   <body>
     <div id="infobar">
       <span id="axis"></span> <span id="magnification"></span> <span id="coord"></span> <span id="realcoord"></span> <span id="pxvalue"></span> 
       <br> 
       Last Click: <span id="clickcoord"></span> <span id="clickrealcoord"></span> <span id="clickpxvalue"></span>  <span id="loading"></span>
@@ -1213,19 +1234,22 @@
 
         <p class="segmentation">SELECTION VISIBILITY</p>
         <input class="segmentation" type="checkbox" id="show_hover" name="show_hover" checked="checked"/> <label class="segmentation" for="show_hover">Highlight (H)over?</label>
         <input class="segmentation" type="checkbox" id="show_unselected" name="show_unselected" /> <label class="segmentation" for="show_unselected">Show (U)nselected?</label> <br />
         <input class="segmentation" type="checkbox" id="paint_voxels" name="paint_voxels" /> <label class="segmentation" for="paint_voxels">Direct (P)aint?</label>
 
         <p class="segmentation">BRUSH SIZE</p>
-        <div class="segmentation" id="brush-size">
-          <div class="exact"></div>
-          <div class="small"></div>
-          <div class="medium"></div>
-          <div class="large"></div>
+        <div id="brush-tools" class="segmentation">
+          <div id="brush-size">
+            <div class="exact"></div>
+            <div class="small"></div>
+            <div class="medium"></div>
+            <div class="large"></div>
+          </div>
+          <button id="invert-selection" onclick="invertSelection()">invert selection</button>
         </div>
 
         <p class="segmentation">PAINT LABEL</p>
         <div class="segmentation">
           <input id="paintlabel" type="number" value="1" />
         </div>
 
@@ -1249,14 +1273,15 @@
           <li>Left Click - <span class="segmentation">paint, </span>freeze info about current pixel</li>
           <li class="segmentation">Right Click - erase</li>
           <li class="segmentation">X - clear selected segments</li>
           <li class="hyperview">+/- increase, decrease opacity</li>
           <li class='segmentation'>H - toggle hover highlight</li>
           <li class='segmentation'>U - toggle show unselected</li>
           <li class='segmentation'>P - toggle direct voxel painting</li>
+          <li class='segmentation'>I - invert selection</li>
           <li>1/2 - zoom out/in</li>
           <li>M - show/hide menu</li>
           <li class="segmentation">Q/E - decrease/increase brush size</li>
           <li class="segmentation">ctrl+Z - undo</li>
           <li class="segmentation">ctrl+shift+Z - redo</li>
         </ul>
       </div>
```

#### html2text {}

```diff
@@ -17,14 +17,15 @@
 > dtype:
 resolution:  nm3
 memory:
 SELECTION VISIBILITY
 * Highlight (H)over? ⁰ Show (U)nselected?
 ⁰ Direct (P)aint?
 BRUSH SIZE
+invert selection
 PAINT LABEL
 [Unknown INPUT type]
 SELECTED SEGMENTS copy
 SAVE SEGMENTATION
 .npy .ckl
 CONTROLS
     * W/S ,/. or scroll - advance selected images
@@ -34,12 +35,13 @@
     * Left Click - paint, freeze info about current pixel
     * Right Click - erase
     * X - clear selected segments
     * +/- increase, decrease opacity
     * H - toggle hover highlight
     * U - toggle show unselected
     * P - toggle direct voxel painting
+    * I - invert selection
     * 1/2 - zoom out/in
     * M - show/hide menu
     * Q/E - decrease/increase brush size
     * ctrl+Z - undo
     * ctrl+shift+Z - redo
```

### Comparing `microviewer-1.5.0/microviewer/jquery-3.7.0.min.js` & `microviewer-1.6.0/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer/libcrackle.wasm` & `microviewer-1.6.0/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer.egg-info/PKG-INFO` & `microviewer-1.6.0/microviewer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.5.0
+Version: 1.6.0
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,23 @@
 uview labels.npy.gz --seg # view as segmentation
 ```
 
 ![Segmentation display in microviewer](seg-demo.png "Segmentation display in microviewer.")
 
 Visualize 3D numpy arrays in your browser without difficult installation procedures or reformatting your data.  The code is CPU based and the image is uncompressed in memory. You're limited to images that are at most 2^31 bytes large (~2.1 GB) due to browser limitations.
 
+## Features
+
+- 3 axis visualization of 3D images.
+- Grayscale images with segmentation overlay.
+- Segmentation selection with brush tools.
+- Direct voxel painting.
+- Save segmentation as [.npy](https://numpy.org/neps/nep-0001-npy-format.html) or [.ckl](https://github.com/seung-lab/crackle), an advanced compresssion format.
+- Undo/Redo
+
 ## Supports
 
 - 8-bit grayscale 3D images
 - color images (including 3 channel 3D images)
 - floating point images
 - boolean images
 - segmentation labels
```

### Comparing `microviewer-1.5.0/microviewer.egg-info/SOURCES.txt` & `microviewer-1.6.0/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/microviewer_cli/cli.py` & `microviewer-1.6.0/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.5.0/setup.cfg` & `microviewer-1.6.0/setup.cfg`

 * *Files identical despite different names*

