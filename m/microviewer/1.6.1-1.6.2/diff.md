# Comparing `tmp/microviewer-1.6.1.tar.gz` & `tmp/microviewer-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microviewer-1.6.1.tar", last modified: Tue Jul  4 05:00:02 2023, max compression
+gzip compressed data, was "microviewer-1.6.2.tar", last modified: Tue Jul  4 05:44:26 2023, max compression
```

## Comparing `microviewer-1.6.1.tar` & `microviewer-1.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.466029 microviewer-1.6.1/
--rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 05:00:02.000000 microviewer-1.6.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     3504 2023-07-04 05:00:02.000000 microviewer-1.6.1/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.1/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.1/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:00:02.466215 microviewer-1.6.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.1/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.459872 microviewer-1.6.1/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.1/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.1/microviewer/crackle.js
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.464903 microviewer-1.6.1/microviewer/cursors/
--rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/exact-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/exact.png
--rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/large-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/large.png
--rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/medium-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/medium.png
--rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/small-active.png
--rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.1/microviewer/cursors/small.png
--rw-r--r--   0 wms        (501) staff       (20)    42859 2023-07-04 04:58:01.000000 microviewer-1.6.1/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.1/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    36471 2023-07-04 04:35:18.000000 microviewer-1.6.1/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.1/microviewer/jquery-3.7.0.min.js
--rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.1/microviewer/libcrackle.wasm
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.462864 microviewer-1.6.1/microviewer.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.1/microviewer.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 05:00:02.000000 microviewer-1.6.1/microviewer.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:00:02.465664 microviewer-1.6.1/microviewer_cli/
--rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.1/microviewer_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.1/microviewer_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.1/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.1/seg-demo.png
--rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 05:00:02.466892 microviewer-1.6.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.1/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.531185 microviewer-1.6.2/
+-rw-r--r--   0 wms        (501) staff       (20)       52 2023-07-04 05:44:26.000000 microviewer-1.6.2/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     3615 2023-07-04 05:44:26.000000 microviewer-1.6.2/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    26526 2023-06-05 21:07:17.000000 microviewer-1.6.2/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       65 2023-06-30 16:44:34.000000 microviewer-1.6.2/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:44:26.531589 microviewer-1.6.2/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1987 2023-07-03 23:31:40.000000 microviewer-1.6.2/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.522198 microviewer-1.6.2/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     6155 2023-06-30 18:35:40.000000 microviewer-1.6.2/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     9574 2023-07-02 05:39:04.000000 microviewer-1.6.2/microviewer/crackle.js
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.529319 microviewer-1.6.2/microviewer/cursors/
+-rwxr-xr-x   0 wms        (501) staff       (20)      617 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/exact-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      612 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/exact.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      926 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/large-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      946 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/large.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      563 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/medium-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      560 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/medium.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      348 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/small-active.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      339 2023-06-23 03:27:00.000000 microviewer-1.6.2/microviewer/cursors/small.png
+-rw-r--r--   0 wms        (501) staff       (20)    42865 2023-07-04 05:42:09.000000 microviewer-1.6.2/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2023-06-05 21:09:00.000000 microviewer-1.6.2/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    36691 2023-07-04 05:42:24.000000 microviewer-1.6.2/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    87462 2023-06-06 04:26:20.000000 microviewer-1.6.2/microviewer/jquery-3.7.0.min.js
+-rwxr-xr-x   0 wms        (501) staff       (20)   333433 2023-07-03 19:24:55.000000 microviewer-1.6.2/microviewer/libcrackle.wasm
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.525299 microviewer-1.6.2/microviewer.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3001 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      871 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-06 04:24:32.000000 microviewer-1.6.2/microviewer.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       12 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       28 2023-07-04 05:44:26.000000 microviewer-1.6.2/microviewer.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-07-04 05:44:26.530638 microviewer-1.6.2/microviewer_cli/
+-rw-r--r--   0 wms        (501) staff       (20)       18 2023-06-06 04:44:54.000000 microviewer-1.6.2/microviewer_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     5009 2023-07-01 18:00:31.000000 microviewer-1.6.2/microviewer_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)       11 2023-06-06 04:58:06.000000 microviewer-1.6.2/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)  1240284 2023-07-03 23:07:14.000000 microviewer-1.6.2/seg-demo.png
+-rw-r--r--   0 wms        (501) staff       (20)     1032 2023-07-04 05:44:26.532683 microviewer-1.6.2/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      298 2023-06-28 20:10:25.000000 microviewer-1.6.2/setup.py
```

### Comparing `microviewer-1.6.1/ChangeLog` & `microviewer-1.6.2/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.6.2
+-----
+
+* fix: brushes are circular on rectangular images
+* fix: use pixelated image rendering in chrome
+
 1.6.1
 -----
 
 * perf: faster color assignment and rendering
 
 1.6.0
 -----
```

### Comparing `microviewer-1.6.1/LICENSE` & `microviewer-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/PKG-INFO` & `microviewer-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.1
+Version: 1.6.2
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.1/README.md` & `microviewer-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/__init__.py` & `microviewer-1.6.2/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/crackle.js` & `microviewer-1.6.2/microviewer/crackle.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/exact-active.png` & `microviewer-1.6.2/microviewer/cursors/exact-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/exact.png` & `microviewer-1.6.2/microviewer/cursors/exact.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/large-active.png` & `microviewer-1.6.2/microviewer/cursors/large-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/large.png` & `microviewer-1.6.2/microviewer/cursors/large.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/medium-active.png` & `microviewer-1.6.2/microviewer/cursors/medium-active.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/cursors/medium.png` & `microviewer-1.6.2/microviewer/cursors/medium.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/datacube.js` & `microviewer-1.6.2/microviewer/datacube.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -387,27 +387,27 @@
      * Required:
      *   d: 0..1, Diameter of the circle
      *   cx: 0..1, X coordinate of circle center
      *   cy: 0..1, Y coordinate of circle center
      *
      * Return: [ segids ]
      */
-    getSegsInCircle(axis, slice, d, cx, cy) {
+    getSegsInCircle(axis, slice, dx, dy, cx, cy) {
         let _this = this;
         let [width, height] = _this.getSegmentation().faceDimensions(axis);
 
         // Nullify anything outside the ellipse. Just like a GRE problem.
 
         let buffer = _this.getSegmentation().slice(axis, slice, /*copy=*/ false);
 
         cx = Math.floor(cx * width) + 0.5;
         cy = Math.floor(cy * height) + 0.5;
 
-        let dx = d * width,
-            dy = d * height;
+        dx *= width;
+        dy *= height;
 
         let rx = dx / 2,
             rx2 = dx * dx / 4,
             ry = dy / 2,
             ry2 = dy * dy / 4;
 
         let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
@@ -434,31 +434,31 @@
         }
 
         delete segids[0];
 
         return Object.keys(segids).map((segid) => parseInt(segid, 10));
     }
 
-    selectSegsInCircle(axis, slice, d, cx, cy) {
+    selectSegsInCircle(axis, slice, dx, dy, cx, cy) {
         let _this = this;
-        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
+        let segs = _this.getSegsInCircle(axis, slice, dx, dy, cx, cy);
         segs.forEach((segid) => {
             _this.segments[segid] = true;
         });
     }
 
-    eraseSegsInCircle(axis, slice, d, cx, cy) {
+    eraseSegsInCircle(axis, slice, dx, dy, cx, cy) {
         let _this = this;
-        let segs = _this.getSegsInCircle(axis, slice, d, cx, cy);
+        let segs = _this.getSegsInCircle(axis, slice, dx, dy, cx, cy);
         segs.forEach((segid) => {
             _this.segments[segid] = false;
         });
     }
 
-    paintCircle(axis, slice, d, cx, cy, label) {
+    paintCircle(axis, slice, dx, dy, cx, cy, label) {
         let _this = this;
         let [width, height] = _this.getSegmentation().faceDimensions(axis);
 
         if (_this.inverse_renumbering[label] === undefined) {
             _this.renumbering[_this.max_label] = label;
             _this.inverse_renumbering[label] = _this.max_label;
             _this.assigned_colors[_this.max_label] = _this.colorToUint32({
@@ -470,16 +470,16 @@
         }
         label = _this.inverse_renumbering[label];
         _this.segments[label] = true;
 
         cx = Math.floor(cx * width) + 0.5;
         cy = Math.floor(cy * height) + 0.5;
 
-        let dx = d * width,
-            dy = d * height;
+        dx *= width;
+        dy *= height;
 
         let rx = dx / 2,
             rx2 = dx * dx / 4,
             ry = dy / 2,
             ry2 = dy * dy / 4;
 
         let x0 = Math.max(0, Math.trunc(cx - rx) + 0.5),
```

### Comparing `microviewer-1.6.1/microviewer/favicon.ico` & `microviewer-1.6.2/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/index.html` & `microviewer-1.6.2/microviewer/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
         border: 1px dotted white;
         max-width: calc(100vw - 20px);
         max-height: calc(100vh - 100px);
         background: #0d0d0d;
         z-index: 10;
 
         image-rendering: crisp-edges;
+        image-rendering: pixelated; /* chrome  */
         transition: transform .4s ease,bottom .4s ease,left .4s ease;
         cursor: crosshair;
       }
 
       canvas.paintable.exact {
         cursor: url("./cursors/exact.png") 20 20.5, crosshair;
       }
@@ -471,54 +472,58 @@
           var x = evt.offsetX / $(channel).innerWidth(), 
             y = evt.offsetY / $(channel).innerHeight();
 
           x = clamp(x, 0, 0.999999999);
           y = clamp(y, 0, 0.999999999); 
 
           let diameter = BRUSH_DIAMETERS[BRUSH];
-          diameter /= $(channel).innerWidth();
+          let dx = diameter / $(channel).innerWidth();
+          let dy = diameter / $(channel).innerHeight();
 
           if (ZOOMED) {
-            diameter /= ZOOM_FACTOR;
+            dx /= ZOOM_FACTOR;
+            dy /= ZOOM_FACTOR;
           }
           
           if (evt.which === 1) {
             if (elems.paintmode.prop("checked")) {
               let label = parseInt(elems.paintlabel.val());
               if (!isNaN(label)) {
-                vol.paintCircle(AXIS, SLICE[AXIS], diameter, x, y, label);
+                vol.paintCircle(AXIS, SLICE[AXIS], dx, dy, x, y, label);
               }
             }
             else {
-              vol.selectSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+              vol.selectSegsInCircle(AXIS, SLICE[AXIS], dx, dy, x, y);
             }
           }
     
           render(true);
         }
 
         function erase (evt) {
           var x = evt.offsetX / $(channel).innerWidth(), 
             y = evt.offsetY / $(channel).innerHeight();
 
           x = clamp(x, 0, 0.999999999);
           y = clamp(y, 0, 0.999999999); 
 
           let diameter = BRUSH_DIAMETERS[BRUSH];
-          diameter /= $(channel).innerWidth();
+          let dx = diameter / $(channel).innerWidth();
+          let dy = diameter / $(channel).innerHeight();
 
           if (ZOOMED) {
-            diameter /= ZOOM_FACTOR;
+            dx /= ZOOM_FACTOR;
+            dy /= ZOOM_FACTOR;
           }
 
           if (elems.paintmode.prop("checked")) {
-            vol.paintCircle(AXIS, SLICE[AXIS], diameter, x, y, 0);
+            vol.paintCircle(AXIS, SLICE[AXIS], dx, dy, x, y, 0);
           }
           else {
-            vol.eraseSegsInCircle(AXIS, SLICE[AXIS], diameter, x, y);
+            vol.eraseSegsInCircle(AXIS, SLICE[AXIS], dx, dy, x, y);
           }
           render(true);  
         }
 
         if (vol.has_segmentation) {
           $(document).on("mousemove", function () {
             MOUSE_OVER_IMAGE = false;
```

### Comparing `microviewer-1.6.1/microviewer/jquery-3.7.0.min.js` & `microviewer-1.6.2/microviewer/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer/libcrackle.wasm` & `microviewer-1.6.2/microviewer/libcrackle.wasm`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer.egg-info/PKG-INFO` & `microviewer-1.6.2/microviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microviewer
-Version: 1.6.1
+Version: 1.6.2
 Summary: Visualize 3D numpy arrays in the browser.
 Home-page: https://github.com/seung-lab/microviewer/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microviewer-1.6.1/microviewer.egg-info/SOURCES.txt` & `microviewer-1.6.2/microviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/microviewer_cli/cli.py` & `microviewer-1.6.2/microviewer_cli/cli.py`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/seg-demo.png` & `microviewer-1.6.2/seg-demo.png`

 * *Files identical despite different names*

### Comparing `microviewer-1.6.1/setup.cfg` & `microviewer-1.6.2/setup.cfg`

 * *Files identical despite different names*

