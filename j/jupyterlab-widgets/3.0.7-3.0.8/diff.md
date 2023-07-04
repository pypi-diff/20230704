# Comparing `tmp/jupyterlab_widgets-3.0.7.tar.gz` & `tmp/jupyterlab_widgets-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_widgets-3.0.7.tar", last modified: Tue Mar 28 15:13:40 2023, max compression
+gzip compressed data, was "jupyterlab_widgets-3.0.8.tar", last modified: Tue Jul  4 15:06:35 2023, max compression
```

## Comparing `jupyterlab_widgets-3.0.7.tar` & `jupyterlab_widgets-3.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.960450 jupyterlab_widgets-3.0.7/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    13847 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/LICENSE
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      383 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/MANIFEST.in
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4102 2023-03-28 15:13:40.960577 jupyterlab_widgets-3.0.7/PKG-INFO
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     2741 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/README.md
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      197 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/install.json
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.955274 jupyterlab_widgets-3.0.7/jupyterlab_widgets/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      599 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets/__init__.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      124 2023-03-28 15:13:21.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets/_version.py
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.956200 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     4102 2023-03-28 15:13:40.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/PKG-INFO
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1370 2023-03-28 15:13:40.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        1 2023-03-28 15:13:40.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)        1 2023-03-28 15:13:40.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/not-zip-safe
--rw-r--r--   0 maartenbreddels   (501) staff       (20)       19 2023-03-28 15:13:40.000000 jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.956354 jupyterlab_widgets-3.0.7/labextension/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3274 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/package.json
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.952697 jupyterlab_widgets-3.0.7/labextension/schemas/
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.952819 jupyterlab_widgets-3.0.7/labextension/schemas/@jupyter-widgets/
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.956672 jupyterlab_widgets-3.0.7/labextension/schemas/@jupyter-widgets/jupyterlab-manager/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3158 2023-03-28 15:12:08.000000 jupyterlab_widgets-3.0.7/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      375 2023-03-28 15:12:08.000000 jupyterlab_widgets-3.0.7/labextension/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
-drwxr-xr-x   0 maartenbreddels   (501) staff       (20)        0 2023-03-28 15:13:40.960300 jupyterlab_widgets-3.0.7/labextension/static/
--rw-r--r--   0 maartenbreddels   (501) staff       (20)   155207 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/113.270dbb43db912c1b3723.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      160 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/113.270dbb43db912c1b3723.js.LICENSE.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    85596 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/134.402424ef4079078b2e0e.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    11740 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/150.1a6d6a3a0542a41bec5a.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    90194 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/291.0b98a9cbc7337e1749ed.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      475 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/291.0b98a9cbc7337e1749ed.js.LICENSE.txt
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    38441 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/345.03be96cd091aac4797a5.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)   111280 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/495.ea5e18a84b54f152ae61.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    24347 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/595.b7741b41fd98f8f3d844.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      584 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/596.340cb969418e72309eb4.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      187 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/61.21f571face17e35076c2.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    60062 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/644.7d1bff49f8e38fac4070.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    32828 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/699.2ea6ecfcddb8f3bb4732.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      584 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/965.b0caf50c6bbde92efb37.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    10634 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/remoteEntry.35e76720037cafa02724.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      118 2023-03-28 15:12:08.000000 jupyterlab_widgets-3.0.7/labextension/static/style.js
--rw-r--r--   0 maartenbreddels   (501) staff       (20)    40923 2023-03-28 15:12:10.000000 jupyterlab_widgets-3.0.7/labextension/static/third-party-licenses.json
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     3101 2023-03-28 15:12:27.000000 jupyterlab_widgets-3.0.7/package.json
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      496 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/pyproject.toml
--rw-r--r--   0 maartenbreddels   (501) staff       (20)     1371 2023-03-28 15:13:40.960974 jupyterlab_widgets-3.0.7/setup.cfg
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      907 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/setup.py
--rw-r--r--   0 maartenbreddels   (501) staff       (20)      310 2023-03-28 15:07:31.000000 jupyterlab_widgets-3.0.7/tsconfig.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    13847 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/LICENSE
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      383 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/MANIFEST.in
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     2741 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/README.md
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      197 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/install.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.803618 jupyterlab_widgets-3.0.8/jupyterlab_widgets/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      599 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets/__init__.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      124 2023-07-04 15:06:04.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets/_version.py
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.805618 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     4102 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1370 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)        1 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)       19 2023-07-04 15:06:35.000000 jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.805618 jupyterlab_widgets-3.0.8/labextension/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3532 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/package.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.801618 jupyterlab_widgets-3.0.8/labextension/schemas/
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.801618 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.806618 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3416 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      375 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
+drwxr-xr-x   0 martinrenou  (1000) martinrenou  (1000)        0 2023-07-04 15:06:35.810618 jupyterlab_widgets-3.0.8/labextension/static/
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   181710 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/113.6113d19fca7ff66ccc66.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      160 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/113.6113d19fca7ff66ccc66.js.LICENSE.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    85828 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/134.b4eddbb09f5fd50a4007.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    87175 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      218 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js.LICENSE.txt
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    11738 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/336.9f709c2076672b1bfe2b.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    38492 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/345.17494fea1ff555b26294.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)   111313 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/495.b58859516292ffe4bc96.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    24347 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/595.942a65706d9bc281d5ca.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/596.1f32fb4ed861227b46e2.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      187 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/61.21f571face17e35076c2.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    60054 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/644.52a1098a3a5f3e45abff.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    33147 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/699.e966b1425a7d4e8c3f4e.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      584 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/965.22fa53da8ad2a8da593a.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    10607 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/remoteEntry.98b8a827bfc5f86e95d2.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      118 2023-07-04 15:05:00.000000 jupyterlab_widgets-3.0.8/labextension/static/style.js
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)    40924 2023-07-04 15:05:09.000000 jupyterlab_widgets-3.0.8/labextension/static/third-party-licenses.json
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     3359 2023-07-04 15:05:15.000000 jupyterlab_widgets-3.0.8/package.json
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      496 2023-07-04 14:25:30.000000 jupyterlab_widgets-3.0.8/pyproject.toml
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)     1371 2023-07-04 15:06:35.811618 jupyterlab_widgets-3.0.8/setup.cfg
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      907 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/setup.py
+-rw-r--r--   0 martinrenou  (1000) martinrenou  (1000)      310 2023-03-22 12:27:09.000000 jupyterlab_widgets-3.0.8/tsconfig.json
```

### Comparing `jupyterlab_widgets-3.0.7/LICENSE` & `jupyterlab_widgets-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.7/PKG-INFO` & `jupyterlab_widgets-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_widgets
-Version: 3.0.7
+Version: 3.0.8
 Summary: Jupyter interactive widgets for JupyterLab
 Home-page: https://github.com/jupyter-widgets/ipywidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD-3-Clause
 Keywords: Interactive,Interpreter,Shell,Web,notebook,widgets,Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_widgets-3.0.7/README.md` & `jupyterlab_widgets-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.7/jupyterlab_widgets/__init__.py` & `jupyterlab_widgets-3.0.8/jupyterlab_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.7/jupyterlab_widgets.egg-info/PKG-INFO` & `jupyterlab_widgets-3.0.8/jupyterlab_widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-widgets
-Version: 3.0.7
+Version: 3.0.8
 Summary: Jupyter interactive widgets for JupyterLab
 Home-page: https://github.com/jupyter-widgets/ipywidgets
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD-3-Clause
 Keywords: Interactive,Interpreter,Shell,Web,notebook,widgets,Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/package.json` & `jupyterlab_widgets-3.0.8/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9193253968253967%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.5', '@jupyter-widgets/base-manager': '^1.0.6', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.6', '@jupyter-widgets/output': '^6.0.5', "*

 * *                   "'@jupyterlab/application': '^3.0.0 || ^4.0.0', '@jupyterlab/docregistry': "*

 * *                   "'^3.0.0 || ^4.0.0', '@jupyterlab/logconsole': '^3.0.0 || ^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.0.0 || ^4.0.0', '@jupyterlab/nbformat': '^3.0.0 || "*

 * *                   "^4.0.0', […]*

```diff
@@ -1,67 +1,65 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.4",
-        "@jupyter-widgets/base-manager": "^1.0.5",
-        "@jupyter-widgets/controls": "^5.0.5",
-        "@jupyter-widgets/output": "^6.0.4",
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/logconsole": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/outputarea": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/rendermime-interfaces": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/translation": "^3.0.0",
-        "@lumino/algorithm": "^1.9.1",
-        "@lumino/coreutils": "^1.11.1",
-        "@lumino/disposable": "^1.10.1",
-        "@lumino/properties": "^1.8.1",
-        "@lumino/signaling": "^1.10.1",
-        "@lumino/widgets": "^1.30.0",
+        "@jupyter-widgets/base": "^6.0.5",
+        "@jupyter-widgets/base-manager": "^1.0.6",
+        "@jupyter-widgets/controls": "^5.0.6",
+        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyterlab/application": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime-interfaces": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/services": "^6.0.0 || ^7.0.0",
+        "@jupyterlab/settingregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/translation": "^3.0.0 || ^4.0.0",
+        "@lumino/algorithm": "^1.11.1 || ^2.0.0",
+        "@lumino/coreutils": "^1.11.1 || ^2.1",
+        "@lumino/disposable": "^1.10.1 || ^2.1",
+        "@lumino/properties": "^1.8.1 || ^2.1",
+        "@lumino/signaling": "^1.10.1 || ^2.1",
+        "@lumino/widgets": "^1.30.0 || ^2.1",
         "@types/backbone": "1.4.14",
         "jquery": "^3.1.1",
         "semver": "^7.3.5"
     },
     "description": "The JupyterLab extension providing Jupyter widgets.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@jupyterlab/cells": "^3.0.0",
+        "@jupyterlab/builder": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/cells": "^3.0.0 || ^4.0.0",
+        "@types/jquery": "^3.5.16",
         "@types/semver": "^7.3.6",
         "@typescript-eslint/eslint-plugin": "^5.8.0",
         "@typescript-eslint/parser": "^5.8.0",
         "eslint": "^8.5.0",
         "eslint-config-prettier": "^8.3.0",
         "eslint-plugin-prettier": "^4.0.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.3.2",
         "rimraf": "^3.0.2",
+        "source-map-loader": "^4.0.1",
         "typescript": "~4.9.4"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
-    "gitHead": "80cef4439d02cd4865fcc6e9a00aeef124f95e82",
+    "gitHead": "5e86a96c0138b837a1b0e609f02dd79de71f5bd6",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.35e76720037cafa02724.js"
-        },
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -91,9 +89,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.7"
+    "version": "5.0.8"
 }
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig` & `jupyterlab_widgets-3.0.8/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8984920634920633%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.5', '@jupyter-widgets/base-manager': '^1.0.6', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.6', '@jupyter-widgets/output': '^6.0.5', "*

 * *                   "'@jupyterlab/application': '^3.0.0 || ^4.0.0', '@jupyterlab/docregistry': "*

 * *                   "'^3.0.0 || ^4.0.0', '@jupyterlab/logconsole': '^3.0.0 || ^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.0.0 || ^4.0.0', '@jupyterlab/nbformat': '^3.0.0 || "*

 * *                   "^4.0.0', […]*

```diff
@@ -1,61 +1,62 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.4",
-        "@jupyter-widgets/base-manager": "^1.0.5",
-        "@jupyter-widgets/controls": "^5.0.5",
-        "@jupyter-widgets/output": "^6.0.4",
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/logconsole": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/outputarea": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/rendermime-interfaces": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/translation": "^3.0.0",
-        "@lumino/algorithm": "^1.9.1",
-        "@lumino/coreutils": "^1.11.1",
-        "@lumino/disposable": "^1.10.1",
-        "@lumino/properties": "^1.8.1",
-        "@lumino/signaling": "^1.10.1",
-        "@lumino/widgets": "^1.30.0",
+        "@jupyter-widgets/base": "^6.0.5",
+        "@jupyter-widgets/base-manager": "^1.0.6",
+        "@jupyter-widgets/controls": "^5.0.6",
+        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyterlab/application": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime-interfaces": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/services": "^6.0.0 || ^7.0.0",
+        "@jupyterlab/settingregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/translation": "^3.0.0 || ^4.0.0",
+        "@lumino/algorithm": "^1.11.1 || ^2.0.0",
+        "@lumino/coreutils": "^1.11.1 || ^2.1",
+        "@lumino/disposable": "^1.10.1 || ^2.1",
+        "@lumino/properties": "^1.8.1 || ^2.1",
+        "@lumino/signaling": "^1.10.1 || ^2.1",
+        "@lumino/widgets": "^1.30.0 || ^2.1",
         "@types/backbone": "1.4.14",
         "jquery": "^3.1.1",
         "semver": "^7.3.5"
     },
     "description": "The JupyterLab extension providing Jupyter widgets.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@jupyterlab/cells": "^3.0.0",
+        "@jupyterlab/builder": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/cells": "^3.0.0 || ^4.0.0",
+        "@types/jquery": "^3.5.16",
         "@types/semver": "^7.3.6",
         "@typescript-eslint/eslint-plugin": "^5.8.0",
         "@typescript-eslint/parser": "^5.8.0",
         "eslint": "^8.5.0",
         "eslint-config-prettier": "^8.3.0",
         "eslint-plugin-prettier": "^4.0.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.3.2",
         "rimraf": "^3.0.2",
+        "source-map-loader": "^4.0.1",
         "typescript": "~4.9.4"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
-    "gitHead": "80cef4439d02cd4865fcc6e9a00aeef124f95e82",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
@@ -87,9 +88,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.7"
+    "version": "5.0.8"
 }
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/134.402424ef4079078b2e0e.js` & `jupyterlab_widgets-3.0.8/labextension/static/134.b4eddbb09f5fd50a4007.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -184,14 +184,18 @@
             e.exports = function(e) {
                 var n = t.nc;
                 n && e.setAttribute("nonce", n)
             }
         },
         4036: e => {
             e.exports = function(e) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
+                };
                 var n = e.insertStyleElement(e);
                 return {
                     update: function(t) {
                         ! function(e, n, t) {
                             var i = "";
                             t.supports && (i += "@supports (".concat(t.supports, ") {")), t.media && (i += "@media ".concat(t.media, " {"));
                             var r = void 0 !== t.layer;
@@ -236,24 +240,24 @@
             });
             var i = {};
             t.r(i), t.d(i, {
                 OUTPUT_WIDGET_VERSION: () => P,
                 OutputModel: () => U,
                 OutputView: () => k
             });
-            var r = t(4411),
-                o = t(6165),
-                a = t(2634),
-                d = t(9101),
-                s = t(8714),
-                l = t(8918),
-                g = t(5923),
-                p = t(5658),
-                c = t(1526),
-                u = t(3992);
+            var r = t(56),
+                o = t(1919),
+                a = t(4826),
+                d = t(4470),
+                s = t(9350),
+                l = t(6697),
+                g = t(7717),
+                p = t(3004),
+                c = t(7930),
+                u = t(8778);
             class w extends u.Panel {
                 constructor(e, n) {
                     super(), this._manager = new c.PromiseDelegate, this._rerenderMimeModel = null, this.mimeType = e.mimeType, n && (this.manager = n)
                 }
                 set manager(e) {
                     e.restored.connect(this._rerender, this), this._manager.resolve(e)
                 }
@@ -281,17 +285,17 @@
                 dispose() {
                     this.isDisposed || (this._manager = null, super.dispose())
                 }
                 _rerender() {
                     this._rerenderMimeModel && (this.node.textContent = "", this.removeClass("jupyter-widgets"), this.renderModel(this._rerenderMimeModel))
                 }
             }
-            var h = t(7193),
-                E = t(183),
-                b = t(1840),
+            var h = t(9890),
+                E = t(7482),
+                b = t(4901),
                 j = t(9e3);
             class y {
                 constructor() {
                     this._cache = Object.create(null)
                 }
                 set(e, n, t) {
                     if (e in this._cache || (this._cache[e] = Object.create(null)), n in this._cache[e]) throw `Version ${n} of key ${e} already registered.`;
@@ -457,15 +461,17 @@
                         "started" === n && t.saveState && this._saveState()
                     }))
                 }
                 _saveState() {
                     const e = this.get_state_sync({
                         drop_defaults: !0
                     });
-                    this._context.model.metadata.set("widgets", {
+                    this._context.model.setMetadata ? this._context.model.setMetadata("widgets", {
+                        "application/vnd.jupyter.widget-state+json": e
+                    }) : this._context.model.metadata.set("widgets", {
                         "application/vnd.jupyter.widget-state+json": e
                     })
                 }
                 _handleKernelConnectionStatusChange(e) {
                     "connected" === e && (this._kernelRestoreInProgress || this.restoreWidgets(this._context.model, {
                         loadKernel: !0,
                         loadNotebook: !1
@@ -487,15 +493,15 @@
                         } finally {
                             this._kernelRestoreInProgress = !1
                         }
                         t && await this._loadFromNotebook(e), this._restoredStatus = !0, this._restored.emit()
                     } catch (e) {}
                 }
                 async _loadFromNotebook(e) {
-                    const n = e.metadata.get("widgets");
+                    const n = e.getMetadata ? e.getMetadata("widgets") : e.metadata.get("widgets");
                     if (n && n[D]) {
                         let e = n[D];
                         e = this.filterExistingModelState(e), await this.set_state(e)
                     }
                 }
                 dispose() {
                     this.isDisposed || (this._context = null, super.dispose())
@@ -517,16 +523,16 @@
                 async clear_state() {
                     await super.clear_state(), this.setDirty()
                 }
                 setDirty() {
                     this._settings.saveState && (this._context.model.dirty = !0)
                 }
             }
-            var x = t(7787),
-                C = t(8097),
+            var x = t(8409),
+                C = t(3363),
                 R = t(2994),
                 A = t.n(R);
             const P = x.OUTPUT_WIDGET_VERSION;
             class U extends x.OutputModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         msg_id: "",
@@ -616,33 +622,33 @@
                 V = t.n(F),
                 G = t(937),
                 Y = {};
             Y.styleTagTransform = V(), Y.setAttributes = L(), Y.insert = N().bind(null, "head"), Y.domAPI = _(), Y.insertStyleElement = H(), B()(G.Z, Y), G.Z && G.Z.locals && G.Z.locals;
             var Z = t(5309),
                 K = {};
             K.styleTagTransform = V(), K.setAttributes = L(), K.insert = N().bind(null, "head"), K.domAPI = _(), K.insertStyleElement = H(), B()(Z.Z, K), Z.Z && Z.Z.locals && Z.Z.locals;
-            var J = t(4579),
-                $ = t(2856);
+            var J = t(4238),
+                $ = t(926);
             const X = [],
                 q = {
                     saveState: !1
                 };
 
             function* Q(e) {
                 for (const n of e.widgets)
                     if ("code" === n.model.type)
                         for (const e of n.outputArea.widgets)
-                            for (const n of (0, l.toArray)(e.children())) n instanceof w && (yield n)
+                            for (const n of Array.from(e.children())) n instanceof w && (yield n)
             }
 
             function* ee(e, n) {
                 const t = (0, l.filter)(e.shell.widgets(), (e => e.id.startsWith("LinkedOutputView-") && e.path === n));
-                for (const e of (0, l.toArray)(t))
-                    for (const n of (0, l.toArray)(e.children()))
-                        for (const e of (0, l.toArray)(n.children())) e instanceof w && (yield e)
+                for (const e of Array.from(t))
+                    for (const n of Array.from(e.children()))
+                        for (const e of Array.from(n.children())) e instanceof w && (yield e)
             }
 
             function* ne(...e) {
                 for (const n of e) yield* n
             }
 
             function te(e, n, t) {
@@ -742,15 +748,15 @@
                     autoStart: !0,
                     activate: (e, n) => {
                         n.registerWidget({
                             name: "@jupyter-widgets/controls",
                             version: I.N,
                             exports: () => new Promise(((e, n) => {
                                 t.e(863).then((n => {
-                                    e(t(2534))
+                                    e(t(6530))
                                 }).bind(null, t)).catch((e => {
                                     n(e)
                                 }))
                             }))
                         })
                     }
                 },
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/150.1a6d6a3a0542a41bec5a.js` & `jupyterlab_widgets-3.0.8/labextension/static/336.9f709c2076672b1bfe2b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 (self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || []).push([
-    [150], {
+    [336], {
         6110: (e, t, o) => {
             "use strict";
             o.r(t), o.d(t, {
                 CONTROL_COMM_PROTOCOL_VERSION: () => g,
                 CONTROL_COMM_TARGET: () => f,
                 CONTROL_COMM_TIMEOUT: () => p,
                 ManagerBase: () => v,
                 base64ToBuffer: () => d,
                 bufferToBase64: () => m,
                 bufferToHex: () => a,
                 hexToBuffer: () => i,
                 serialize_state: () => b
             });
-            var s = o(7193),
-                n = o(1526),
+            var s = o(9890),
+                n = o(7930),
                 r = o(5766);
             const l = ["00", "01", "02", "03", "04", "05", "06", "07", "08", "09", "0A", "0B", "0C", "0D", "0E", "0F", "10", "11", "12", "13", "14", "15", "16", "17", "18", "19", "1A", "1B", "1C", "1D", "1E", "1F", "20", "21", "22", "23", "24", "25", "26", "27", "28", "29", "2A", "2B", "2C", "2D", "2E", "2F", "30", "31", "32", "33", "34", "35", "36", "37", "38", "39", "3A", "3B", "3C", "3D", "3E", "3F", "40", "41", "42", "43", "44", "45", "46", "47", "48", "49", "4A", "4B", "4C", "4D", "4E", "4F", "50", "51", "52", "53", "54", "55", "56", "57", "58", "59", "5A", "5B", "5C", "5D", "5E", "5F", "60", "61", "62", "63", "64", "65", "66", "67", "68", "69", "6A", "6B", "6C", "6D", "6E", "6F", "70", "71", "72", "73", "74", "75", "76", "77", "78", "79", "7A", "7B", "7C", "7D", "7E", "7F", "80", "81", "82", "83", "84", "85", "86", "87", "88", "89", "8A", "8B", "8C", "8D", "8E", "8F", "90", "91", "92", "93", "94", "95", "96", "97", "98", "99", "9A", "9B", "9C", "9D", "9E", "9F", "A0", "A1", "A2", "A3", "A4", "A5", "A6", "A7", "A8", "A9", "AA", "AB", "AC", "AD", "AE", "AF", "B0", "B1", "B2", "B3", "B4", "B5", "B6", "B7", "B8", "B9", "BA", "BB", "BC", "BD", "BE", "BF", "C0", "C1", "C2", "C3", "C4", "C5", "C6", "C7", "C8", "C9", "CA", "CB", "CC", "CD", "CE", "CF", "D0", "D1", "D2", "D3", "D4", "D5", "D6", "D7", "D8", "D9", "DA", "DB", "DC", "DD", "DE", "DF", "E0", "E1", "E2", "E3", "E4", "E5", "E6", "E7", "E8", "E9", "EA", "EB", "EC", "ED", "EE", "EF", "F0", "F1", "F2", "F3", "F4", "F5", "F6", "F7", "F8", "F9", "FA", "FB", "FC", "FD", "FE", "FF"];
 
             function a(e) {
                 const t = new Uint8Array(e),
                     o = [];
                 for (let e = 0; e < t.length; e++) o.push(l[t[e]]);
@@ -378,14 +378,14 @@
                 })), {
                     version_major: 2,
                     version_minor: 0,
                     state: o
                 }
             }
         },
-        6527: () => {},
-        6969: () => {},
-        2232: () => {},
-        4195: () => {},
-        3443: () => {}
+        764: () => {},
+        5158: () => {},
+        8635: () => {},
+        139: () => {},
+        3653: () => {}
     }
 ]);
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/291.0b98a9cbc7337e1749ed.js` & `jupyterlab_widgets-3.0.8/labextension/static/291.cff5ef71b29e18850479.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 291.0b98a9cbc7337e1749ed.js.LICENSE.txt */
+/*! For license information please see 291.cff5ef71b29e18850479.js.LICENSE.txt */
 (self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || []).push([
     [291], {
         8291: function(e, t) {
             var n;
             ! function(t, n) {
                 "use strict";
                 "object" == typeof e.exports ? e.exports = t.document ? n(t, !0) : function(e) {
@@ -47,24 +47,29 @@
                         for (r in b)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
                     n.head.appendChild(o).parentNode.removeChild(o)
                 }
 
                 function T(e) {
                     return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? f[p.call(e)] || "object" : typeof e
                 }
-                var C = "3.6.3",
+                var C = "3.7.0",
+                    k = /HTML$/i,
                     S = function(e, t) {
                         return new S.fn.init(e, t)
                     };
 
                 function E(e) {
                     var t = !!e && "length" in e && e.length,
                         n = T(e);
                     return !y(e) && !m(e) && ("array" === n || 0 === t || "number" == typeof t && t > 0 && t - 1 in e)
                 }
+
+                function j(e, t) {
+                    return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
+                }
                 S.fn = S.prototype = {
                     jquery: C,
                     constructor: S,
                     length: 0,
                     toArray: function() {
                         return s.call(this)
                     },
@@ -148,21 +153,37 @@
                         if (E(e))
                             for (n = e.length; r < n && !1 !== t.call(e[r], r, e[r]); r++);
                         else
                             for (r in e)
                                 if (!1 === t.call(e[r], r, e[r])) break;
                         return e
                     },
+                    text: function(e) {
+                        var t, n = "",
+                            r = 0,
+                            i = e.nodeType;
+                        if (i) {
+                            if (1 === i || 9 === i || 11 === i) return e.textContent;
+                            if (3 === i || 4 === i) return e.nodeValue
+                        } else
+                            for (; t = e[r++];) n += S.text(t);
+                        return n
+                    },
                     makeArray: function(e, t) {
                         var n = t || [];
                         return null != e && (E(Object(e)) ? S.merge(n, "string" == typeof e ? [e] : e) : l.call(n, e)), n
                     },
                     inArray: function(e, t, n) {
                         return null == t ? -1 : c.call(t, e, n)
                     },
+                    isXMLDoc: function(e) {
+                        var t = e && e.namespaceURI,
+                            n = e && (e.ownerDocument || e).documentElement;
+                        return !k.test(t || n && n.nodeName || "HTML")
+                    },
                     merge: function(e, t) {
                         for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
                         return e.length = i, e
                     },
                     grep: function(e, t, n) {
                         for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
                         return r
@@ -177,331 +198,266 @@
                         return u(a)
                     },
                     guid: 1,
                     support: v
                 }), "function" == typeof Symbol && (S.fn[Symbol.iterator] = o[Symbol.iterator]), S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), (function(e, t) {
                     f["[object " + t + "]"] = t.toLowerCase()
                 }));
-                var k = function(e) {
-                    var t, n, r, i, o, a, s, u, l, c, f, p, d, h, g, v, y, m, x, b = "sizzle" + 1 * new Date,
-                        w = e.document,
-                        T = 0,
-                        C = 0,
-                        S = ue(),
-                        E = ue(),
-                        k = ue(),
-                        A = ue(),
-                        j = function(e, t) {
-                            return e === t && (f = !0), 0
-                        },
-                        N = {}.hasOwnProperty,
-                        D = [],
-                        q = D.pop,
-                        L = D.push,
-                        H = D.push,
-                        O = D.slice,
-                        P = function(e, t) {
-                            for (var n = 0, r = e.length; n < r; n++)
-                                if (e[n] === t) return n;
-                            return -1
-                        },
-                        R = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
-                        M = "[\\x20\\t\\r\\n\\f]",
-                        I = "(?:\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
-                        W = "\\[" + M + "*(" + I + ")(?:" + M + "*([*^$|!~]?=)" + M + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + I + "))|)" + M + "*\\]",
-                        F = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
-                        $ = new RegExp(M + "+", "g"),
-                        B = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
-                        _ = new RegExp("^" + M + "*," + M + "*"),
-                        z = new RegExp("^" + M + "*([>+~]|" + M + ")" + M + "*"),
-                        U = new RegExp(M + "|>"),
-                        X = new RegExp(F),
-                        V = new RegExp("^" + I + "$"),
-                        G = {
-                            ID: new RegExp("^#(" + I + ")"),
-                            CLASS: new RegExp("^\\.(" + I + ")"),
-                            TAG: new RegExp("^(" + I + "|[*])"),
-                            ATTR: new RegExp("^" + W),
-                            PSEUDO: new RegExp("^" + F),
-                            CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + M + "*(even|odd|(([+-]|)(\\d*)n|)" + M + "*(?:([+-]|)" + M + "*(\\d+)|))" + M + "*\\)|)", "i"),
-                            bool: new RegExp("^(?:" + R + ")$", "i"),
-                            needsContext: new RegExp("^" + M + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + M + "*((?:-\\d)?\\d*)" + M + "*\\)|)(?=[^-]|$)", "i")
-                        },
-                        Y = /HTML$/i,
-                        Q = /^(?:input|select|textarea|button)$/i,
-                        J = /^h\d$/i,
-                        K = /^[^{]+\{\s*\[native \w/,
-                        Z = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-                        ee = /[+~]/,
-                        te = new RegExp("\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\([^\\r\\n\\f])", "g"),
-                        ne = function(e, t) {
+                var A = o.pop,
+                    D = o.sort,
+                    N = o.splice,
+                    q = "[\\x20\\t\\r\\n\\f]",
+                    L = new RegExp("^" + q + "+|((?:^|[^\\\\])(?:\\\\.)*)" + q + "+$", "g");
+                S.contains = function(e, t) {
+                    var n = t && t.parentNode;
+                    return e === n || !(!n || 1 !== n.nodeType || !(e.contains ? e.contains(n) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(n)))
+                };
+                var H = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\x80-\uFFFF\w-]/g;
+
+                function O(e, t) {
+                    return t ? "\0" === e ? "�" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
+                }
+                S.escapeSelector = function(e) {
+                    return (e + "").replace(H, O)
+                };
+                var P = x,
+                    R = l;
+                ! function() {
+                    var e, t, n, i, a, u, l, f, p, h, g = R,
+                        y = S.expando,
+                        m = 0,
+                        x = 0,
+                        b = ee(),
+                        w = ee(),
+                        T = ee(),
+                        C = ee(),
+                        k = function(e, t) {
+                            return e === t && (a = !0), 0
+                        },
+                        E = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+                        H = "(?:\\\\[\\da-fA-F]{1,6}" + q + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
+                        O = "\\[" + q + "*(" + H + ")(?:" + q + "*([*^$|!~]?=)" + q + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + H + "))|)" + q + "*\\]",
+                        M = ":(" + H + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + O + ")*)|.*)\\)|)",
+                        I = new RegExp(q + "+", "g"),
+                        W = new RegExp("^" + q + "*," + q + "*"),
+                        F = new RegExp("^" + q + "*([>+~]|" + q + ")" + q + "*"),
+                        $ = new RegExp(q + "|>"),
+                        _ = new RegExp(M),
+                        B = new RegExp("^" + H + "$"),
+                        X = {
+                            ID: new RegExp("^#(" + H + ")"),
+                            CLASS: new RegExp("^\\.(" + H + ")"),
+                            TAG: new RegExp("^(" + H + "|[*])"),
+                            ATTR: new RegExp("^" + O),
+                            PSEUDO: new RegExp("^" + M),
+                            CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + q + "*(even|odd|(([+-]|)(\\d*)n|)" + q + "*(?:([+-]|)" + q + "*(\\d+)|))" + q + "*\\)|)", "i"),
+                            bool: new RegExp("^(?:" + E + ")$", "i"),
+                            needsContext: new RegExp("^" + q + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + q + "*((?:-\\d)?\\d*)" + q + "*\\)|)(?=[^-]|$)", "i")
+                        },
+                        U = /^(?:input|select|textarea|button)$/i,
+                        z = /^h\d$/i,
+                        V = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
+                        G = /[+~]/,
+                        Y = new RegExp("\\\\[\\da-fA-F]{1,6}" + q + "?|\\\\([^\\r\\n\\f])", "g"),
+                        Q = function(e, t) {
                             var n = "0x" + e.slice(1) - 65536;
                             return t || (n < 0 ? String.fromCharCode(n + 65536) : String.fromCharCode(n >> 10 | 55296, 1023 & n | 56320))
                         },
-                        re = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
-                        ie = function(e, t) {
-                            return t ? "\0" === e ? "�" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
-                        },
-                        oe = function() {
-                            p()
+                        J = function() {
+                            ue()
                         },
-                        ae = be((function(e) {
-                            return !0 === e.disabled && "fieldset" === e.nodeName.toLowerCase()
+                        K = pe((function(e) {
+                            return !0 === e.disabled && j(e, "fieldset")
                         }), {
                             dir: "parentNode",
                             next: "legend"
                         });
                     try {
-                        H.apply(D = O.call(w.childNodes), w.childNodes), D[w.childNodes.length].nodeType
+                        g.apply(o = s.call(P.childNodes), P.childNodes), o[P.childNodes.length].nodeType
                     } catch (e) {
-                        H = {
-                            apply: D.length ? function(e, t) {
-                                L.apply(e, O.call(t))
-                            } : function(e, t) {
-                                for (var n = e.length, r = 0; e[n++] = t[r++];);
-                                e.length = n - 1
+                        g = {
+                            apply: function(e, t) {
+                                R.apply(e, s.call(t))
+                            },
+                            call: function(e) {
+                                R.apply(e, s.call(arguments, 1))
                             }
                         }
                     }
 
-                    function se(e, t, r, i) {
-                        var o, s, l, c, f, h, y, m = t && t.ownerDocument,
-                            w = t ? t.nodeType : 9;
-                        if (r = r || [], "string" != typeof e || !e || 1 !== w && 9 !== w && 11 !== w) return r;
-                        if (!i && (p(t), t = t || d, g)) {
-                            if (11 !== w && (f = Z.exec(e)))
-                                if (o = f[1]) {
-                                    if (9 === w) {
-                                        if (!(l = t.getElementById(o))) return r;
-                                        if (l.id === o) return r.push(l), r
-                                    } else if (m && (l = m.getElementById(o)) && x(t, l) && l.id === o) return r.push(l), r
+                    function Z(e, t, n, r) {
+                        var i, o, a, s, l, c, d, h = t && t.ownerDocument,
+                            m = t ? t.nodeType : 9;
+                        if (n = n || [], "string" != typeof e || !e || 1 !== m && 9 !== m && 11 !== m) return n;
+                        if (!r && (ue(t), t = t || u, f)) {
+                            if (11 !== m && (l = V.exec(e)))
+                                if (i = l[1]) {
+                                    if (9 === m) {
+                                        if (!(a = t.getElementById(i))) return n;
+                                        if (a.id === i) return g.call(n, a), n
+                                    } else if (h && (a = h.getElementById(i)) && Z.contains(t, a) && a.id === i) return g.call(n, a), n
                                 } else {
-                                    if (f[2]) return H.apply(r, t.getElementsByTagName(e)), r;
-                                    if ((o = f[3]) && n.getElementsByClassName && t.getElementsByClassName) return H.apply(r, t.getElementsByClassName(o)), r
-                                } if (n.qsa && !A[e + " "] && (!v || !v.test(e)) && (1 !== w || "object" !== t.nodeName.toLowerCase())) {
-                                if (y = e, m = t, 1 === w && (U.test(e) || z.test(e))) {
-                                    for ((m = ee.test(e) && ye(t.parentNode) || t) === t && n.scope || ((c = t.getAttribute("id")) ? c = c.replace(re, ie) : t.setAttribute("id", c = b)), s = (h = a(e)).length; s--;) h[s] = (c ? "#" + c : ":scope") + " " + xe(h[s]);
-                                    y = h.join(",")
+                                    if (l[2]) return g.apply(n, t.getElementsByTagName(e)), n;
+                                    if ((i = l[3]) && t.getElementsByClassName) return g.apply(n, t.getElementsByClassName(i)), n
+                                } if (!(C[e + " "] || p && p.test(e))) {
+                                if (d = e, h = t, 1 === m && ($.test(e) || F.test(e))) {
+                                    for ((h = G.test(e) && se(t.parentNode) || t) == t && v.scope || ((s = t.getAttribute("id")) ? s = S.escapeSelector(s) : t.setAttribute("id", s = y)), o = (c = ce(e)).length; o--;) c[o] = (s ? "#" + s : ":scope") + " " + fe(c[o]);
+                                    d = c.join(",")
                                 }
                                 try {
-                                    if (n.cssSupportsSelector && !CSS.supports("selector(:is(" + y + "))")) throw new Error;
-                                    return H.apply(r, m.querySelectorAll(y)), r
+                                    return g.apply(n, h.querySelectorAll(d)), n
                                 } catch (t) {
-                                    A(e, !0)
+                                    C(e, !0)
                                 } finally {
-                                    c === b && t.removeAttribute("id")
+                                    s === y && t.removeAttribute("id")
                                 }
                             }
                         }
-                        return u(e.replace(B, "$1"), t, r, i)
+                        return me(e.replace(L, "$1"), t, n, r)
                     }
 
-                    function ue() {
+                    function ee() {
                         var e = [];
-                        return function t(n, i) {
-                            return e.push(n + " ") > r.cacheLength && delete t[e.shift()], t[n + " "] = i
+                        return function n(r, i) {
+                            return e.push(r + " ") > t.cacheLength && delete n[e.shift()], n[r + " "] = i
                         }
                     }
 
-                    function le(e) {
-                        return e[b] = !0, e
+                    function te(e) {
+                        return e[y] = !0, e
                     }
 
-                    function ce(e) {
-                        var t = d.createElement("fieldset");
+                    function ne(e) {
+                        var t = u.createElement("fieldset");
                         try {
                             return !!e(t)
                         } catch (e) {
                             return !1
                         } finally {
                             t.parentNode && t.parentNode.removeChild(t), t = null
                         }
                     }
 
-                    function fe(e, t) {
-                        for (var n = e.split("|"), i = n.length; i--;) r.attrHandle[n[i]] = t
-                    }
-
-                    function pe(e, t) {
-                        var n = t && e,
-                            r = n && 1 === e.nodeType && 1 === t.nodeType && e.sourceIndex - t.sourceIndex;
-                        if (r) return r;
-                        if (n)
-                            for (; n = n.nextSibling;)
-                                if (n === t) return -1;
-                        return e ? 1 : -1
-                    }
-
-                    function de(e) {
+                    function re(e) {
                         return function(t) {
-                            return "input" === t.nodeName.toLowerCase() && t.type === e
+                            return j(t, "input") && t.type === e
                         }
                     }
 
-                    function he(e) {
+                    function ie(e) {
                         return function(t) {
-                            var n = t.nodeName.toLowerCase();
-                            return ("input" === n || "button" === n) && t.type === e
+                            return (j(t, "input") || j(t, "button")) && t.type === e
                         }
                     }
 
-                    function ge(e) {
+                    function oe(e) {
                         return function(t) {
-                            return "form" in t ? t.parentNode && !1 === t.disabled ? "label" in t ? "label" in t.parentNode ? t.parentNode.disabled === e : t.disabled === e : t.isDisabled === e || t.isDisabled !== !e && ae(t) === e : t.disabled === e : "label" in t && t.disabled === e
+                            return "form" in t ? t.parentNode && !1 === t.disabled ? "label" in t ? "label" in t.parentNode ? t.parentNode.disabled === e : t.disabled === e : t.isDisabled === e || t.isDisabled !== !e && K(t) === e : t.disabled === e : "label" in t && t.disabled === e
                         }
                     }
 
-                    function ve(e) {
-                        return le((function(t) {
-                            return t = +t, le((function(n, r) {
+                    function ae(e) {
+                        return te((function(t) {
+                            return t = +t, te((function(n, r) {
                                 for (var i, o = e([], n.length, t), a = o.length; a--;) n[i = o[a]] && (n[i] = !(r[i] = n[i]))
                             }))
                         }))
                     }
 
-                    function ye(e) {
+                    function se(e) {
                         return e && void 0 !== e.getElementsByTagName && e
                     }
-                    for (t in n = se.support = {}, o = se.isXML = function(e) {
-                            var t = e && e.namespaceURI,
-                                n = e && (e.ownerDocument || e).documentElement;
-                            return !Y.test(t || n && n.nodeName || "HTML")
-                        }, p = se.setDocument = function(e) {
-                            var t, i, a = e ? e.ownerDocument || e : w;
-                            return a != d && 9 === a.nodeType && a.documentElement ? (h = (d = a).documentElement, g = !o(d), w != d && (i = d.defaultView) && i.top !== i && (i.addEventListener ? i.addEventListener("unload", oe, !1) : i.attachEvent && i.attachEvent("onunload", oe)), n.scope = ce((function(e) {
-                                return h.appendChild(e).appendChild(d.createElement("div")), void 0 !== e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
-                            })), n.cssSupportsSelector = ce((function() {
-                                return CSS.supports("selector(*)") && d.querySelectorAll(":is(:jqfake)") && !CSS.supports("selector(:is(*,:jqfake))")
-                            })), n.attributes = ce((function(e) {
-                                return e.className = "i", !e.getAttribute("className")
-                            })), n.getElementsByTagName = ce((function(e) {
-                                return e.appendChild(d.createComment("")), !e.getElementsByTagName("*").length
-                            })), n.getElementsByClassName = K.test(d.getElementsByClassName), n.getById = ce((function(e) {
-                                return h.appendChild(e).id = b, !d.getElementsByName || !d.getElementsByName(b).length
-                            })), n.getById ? (r.filter.ID = function(e) {
-                                var t = e.replace(te, ne);
-                                return function(e) {
-                                    return e.getAttribute("id") === t
-                                }
-                            }, r.find.ID = function(e, t) {
-                                if (void 0 !== t.getElementById && g) {
-                                    var n = t.getElementById(e);
-                                    return n ? [n] : []
-                                }
-                            }) : (r.filter.ID = function(e) {
-                                var t = e.replace(te, ne);
-                                return function(e) {
-                                    var n = void 0 !== e.getAttributeNode && e.getAttributeNode("id");
-                                    return n && n.value === t
-                                }
-                            }, r.find.ID = function(e, t) {
-                                if (void 0 !== t.getElementById && g) {
-                                    var n, r, i, o = t.getElementById(e);
-                                    if (o) {
-                                        if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
-                                        for (i = t.getElementsByName(e), r = 0; o = i[r++];)
-                                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
-                                    }
-                                    return []
-                                }
-                            }), r.find.TAG = n.getElementsByTagName ? function(e, t) {
-                                return void 0 !== t.getElementsByTagName ? t.getElementsByTagName(e) : n.qsa ? t.querySelectorAll(e) : void 0
-                            } : function(e, t) {
-                                var n, r = [],
-                                    i = 0,
-                                    o = t.getElementsByTagName(e);
-                                if ("*" === e) {
-                                    for (; n = o[i++];) 1 === n.nodeType && r.push(n);
-                                    return r
-                                }
-                                return o
-                            }, r.find.CLASS = n.getElementsByClassName && function(e, t) {
-                                if (void 0 !== t.getElementsByClassName && g) return t.getElementsByClassName(e)
-                            }, y = [], v = [], (n.qsa = K.test(d.querySelectorAll)) && (ce((function(e) {
-                                var t;
-                                h.appendChild(e).innerHTML = "<a id='" + b + "'></a><select id='" + b + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && v.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || v.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + b + "-]").length || v.push("~="), (t = d.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || v.push("\\[" + M + "*name" + M + "*=" + M + "*(?:''|\"\")"), e.querySelectorAll(":checked").length || v.push(":checked"), e.querySelectorAll("a#" + b + "+*").length || v.push(".#.+[+~]"), e.querySelectorAll("\\\f"), v.push("[\\r\\n\\f]")
-                            })), ce((function(e) {
-                                e.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
-                                var t = d.createElement("input");
-                                t.setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), e.querySelectorAll("[name=d]").length && v.push("name" + M + "*[*^$|!~]?="), 2 !== e.querySelectorAll(":enabled").length && v.push(":enabled", ":disabled"), h.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && v.push(":enabled", ":disabled"), e.querySelectorAll("*,:x"), v.push(",.*:")
-                            }))), (n.matchesSelector = K.test(m = h.matches || h.webkitMatchesSelector || h.mozMatchesSelector || h.oMatchesSelector || h.msMatchesSelector)) && ce((function(e) {
-                                n.disconnectedMatch = m.call(e, "*"), m.call(e, "[s!='']:x"), y.push("!=", F)
-                            })), n.cssSupportsSelector || v.push(":has"), v = v.length && new RegExp(v.join("|")), y = y.length && new RegExp(y.join("|")), t = K.test(h.compareDocumentPosition), x = t || K.test(h.contains) ? function(e, t) {
-                                var n = 9 === e.nodeType && e.documentElement || e,
-                                    r = t && t.parentNode;
-                                return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
-                            } : function(e, t) {
-                                if (t)
-                                    for (; t = t.parentNode;)
-                                        if (t === e) return !0;
-                                return !1
-                            }, j = t ? function(e, t) {
-                                if (e === t) return f = !0, 0;
-                                var r = !e.compareDocumentPosition - !t.compareDocumentPosition;
-                                return r || (1 & (r = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !n.sortDetached && t.compareDocumentPosition(e) === r ? e == d || e.ownerDocument == w && x(w, e) ? -1 : t == d || t.ownerDocument == w && x(w, t) ? 1 : c ? P(c, e) - P(c, t) : 0 : 4 & r ? -1 : 1)
-                            } : function(e, t) {
-                                if (e === t) return f = !0, 0;
-                                var n, r = 0,
-                                    i = e.parentNode,
-                                    o = t.parentNode,
-                                    a = [e],
-                                    s = [t];
-                                if (!i || !o) return e == d ? -1 : t == d ? 1 : i ? -1 : o ? 1 : c ? P(c, e) - P(c, t) : 0;
-                                if (i === o) return pe(e, t);
-                                for (n = e; n = n.parentNode;) a.unshift(n);
-                                for (n = t; n = n.parentNode;) s.unshift(n);
-                                for (; a[r] === s[r];) r++;
-                                return r ? pe(a[r], s[r]) : a[r] == w ? -1 : s[r] == w ? 1 : 0
-                            }, d) : d
-                        }, se.matches = function(e, t) {
-                            return se(e, null, null, t)
-                        }, se.matchesSelector = function(e, t) {
-                            if (p(e), n.matchesSelector && g && !A[t + " "] && (!y || !y.test(t)) && (!v || !v.test(t))) try {
-                                var r = m.call(e, t);
-                                if (r || n.disconnectedMatch || e.document && 11 !== e.document.nodeType) return r
+
+                    function ue(e) {
+                        var n, r = e ? e.ownerDocument || e : P;
+                        return r != u && 9 === r.nodeType && r.documentElement ? (l = (u = r).documentElement, f = !S.isXMLDoc(u), h = l.matches || l.webkitMatchesSelector || l.msMatchesSelector, P != u && (n = u.defaultView) && n.top !== n && n.addEventListener("unload", J), v.getById = ne((function(e) {
+                            return l.appendChild(e).id = S.expando, !u.getElementsByName || !u.getElementsByName(S.expando).length
+                        })), v.disconnectedMatch = ne((function(e) {
+                            return h.call(e, "*")
+                        })), v.scope = ne((function() {
+                            return u.querySelectorAll(":scope")
+                        })), v.cssHas = ne((function() {
+                            try {
+                                return u.querySelector(":has(*,:jqfake)"), !1
                             } catch (e) {
-                                A(t, !0)
+                                return !0
                             }
-                            return se(t, d, null, [e]).length > 0
-                        }, se.contains = function(e, t) {
-                            return (e.ownerDocument || e) != d && p(e), x(e, t)
-                        }, se.attr = function(e, t) {
-                            (e.ownerDocument || e) != d && p(e);
-                            var i = r.attrHandle[t.toLowerCase()],
-                                o = i && N.call(r.attrHandle, t.toLowerCase()) ? i(e, t, !g) : void 0;
-                            return void 0 !== o ? o : n.attributes || !g ? e.getAttribute(t) : (o = e.getAttributeNode(t)) && o.specified ? o.value : null
-                        }, se.escape = function(e) {
-                            return (e + "").replace(re, ie)
-                        }, se.error = function(e) {
+                        })), v.getById ? (t.filter.ID = function(e) {
+                            var t = e.replace(Y, Q);
+                            return function(e) {
+                                return e.getAttribute("id") === t
+                            }
+                        }, t.find.ID = function(e, t) {
+                            if (void 0 !== t.getElementById && f) {
+                                var n = t.getElementById(e);
+                                return n ? [n] : []
+                            }
+                        }) : (t.filter.ID = function(e) {
+                            var t = e.replace(Y, Q);
+                            return function(e) {
+                                var n = void 0 !== e.getAttributeNode && e.getAttributeNode("id");
+                                return n && n.value === t
+                            }
+                        }, t.find.ID = function(e, t) {
+                            if (void 0 !== t.getElementById && f) {
+                                var n, r, i, o = t.getElementById(e);
+                                if (o) {
+                                    if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
+                                    for (i = t.getElementsByName(e), r = 0; o = i[r++];)
+                                        if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
+                                }
+                                return []
+                            }
+                        }), t.find.TAG = function(e, t) {
+                            return void 0 !== t.getElementsByTagName ? t.getElementsByTagName(e) : t.querySelectorAll(e)
+                        }, t.find.CLASS = function(e, t) {
+                            if (void 0 !== t.getElementsByClassName && f) return t.getElementsByClassName(e)
+                        }, p = [], ne((function(e) {
+                            var t;
+                            l.appendChild(e).innerHTML = "<a id='" + y + "' href='' disabled='disabled'></a><select id='" + y + "-\r\\' disabled='disabled'><option selected=''></option></select>", e.querySelectorAll("[selected]").length || p.push("\\[" + q + "*(?:value|" + E + ")"), e.querySelectorAll("[id~=" + y + "-]").length || p.push("~="), e.querySelectorAll("a#" + y + "+*").length || p.push(".#.+[+~]"), e.querySelectorAll(":checked").length || p.push(":checked"), (t = u.createElement("input")).setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), l.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && p.push(":enabled", ":disabled"), (t = u.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || p.push("\\[" + q + "*name" + q + "*=" + q + "*(?:''|\"\")")
+                        })), v.cssHas || p.push(":has"), p = p.length && new RegExp(p.join("|")), k = function(e, t) {
+                            if (e === t) return a = !0, 0;
+                            var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
+                            return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !v.sortDetached && t.compareDocumentPosition(e) === n ? e === u || e.ownerDocument == P && Z.contains(P, e) ? -1 : t === u || t.ownerDocument == P && Z.contains(P, t) ? 1 : i ? c.call(i, e) - c.call(i, t) : 0 : 4 & n ? -1 : 1)
+                        }, u) : u
+                    }
+                    for (e in Z.matches = function(e, t) {
+                            return Z(e, null, null, t)
+                        }, Z.matchesSelector = function(e, t) {
+                            if (ue(e), f && !C[t + " "] && (!p || !p.test(t))) try {
+                                var n = h.call(e, t);
+                                if (n || v.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
+                            } catch (e) {
+                                C(t, !0)
+                            }
+                            return Z(t, u, null, [e]).length > 0
+                        }, Z.contains = function(e, t) {
+                            return (e.ownerDocument || e) != u && ue(e), S.contains(e, t)
+                        }, Z.attr = function(e, n) {
+                            (e.ownerDocument || e) != u && ue(e);
+                            var r = t.attrHandle[n.toLowerCase()],
+                                i = r && d.call(t.attrHandle, n.toLowerCase()) ? r(e, n, !f) : void 0;
+                            return void 0 !== i ? i : e.getAttribute(n)
+                        }, Z.error = function(e) {
                             throw new Error("Syntax error, unrecognized expression: " + e)
-                        }, se.uniqueSort = function(e) {
-                            var t, r = [],
-                                i = 0,
-                                o = 0;
-                            if (f = !n.detectDuplicates, c = !n.sortStable && e.slice(0), e.sort(j), f) {
-                                for (; t = e[o++];) t === e[o] && (i = r.push(o));
-                                for (; i--;) e.splice(r[i], 1)
-                            }
-                            return c = null, e
-                        }, i = se.getText = function(e) {
-                            var t, n = "",
+                        }, S.uniqueSort = function(e) {
+                            var t, n = [],
                                 r = 0,
-                                o = e.nodeType;
-                            if (o) {
-                                if (1 === o || 9 === o || 11 === o) {
-                                    if ("string" == typeof e.textContent) return e.textContent;
-                                    for (e = e.firstChild; e; e = e.nextSibling) n += i(e)
-                                } else if (3 === o || 4 === o) return e.nodeValue
-                            } else
-                                for (; t = e[r++];) n += i(t);
-                            return n
-                        }, r = se.selectors = {
+                                o = 0;
+                            if (a = !v.sortStable, i = !v.sortStable && s.call(e, 0), D.call(e, k), a) {
+                                for (; t = e[o++];) t === e[o] && (r = n.push(o));
+                                for (; r--;) N.call(e, n[r], 1)
+                            }
+                            return i = null, e
+                        }, S.fn.uniqueSort = function() {
+                            return this.pushStack(S.uniqueSort(s.apply(this)))
+                        }, t = S.expr = {
                             cacheLength: 50,
-                            createPseudo: le,
-                            match: G,
+                            createPseudo: te,
+                            match: X,
                             attrHandle: {},
                             find: {},
                             relative: {
                                 ">": {
                                     dir: "parentNode",
                                     first: !0
                                 },
@@ -514,401 +470,391 @@
                                 },
                                 "~": {
                                     dir: "previousSibling"
                                 }
                             },
                             preFilter: {
                                 ATTR: function(e) {
-                                    return e[1] = e[1].replace(te, ne), e[3] = (e[3] || e[4] || e[5] || "").replace(te, ne), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
+                                    return e[1] = e[1].replace(Y, Q), e[3] = (e[3] || e[4] || e[5] || "").replace(Y, Q), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
                                 },
                                 CHILD: function(e) {
-                                    return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || se.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && se.error(e[0]), e
+                                    return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || Z.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && Z.error(e[0]), e
                                 },
                                 PSEUDO: function(e) {
                                     var t, n = !e[6] && e[2];
-                                    return G.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && X.test(n) && (t = a(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
+                                    return X.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && _.test(n) && (t = ce(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
                                 }
                             },
                             filter: {
                                 TAG: function(e) {
-                                    var t = e.replace(te, ne).toLowerCase();
+                                    var t = e.replace(Y, Q).toLowerCase();
                                     return "*" === e ? function() {
                                         return !0
                                     } : function(e) {
-                                        return e.nodeName && e.nodeName.toLowerCase() === t
+                                        return j(e, t)
                                     }
                                 },
                                 CLASS: function(e) {
-                                    var t = S[e + " "];
-                                    return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && S(e, (function(e) {
+                                    var t = b[e + " "];
+                                    return t || (t = new RegExp("(^|" + q + ")" + e + "(" + q + "|$)")) && b(e, (function(e) {
                                         return t.test("string" == typeof e.className && e.className || void 0 !== e.getAttribute && e.getAttribute("class") || "")
                                     }))
                                 },
                                 ATTR: function(e, t, n) {
                                     return function(r) {
-                                        var i = se.attr(r, e);
-                                        return null == i ? "!=" === t : !t || (i += "", "=" === t ? i === n : "!=" === t ? i !== n : "^=" === t ? n && 0 === i.indexOf(n) : "*=" === t ? n && i.indexOf(n) > -1 : "$=" === t ? n && i.slice(-n.length) === n : "~=" === t ? (" " + i.replace($, " ") + " ").indexOf(n) > -1 : "|=" === t && (i === n || i.slice(0, n.length + 1) === n + "-"))
+                                        var i = Z.attr(r, e);
+                                        return null == i ? "!=" === t : !t || (i += "", "=" === t ? i === n : "!=" === t ? i !== n : "^=" === t ? n && 0 === i.indexOf(n) : "*=" === t ? n && i.indexOf(n) > -1 : "$=" === t ? n && i.slice(-n.length) === n : "~=" === t ? (" " + i.replace(I, " ") + " ").indexOf(n) > -1 : "|=" === t && (i === n || i.slice(0, n.length + 1) === n + "-"))
                                     }
                                 },
                                 CHILD: function(e, t, n, r, i) {
                                     var o = "nth" !== e.slice(0, 3),
                                         a = "last" !== e.slice(-4),
                                         s = "of-type" === t;
                                     return 1 === r && 0 === i ? function(e) {
                                         return !!e.parentNode
                                     } : function(t, n, u) {
-                                        var l, c, f, p, d, h, g = o !== a ? "nextSibling" : "previousSibling",
-                                            v = t.parentNode,
-                                            y = s && t.nodeName.toLowerCase(),
-                                            m = !u && !s,
-                                            x = !1;
-                                        if (v) {
+                                        var l, c, f, p, d, h = o !== a ? "nextSibling" : "previousSibling",
+                                            g = t.parentNode,
+                                            v = s && t.nodeName.toLowerCase(),
+                                            x = !u && !s,
+                                            b = !1;
+                                        if (g) {
                                             if (o) {
-                                                for (; g;) {
-                                                    for (p = t; p = p[g];)
-                                                        if (s ? p.nodeName.toLowerCase() === y : 1 === p.nodeType) return !1;
-                                                    h = g = "only" === e && !h && "nextSibling"
+                                                for (; h;) {
+                                                    for (f = t; f = f[h];)
+                                                        if (s ? j(f, v) : 1 === f.nodeType) return !1;
+                                                    d = h = "only" === e && !d && "nextSibling"
                                                 }
                                                 return !0
                                             }
-                                            if (h = [a ? v.firstChild : v.lastChild], a && m) {
-                                                for (x = (d = (l = (c = (f = (p = v)[b] || (p[b] = {}))[p.uniqueID] || (f[p.uniqueID] = {}))[e] || [])[0] === T && l[1]) && l[2], p = d && v.childNodes[d]; p = ++d && p && p[g] || (x = d = 0) || h.pop();)
-                                                    if (1 === p.nodeType && ++x && p === t) {
-                                                        c[e] = [T, d, x];
+                                            if (d = [a ? g.firstChild : g.lastChild], a && x) {
+                                                for (b = (p = (l = (c = g[y] || (g[y] = {}))[e] || [])[0] === m && l[1]) && l[2], f = p && g.childNodes[p]; f = ++p && f && f[h] || (b = p = 0) || d.pop();)
+                                                    if (1 === f.nodeType && ++b && f === t) {
+                                                        c[e] = [m, p, b];
                                                         break
                                                     }
-                                            } else if (m && (x = d = (l = (c = (f = (p = t)[b] || (p[b] = {}))[p.uniqueID] || (f[p.uniqueID] = {}))[e] || [])[0] === T && l[1]), !1 === x)
+                                            } else if (x && (b = p = (l = (c = t[y] || (t[y] = {}))[e] || [])[0] === m && l[1]), !1 === b)
                                                 for (;
-                                                    (p = ++d && p && p[g] || (x = d = 0) || h.pop()) && ((s ? p.nodeName.toLowerCase() !== y : 1 !== p.nodeType) || !++x || (m && ((c = (f = p[b] || (p[b] = {}))[p.uniqueID] || (f[p.uniqueID] = {}))[e] = [T, x]), p !== t)););
-                                            return (x -= i) === r || x % r == 0 && x / r >= 0
+                                                    (f = ++p && f && f[h] || (b = p = 0) || d.pop()) && (!(s ? j(f, v) : 1 === f.nodeType) || !++b || (x && ((c = f[y] || (f[y] = {}))[e] = [m, b]), f !== t)););
+                                            return (b -= i) === r || b % r == 0 && b / r >= 0
                                         }
                                     }
                                 },
-                                PSEUDO: function(e, t) {
-                                    var n, i = r.pseudos[e] || r.setFilters[e.toLowerCase()] || se.error("unsupported pseudo: " + e);
-                                    return i[b] ? i(t) : i.length > 1 ? (n = [e, e, "", t], r.setFilters.hasOwnProperty(e.toLowerCase()) ? le((function(e, n) {
-                                        for (var r, o = i(e, t), a = o.length; a--;) e[r = P(e, o[a])] = !(n[r] = o[a])
+                                PSEUDO: function(e, n) {
+                                    var r, i = t.pseudos[e] || t.setFilters[e.toLowerCase()] || Z.error("unsupported pseudo: " + e);
+                                    return i[y] ? i(n) : i.length > 1 ? (r = [e, e, "", n], t.setFilters.hasOwnProperty(e.toLowerCase()) ? te((function(e, t) {
+                                        for (var r, o = i(e, n), a = o.length; a--;) e[r = c.call(e, o[a])] = !(t[r] = o[a])
                                     })) : function(e) {
-                                        return i(e, 0, n)
+                                        return i(e, 0, r)
                                     }) : i
                                 }
                             },
                             pseudos: {
-                                not: le((function(e) {
+                                not: te((function(e) {
                                     var t = [],
                                         n = [],
-                                        r = s(e.replace(B, "$1"));
-                                    return r[b] ? le((function(e, t, n, i) {
+                                        r = ye(e.replace(L, "$1"));
+                                    return r[y] ? te((function(e, t, n, i) {
                                         for (var o, a = r(e, null, i, []), s = e.length; s--;)(o = a[s]) && (e[s] = !(t[s] = o))
                                     })) : function(e, i, o) {
                                         return t[0] = e, r(t, null, o, n), t[0] = null, !n.pop()
                                     }
                                 })),
-                                has: le((function(e) {
+                                has: te((function(e) {
                                     return function(t) {
-                                        return se(e, t).length > 0
+                                        return Z(e, t).length > 0
                                     }
                                 })),
-                                contains: le((function(e) {
-                                    return e = e.replace(te, ne),
+                                contains: te((function(e) {
+                                    return e = e.replace(Y, Q),
                                         function(t) {
-                                            return (t.textContent || i(t)).indexOf(e) > -1
+                                            return (t.textContent || S.text(t)).indexOf(e) > -1
                                         }
                                 })),
-                                lang: le((function(e) {
-                                    return V.test(e || "") || se.error("unsupported lang: " + e), e = e.replace(te, ne).toLowerCase(),
+                                lang: te((function(e) {
+                                    return B.test(e || "") || Z.error("unsupported lang: " + e), e = e.replace(Y, Q).toLowerCase(),
                                         function(t) {
                                             var n;
                                             do {
-                                                if (n = g ? t.lang : t.getAttribute("xml:lang") || t.getAttribute("lang")) return (n = n.toLowerCase()) === e || 0 === n.indexOf(e + "-")
+                                                if (n = f ? t.lang : t.getAttribute("xml:lang") || t.getAttribute("lang")) return (n = n.toLowerCase()) === e || 0 === n.indexOf(e + "-")
                                             } while ((t = t.parentNode) && 1 === t.nodeType);
                                             return !1
                                         }
                                 })),
-                                target: function(t) {
-                                    var n = e.location && e.location.hash;
-                                    return n && n.slice(1) === t.id
+                                target: function(e) {
+                                    var t = r.location && r.location.hash;
+                                    return t && t.slice(1) === e.id
                                 },
                                 root: function(e) {
-                                    return e === h
+                                    return e === l
                                 },
                                 focus: function(e) {
-                                    return e === d.activeElement && (!d.hasFocus || d.hasFocus()) && !!(e.type || e.href || ~e.tabIndex)
+                                    return e === function() {
+                                        try {
+                                            return u.activeElement
+                                        } catch (e) {}
+                                    }() && u.hasFocus() && !!(e.type || e.href || ~e.tabIndex)
                                 },
-                                enabled: ge(!1),
-                                disabled: ge(!0),
+                                enabled: oe(!1),
+                                disabled: oe(!0),
                                 checked: function(e) {
-                                    var t = e.nodeName.toLowerCase();
-                                    return "input" === t && !!e.checked || "option" === t && !!e.selected
+                                    return j(e, "input") && !!e.checked || j(e, "option") && !!e.selected
                                 },
                                 selected: function(e) {
                                     return e.parentNode && e.parentNode.selectedIndex, !0 === e.selected
                                 },
                                 empty: function(e) {
                                     for (e = e.firstChild; e; e = e.nextSibling)
                                         if (e.nodeType < 6) return !1;
                                     return !0
                                 },
                                 parent: function(e) {
-                                    return !r.pseudos.empty(e)
+                                    return !t.pseudos.empty(e)
                                 },
                                 header: function(e) {
-                                    return J.test(e.nodeName)
+                                    return z.test(e.nodeName)
                                 },
                                 input: function(e) {
-                                    return Q.test(e.nodeName)
+                                    return U.test(e.nodeName)
                                 },
                                 button: function(e) {
-                                    var t = e.nodeName.toLowerCase();
-                                    return "input" === t && "button" === e.type || "button" === t
+                                    return j(e, "input") && "button" === e.type || j(e, "button")
                                 },
                                 text: function(e) {
                                     var t;
-                                    return "input" === e.nodeName.toLowerCase() && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
+                                    return j(e, "input") && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
                                 },
-                                first: ve((function() {
+                                first: ae((function() {
                                     return [0]
                                 })),
-                                last: ve((function(e, t) {
+                                last: ae((function(e, t) {
                                     return [t - 1]
                                 })),
-                                eq: ve((function(e, t, n) {
+                                eq: ae((function(e, t, n) {
                                     return [n < 0 ? n + t : n]
                                 })),
-                                even: ve((function(e, t) {
+                                even: ae((function(e, t) {
                                     for (var n = 0; n < t; n += 2) e.push(n);
                                     return e
                                 })),
-                                odd: ve((function(e, t) {
+                                odd: ae((function(e, t) {
                                     for (var n = 1; n < t; n += 2) e.push(n);
                                     return e
                                 })),
-                                lt: ve((function(e, t, n) {
-                                    for (var r = n < 0 ? n + t : n > t ? t : n; --r >= 0;) e.push(r);
+                                lt: ae((function(e, t, n) {
+                                    var r;
+                                    for (r = n < 0 ? n + t : n > t ? t : n; --r >= 0;) e.push(r);
                                     return e
                                 })),
-                                gt: ve((function(e, t, n) {
+                                gt: ae((function(e, t, n) {
                                     for (var r = n < 0 ? n + t : n; ++r < t;) e.push(r);
                                     return e
                                 }))
                             }
-                        }, r.pseudos.nth = r.pseudos.eq, {
+                        }, t.pseudos.nth = t.pseudos.eq, {
                             radio: !0,
                             checkbox: !0,
                             file: !0,
                             password: !0,
                             image: !0
-                        }) r.pseudos[t] = de(t);
-                    for (t in {
+                        }) t.pseudos[e] = re(e);
+                    for (e in {
                             submit: !0,
                             reset: !0
-                        }) r.pseudos[t] = he(t);
+                        }) t.pseudos[e] = ie(e);
 
-                    function me() {}
+                    function le() {}
 
-                    function xe(e) {
+                    function ce(e, n) {
+                        var r, i, o, a, s, u, l, c = w[e + " "];
+                        if (c) return n ? 0 : c.slice(0);
+                        for (s = e, u = [], l = t.preFilter; s;) {
+                            for (a in r && !(i = W.exec(s)) || (i && (s = s.slice(i[0].length) || s), u.push(o = [])), r = !1, (i = F.exec(s)) && (r = i.shift(), o.push({
+                                    value: r,
+                                    type: i[0].replace(L, " ")
+                                }), s = s.slice(r.length)), t.filter) !(i = X[a].exec(s)) || l[a] && !(i = l[a](i)) || (r = i.shift(), o.push({
+                                value: r,
+                                type: a,
+                                matches: i
+                            }), s = s.slice(r.length));
+                            if (!r) break
+                        }
+                        return n ? s.length : s ? Z.error(e) : w(e, u).slice(0)
+                    }
+
+                    function fe(e) {
                         for (var t = 0, n = e.length, r = ""; t < n; t++) r += e[t].value;
                         return r
                     }
 
-                    function be(e, t, n) {
+                    function pe(e, t, n) {
                         var r = t.dir,
                             i = t.next,
                             o = i || r,
                             a = n && "parentNode" === o,
-                            s = C++;
+                            s = x++;
                         return t.first ? function(t, n, i) {
                             for (; t = t[r];)
                                 if (1 === t.nodeType || a) return e(t, n, i);
                             return !1
                         } : function(t, n, u) {
-                            var l, c, f, p = [T, s];
+                            var l, c, f = [m, s];
                             if (u) {
                                 for (; t = t[r];)
                                     if ((1 === t.nodeType || a) && e(t, n, u)) return !0
                             } else
                                 for (; t = t[r];)
                                     if (1 === t.nodeType || a)
-                                        if (c = (f = t[b] || (t[b] = {}))[t.uniqueID] || (f[t.uniqueID] = {}), i && i === t.nodeName.toLowerCase()) t = t[r] || t;
+                                        if (c = t[y] || (t[y] = {}), i && j(t, i)) t = t[r] || t;
                                         else {
-                                            if ((l = c[o]) && l[0] === T && l[1] === s) return p[2] = l[2];
-                                            if (c[o] = p, p[2] = e(t, n, u)) return !0
+                                            if ((l = c[o]) && l[0] === m && l[1] === s) return f[2] = l[2];
+                                            if (c[o] = f, f[2] = e(t, n, u)) return !0
                                         } return !1
                         }
                     }
 
-                    function we(e) {
+                    function de(e) {
                         return e.length > 1 ? function(t, n, r) {
                             for (var i = e.length; i--;)
                                 if (!e[i](t, n, r)) return !1;
                             return !0
                         } : e[0]
                     }
 
-                    function Te(e, t, n, r, i) {
+                    function he(e, t, n, r, i) {
                         for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
                         return a
                     }
 
-                    function Ce(e, t, n, r, i, o) {
-                        return r && !r[b] && (r = Ce(r)), i && !i[b] && (i = Ce(i, o)), le((function(o, a, s, u) {
-                            var l, c, f, p = [],
-                                d = [],
-                                h = a.length,
-                                g = o || function(e, t, n) {
-                                    for (var r = 0, i = t.length; r < i; r++) se(e, t[r], n);
+                    function ge(e, t, n, r, i, o) {
+                        return r && !r[y] && (r = ge(r)), i && !i[y] && (i = ge(i, o)), te((function(o, a, s, u) {
+                            var l, f, p, d, h = [],
+                                v = [],
+                                y = a.length,
+                                m = o || function(e, t, n) {
+                                    for (var r = 0, i = t.length; r < i; r++) Z(e, t[r], n);
                                     return n
                                 }(t || "*", s.nodeType ? [s] : s, []),
-                                v = !e || !o && t ? g : Te(g, p, e, s, u),
-                                y = n ? i || (o ? e : h || r) ? [] : a : v;
-                            if (n && n(v, y, s, u), r)
-                                for (l = Te(y, d), r(l, [], s, u), c = l.length; c--;)(f = l[c]) && (y[d[c]] = !(v[d[c]] = f));
+                                x = !e || !o && t ? m : he(m, h, e, s, u);
+                            if (n ? n(x, d = i || (o ? e : y || r) ? [] : a, s, u) : d = x, r)
+                                for (l = he(d, v), r(l, [], s, u), f = l.length; f--;)(p = l[f]) && (d[v[f]] = !(x[v[f]] = p));
                             if (o) {
                                 if (i || e) {
                                     if (i) {
-                                        for (l = [], c = y.length; c--;)(f = y[c]) && l.push(v[c] = f);
-                                        i(null, y = [], l, u)
+                                        for (l = [], f = d.length; f--;)(p = d[f]) && l.push(x[f] = p);
+                                        i(null, d = [], l, u)
                                     }
-                                    for (c = y.length; c--;)(f = y[c]) && (l = i ? P(o, f) : p[c]) > -1 && (o[l] = !(a[l] = f))
+                                    for (f = d.length; f--;)(p = d[f]) && (l = i ? c.call(o, p) : h[f]) > -1 && (o[l] = !(a[l] = p))
                                 }
-                            } else y = Te(y === a ? y.splice(h, y.length) : y), i ? i(null, a, y, u) : H.apply(a, y)
+                            } else d = he(d === a ? d.splice(y, d.length) : d), i ? i(null, a, d, u) : g.apply(a, d)
                         }))
                     }
 
-                    function Se(e) {
-                        for (var t, n, i, o = e.length, a = r.relative[e[0].type], s = a || r.relative[" "], u = a ? 1 : 0, c = be((function(e) {
-                                return e === t
-                            }), s, !0), f = be((function(e) {
-                                return P(t, e) > -1
-                            }), s, !0), p = [function(e, n, r) {
-                                var i = !a && (r || n !== l) || ((t = n).nodeType ? c(e, n, r) : f(e, n, r));
-                                return t = null, i
-                            }]; u < o; u++)
-                            if (n = r.relative[e[u].type]) p = [be(we(p), n)];
+                    function ve(e) {
+                        for (var r, i, o, a = e.length, s = t.relative[e[0].type], u = s || t.relative[" "], l = s ? 1 : 0, f = pe((function(e) {
+                                return e === r
+                            }), u, !0), p = pe((function(e) {
+                                return c.call(r, e) > -1
+                            }), u, !0), d = [function(e, t, i) {
+                                var o = !s && (i || t != n) || ((r = t).nodeType ? f(e, t, i) : p(e, t, i));
+                                return r = null, o
+                            }]; l < a; l++)
+                            if (i = t.relative[e[l].type]) d = [pe(de(d), i)];
                             else {
-                                if ((n = r.filter[e[u].type].apply(null, e[u].matches))[b]) {
-                                    for (i = ++u; i < o && !r.relative[e[i].type]; i++);
-                                    return Ce(u > 1 && we(p), u > 1 && xe(e.slice(0, u - 1).concat({
-                                        value: " " === e[u - 2].type ? "*" : ""
-                                    })).replace(B, "$1"), n, u < i && Se(e.slice(u, i)), i < o && Se(e = e.slice(i)), i < o && xe(e))
-                                }
-                                p.push(n)
-                            } return we(p)
+                                if ((i = t.filter[e[l].type].apply(null, e[l].matches))[y]) {
+                                    for (o = ++l; o < a && !t.relative[e[o].type]; o++);
+                                    return ge(l > 1 && de(d), l > 1 && fe(e.slice(0, l - 1).concat({
+                                        value: " " === e[l - 2].type ? "*" : ""
+                                    })).replace(L, "$1"), i, l < o && ve(e.slice(l, o)), o < a && ve(e = e.slice(o)), o < a && fe(e))
+                                }
+                                d.push(i)
+                            } return de(d)
                     }
-                    return me.prototype = r.filters = r.pseudos, r.setFilters = new me, a = se.tokenize = function(e, t) {
-                        var n, i, o, a, s, u, l, c = E[e + " "];
-                        if (c) return t ? 0 : c.slice(0);
-                        for (s = e, u = [], l = r.preFilter; s;) {
-                            for (a in n && !(i = _.exec(s)) || (i && (s = s.slice(i[0].length) || s), u.push(o = [])), n = !1, (i = z.exec(s)) && (n = i.shift(), o.push({
-                                    value: n,
-                                    type: i[0].replace(B, " ")
-                                }), s = s.slice(n.length)), r.filter) !(i = G[a].exec(s)) || l[a] && !(i = l[a](i)) || (n = i.shift(), o.push({
-                                value: n,
-                                type: a,
-                                matches: i
-                            }), s = s.slice(n.length));
-                            if (!n) break
-                        }
-                        return t ? s.length : s ? se.error(e) : E(e, u).slice(0)
-                    }, s = se.compile = function(e, t) {
-                        var n, i = [],
-                            o = [],
-                            s = k[e + " "];
+
+                    function ye(e, r) {
+                        var i, o = [],
+                            a = [],
+                            s = T[e + " "];
                         if (!s) {
-                            for (t || (t = a(e)), n = t.length; n--;)(s = Se(t[n]))[b] ? i.push(s) : o.push(s);
-                            s = k(e, function(e, t) {
-                                var n = t.length > 0,
-                                    i = e.length > 0,
-                                    o = function(o, a, s, u, c) {
-                                        var f, h, v, y = 0,
-                                            m = "0",
-                                            x = o && [],
-                                            b = [],
-                                            w = l,
-                                            C = o || i && r.find.TAG("*", c),
-                                            S = T += null == w ? 1 : Math.random() || .1,
+                            for (r || (r = ce(e)), i = r.length; i--;)(s = ve(r[i]))[y] ? o.push(s) : a.push(s);
+                            s = T(e, function(e, r) {
+                                var i = r.length > 0,
+                                    o = e.length > 0,
+                                    a = function(a, s, l, c, p) {
+                                        var d, h, v, y = 0,
+                                            x = "0",
+                                            b = a && [],
+                                            w = [],
+                                            T = n,
+                                            C = a || o && t.find.TAG("*", p),
+                                            k = m += null == T ? 1 : Math.random() || .1,
                                             E = C.length;
-                                        for (c && (l = a == d || a || c); m !== E && null != (f = C[m]); m++) {
-                                            if (i && f) {
-                                                for (h = 0, a || f.ownerDocument == d || (p(f), s = !g); v = e[h++];)
-                                                    if (v(f, a || d, s)) {
-                                                        u.push(f);
+                                        for (p && (n = s == u || s || p); x !== E && null != (d = C[x]); x++) {
+                                            if (o && d) {
+                                                for (h = 0, s || d.ownerDocument == u || (ue(d), l = !f); v = e[h++];)
+                                                    if (v(d, s || u, l)) {
+                                                        g.call(c, d);
                                                         break
-                                                    } c && (T = S)
+                                                    } p && (m = k)
                                             }
-                                            n && ((f = !v && f) && y--, o && x.push(f))
+                                            i && ((d = !v && d) && y--, a && b.push(d))
                                         }
-                                        if (y += m, n && m !== y) {
-                                            for (h = 0; v = t[h++];) v(x, b, a, s);
-                                            if (o) {
+                                        if (y += x, i && x !== y) {
+                                            for (h = 0; v = r[h++];) v(b, w, s, l);
+                                            if (a) {
                                                 if (y > 0)
-                                                    for (; m--;) x[m] || b[m] || (b[m] = q.call(u));
-                                                b = Te(b)
+                                                    for (; x--;) b[x] || w[x] || (w[x] = A.call(c));
+                                                w = he(w)
                                             }
-                                            H.apply(u, b), c && !o && b.length > 0 && y + t.length > 1 && se.uniqueSort(u)
+                                            g.apply(c, w), p && !a && w.length > 0 && y + r.length > 1 && S.uniqueSort(c)
                                         }
-                                        return c && (T = S, l = w), x
+                                        return p && (m = k, n = T), b
                                     };
-                                return n ? le(o) : o
-                            }(o, i)), s.selector = e
+                                return i ? te(a) : a
+                            }(a, o)), s.selector = e
                         }
                         return s
-                    }, u = se.select = function(e, t, n, i) {
-                        var o, u, l, c, f, p = "function" == typeof e && e,
-                            d = !i && a(e = p.selector || e);
-                        if (n = n || [], 1 === d.length) {
-                            if ((u = d[0] = d[0].slice(0)).length > 2 && "ID" === (l = u[0]).type && 9 === t.nodeType && g && r.relative[u[1].type]) {
-                                if (!(t = (r.find.ID(l.matches[0].replace(te, ne), t) || [])[0])) return n;
-                                p && (t = t.parentNode), e = e.slice(u.shift().value.length)
-                            }
-                            for (o = G.needsContext.test(e) ? 0 : u.length; o-- && (l = u[o], !r.relative[c = l.type]);)
-                                if ((f = r.find[c]) && (i = f(l.matches[0].replace(te, ne), ee.test(u[0].type) && ye(t.parentNode) || t))) {
-                                    if (u.splice(o, 1), !(e = i.length && xe(u))) return H.apply(n, i), n;
+                    }
+
+                    function me(e, n, r, i) {
+                        var o, a, s, u, l, c = "function" == typeof e && e,
+                            p = !i && ce(e = c.selector || e);
+                        if (r = r || [], 1 === p.length) {
+                            if ((a = p[0] = p[0].slice(0)).length > 2 && "ID" === (s = a[0]).type && 9 === n.nodeType && f && t.relative[a[1].type]) {
+                                if (!(n = (t.find.ID(s.matches[0].replace(Y, Q), n) || [])[0])) return r;
+                                c && (n = n.parentNode), e = e.slice(a.shift().value.length)
+                            }
+                            for (o = X.needsContext.test(e) ? 0 : a.length; o-- && (s = a[o], !t.relative[u = s.type]);)
+                                if ((l = t.find[u]) && (i = l(s.matches[0].replace(Y, Q), G.test(a[0].type) && se(n.parentNode) || n))) {
+                                    if (a.splice(o, 1), !(e = i.length && fe(a))) return g.apply(r, i), r;
                                     break
                                 }
                         }
-                        return (p || s(e, d))(i, t, !g, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-                    }, n.sortStable = b.split("").sort(j).join("") === b, n.detectDuplicates = !!f, p(), n.sortDetached = ce((function(e) {
-                        return 1 & e.compareDocumentPosition(d.createElement("fieldset"))
-                    })), ce((function(e) {
-                        return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
-                    })) || fe("type|href|height|width", (function(e, t, n) {
-                        if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
-                    })), n.attributes && ce((function(e) {
-                        return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
-                    })) || fe("value", (function(e, t, n) {
-                        if (!n && "input" === e.nodeName.toLowerCase()) return e.defaultValue
-                    })), ce((function(e) {
-                        return null == e.getAttribute("disabled")
-                    })) || fe(R, (function(e, t, n) {
-                        var r;
-                        if (!n) return !0 === e[t] ? t.toLowerCase() : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
-                    })), se
-                }(r);
-                S.find = k, S.expr = k.selectors, S.expr[":"] = S.expr.pseudos, S.uniqueSort = S.unique = k.uniqueSort, S.text = k.getText, S.isXMLDoc = k.isXML, S.contains = k.contains, S.escapeSelector = k.escape;
-                var A = function(e, t, n) {
+                        return (c || ye(e, p))(i, n, !f, r, !n || G.test(e) && se(n.parentNode) || n), r
+                    }
+                    le.prototype = t.filters = t.pseudos, t.setFilters = new le, v.sortStable = y.split("").sort(k).join("") === y, ue(), v.sortDetached = ne((function(e) {
+                        return 1 & e.compareDocumentPosition(u.createElement("fieldset"))
+                    })), S.find = Z, S.expr[":"] = S.expr.pseudos, S.unique = S.uniqueSort, Z.compile = ye, Z.select = me, Z.setDocument = ue, Z.escape = S.escapeSelector, Z.getText = S.text, Z.isXML = S.isXMLDoc, Z.selectors = S.expr, Z.support = S.support, Z.uniqueSort = S.uniqueSort
+                }();
+                var M = function(e, t, n) {
                         for (var r = [], i = void 0 !== n;
                             (e = e[t]) && 9 !== e.nodeType;)
                             if (1 === e.nodeType) {
                                 if (i && S(e).is(n)) break;
                                 r.push(e)
                             } return r
                     },
-                    j = function(e, t) {
+                    I = function(e, t) {
                         for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
                         return n
                     },
-                    N = S.expr.match.needsContext;
+                    W = S.expr.match.needsContext,
+                    F = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-                function D(e, t) {
-                    return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
-                }
-                var q = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
-
-                function L(e, t, n) {
+                function $(e, t, n) {
                     return y(t) ? S.grep(e, (function(e, r) {
                         return !!t.call(e, r, e) !== n
                     })) : t.nodeType ? S.grep(e, (function(e) {
                         return e === t !== n
                     })) : "string" != typeof t ? S.grep(e, (function(e) {
                         return c.call(t, e) > -1 !== n
                     })) : S.filter(t, e, n)
@@ -926,47 +872,47 @@
                             for (t = 0; t < r; t++)
                                 if (S.contains(i[t], this)) return !0
                         })));
                         for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
                         return r > 1 ? S.uniqueSort(n) : n
                     },
                     filter: function(e) {
-                        return this.pushStack(L(this, e || [], !1))
+                        return this.pushStack($(this, e || [], !1))
                     },
                     not: function(e) {
-                        return this.pushStack(L(this, e || [], !0))
+                        return this.pushStack($(this, e || [], !0))
                     },
                     is: function(e) {
-                        return !!L(this, "string" == typeof e && N.test(e) ? S(e) : e || [], !1).length
+                        return !!$(this, "string" == typeof e && W.test(e) ? S(e) : e || [], !1).length
                     }
                 });
-                var H, O = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+                var _, B = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
                 (S.fn.init = function(e, t, n) {
                     var r, i;
                     if (!e) return this;
-                    if (n = n || H, "string" == typeof e) {
-                        if (!(r = "<" === e[0] && ">" === e[e.length - 1] && e.length >= 3 ? [null, e, null] : O.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
+                    if (n = n || _, "string" == typeof e) {
+                        if (!(r = "<" === e[0] && ">" === e[e.length - 1] && e.length >= 3 ? [null, e, null] : B.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
                         if (r[1]) {
-                            if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : x, !0)), q.test(r[1]) && S.isPlainObject(t))
+                            if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : x, !0)), F.test(r[1]) && S.isPlainObject(t))
                                 for (r in t) y(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                             return this
                         }
                         return (i = x.getElementById(r[2])) && (this[0] = i, this.length = 1), this
                     }
                     return e.nodeType ? (this[0] = e, this.length = 1, this) : y(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
-                }).prototype = S.fn, H = S(x);
-                var P = /^(?:parents|prev(?:Until|All))/,
-                    R = {
+                }).prototype = S.fn, _ = S(x);
+                var X = /^(?:parents|prev(?:Until|All))/,
+                    U = {
                         children: !0,
                         contents: !0,
                         next: !0,
                         prev: !0
                     };
 
-                function M(e, t) {
+                function z(e, t) {
                     for (;
                         (e = e[t]) && 1 !== e.nodeType;);
                     return e
                 }
                 S.fn.extend({
                     has: function(e) {
                         var t = S(e, this),
@@ -977,15 +923,15 @@
                         }))
                     },
                     closest: function(e, t) {
                         var n, r = 0,
                             i = this.length,
                             o = [],
                             a = "string" != typeof e && S(e);
-                        if (!N.test(e))
+                        if (!W.test(e))
                             for (; r < i; r++)
                                 for (n = this[r]; n && n !== t; n = n.parentNode)
                                     if (n.nodeType < 11 && (a ? a.index(n) > -1 : 1 === n.nodeType && S.find.matchesSelector(n, e))) {
                                         o.push(n);
                                         break
                                     } return this.pushStack(o.length > 1 ? S.uniqueSort(o) : o)
                     },
@@ -1000,74 +946,74 @@
                     }
                 }), S.each({
                     parent: function(e) {
                         var t = e.parentNode;
                         return t && 11 !== t.nodeType ? t : null
                     },
                     parents: function(e) {
-                        return A(e, "parentNode")
+                        return M(e, "parentNode")
                     },
                     parentsUntil: function(e, t, n) {
-                        return A(e, "parentNode", n)
+                        return M(e, "parentNode", n)
                     },
                     next: function(e) {
-                        return M(e, "nextSibling")
+                        return z(e, "nextSibling")
                     },
                     prev: function(e) {
-                        return M(e, "previousSibling")
+                        return z(e, "previousSibling")
                     },
                     nextAll: function(e) {
-                        return A(e, "nextSibling")
+                        return M(e, "nextSibling")
                     },
                     prevAll: function(e) {
-                        return A(e, "previousSibling")
+                        return M(e, "previousSibling")
                     },
                     nextUntil: function(e, t, n) {
-                        return A(e, "nextSibling", n)
+                        return M(e, "nextSibling", n)
                     },
                     prevUntil: function(e, t, n) {
-                        return A(e, "previousSibling", n)
+                        return M(e, "previousSibling", n)
                     },
                     siblings: function(e) {
-                        return j((e.parentNode || {}).firstChild, e)
+                        return I((e.parentNode || {}).firstChild, e)
                     },
                     children: function(e) {
-                        return j(e.firstChild)
+                        return I(e.firstChild)
                     },
                     contents: function(e) {
-                        return null != e.contentDocument && a(e.contentDocument) ? e.contentDocument : (D(e, "template") && (e = e.content || e), S.merge([], e.childNodes))
+                        return null != e.contentDocument && a(e.contentDocument) ? e.contentDocument : (j(e, "template") && (e = e.content || e), S.merge([], e.childNodes))
                     }
                 }, (function(e, t) {
                     S.fn[e] = function(n, r) {
                         var i = S.map(this, t, n);
-                        return "Until" !== e.slice(-5) && (r = n), r && "string" == typeof r && (i = S.filter(r, i)), this.length > 1 && (R[e] || S.uniqueSort(i), P.test(e) && i.reverse()), this.pushStack(i)
+                        return "Until" !== e.slice(-5) && (r = n), r && "string" == typeof r && (i = S.filter(r, i)), this.length > 1 && (U[e] || S.uniqueSort(i), X.test(e) && i.reverse()), this.pushStack(i)
                     }
                 }));
-                var I = /[^\x20\t\r\n\f]+/g;
+                var V = /[^\x20\t\r\n\f]+/g;
 
-                function W(e) {
+                function G(e) {
                     return e
                 }
 
-                function F(e) {
+                function Y(e) {
                     throw e
                 }
 
-                function $(e, t, n, r) {
+                function Q(e, t, n, r) {
                     var i;
                     try {
                         e && y(i = e.promise) ? i.call(e).done(t).fail(n) : e && y(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
                     } catch (e) {
                         n.apply(void 0, [e])
                     }
                 }
                 S.Callbacks = function(e) {
                     e = "string" == typeof e ? function(e) {
                         var t = {};
-                        return S.each(e.match(I) || [], (function(e, n) {
+                        return S.each(e.match(V) || [], (function(e, n) {
                             t[n] = !0
                         })), t
                     }(e) : S.extend({}, e);
                     var t, n, r, i, o = [],
                         a = [],
                         s = -1,
                         u = function() {
@@ -1155,29 +1101,29 @@
                                         return function() {
                                             var s = this,
                                                 u = arguments,
                                                 l = function() {
                                                     var r, l;
                                                     if (!(e < o)) {
                                                         if ((r = n.apply(s, u)) === t.promise()) throw new TypeError("Thenable self-resolution");
-                                                        l = r && ("object" == typeof r || "function" == typeof r) && r.then, y(l) ? i ? l.call(r, a(o, t, W, i), a(o, t, F, i)) : (o++, l.call(r, a(o, t, W, i), a(o, t, F, i), a(o, t, W, t.notifyWith))) : (n !== W && (s = void 0, u = [r]), (i || t.resolveWith)(s, u))
+                                                        l = r && ("object" == typeof r || "function" == typeof r) && r.then, y(l) ? i ? l.call(r, a(o, t, G, i), a(o, t, Y, i)) : (o++, l.call(r, a(o, t, G, i), a(o, t, Y, i), a(o, t, G, t.notifyWith))) : (n !== G && (s = void 0, u = [r]), (i || t.resolveWith)(s, u))
                                                     }
                                                 },
                                                 c = i ? l : function() {
                                                     try {
                                                         l()
                                                     } catch (r) {
-                                                        S.Deferred.exceptionHook && S.Deferred.exceptionHook(r, c.stackTrace), e + 1 >= o && (n !== F && (s = void 0, u = [r]), t.rejectWith(s, u))
+                                                        S.Deferred.exceptionHook && S.Deferred.exceptionHook(r, c.error), e + 1 >= o && (n !== Y && (s = void 0, u = [r]), t.rejectWith(s, u))
                                                     }
                                                 };
-                                            e ? c() : (S.Deferred.getStackHook && (c.stackTrace = S.Deferred.getStackHook()), r.setTimeout(c))
+                                            e ? c() : (S.Deferred.getErrorHook ? c.error = S.Deferred.getErrorHook() : S.Deferred.getStackHook && (c.error = S.Deferred.getStackHook()), r.setTimeout(c))
                                         }
                                     }
                                     return S.Deferred((function(r) {
-                                        t[0][3].add(a(0, r, y(i) ? i : W, r.notifyWith)), t[1][3].add(a(0, r, y(e) ? e : W)), t[2][3].add(a(0, r, y(n) ? n : F))
+                                        t[0][3].add(a(0, r, y(i) ? i : G, r.notifyWith)), t[1][3].add(a(0, r, y(e) ? e : G)), t[2][3].add(a(0, r, y(n) ? n : Y))
                                     })).promise()
                                 },
                                 promise: function(e) {
                                     return null != e ? S.extend(e, i) : i
                                 }
                             },
                             o = {};
@@ -1198,187 +1144,187 @@
                             i = s.call(arguments),
                             o = S.Deferred(),
                             a = function(e) {
                                 return function(n) {
                                     r[e] = this, i[e] = arguments.length > 1 ? s.call(arguments) : n, --t || o.resolveWith(r, i)
                                 }
                             };
-                        if (t <= 1 && ($(e, o.done(a(n)).resolve, o.reject, !t), "pending" === o.state() || y(i[n] && i[n].then))) return o.then();
-                        for (; n--;) $(i[n], a(n), o.reject);
+                        if (t <= 1 && (Q(e, o.done(a(n)).resolve, o.reject, !t), "pending" === o.state() || y(i[n] && i[n].then))) return o.then();
+                        for (; n--;) Q(i[n], a(n), o.reject);
                         return o.promise()
                     }
                 });
-                var B = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+                var J = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
                 S.Deferred.exceptionHook = function(e, t) {
-                    r.console && r.console.warn && e && B.test(e.name) && r.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
+                    r.console && r.console.warn && e && J.test(e.name) && r.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
                 }, S.readyException = function(e) {
                     r.setTimeout((function() {
                         throw e
                     }))
                 };
-                var _ = S.Deferred();
+                var K = S.Deferred();
 
-                function z() {
-                    x.removeEventListener("DOMContentLoaded", z), r.removeEventListener("load", z), S.ready()
+                function Z() {
+                    x.removeEventListener("DOMContentLoaded", Z), r.removeEventListener("load", Z), S.ready()
                 }
                 S.fn.ready = function(e) {
-                    return _.then(e).catch((function(e) {
+                    return K.then(e).catch((function(e) {
                         S.readyException(e)
                     })), this
                 }, S.extend({
                     isReady: !1,
                     readyWait: 1,
                     ready: function(e) {
-                        (!0 === e ? --S.readyWait : S.isReady) || (S.isReady = !0, !0 !== e && --S.readyWait > 0 || _.resolveWith(x, [S]))
+                        (!0 === e ? --S.readyWait : S.isReady) || (S.isReady = !0, !0 !== e && --S.readyWait > 0 || K.resolveWith(x, [S]))
                     }
-                }), S.ready.then = _.then, "complete" === x.readyState || "loading" !== x.readyState && !x.documentElement.doScroll ? r.setTimeout(S.ready) : (x.addEventListener("DOMContentLoaded", z), r.addEventListener("load", z));
-                var U = function(e, t, n, r, i, o, a) {
+                }), S.ready.then = K.then, "complete" === x.readyState || "loading" !== x.readyState && !x.documentElement.doScroll ? r.setTimeout(S.ready) : (x.addEventListener("DOMContentLoaded", Z), r.addEventListener("load", Z));
+                var ee = function(e, t, n, r, i, o, a) {
                         var s = 0,
                             u = e.length,
                             l = null == n;
                         if ("object" === T(n))
-                            for (s in i = !0, n) U(e, t, s, n[s], !0, o, a);
+                            for (s in i = !0, n) ee(e, t, s, n[s], !0, o, a);
                         else if (void 0 !== r && (i = !0, y(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
                                 return l.call(S(e), n)
                             })), t))
                             for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
                         return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
                     },
-                    X = /^-ms-/,
-                    V = /-([a-z])/g;
+                    te = /^-ms-/,
+                    ne = /-([a-z])/g;
 
-                function G(e, t) {
+                function re(e, t) {
                     return t.toUpperCase()
                 }
 
-                function Y(e) {
-                    return e.replace(X, "ms-").replace(V, G)
+                function ie(e) {
+                    return e.replace(te, "ms-").replace(ne, re)
                 }
-                var Q = function(e) {
+                var oe = function(e) {
                     return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
                 };
 
-                function J() {
-                    this.expando = S.expando + J.uid++
+                function ae() {
+                    this.expando = S.expando + ae.uid++
                 }
-                J.uid = 1, J.prototype = {
+                ae.uid = 1, ae.prototype = {
                     cache: function(e) {
                         var t = e[this.expando];
-                        return t || (t = {}, Q(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
+                        return t || (t = {}, oe(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
                             value: t,
                             configurable: !0
                         }))), t
                     },
                     set: function(e, t, n) {
                         var r, i = this.cache(e);
-                        if ("string" == typeof t) i[Y(t)] = n;
+                        if ("string" == typeof t) i[ie(t)] = n;
                         else
-                            for (r in t) i[Y(r)] = t[r];
+                            for (r in t) i[ie(r)] = t[r];
                         return i
                     },
                     get: function(e, t) {
-                        return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][Y(t)]
+                        return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][ie(t)]
                     },
                     access: function(e, t, n) {
                         return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
                     },
                     remove: function(e, t) {
                         var n, r = e[this.expando];
                         if (void 0 !== r) {
                             if (void 0 !== t) {
-                                n = (t = Array.isArray(t) ? t.map(Y) : (t = Y(t)) in r ? [t] : t.match(I) || []).length;
+                                n = (t = Array.isArray(t) ? t.map(ie) : (t = ie(t)) in r ? [t] : t.match(V) || []).length;
                                 for (; n--;) delete r[t[n]]
                             }(void 0 === t || S.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
                         }
                     },
                     hasData: function(e) {
                         var t = e[this.expando];
                         return void 0 !== t && !S.isEmptyObject(t)
                     }
                 };
-                var K = new J,
-                    Z = new J,
-                    ee = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-                    te = /[A-Z]/g;
+                var se = new ae,
+                    ue = new ae,
+                    le = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+                    ce = /[A-Z]/g;
 
-                function ne(e, t, n) {
+                function fe(e, t, n) {
                     var r;
                     if (void 0 === n && 1 === e.nodeType)
-                        if (r = "data-" + t.replace(te, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
+                        if (r = "data-" + t.replace(ce, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
                             try {
                                 n = function(e) {
-                                    return "true" === e || "false" !== e && ("null" === e ? null : e === +e + "" ? +e : ee.test(e) ? JSON.parse(e) : e)
+                                    return "true" === e || "false" !== e && ("null" === e ? null : e === +e + "" ? +e : le.test(e) ? JSON.parse(e) : e)
                                 }(n)
                             } catch (e) {}
-                            Z.set(e, t, n)
+                            ue.set(e, t, n)
                         } else n = void 0;
                     return n
                 }
                 S.extend({
                     hasData: function(e) {
-                        return Z.hasData(e) || K.hasData(e)
+                        return ue.hasData(e) || se.hasData(e)
                     },
                     data: function(e, t, n) {
-                        return Z.access(e, t, n)
+                        return ue.access(e, t, n)
                     },
                     removeData: function(e, t) {
-                        Z.remove(e, t)
+                        ue.remove(e, t)
                     },
                     _data: function(e, t, n) {
-                        return K.access(e, t, n)
+                        return se.access(e, t, n)
                     },
                     _removeData: function(e, t) {
-                        K.remove(e, t)
+                        se.remove(e, t)
                     }
                 }), S.fn.extend({
                     data: function(e, t) {
                         var n, r, i, o = this[0],
                             a = o && o.attributes;
                         if (void 0 === e) {
-                            if (this.length && (i = Z.get(o), 1 === o.nodeType && !K.get(o, "hasDataAttrs"))) {
-                                for (n = a.length; n--;) a[n] && 0 === (r = a[n].name).indexOf("data-") && (r = Y(r.slice(5)), ne(o, r, i[r]));
-                                K.set(o, "hasDataAttrs", !0)
+                            if (this.length && (i = ue.get(o), 1 === o.nodeType && !se.get(o, "hasDataAttrs"))) {
+                                for (n = a.length; n--;) a[n] && 0 === (r = a[n].name).indexOf("data-") && (r = ie(r.slice(5)), fe(o, r, i[r]));
+                                se.set(o, "hasDataAttrs", !0)
                             }
                             return i
                         }
                         return "object" == typeof e ? this.each((function() {
-                            Z.set(this, e)
-                        })) : U(this, (function(t) {
+                            ue.set(this, e)
+                        })) : ee(this, (function(t) {
                             var n;
-                            if (o && void 0 === t) return void 0 !== (n = Z.get(o, e)) || void 0 !== (n = ne(o, e)) ? n : void 0;
+                            if (o && void 0 === t) return void 0 !== (n = ue.get(o, e)) || void 0 !== (n = fe(o, e)) ? n : void 0;
                             this.each((function() {
-                                Z.set(this, e, t)
+                                ue.set(this, e, t)
                             }))
                         }), null, t, arguments.length > 1, null, !0)
                     },
                     removeData: function(e) {
                         return this.each((function() {
-                            Z.remove(this, e)
+                            ue.remove(this, e)
                         }))
                     }
                 }), S.extend({
                     queue: function(e, t, n) {
                         var r;
-                        if (e) return t = (t || "fx") + "queue", r = K.get(e, t), n && (!r || Array.isArray(n) ? r = K.access(e, t, S.makeArray(n)) : r.push(n)), r || []
+                        if (e) return t = (t || "fx") + "queue", r = se.get(e, t), n && (!r || Array.isArray(n) ? r = se.access(e, t, S.makeArray(n)) : r.push(n)), r || []
                     },
                     dequeue: function(e, t) {
                         t = t || "fx";
                         var n = S.queue(e, t),
                             r = n.length,
                             i = n.shift(),
                             o = S._queueHooks(e, t);
                         "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, (function() {
                             S.dequeue(e, t)
                         }), o)), !r && o && o.empty.fire()
                     },
                     _queueHooks: function(e, t) {
                         var n = t + "queueHooks";
-                        return K.get(e, n) || K.access(e, n, {
+                        return se.get(e, n) || se.access(e, n, {
                             empty: S.Callbacks("once memory").add((function() {
-                                K.remove(e, [t + "queue", n])
+                                se.remove(e, [t + "queue", n])
                             }))
                         })
                     }
                 }), S.fn.extend({
                     queue: function(e, t) {
                         var n = 2;
                         return "string" != typeof e && (t = e, e = "fx", n--), arguments.length < n ? S.queue(this[0], e) : void 0 === t ? this : this.each((function() {
@@ -1398,196 +1344,186 @@
                         var n, r = 1,
                             i = S.Deferred(),
                             o = this,
                             a = this.length,
                             s = function() {
                                 --r || i.resolveWith(o, [o])
                             };
-                        for ("string" != typeof e && (t = e, e = void 0), e = e || "fx"; a--;)(n = K.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
+                        for ("string" != typeof e && (t = e, e = void 0), e = e || "fx"; a--;)(n = se.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
                         return s(), i.promise(t)
                     }
                 });
-                var re = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-                    ie = new RegExp("^(?:([+-])=|)(" + re + ")([a-z%]*)$", "i"),
-                    oe = ["Top", "Right", "Bottom", "Left"],
-                    ae = x.documentElement,
-                    se = function(e) {
+                var pe = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+                    de = new RegExp("^(?:([+-])=|)(" + pe + ")([a-z%]*)$", "i"),
+                    he = ["Top", "Right", "Bottom", "Left"],
+                    ge = x.documentElement,
+                    ve = function(e) {
                         return S.contains(e.ownerDocument, e)
                     },
-                    ue = {
+                    ye = {
                         composed: !0
                     };
-                ae.getRootNode && (se = function(e) {
-                    return S.contains(e.ownerDocument, e) || e.getRootNode(ue) === e.ownerDocument
+                ge.getRootNode && (ve = function(e) {
+                    return S.contains(e.ownerDocument, e) || e.getRootNode(ye) === e.ownerDocument
                 });
-                var le = function(e, t) {
-                    return "none" === (e = t || e).style.display || "" === e.style.display && se(e) && "none" === S.css(e, "display")
+                var me = function(e, t) {
+                    return "none" === (e = t || e).style.display || "" === e.style.display && ve(e) && "none" === S.css(e, "display")
                 };
 
-                function ce(e, t, n, r) {
+                function xe(e, t, n, r) {
                     var i, o, a = 20,
                         s = r ? function() {
                             return r.cur()
                         } : function() {
                             return S.css(e, t, "")
                         },
                         u = s(),
                         l = n && n[3] || (S.cssNumber[t] ? "" : "px"),
-                        c = e.nodeType && (S.cssNumber[t] || "px" !== l && +u) && ie.exec(S.css(e, t));
+                        c = e.nodeType && (S.cssNumber[t] || "px" !== l && +u) && de.exec(S.css(e, t));
                     if (c && c[3] !== l) {
                         for (u /= 2, l = l || c[3], c = +u || 1; a--;) S.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
                         c *= 2, S.style(e, t, c + l), n = n || []
                     }
                     return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
                 }
-                var fe = {};
+                var be = {};
 
-                function pe(e) {
+                function we(e) {
                     var t, n = e.ownerDocument,
                         r = e.nodeName,
-                        i = fe[r];
-                    return i || (t = n.body.appendChild(n.createElement(r)), i = S.css(t, "display"), t.parentNode.removeChild(t), "none" === i && (i = "block"), fe[r] = i, i)
+                        i = be[r];
+                    return i || (t = n.body.appendChild(n.createElement(r)), i = S.css(t, "display"), t.parentNode.removeChild(t), "none" === i && (i = "block"), be[r] = i, i)
                 }
 
-                function de(e, t) {
-                    for (var n, r, i = [], o = 0, a = e.length; o < a; o++)(r = e[o]).style && (n = r.style.display, t ? ("none" === n && (i[o] = K.get(r, "display") || null, i[o] || (r.style.display = "")), "" === r.style.display && le(r) && (i[o] = pe(r))) : "none" !== n && (i[o] = "none", K.set(r, "display", n)));
+                function Te(e, t) {
+                    for (var n, r, i = [], o = 0, a = e.length; o < a; o++)(r = e[o]).style && (n = r.style.display, t ? ("none" === n && (i[o] = se.get(r, "display") || null, i[o] || (r.style.display = "")), "" === r.style.display && me(r) && (i[o] = we(r))) : "none" !== n && (i[o] = "none", se.set(r, "display", n)));
                     for (o = 0; o < a; o++) null != i[o] && (e[o].style.display = i[o]);
                     return e
                 }
                 S.fn.extend({
                     show: function() {
-                        return de(this, !0)
+                        return Te(this, !0)
                     },
                     hide: function() {
-                        return de(this)
+                        return Te(this)
                     },
                     toggle: function(e) {
                         return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each((function() {
-                            le(this) ? S(this).show() : S(this).hide()
+                            me(this) ? S(this).show() : S(this).hide()
                         }))
                     }
                 });
-                var he, ge, ve = /^(?:checkbox|radio)$/i,
-                    ye = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-                    me = /^$|^module$|\/(?:java|ecma)script/i;
-                he = x.createDocumentFragment().appendChild(x.createElement("div")), (ge = x.createElement("input")).setAttribute("type", "radio"), ge.setAttribute("checked", "checked"), ge.setAttribute("name", "t"), he.appendChild(ge), v.checkClone = he.cloneNode(!0).cloneNode(!0).lastChild.checked, he.innerHTML = "<textarea>x</textarea>", v.noCloneChecked = !!he.cloneNode(!0).lastChild.defaultValue, he.innerHTML = "<option></option>", v.option = !!he.lastChild;
-                var xe = {
+                var Ce, ke, Se = /^(?:checkbox|radio)$/i,
+                    Ee = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+                    je = /^$|^module$|\/(?:java|ecma)script/i;
+                Ce = x.createDocumentFragment().appendChild(x.createElement("div")), (ke = x.createElement("input")).setAttribute("type", "radio"), ke.setAttribute("checked", "checked"), ke.setAttribute("name", "t"), Ce.appendChild(ke), v.checkClone = Ce.cloneNode(!0).cloneNode(!0).lastChild.checked, Ce.innerHTML = "<textarea>x</textarea>", v.noCloneChecked = !!Ce.cloneNode(!0).lastChild.defaultValue, Ce.innerHTML = "<option></option>", v.option = !!Ce.lastChild;
+                var Ae = {
                     thead: [1, "<table>", "</table>"],
                     col: [2, "<table><colgroup>", "</colgroup></table>"],
                     tr: [2, "<table><tbody>", "</tbody></table>"],
                     td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
                     _default: [0, "", ""]
                 };
 
-                function be(e, t) {
+                function De(e, t) {
                     var n;
-                    return n = void 0 !== e.getElementsByTagName ? e.getElementsByTagName(t || "*") : void 0 !== e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && D(e, t) ? S.merge([e], n) : n
+                    return n = void 0 !== e.getElementsByTagName ? e.getElementsByTagName(t || "*") : void 0 !== e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && j(e, t) ? S.merge([e], n) : n
                 }
 
-                function we(e, t) {
-                    for (var n = 0, r = e.length; n < r; n++) K.set(e[n], "globalEval", !t || K.get(t[n], "globalEval"))
+                function Ne(e, t) {
+                    for (var n = 0, r = e.length; n < r; n++) se.set(e[n], "globalEval", !t || se.get(t[n], "globalEval"))
                 }
-                xe.tbody = xe.tfoot = xe.colgroup = xe.caption = xe.thead, xe.th = xe.td, v.option || (xe.optgroup = xe.option = [1, "<select multiple='multiple'>", "</select>"]);
-                var Te = /<|&#?\w+;/;
+                Ae.tbody = Ae.tfoot = Ae.colgroup = Ae.caption = Ae.thead, Ae.th = Ae.td, v.option || (Ae.optgroup = Ae.option = [1, "<select multiple='multiple'>", "</select>"]);
+                var qe = /<|&#?\w+;/;
 
-                function Ce(e, t, n, r, i) {
+                function Le(e, t, n, r, i) {
                     for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
                         if ((o = e[d]) || 0 === o)
                             if ("object" === T(o)) S.merge(p, o.nodeType ? [o] : o);
-                            else if (Te.test(o)) {
-                        for (a = a || f.appendChild(t.createElement("div")), s = (ye.exec(o) || ["", ""])[1].toLowerCase(), u = xe[s] || xe._default, a.innerHTML = u[1] + S.htmlPrefilter(o) + u[2], c = u[0]; c--;) a = a.lastChild;
+                            else if (qe.test(o)) {
+                        for (a = a || f.appendChild(t.createElement("div")), s = (Ee.exec(o) || ["", ""])[1].toLowerCase(), u = Ae[s] || Ae._default, a.innerHTML = u[1] + S.htmlPrefilter(o) + u[2], c = u[0]; c--;) a = a.lastChild;
                         S.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
                     } else p.push(t.createTextNode(o));
                     for (f.textContent = "", d = 0; o = p[d++];)
                         if (r && S.inArray(o, r) > -1) i && i.push(o);
-                        else if (l = se(o), a = be(f.appendChild(o), "script"), l && we(a), n)
-                        for (c = 0; o = a[c++];) me.test(o.type || "") && n.push(o);
+                        else if (l = ve(o), a = De(f.appendChild(o), "script"), l && Ne(a), n)
+                        for (c = 0; o = a[c++];) je.test(o.type || "") && n.push(o);
                     return f
                 }
-                var Se = /^([^.]*)(?:\.(.+)|)/;
+                var He = /^([^.]*)(?:\.(.+)|)/;
 
-                function Ee() {
+                function Oe() {
                     return !0
                 }
 
-                function ke() {
+                function Pe() {
                     return !1
                 }
 
-                function Ae(e, t) {
-                    return e === function() {
-                        try {
-                            return x.activeElement
-                        } catch (e) {}
-                    }() == ("focus" === t)
-                }
-
-                function je(e, t, n, r, i, o) {
+                function Re(e, t, n, r, i, o) {
                     var a, s;
                     if ("object" == typeof t) {
-                        for (s in "string" != typeof n && (r = r || n, n = void 0), t) je(e, s, n, r, t[s], o);
+                        for (s in "string" != typeof n && (r = r || n, n = void 0), t) Re(e, s, n, r, t[s], o);
                         return e
                     }
-                    if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = ke;
+                    if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Pe;
                     else if (!i) return e;
                     return 1 === o && (a = i, i = function(e) {
                         return S().off(e), a.apply(this, arguments)
                     }, i.guid = a.guid || (a.guid = S.guid++)), e.each((function() {
                         S.event.add(this, t, i, r, n)
                     }))
                 }
 
-                function Ne(e, t, n) {
-                    n ? (K.set(e, t, !1), S.event.add(e, t, {
+                function Me(e, t, n) {
+                    n ? (se.set(e, t, !1), S.event.add(e, t, {
                         namespace: !1,
                         handler: function(e) {
-                            var r, i, o = K.get(this, t);
+                            var n, r = se.get(this, t);
                             if (1 & e.isTrigger && this[t]) {
-                                if (o.length)(S.event.special[t] || {}).delegateType && e.stopPropagation();
-                                else if (o = s.call(arguments), K.set(this, t, o), r = n(this, t), this[t](), o !== (i = K.get(this, t)) || r ? K.set(this, t, !1) : i = {}, o !== i) return e.stopImmediatePropagation(), e.preventDefault(), i && i.value
-                            } else o.length && (K.set(this, t, {
-                                value: S.event.trigger(S.extend(o[0], S.Event.prototype), o.slice(1), this)
-                            }), e.stopImmediatePropagation())
+                                if (r)(S.event.special[t] || {}).delegateType && e.stopPropagation();
+                                else if (r = s.call(arguments), se.set(this, t, r), this[t](), n = se.get(this, t), se.set(this, t, !1), r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n
+                            } else r && (se.set(this, t, S.event.trigger(r[0], r.slice(1), this)), e.stopPropagation(), e.isImmediatePropagationStopped = Oe)
                         }
-                    })) : void 0 === K.get(e, t) && S.event.add(e, t, Ee)
+                    })) : void 0 === se.get(e, t) && S.event.add(e, t, Oe)
                 }
                 S.event = {
                     global: {},
                     add: function(e, t, n, r, i) {
-                        var o, a, s, u, l, c, f, p, d, h, g, v = K.get(e);
-                        if (Q(e))
-                            for (n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(ae, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(t) {
+                        var o, a, s, u, l, c, f, p, d, h, g, v = se.get(e);
+                        if (oe(e))
+                            for (n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(ge, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(t) {
                                     return void 0 !== S && S.event.triggered !== t.type ? S.event.dispatch.apply(e, arguments) : void 0
-                                }), l = (t = (t || "").match(I) || [""]).length; l--;) d = g = (s = Se.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                                }), l = (t = (t || "").match(V) || [""]).length; l--;) d = g = (s = He.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                                 type: d,
                                 origType: g,
                                 data: r,
                                 handler: n,
                                 guid: n.guid,
                                 selector: i,
                                 needsContext: i && S.expr.match.needsContext.test(i),
                                 namespace: h.join(".")
                             }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(e, r, h, a) || e.addEventListener && e.addEventListener(d, a)), f.add && (f.add.call(e, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), S.event.global[d] = !0)
                     },
                     remove: function(e, t, n, r, i) {
-                        var o, a, s, u, l, c, f, p, d, h, g, v = K.hasData(e) && K.get(e);
+                        var o, a, s, u, l, c, f, p, d, h, g, v = se.hasData(e) && se.get(e);
                         if (v && (u = v.events)) {
-                            for (l = (t = (t || "").match(I) || [""]).length; l--;)
-                                if (d = g = (s = Se.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                            for (l = (t = (t || "").match(V) || [""]).length; l--;)
+                                if (d = g = (s = He.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
                                     for (f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length; o--;) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
                                     a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                                 } else
                                     for (d in u) S.event.remove(e, d + t[l], n, r, !0);
-                            S.isEmptyObject(u) && K.remove(e, "handle events")
+                            S.isEmptyObject(u) && se.remove(e, "handle events")
                         }
                     },
                     dispatch: function(e) {
                         var t, n, r, i, o, a, s = new Array(arguments.length),
                             u = S.event.fix(e),
-                            l = (K.get(this, "events") || Object.create(null))[u.type] || [],
+                            l = (se.get(this, "events") || Object.create(null))[u.type] || [],
                             c = S.event.special[u.type] || {};
                         for (s[0] = u, t = 1; t < arguments.length; t++) s[t] = arguments[t];
                         if (u.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, u)) {
                             for (a = S.event.handlers.call(this, u, l), t = 0;
                                 (i = a[t++]) && !u.isPropagationStopped();)
                                 for (u.currentTarget = i.elem, n = 0;
                                     (o = i.handlers[n++]) && !u.isImmediatePropagationStopped();) u.rnamespace && !1 !== o.namespace && !u.rnamespace.test(o.namespace) || (u.handleObj = o, u.data = o.data, void 0 !== (r = ((S.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, s)) && !1 === (u.result = r) && (u.preventDefault(), u.stopPropagation()));
@@ -1636,53 +1572,53 @@
                     special: {
                         load: {
                             noBubble: !0
                         },
                         click: {
                             setup: function(e) {
                                 var t = this || e;
-                                return ve.test(t.type) && t.click && D(t, "input") && Ne(t, "click", Ee), !1
+                                return Se.test(t.type) && t.click && j(t, "input") && Me(t, "click", !0), !1
                             },
                             trigger: function(e) {
                                 var t = this || e;
-                                return ve.test(t.type) && t.click && D(t, "input") && Ne(t, "click"), !0
+                                return Se.test(t.type) && t.click && j(t, "input") && Me(t, "click"), !0
                             },
                             _default: function(e) {
                                 var t = e.target;
-                                return ve.test(t.type) && t.click && D(t, "input") && K.get(t, "click") || D(t, "a")
+                                return Se.test(t.type) && t.click && j(t, "input") && se.get(t, "click") || j(t, "a")
                             }
                         },
                         beforeunload: {
                             postDispatch: function(e) {
                                 void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
                             }
                         }
                     }
                 }, S.removeEvent = function(e, t, n) {
                     e.removeEventListener && e.removeEventListener(t, n)
                 }, S.Event = function(e, t) {
                     if (!(this instanceof S.Event)) return new S.Event(e, t);
-                    e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ee : ke, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+                    e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Oe : Pe, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
                 }, S.Event.prototype = {
                     constructor: S.Event,
-                    isDefaultPrevented: ke,
-                    isPropagationStopped: ke,
-                    isImmediatePropagationStopped: ke,
+                    isDefaultPrevented: Pe,
+                    isPropagationStopped: Pe,
+                    isImmediatePropagationStopped: Pe,
                     isSimulated: !1,
                     preventDefault: function() {
                         var e = this.originalEvent;
-                        this.isDefaultPrevented = Ee, e && !this.isSimulated && e.preventDefault()
+                        this.isDefaultPrevented = Oe, e && !this.isSimulated && e.preventDefault()
                     },
                     stopPropagation: function() {
                         var e = this.originalEvent;
-                        this.isPropagationStopped = Ee, e && !this.isSimulated && e.stopPropagation()
+                        this.isPropagationStopped = Oe, e && !this.isSimulated && e.stopPropagation()
                     },
                     stopImmediatePropagation: function() {
                         var e = this.originalEvent;
-                        this.isImmediatePropagationStopped = Ee, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+                        this.isImmediatePropagationStopped = Oe, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
                     }
                 }, S.each({
                     altKey: !0,
                     bubbles: !0,
                     cancelable: !0,
                     changedTouches: !0,
                     ctrlKey: !0,
@@ -1712,259 +1648,283 @@
                     toElement: !0,
                     touches: !0,
                     which: !0
                 }, S.event.addProp), S.each({
                     focus: "focusin",
                     blur: "focusout"
                 }, (function(e, t) {
+                    function n(e) {
+                        if (x.documentMode) {
+                            var n = se.get(this, "handle"),
+                                r = S.event.fix(e);
+                            r.type = "focusin" === e.type ? "focus" : "blur", r.isSimulated = !0, n(e), r.target === r.currentTarget && n(r)
+                        } else S.event.simulate(t, e.target, S.event.fix(e))
+                    }
                     S.event.special[e] = {
                         setup: function() {
-                            return Ne(this, e, Ae), !1
+                            var r;
+                            if (Me(this, e, !0), !x.documentMode) return !1;
+                            (r = se.get(this, t)) || this.addEventListener(t, n), se.set(this, t, (r || 0) + 1)
                         },
                         trigger: function() {
-                            return Ne(this, e), !0
+                            return Me(this, e), !0
+                        },
+                        teardown: function() {
+                            var e;
+                            if (!x.documentMode) return !1;
+                            (e = se.get(this, t) - 1) ? se.set(this, t, e): (this.removeEventListener(t, n), se.remove(this, t))
                         },
                         _default: function(t) {
-                            return K.get(t.target, e)
+                            return se.get(t.target, e)
                         },
                         delegateType: t
+                    }, S.event.special[t] = {
+                        setup: function() {
+                            var r = this.ownerDocument || this.document || this,
+                                i = x.documentMode ? this : r,
+                                o = se.get(i, t);
+                            o || (x.documentMode ? this.addEventListener(t, n) : r.addEventListener(e, n, !0)), se.set(i, t, (o || 0) + 1)
+                        },
+                        teardown: function() {
+                            var r = this.ownerDocument || this.document || this,
+                                i = x.documentMode ? this : r,
+                                o = se.get(i, t) - 1;
+                            o ? se.set(i, t, o) : (x.documentMode ? this.removeEventListener(t, n) : r.removeEventListener(e, n, !0), se.remove(i, t))
+                        }
                     }
                 })), S.each({
                     mouseenter: "mouseover",
                     mouseleave: "mouseout",
                     pointerenter: "pointerover",
                     pointerleave: "pointerout"
                 }, (function(e, t) {
                     S.event.special[e] = {
                         delegateType: t,
                         bindType: t,
                         handle: function(e) {
-                            var n, r = this,
-                                i = e.relatedTarget,
-                                o = e.handleObj;
-                            return i && (i === r || S.contains(r, i)) || (e.type = o.origType, n = o.handler.apply(this, arguments), e.type = t), n
+                            var n, r = e.relatedTarget,
+                                i = e.handleObj;
+                            return r && (r === this || S.contains(this, r)) || (e.type = i.origType, n = i.handler.apply(this, arguments), e.type = t), n
                         }
                     }
                 })), S.fn.extend({
                     on: function(e, t, n, r) {
-                        return je(this, e, t, n, r)
+                        return Re(this, e, t, n, r)
                     },
                     one: function(e, t, n, r) {
-                        return je(this, e, t, n, r, 1)
+                        return Re(this, e, t, n, r, 1)
                     },
                     off: function(e, t, n) {
                         var r, i;
                         if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
                         if ("object" == typeof e) {
                             for (i in e) this.off(i, t, e[i]);
                             return this
                         }
-                        return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = ke), this.each((function() {
+                        return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Pe), this.each((function() {
                             S.event.remove(this, e, n, t)
                         }))
                     }
                 });
-                var De = /<script|<style|<link/i,
-                    qe = /checked\s*(?:[^=]|=\s*.checked.)/i,
-                    Le = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
+                var Ie = /<script|<style|<link/i,
+                    We = /checked\s*(?:[^=]|=\s*.checked.)/i,
+                    Fe = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
-                function He(e, t) {
-                    return D(e, "table") && D(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
+                function $e(e, t) {
+                    return j(e, "table") && j(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
                 }
 
-                function Oe(e) {
+                function _e(e) {
                     return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
                 }
 
-                function Pe(e) {
+                function Be(e) {
                     return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
                 }
 
-                function Re(e, t) {
+                function Xe(e, t) {
                     var n, r, i, o, a, s;
                     if (1 === t.nodeType) {
-                        if (K.hasData(e) && (s = K.get(e).events))
-                            for (i in K.remove(t, "handle events"), s)
+                        if (se.hasData(e) && (s = se.get(e).events))
+                            for (i in se.remove(t, "handle events"), s)
                                 for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
-                        Z.hasData(e) && (o = Z.access(e), a = S.extend({}, o), Z.set(t, a))
+                        ue.hasData(e) && (o = ue.access(e), a = S.extend({}, o), ue.set(t, a))
                     }
                 }
 
-                function Me(e, t) {
+                function Ue(e, t) {
                     var n = t.nodeName.toLowerCase();
-                    "input" === n && ve.test(e.type) ? t.checked = e.checked : "input" !== n && "textarea" !== n || (t.defaultValue = e.defaultValue)
+                    "input" === n && Se.test(e.type) ? t.checked = e.checked : "input" !== n && "textarea" !== n || (t.defaultValue = e.defaultValue)
                 }
 
-                function Ie(e, t, n, r) {
+                function ze(e, t, n, r) {
                     t = u(t);
                     var i, o, a, s, l, c, f = 0,
                         p = e.length,
                         d = p - 1,
                         h = t[0],
                         g = y(h);
-                    if (g || p > 1 && "string" == typeof h && !v.checkClone && qe.test(h)) return e.each((function(i) {
+                    if (g || p > 1 && "string" == typeof h && !v.checkClone && We.test(h)) return e.each((function(i) {
                         var o = e.eq(i);
-                        g && (t[0] = h.call(this, i, o.html())), Ie(o, t, n, r)
+                        g && (t[0] = h.call(this, i, o.html())), ze(o, t, n, r)
                     }));
-                    if (p && (o = (i = Ce(t, e[0].ownerDocument, !1, e, r)).firstChild, 1 === i.childNodes.length && (i = o), o || r)) {
-                        for (s = (a = S.map(be(i, "script"), Oe)).length; f < p; f++) l = i, f !== d && (l = S.clone(l, !0, !0), s && S.merge(a, be(l, "script"))), n.call(e[f], l, f);
+                    if (p && (o = (i = Le(t, e[0].ownerDocument, !1, e, r)).firstChild, 1 === i.childNodes.length && (i = o), o || r)) {
+                        for (s = (a = S.map(De(i, "script"), _e)).length; f < p; f++) l = i, f !== d && (l = S.clone(l, !0, !0), s && S.merge(a, De(l, "script"))), n.call(e[f], l, f);
                         if (s)
-                            for (c = a[a.length - 1].ownerDocument, S.map(a, Pe), f = 0; f < s; f++) l = a[f], me.test(l.type || "") && !K.access(l, "globalEval") && S.contains(c, l) && (l.src && "module" !== (l.type || "").toLowerCase() ? S._evalUrl && !l.noModule && S._evalUrl(l.src, {
+                            for (c = a[a.length - 1].ownerDocument, S.map(a, Be), f = 0; f < s; f++) l = a[f], je.test(l.type || "") && !se.access(l, "globalEval") && S.contains(c, l) && (l.src && "module" !== (l.type || "").toLowerCase() ? S._evalUrl && !l.noModule && S._evalUrl(l.src, {
                                 nonce: l.nonce || l.getAttribute("nonce")
-                            }, c) : w(l.textContent.replace(Le, ""), l, c))
+                            }, c) : w(l.textContent.replace(Fe, ""), l, c))
                     }
                     return e
                 }
 
-                function We(e, t, n) {
-                    for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(be(r)), r.parentNode && (n && se(r) && we(be(r, "script")), r.parentNode.removeChild(r));
+                function Ve(e, t, n) {
+                    for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(De(r)), r.parentNode && (n && ve(r) && Ne(De(r, "script")), r.parentNode.removeChild(r));
                     return e
                 }
                 S.extend({
                     htmlPrefilter: function(e) {
                         return e
                     },
                     clone: function(e, t, n) {
                         var r, i, o, a, s = e.cloneNode(!0),
-                            u = se(e);
+                            u = ve(e);
                         if (!(v.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
-                            for (a = be(s), r = 0, i = (o = be(e)).length; r < i; r++) Me(o[r], a[r]);
+                            for (a = De(s), r = 0, i = (o = De(e)).length; r < i; r++) Ue(o[r], a[r]);
                         if (t)
                             if (n)
-                                for (o = o || be(e), a = a || be(s), r = 0, i = o.length; r < i; r++) Re(o[r], a[r]);
-                            else Re(e, s);
-                        return (a = be(s, "script")).length > 0 && we(a, !u && be(e, "script")), s
+                                for (o = o || De(e), a = a || De(s), r = 0, i = o.length; r < i; r++) Xe(o[r], a[r]);
+                            else Xe(e, s);
+                        return (a = De(s, "script")).length > 0 && Ne(a, !u && De(e, "script")), s
                     },
                     cleanData: function(e) {
                         for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
-                            if (Q(n)) {
-                                if (t = n[K.expando]) {
+                            if (oe(n)) {
+                                if (t = n[se.expando]) {
                                     if (t.events)
                                         for (r in t.events) i[r] ? S.event.remove(n, r) : S.removeEvent(n, r, t.handle);
-                                    n[K.expando] = void 0
+                                    n[se.expando] = void 0
                                 }
-                                n[Z.expando] && (n[Z.expando] = void 0)
+                                n[ue.expando] && (n[ue.expando] = void 0)
                             }
                     }
                 }), S.fn.extend({
                     detach: function(e) {
-                        return We(this, e, !0)
+                        return Ve(this, e, !0)
                     },
                     remove: function(e) {
-                        return We(this, e)
+                        return Ve(this, e)
                     },
                     text: function(e) {
-                        return U(this, (function(e) {
+                        return ee(this, (function(e) {
                             return void 0 === e ? S.text(this) : this.empty().each((function() {
                                 1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                             }))
                         }), null, e, arguments.length)
                     },
                     append: function() {
-                        return Ie(this, arguments, (function(e) {
-                            1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || He(this, e).appendChild(e)
+                        return ze(this, arguments, (function(e) {
+                            1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || $e(this, e).appendChild(e)
                         }))
                     },
                     prepend: function() {
-                        return Ie(this, arguments, (function(e) {
+                        return ze(this, arguments, (function(e) {
                             if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                                var t = He(this, e);
+                                var t = $e(this, e);
                                 t.insertBefore(e, t.firstChild)
                             }
                         }))
                     },
                     before: function() {
-                        return Ie(this, arguments, (function(e) {
+                        return ze(this, arguments, (function(e) {
                             this.parentNode && this.parentNode.insertBefore(e, this)
                         }))
                     },
                     after: function() {
-                        return Ie(this, arguments, (function(e) {
+                        return ze(this, arguments, (function(e) {
                             this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
                         }))
                     },
                     empty: function() {
-                        for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(be(e, !1)), e.textContent = "");
+                        for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(De(e, !1)), e.textContent = "");
                         return this
                     },
                     clone: function(e, t) {
                         return e = null != e && e, t = null == t ? e : t, this.map((function() {
                             return S.clone(this, e, t)
                         }))
                     },
                     html: function(e) {
-                        return U(this, (function(e) {
+                        return ee(this, (function(e) {
                             var t = this[0] || {},
                                 n = 0,
                                 r = this.length;
                             if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                            if ("string" == typeof e && !De.test(e) && !xe[(ye.exec(e) || ["", ""])[1].toLowerCase()]) {
+                            if ("string" == typeof e && !Ie.test(e) && !Ae[(Ee.exec(e) || ["", ""])[1].toLowerCase()]) {
                                 e = S.htmlPrefilter(e);
                                 try {
-                                    for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(be(t, !1)), t.innerHTML = e);
+                                    for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(De(t, !1)), t.innerHTML = e);
                                     t = 0
                                 } catch (e) {}
                             }
                             t && this.empty().append(e)
                         }), null, e, arguments.length)
                     },
                     replaceWith: function() {
                         var e = [];
-                        return Ie(this, arguments, (function(t) {
+                        return ze(this, arguments, (function(t) {
                             var n = this.parentNode;
-                            S.inArray(this, e) < 0 && (S.cleanData(be(this)), n && n.replaceChild(t, this))
+                            S.inArray(this, e) < 0 && (S.cleanData(De(this)), n && n.replaceChild(t, this))
                         }), e)
                     }
                 }), S.each({
                     appendTo: "append",
                     prependTo: "prepend",
                     insertBefore: "before",
                     insertAfter: "after",
                     replaceAll: "replaceWith"
                 }, (function(e, t) {
                     S.fn[e] = function(e) {
                         for (var n, r = [], i = S(e), o = i.length - 1, a = 0; a <= o; a++) n = a === o ? this : this.clone(!0), S(i[a])[t](n), l.apply(r, n.get());
                         return this.pushStack(r)
                     }
                 }));
-                var Fe = new RegExp("^(" + re + ")(?!px)[a-z%]+$", "i"),
-                    $e = /^--/,
-                    Be = function(e) {
+                var Ge = new RegExp("^(" + pe + ")(?!px)[a-z%]+$", "i"),
+                    Ye = /^--/,
+                    Qe = function(e) {
                         var t = e.ownerDocument.defaultView;
                         return t && t.opener || (t = r), t.getComputedStyle(e)
                     },
-                    _e = function(e, t, n) {
+                    Je = function(e, t, n) {
                         var r, i, o = {};
                         for (i in t) o[i] = e.style[i], e.style[i] = t[i];
                         for (i in r = n.call(e), t) e.style[i] = o[i];
                         return r
                     },
-                    ze = new RegExp(oe.join("|"), "i"),
-                    Ue = "[\\x20\\t\\r\\n\\f]",
-                    Xe = new RegExp("^" + Ue + "+|((?:^|[^\\\\])(?:\\\\.)*)" + Ue + "+$", "g");
+                    Ke = new RegExp(he.join("|"), "i");
 
-                function Ve(e, t, n) {
-                    var r, i, o, a, s = $e.test(t),
+                function Ze(e, t, n) {
+                    var r, i, o, a, s = Ye.test(t),
                         u = e.style;
-                    return (n = n || Be(e)) && (a = n.getPropertyValue(t) || n[t], s && a && (a = a.replace(Xe, "$1") || void 0), "" !== a || se(e) || (a = S.style(e, t)), !v.pixelBoxStyles() && Fe.test(a) && ze.test(t) && (r = u.width, i = u.minWidth, o = u.maxWidth, u.minWidth = u.maxWidth = u.width = a, a = n.width, u.width = r, u.minWidth = i, u.maxWidth = o)), void 0 !== a ? a + "" : a
+                    return (n = n || Qe(e)) && (a = n.getPropertyValue(t) || n[t], s && a && (a = a.replace(L, "$1") || void 0), "" !== a || ve(e) || (a = S.style(e, t)), !v.pixelBoxStyles() && Ge.test(a) && Ke.test(t) && (r = u.width, i = u.minWidth, o = u.maxWidth, u.minWidth = u.maxWidth = u.width = a, a = n.width, u.width = r, u.minWidth = i, u.maxWidth = o)), void 0 !== a ? a + "" : a
                 }
 
-                function Ge(e, t) {
+                function et(e, t) {
                     return {
                         get: function() {
                             if (!e()) return (this.get = t).apply(this, arguments);
                             delete this.get
                         }
                     }
                 }! function() {
                     function e() {
                         if (c) {
-                            l.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", c.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ae.appendChild(l).appendChild(c);
+                            l.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", c.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ge.appendChild(l).appendChild(c);
                             var e = r.getComputedStyle(c);
-                            n = "1%" !== e.top, u = 12 === t(e.marginLeft), c.style.right = "60%", a = 36 === t(e.right), i = 36 === t(e.width), c.style.position = "absolute", o = 12 === t(c.offsetWidth / 3), ae.removeChild(l), c = null
+                            n = "1%" !== e.top, u = 12 === t(e.marginLeft), c.style.right = "60%", a = 36 === t(e.right), i = 36 === t(e.width), c.style.position = "absolute", o = 12 === t(c.offsetWidth / 3), ge.removeChild(l), c = null
                         }
                     }
 
                     function t(e) {
                         return Math.round(parseFloat(e))
                     }
                     var n, i, o, a, s, u, l = x.createElement("div"),
@@ -1983,244 +1943,252 @@
                             return e(), u
                         },
                         scrollboxSize: function() {
                             return e(), o
                         },
                         reliableTrDimensions: function() {
                             var e, t, n, i;
-                            return null == s && (e = x.createElement("table"), t = x.createElement("tr"), n = x.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", ae.appendChild(e).appendChild(t).appendChild(n), i = r.getComputedStyle(t), s = parseInt(i.height, 10) + parseInt(i.borderTopWidth, 10) + parseInt(i.borderBottomWidth, 10) === t.offsetHeight, ae.removeChild(e)), s
+                            return null == s && (e = x.createElement("table"), t = x.createElement("tr"), n = x.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", ge.appendChild(e).appendChild(t).appendChild(n), i = r.getComputedStyle(t), s = parseInt(i.height, 10) + parseInt(i.borderTopWidth, 10) + parseInt(i.borderBottomWidth, 10) === t.offsetHeight, ge.removeChild(e)), s
                         }
                     }))
                 }();
-                var Ye = ["Webkit", "Moz", "ms"],
-                    Qe = x.createElement("div").style,
-                    Je = {};
-
-                function Ke(e) {
-                    return S.cssProps[e] || Je[e] || (e in Qe ? e : Je[e] = function(e) {
-                        for (var t = e[0].toUpperCase() + e.slice(1), n = Ye.length; n--;)
-                            if ((e = Ye[n] + t) in Qe) return e
+                var tt = ["Webkit", "Moz", "ms"],
+                    nt = x.createElement("div").style,
+                    rt = {};
+
+                function it(e) {
+                    return S.cssProps[e] || rt[e] || (e in nt ? e : rt[e] = function(e) {
+                        for (var t = e[0].toUpperCase() + e.slice(1), n = tt.length; n--;)
+                            if ((e = tt[n] + t) in nt) return e
                     }(e) || e)
                 }
-                var Ze = /^(none|table(?!-c[ea]).+)/,
-                    et = {
+                var ot = /^(none|table(?!-c[ea]).+)/,
+                    at = {
                         position: "absolute",
                         visibility: "hidden",
                         display: "block"
                     },
-                    tt = {
+                    st = {
                         letterSpacing: "0",
                         fontWeight: "400"
                     };
 
-                function nt(e, t, n) {
-                    var r = ie.exec(t);
+                function ut(e, t, n) {
+                    var r = de.exec(t);
                     return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
                 }
 
-                function rt(e, t, n, r, i, o) {
+                function lt(e, t, n, r, i, o) {
                     var a = "width" === t ? 1 : 0,
                         s = 0,
-                        u = 0;
+                        u = 0,
+                        l = 0;
                     if (n === (r ? "border" : "content")) return 0;
-                    for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + oe[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + oe[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + oe[a] + "Width", !0, i))) : (u += S.css(e, "padding" + oe[a], !0, i), "padding" !== n ? u += S.css(e, "border" + oe[a] + "Width", !0, i) : s += S.css(e, "border" + oe[a] + "Width", !0, i));
-                    return !r && o >= 0 && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
+                    for (; a < 4; a += 2) "margin" === n && (l += S.css(e, n + he[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + he[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + he[a] + "Width", !0, i))) : (u += S.css(e, "padding" + he[a], !0, i), "padding" !== n ? u += S.css(e, "border" + he[a] + "Width", !0, i) : s += S.css(e, "border" + he[a] + "Width", !0, i));
+                    return !r && o >= 0 && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u + l
                 }
 
-                function it(e, t, n) {
-                    var r = Be(e),
+                function ct(e, t, n) {
+                    var r = Qe(e),
                         i = (!v.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
                         o = i,
-                        a = Ve(e, t, r),
+                        a = Ze(e, t, r),
                         s = "offset" + t[0].toUpperCase() + t.slice(1);
-                    if (Fe.test(a)) {
+                    if (Ge.test(a)) {
                         if (!n) return a;
                         a = "auto"
                     }
-                    return (!v.boxSizingReliable() && i || !v.reliableTrDimensions() && D(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + rt(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+                    return (!v.boxSizingReliable() && i || !v.reliableTrDimensions() && j(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + lt(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
                 }
 
-                function ot(e, t, n, r, i) {
-                    return new ot.prototype.init(e, t, n, r, i)
+                function ft(e, t, n, r, i) {
+                    return new ft.prototype.init(e, t, n, r, i)
                 }
                 S.extend({
                     cssHooks: {
                         opacity: {
                             get: function(e, t) {
                                 if (t) {
-                                    var n = Ve(e, "opacity");
+                                    var n = Ze(e, "opacity");
                                     return "" === n ? "1" : n
                                 }
                             }
                         }
                     },
                     cssNumber: {
                         animationIterationCount: !0,
+                        aspectRatio: !0,
+                        borderImageSlice: !0,
                         columnCount: !0,
-                        fillOpacity: !0,
                         flexGrow: !0,
                         flexShrink: !0,
                         fontWeight: !0,
                         gridArea: !0,
                         gridColumn: !0,
                         gridColumnEnd: !0,
                         gridColumnStart: !0,
                         gridRow: !0,
                         gridRowEnd: !0,
                         gridRowStart: !0,
                         lineHeight: !0,
                         opacity: !0,
                         order: !0,
                         orphans: !0,
+                        scale: !0,
                         widows: !0,
                         zIndex: !0,
-                        zoom: !0
+                        zoom: !0,
+                        fillOpacity: !0,
+                        floodOpacity: !0,
+                        stopOpacity: !0,
+                        strokeMiterlimit: !0,
+                        strokeOpacity: !0
                     },
                     cssProps: {},
                     style: function(e, t, n, r) {
                         if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
-                            var i, o, a, s = Y(t),
-                                u = $e.test(t),
+                            var i, o, a, s = ie(t),
+                                u = Ye.test(t),
                                 l = e.style;
-                            if (u || (t = Ke(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
-                            "string" == (o = typeof n) && (i = ie.exec(n)) && i[1] && (n = ce(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), v.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
+                            if (u || (t = it(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                            "string" == (o = typeof n) && (i = de.exec(n)) && i[1] && (n = xe(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), v.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
                         }
                     },
                     css: function(e, t, n, r) {
-                        var i, o, a, s = Y(t);
-                        return $e.test(t) || (t = Ke(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Ve(e, t, r)), "normal" === i && t in tt && (i = tt[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+                        var i, o, a, s = ie(t);
+                        return Ye.test(t) || (t = it(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Ze(e, t, r)), "normal" === i && t in st && (i = st[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
                     }
                 }), S.each(["height", "width"], (function(e, t) {
                     S.cssHooks[t] = {
                         get: function(e, n, r) {
-                            if (n) return !Ze.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? it(e, t, r) : _e(e, et, (function() {
-                                return it(e, t, r)
+                            if (n) return !ot.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? ct(e, t, r) : Je(e, at, (function() {
+                                return ct(e, t, r)
                             }))
                         },
                         set: function(e, n, r) {
-                            var i, o = Be(e),
+                            var i, o = Qe(e),
                                 a = !v.scrollboxSize() && "absolute" === o.position,
                                 s = (a || r) && "border-box" === S.css(e, "boxSizing", !1, o),
-                                u = r ? rt(e, t, r, s, o) : 0;
-                            return s && a && (u -= Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - parseFloat(o[t]) - rt(e, t, "border", !1, o) - .5)), u && (i = ie.exec(n)) && "px" !== (i[3] || "px") && (e.style[t] = n, n = S.css(e, t)), nt(0, n, u)
+                                u = r ? lt(e, t, r, s, o) : 0;
+                            return s && a && (u -= Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - parseFloat(o[t]) - lt(e, t, "border", !1, o) - .5)), u && (i = de.exec(n)) && "px" !== (i[3] || "px") && (e.style[t] = n, n = S.css(e, t)), ut(0, n, u)
                         }
                     }
-                })), S.cssHooks.marginLeft = Ge(v.reliableMarginLeft, (function(e, t) {
-                    if (t) return (parseFloat(Ve(e, "marginLeft")) || e.getBoundingClientRect().left - _e(e, {
+                })), S.cssHooks.marginLeft = et(v.reliableMarginLeft, (function(e, t) {
+                    if (t) return (parseFloat(Ze(e, "marginLeft")) || e.getBoundingClientRect().left - Je(e, {
                         marginLeft: 0
                     }, (function() {
                         return e.getBoundingClientRect().left
                     }))) + "px"
                 })), S.each({
                     margin: "",
                     padding: "",
                     border: "Width"
                 }, (function(e, t) {
                     S.cssHooks[e + t] = {
                         expand: function(n) {
-                            for (var r = 0, i = {}, o = "string" == typeof n ? n.split(" ") : [n]; r < 4; r++) i[e + oe[r] + t] = o[r] || o[r - 2] || o[0];
+                            for (var r = 0, i = {}, o = "string" == typeof n ? n.split(" ") : [n]; r < 4; r++) i[e + he[r] + t] = o[r] || o[r - 2] || o[0];
                             return i
                         }
-                    }, "margin" !== e && (S.cssHooks[e + t].set = nt)
+                    }, "margin" !== e && (S.cssHooks[e + t].set = ut)
                 })), S.fn.extend({
                     css: function(e, t) {
-                        return U(this, (function(e, t, n) {
+                        return ee(this, (function(e, t, n) {
                             var r, i, o = {},
                                 a = 0;
                             if (Array.isArray(t)) {
-                                for (r = Be(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                                for (r = Qe(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                                 return o
                             }
                             return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
                         }), e, t, arguments.length > 1)
                     }
-                }), S.Tween = ot, ot.prototype = {
-                    constructor: ot,
+                }), S.Tween = ft, ft.prototype = {
+                    constructor: ft,
                     init: function(e, t, n, r, i, o) {
                         this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
                     },
                     cur: function() {
-                        var e = ot.propHooks[this.prop];
-                        return e && e.get ? e.get(this) : ot.propHooks._default.get(this)
+                        var e = ft.propHooks[this.prop];
+                        return e && e.get ? e.get(this) : ft.propHooks._default.get(this)
                     },
                     run: function(e) {
-                        var t, n = ot.propHooks[this.prop];
-                        return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : ot.propHooks._default.set(this), this
+                        var t, n = ft.propHooks[this.prop];
+                        return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : ft.propHooks._default.set(this), this
                     }
-                }, ot.prototype.init.prototype = ot.prototype, ot.propHooks = {
+                }, ft.prototype.init.prototype = ft.prototype, ft.propHooks = {
                     _default: {
                         get: function(e) {
                             var t;
                             return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
                         },
                         set: function(e) {
-                            S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Ke(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
+                            S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[it(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
                         }
                     }
-                }, ot.propHooks.scrollTop = ot.propHooks.scrollLeft = {
+                }, ft.propHooks.scrollTop = ft.propHooks.scrollLeft = {
                     set: function(e) {
                         e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
                     }
                 }, S.easing = {
                     linear: function(e) {
                         return e
                     },
                     swing: function(e) {
                         return .5 - Math.cos(e * Math.PI) / 2
                     },
                     _default: "swing"
-                }, S.fx = ot.prototype.init, S.fx.step = {};
-                var at, st, ut = /^(?:toggle|show|hide)$/,
-                    lt = /queueHooks$/;
+                }, S.fx = ft.prototype.init, S.fx.step = {};
+                var pt, dt, ht = /^(?:toggle|show|hide)$/,
+                    gt = /queueHooks$/;
 
-                function ct() {
-                    st && (!1 === x.hidden && r.requestAnimationFrame ? r.requestAnimationFrame(ct) : r.setTimeout(ct, S.fx.interval), S.fx.tick())
+                function vt() {
+                    dt && (!1 === x.hidden && r.requestAnimationFrame ? r.requestAnimationFrame(vt) : r.setTimeout(vt, S.fx.interval), S.fx.tick())
                 }
 
-                function ft() {
+                function yt() {
                     return r.setTimeout((function() {
-                        at = void 0
-                    })), at = Date.now()
+                        pt = void 0
+                    })), pt = Date.now()
                 }
 
-                function pt(e, t) {
+                function mt(e, t) {
                     var n, r = 0,
                         i = {
                             height: e
                         };
-                    for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = oe[r])] = i["padding" + n] = e;
+                    for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = he[r])] = i["padding" + n] = e;
                     return t && (i.opacity = i.width = e), i
                 }
 
-                function dt(e, t, n) {
-                    for (var r, i = (ht.tweeners[t] || []).concat(ht.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+                function xt(e, t, n) {
+                    for (var r, i = (bt.tweeners[t] || []).concat(bt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
                         if (r = i[o].call(n, t, e)) return r
                 }
 
-                function ht(e, t, n) {
+                function bt(e, t, n) {
                     var r, i, o = 0,
-                        a = ht.prefilters.length,
+                        a = bt.prefilters.length,
                         s = S.Deferred().always((function() {
                             delete u.elem
                         })),
                         u = function() {
                             if (i) return !1;
-                            for (var t = at || ft(), n = Math.max(0, l.startTime + l.duration - t), r = 1 - (n / l.duration || 0), o = 0, a = l.tweens.length; o < a; o++) l.tweens[o].run(r);
+                            for (var t = pt || yt(), n = Math.max(0, l.startTime + l.duration - t), r = 1 - (n / l.duration || 0), o = 0, a = l.tweens.length; o < a; o++) l.tweens[o].run(r);
                             return s.notifyWith(e, [l, r, n]), r < 1 && a ? n : (a || s.notifyWith(e, [l, 1, 0]), s.resolveWith(e, [l]), !1)
                         },
                         l = s.promise({
                             elem: e,
                             props: S.extend({}, t),
                             opts: S.extend(!0, {
                                 specialEasing: {},
                                 easing: S.easing._default
                             }, n),
                             originalProperties: t,
                             originalOptions: n,
-                            startTime: at || ft(),
+                            startTime: pt || yt(),
                             duration: n.duration,
                             tweens: [],
                             createTween: function(t, n) {
                                 var r = S.Tween(e, l.opts, t, n, l.opts.specialEasing[t] || l.opts.easing);
                                 return l.tweens.push(r), r
                             },
                             stop: function(t) {
@@ -2231,132 +2199,132 @@
                                 return t ? (s.notifyWith(e, [l, 1, 0]), s.resolveWith(e, [l, t])) : s.rejectWith(e, [l, t]), this
                             }
                         }),
                         c = l.props;
                     for (function(e, t) {
                             var n, r, i, o, a;
                             for (n in e)
-                                if (i = t[r = Y(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
+                                if (i = t[r = ie(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                                     for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                                 else t[r] = i
                         }(c, l.opts.specialEasing); o < a; o++)
-                        if (r = ht.prefilters[o].call(l, e, c, l.opts)) return y(r.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = r.stop.bind(r)), r;
-                    return S.map(c, dt, l), y(l.opts.start) && l.opts.start.call(e, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+                        if (r = bt.prefilters[o].call(l, e, c, l.opts)) return y(r.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = r.stop.bind(r)), r;
+                    return S.map(c, xt, l), y(l.opts.start) && l.opts.start.call(e, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
                         elem: e,
                         anim: l,
                         queue: l.opts.queue
                     })), l
                 }
-                S.Animation = S.extend(ht, {
+                S.Animation = S.extend(bt, {
                         tweeners: {
                             "*": [function(e, t) {
                                 var n = this.createTween(e, t);
-                                return ce(n.elem, e, ie.exec(t), n), n
+                                return xe(n.elem, e, de.exec(t), n), n
                             }]
                         },
                         tweener: function(e, t) {
-                            y(e) ? (t = e, e = ["*"]) : e = e.match(I);
-                            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ht.tweeners[n] = ht.tweeners[n] || [], ht.tweeners[n].unshift(t)
+                            y(e) ? (t = e, e = ["*"]) : e = e.match(V);
+                            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], bt.tweeners[n] = bt.tweeners[n] || [], bt.tweeners[n].unshift(t)
                         },
                         prefilters: [function(e, t, n) {
                             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                                 p = this,
                                 d = {},
                                 h = e.style,
-                                g = e.nodeType && le(e),
-                                v = K.get(e, "fxshow");
+                                g = e.nodeType && me(e),
+                                v = se.get(e, "fxshow");
                             for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                                     a.unqueued || s()
                                 }), a.unqueued++, p.always((function() {
                                     p.always((function() {
                                         a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                                     }))
                                 }))), t)
-                                if (i = t[r], ut.test(i)) {
+                                if (i = t[r], ht.test(i)) {
                                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                                         if ("show" !== i || !v || void 0 === v[r]) continue;
                                         g = !0
                                     }
                                     d[r] = v && v[r] || S.style(e, r)
                                 } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
-                                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = K.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (de([e], !0), l = e.style.display || l, c = S.css(e, "display"), de([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done((function() {
+                                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = se.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (Te([e], !0), l = e.style.display || l, c = S.css(e, "display"), Te([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done((function() {
                                         h.display = l
                                     })), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always((function() {
                                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
-                                    }))), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = K.access(e, "fxshow", {
+                                    }))), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = se.access(e, "fxshow", {
                                     display: l
-                                }), o && (v.hidden = !g), g && de([e], !0), p.done((function() {
-                                    for (r in g || de([e]), K.remove(e, "fxshow"), d) S.style(e, r, d[r])
-                                }))), u = dt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                                }), o && (v.hidden = !g), g && Te([e], !0), p.done((function() {
+                                    for (r in g || Te([e]), se.remove(e, "fxshow"), d) S.style(e, r, d[r])
+                                }))), u = xt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
                         }],
                         prefilter: function(e, t) {
-                            t ? ht.prefilters.unshift(e) : ht.prefilters.push(e)
+                            t ? bt.prefilters.unshift(e) : bt.prefilters.push(e)
                         }
                     }), S.speed = function(e, t, n) {
                         var r = e && "object" == typeof e ? S.extend({}, e) : {
                             complete: n || !n && t || y(e) && e,
                             duration: e,
                             easing: n && t || t && !y(t) && t
                         };
                         return S.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in S.fx.speeds ? r.duration = S.fx.speeds[r.duration] : r.duration = S.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
                             y(r.old) && r.old.call(this), r.queue && S.dequeue(this, r.queue)
                         }, r
                     }, S.fn.extend({
                         fadeTo: function(e, t, n, r) {
-                            return this.filter(le).css("opacity", 0).show().end().animate({
+                            return this.filter(me).css("opacity", 0).show().end().animate({
                                 opacity: t
                             }, e, n, r)
                         },
                         animate: function(e, t, n, r) {
                             var i = S.isEmptyObject(e),
                                 o = S.speed(t, n, r),
                                 a = function() {
-                                    var t = ht(this, S.extend({}, e), o);
-                                    (i || K.get(this, "finish")) && t.stop(!0)
+                                    var t = bt(this, S.extend({}, e), o);
+                                    (i || se.get(this, "finish")) && t.stop(!0)
                                 };
                             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
                         },
                         stop: function(e, t, n) {
                             var r = function(e) {
                                 var t = e.stop;
                                 delete e.stop, t(n)
                             };
                             return "string" != typeof e && (n = t, t = e, e = void 0), t && this.queue(e || "fx", []), this.each((function() {
                                 var t = !0,
                                     i = null != e && e + "queueHooks",
                                     o = S.timers,
-                                    a = K.get(this);
+                                    a = se.get(this);
                                 if (i) a[i] && a[i].stop && r(a[i]);
                                 else
-                                    for (i in a) a[i] && a[i].stop && lt.test(i) && r(a[i]);
+                                    for (i in a) a[i] && a[i].stop && gt.test(i) && r(a[i]);
                                 for (i = o.length; i--;) o[i].elem !== this || null != e && o[i].queue !== e || (o[i].anim.stop(n), t = !1, o.splice(i, 1));
                                 !t && n || S.dequeue(this, e)
                             }))
                         },
                         finish: function(e) {
                             return !1 !== e && (e = e || "fx"), this.each((function() {
-                                var t, n = K.get(this),
+                                var t, n = se.get(this),
                                     r = n[e + "queue"],
                                     i = n[e + "queueHooks"],
                                     o = S.timers,
                                     a = r ? r.length : 0;
                                 for (n.finish = !0, S.queue(this, e, []), i && i.stop && i.stop.call(this, !0), t = o.length; t--;) o[t].elem === this && o[t].queue === e && (o[t].anim.stop(!0), o.splice(t, 1));
                                 for (t = 0; t < a; t++) r[t] && r[t].finish && r[t].finish.call(this);
                                 delete n.finish
                             }))
                         }
                     }), S.each(["toggle", "show", "hide"], (function(e, t) {
                         var n = S.fn[t];
                         S.fn[t] = function(e, r, i) {
-                            return null == e || "boolean" == typeof e ? n.apply(this, arguments) : this.animate(pt(t, !0), e, r, i)
+                            return null == e || "boolean" == typeof e ? n.apply(this, arguments) : this.animate(mt(t, !0), e, r, i)
                         }
                     })), S.each({
-                        slideDown: pt("show"),
-                        slideUp: pt("hide"),
-                        slideToggle: pt("toggle"),
+                        slideDown: mt("show"),
+                        slideUp: mt("hide"),
+                        slideToggle: mt("toggle"),
                         fadeIn: {
                             opacity: "show"
                         },
                         fadeOut: {
                             opacity: "hide"
                         },
                         fadeToggle: {
@@ -2365,22 +2333,22 @@
                     }, (function(e, t) {
                         S.fn[e] = function(e, n, r) {
                             return this.animate(t, e, n, r)
                         }
                     })), S.timers = [], S.fx.tick = function() {
                         var e, t = 0,
                             n = S.timers;
-                        for (at = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-                        n.length || S.fx.stop(), at = void 0
+                        for (pt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+                        n.length || S.fx.stop(), pt = void 0
                     }, S.fx.timer = function(e) {
                         S.timers.push(e), S.fx.start()
                     }, S.fx.interval = 13, S.fx.start = function() {
-                        st || (st = !0, ct())
+                        dt || (dt = !0, vt())
                     }, S.fx.stop = function() {
-                        st = null
+                        dt = null
                     }, S.fx.speeds = {
                         slow: 600,
                         fast: 200,
                         _default: 400
                     }, S.fn.delay = function(e, t) {
                         return e = S.fx && S.fx.speeds[e] || e, t = t || "fx", this.queue(t, (function(t, n) {
                             var i = r.setTimeout(t, e);
@@ -2390,73 +2358,73 @@
                         }))
                     },
                     function() {
                         var e = x.createElement("input"),
                             t = x.createElement("select").appendChild(x.createElement("option"));
                         e.type = "checkbox", v.checkOn = "" !== e.value, v.optSelected = t.selected, (e = x.createElement("input")).value = "t", e.type = "radio", v.radioValue = "t" === e.value
                     }();
-                var gt, vt = S.expr.attrHandle;
+                var wt, Tt = S.expr.attrHandle;
                 S.fn.extend({
                     attr: function(e, t) {
-                        return U(this, S.attr, e, t, arguments.length > 1)
+                        return ee(this, S.attr, e, t, arguments.length > 1)
                     },
                     removeAttr: function(e) {
                         return this.each((function() {
                             S.removeAttr(this, e)
                         }))
                     }
                 }), S.extend({
                     attr: function(e, t, n) {
                         var r, i, o = e.nodeType;
-                        if (3 !== o && 8 !== o && 2 !== o) return void 0 === e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? gt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
+                        if (3 !== o && 8 !== o && 2 !== o) return void 0 === e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? wt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
                     },
                     attrHooks: {
                         type: {
                             set: function(e, t) {
-                                if (!v.radioValue && "radio" === t && D(e, "input")) {
+                                if (!v.radioValue && "radio" === t && j(e, "input")) {
                                     var n = e.value;
                                     return e.setAttribute("type", t), n && (e.value = n), t
                                 }
                             }
                         }
                     },
                     removeAttr: function(e, t) {
                         var n, r = 0,
-                            i = t && t.match(I);
+                            i = t && t.match(V);
                         if (i && 1 === e.nodeType)
                             for (; n = i[r++];) e.removeAttribute(n)
                     }
-                }), gt = {
+                }), wt = {
                     set: function(e, t, n) {
                         return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
                     }
                 }, S.each(S.expr.match.bool.source.match(/\w+/g), (function(e, t) {
-                    var n = vt[t] || S.find.attr;
-                    vt[t] = function(e, t, r) {
+                    var n = Tt[t] || S.find.attr;
+                    Tt[t] = function(e, t, r) {
                         var i, o, a = t.toLowerCase();
-                        return r || (o = vt[a], vt[a] = i, i = null != n(e, t, r) ? a : null, vt[a] = o), i
+                        return r || (o = Tt[a], Tt[a] = i, i = null != n(e, t, r) ? a : null, Tt[a] = o), i
                     }
                 }));
-                var yt = /^(?:input|select|textarea|button)$/i,
-                    mt = /^(?:a|area)$/i;
+                var Ct = /^(?:input|select|textarea|button)$/i,
+                    kt = /^(?:a|area)$/i;
 
-                function xt(e) {
-                    return (e.match(I) || []).join(" ")
+                function St(e) {
+                    return (e.match(V) || []).join(" ")
                 }
 
-                function bt(e) {
+                function Et(e) {
                     return e.getAttribute && e.getAttribute("class") || ""
                 }
 
-                function wt(e) {
-                    return Array.isArray(e) ? e : "string" == typeof e && e.match(I) || []
+                function jt(e) {
+                    return Array.isArray(e) ? e : "string" == typeof e && e.match(V) || []
                 }
                 S.fn.extend({
                     prop: function(e, t) {
-                        return U(this, S.prop, e, t, arguments.length > 1)
+                        return ee(this, S.prop, e, t, arguments.length > 1)
                     },
                     removeProp: function(e) {
                         return this.each((function() {
                             delete this[S.propFix[e] || e]
                         }))
                     }
                 }), S.extend({
@@ -2464,15 +2432,15 @@
                         var r, i, o = e.nodeType;
                         if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
                     },
                     propHooks: {
                         tabIndex: {
                             get: function(e) {
                                 var t = S.find.attr(e, "tabindex");
-                                return t ? parseInt(t, 10) : yt.test(e.nodeName) || mt.test(e.nodeName) && e.href ? 0 : -1
+                                return t ? parseInt(t, 10) : Ct.test(e.nodeName) || kt.test(e.nodeName) && e.href ? 0 : -1
                             }
                         }
                     },
                     propFix: {
                         for: "htmlFor",
                         class: "className"
                     }
@@ -2487,80 +2455,80 @@
                     }
                 }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], (function() {
                     S.propFix[this.toLowerCase()] = this
                 })), S.fn.extend({
                     addClass: function(e) {
                         var t, n, r, i, o, a;
                         return y(e) ? this.each((function(t) {
-                            S(this).addClass(e.call(this, t, bt(this)))
-                        })) : (t = wt(e)).length ? this.each((function() {
-                            if (r = bt(this), n = 1 === this.nodeType && " " + xt(r) + " ") {
+                            S(this).addClass(e.call(this, t, Et(this)))
+                        })) : (t = jt(e)).length ? this.each((function() {
+                            if (r = Et(this), n = 1 === this.nodeType && " " + St(r) + " ") {
                                 for (o = 0; o < t.length; o++) i = t[o], n.indexOf(" " + i + " ") < 0 && (n += i + " ");
-                                a = xt(n), r !== a && this.setAttribute("class", a)
+                                a = St(n), r !== a && this.setAttribute("class", a)
                             }
                         })) : this
                     },
                     removeClass: function(e) {
                         var t, n, r, i, o, a;
                         return y(e) ? this.each((function(t) {
-                            S(this).removeClass(e.call(this, t, bt(this)))
-                        })) : arguments.length ? (t = wt(e)).length ? this.each((function() {
-                            if (r = bt(this), n = 1 === this.nodeType && " " + xt(r) + " ") {
+                            S(this).removeClass(e.call(this, t, Et(this)))
+                        })) : arguments.length ? (t = jt(e)).length ? this.each((function() {
+                            if (r = Et(this), n = 1 === this.nodeType && " " + St(r) + " ") {
                                 for (o = 0; o < t.length; o++)
                                     for (i = t[o]; n.indexOf(" " + i + " ") > -1;) n = n.replace(" " + i + " ", " ");
-                                a = xt(n), r !== a && this.setAttribute("class", a)
+                                a = St(n), r !== a && this.setAttribute("class", a)
                             }
                         })) : this : this.attr("class", "")
                     },
                     toggleClass: function(e, t) {
                         var n, r, i, o, a = typeof e,
                             s = "string" === a || Array.isArray(e);
                         return y(e) ? this.each((function(n) {
-                            S(this).toggleClass(e.call(this, n, bt(this), t), t)
-                        })) : "boolean" == typeof t && s ? t ? this.addClass(e) : this.removeClass(e) : (n = wt(e), this.each((function() {
+                            S(this).toggleClass(e.call(this, n, Et(this), t), t)
+                        })) : "boolean" == typeof t && s ? t ? this.addClass(e) : this.removeClass(e) : (n = jt(e), this.each((function() {
                             if (s)
                                 for (o = S(this), i = 0; i < n.length; i++) r = n[i], o.hasClass(r) ? o.removeClass(r) : o.addClass(r);
-                            else void 0 !== e && "boolean" !== a || ((r = bt(this)) && K.set(this, "__className__", r), this.setAttribute && this.setAttribute("class", r || !1 === e ? "" : K.get(this, "__className__") || ""))
+                            else void 0 !== e && "boolean" !== a || ((r = Et(this)) && se.set(this, "__className__", r), this.setAttribute && this.setAttribute("class", r || !1 === e ? "" : se.get(this, "__className__") || ""))
                         })))
                     },
                     hasClass: function(e) {
                         var t, n, r = 0;
                         for (t = " " + e + " "; n = this[r++];)
-                            if (1 === n.nodeType && (" " + xt(bt(n)) + " ").indexOf(t) > -1) return !0;
+                            if (1 === n.nodeType && (" " + St(Et(n)) + " ").indexOf(t) > -1) return !0;
                         return !1
                     }
                 });
-                var Tt = /\r/g;
+                var At = /\r/g;
                 S.fn.extend({
                     val: function(e) {
                         var t, n, r, i = this[0];
                         return arguments.length ? (r = y(e), this.each((function(n) {
                             var i;
                             1 === this.nodeType && (null == (i = r ? e.call(this, n, S(this).val()) : e) ? i = "" : "number" == typeof i ? i += "" : Array.isArray(i) && (i = S.map(i, (function(e) {
                                 return null == e ? "" : e + ""
                             }))), (t = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in t && void 0 !== t.set(this, i, "value") || (this.value = i))
-                        }))) : i ? (t = S.valHooks[i.type] || S.valHooks[i.nodeName.toLowerCase()]) && "get" in t && void 0 !== (n = t.get(i, "value")) ? n : "string" == typeof(n = i.value) ? n.replace(Tt, "") : null == n ? "" : n : void 0
+                        }))) : i ? (t = S.valHooks[i.type] || S.valHooks[i.nodeName.toLowerCase()]) && "get" in t && void 0 !== (n = t.get(i, "value")) ? n : "string" == typeof(n = i.value) ? n.replace(At, "") : null == n ? "" : n : void 0
                     }
                 }), S.extend({
                     valHooks: {
                         option: {
                             get: function(e) {
                                 var t = S.find.attr(e, "value");
-                                return null != t ? t : xt(S.text(e))
+                                return null != t ? t : St(S.text(e))
                             }
                         },
                         select: {
                             get: function(e) {
                                 var t, n, r, i = e.options,
                                     o = e.selectedIndex,
                                     a = "select-one" === e.type,
                                     s = a ? null : [],
                                     u = a ? o + 1 : i.length;
                                 for (r = o < 0 ? u : a ? o : 0; r < u; r++)
-                                    if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !D(n.parentNode, "optgroup"))) {
+                                    if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !j(n.parentNode, "optgroup"))) {
                                         if (t = S(n).val(), a) return t;
                                         s.push(t)
                                     } return s
                             },
                             set: function(e, t) {
                                 for (var n, r, i = e.options, o = S.makeArray(t), a = i.length; a--;)((r = i[a]).selected = S.inArray(S.valHooks.option.get(r), o) > -1) && (n = !0);
                                 return n || (e.selectedIndex = -1), o
@@ -2571,32 +2539,47 @@
                     S.valHooks[this] = {
                         set: function(e, t) {
                             if (Array.isArray(t)) return e.checked = S.inArray(S(e).val(), t) > -1
                         }
                     }, v.checkOn || (S.valHooks[this].get = function(e) {
                         return null === e.getAttribute("value") ? "on" : e.value
                     })
-                })), v.focusin = "onfocusin" in r;
-                var Ct = /^(?:focusinfocus|focusoutblur)$/,
-                    St = function(e) {
+                }));
+                var Dt = r.location,
+                    Nt = {
+                        guid: Date.now()
+                    },
+                    qt = /\?/;
+                S.parseXML = function(e) {
+                    var t, n;
+                    if (!e || "string" != typeof e) return null;
+                    try {
+                        t = (new r.DOMParser).parseFromString(e, "text/xml")
+                    } catch (e) {}
+                    return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, (function(e) {
+                        return e.textContent
+                    })).join("\n") : e)), t
+                };
+                var Lt = /^(?:focusinfocus|focusoutblur)$/,
+                    Ht = function(e) {
                         e.stopPropagation()
                     };
                 S.extend(S.event, {
                     trigger: function(e, t, n, i) {
                         var o, a, s, u, l, c, f, p, h = [n || x],
                             g = d.call(e, "type") ? e.type : e,
                             v = d.call(e, "namespace") ? e.namespace.split(".") : [];
-                        if (a = p = s = n = n || x, 3 !== n.nodeType && 8 !== n.nodeType && !Ct.test(g + S.event.triggered) && (g.indexOf(".") > -1 && (v = g.split("."), g = v.shift(), v.sort()), l = g.indexOf(":") < 0 && "on" + g, (e = e[S.expando] ? e : new S.Event(g, "object" == typeof e && e)).isTrigger = i ? 2 : 3, e.namespace = v.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + v.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), f = S.event.special[g] || {}, i || !f.trigger || !1 !== f.trigger.apply(n, t))) {
+                        if (a = p = s = n = n || x, 3 !== n.nodeType && 8 !== n.nodeType && !Lt.test(g + S.event.triggered) && (g.indexOf(".") > -1 && (v = g.split("."), g = v.shift(), v.sort()), l = g.indexOf(":") < 0 && "on" + g, (e = e[S.expando] ? e : new S.Event(g, "object" == typeof e && e)).isTrigger = i ? 2 : 3, e.namespace = v.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + v.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), f = S.event.special[g] || {}, i || !f.trigger || !1 !== f.trigger.apply(n, t))) {
                             if (!i && !f.noBubble && !m(n)) {
-                                for (u = f.delegateType || g, Ct.test(u + g) || (a = a.parentNode); a; a = a.parentNode) h.push(a), s = a;
+                                for (u = f.delegateType || g, Lt.test(u + g) || (a = a.parentNode); a; a = a.parentNode) h.push(a), s = a;
                                 s === (n.ownerDocument || x) && h.push(s.defaultView || s.parentWindow || r)
                             }
                             for (o = 0;
-                                (a = h[o++]) && !e.isPropagationStopped();) p = a, e.type = o > 1 ? u : f.bindType || g, (c = (K.get(a, "events") || Object.create(null))[e.type] && K.get(a, "handle")) && c.apply(a, t), (c = l && a[l]) && c.apply && Q(a) && (e.result = c.apply(a, t), !1 === e.result && e.preventDefault());
-                            return e.type = g, i || e.isDefaultPrevented() || f._default && !1 !== f._default.apply(h.pop(), t) || !Q(n) || l && y(n[g]) && !m(n) && ((s = n[l]) && (n[l] = null), S.event.triggered = g, e.isPropagationStopped() && p.addEventListener(g, St), n[g](), e.isPropagationStopped() && p.removeEventListener(g, St), S.event.triggered = void 0, s && (n[l] = s)), e.result
+                                (a = h[o++]) && !e.isPropagationStopped();) p = a, e.type = o > 1 ? u : f.bindType || g, (c = (se.get(a, "events") || Object.create(null))[e.type] && se.get(a, "handle")) && c.apply(a, t), (c = l && a[l]) && c.apply && oe(a) && (e.result = c.apply(a, t), !1 === e.result && e.preventDefault());
+                            return e.type = g, i || e.isDefaultPrevented() || f._default && !1 !== f._default.apply(h.pop(), t) || !oe(n) || l && y(n[g]) && !m(n) && ((s = n[l]) && (n[l] = null), S.event.triggered = g, e.isPropagationStopped() && p.addEventListener(g, Ht), n[g](), e.isPropagationStopped() && p.removeEventListener(g, Ht), S.event.triggered = void 0, s && (n[l] = s)), e.result
                         }
                     },
                     simulate: function(e, t, n) {
                         var r = S.extend(new S.Event, n, {
                             type: e,
                             isSimulated: !0
                         });
@@ -2608,155 +2591,121 @@
                             S.event.trigger(e, t, this)
                         }))
                     },
                     triggerHandler: function(e, t) {
                         var n = this[0];
                         if (n) return S.event.trigger(e, t, n, !0)
                     }
-                }), v.focusin || S.each({
-                    focus: "focusin",
-                    blur: "focusout"
-                }, (function(e, t) {
-                    var n = function(e) {
-                        S.event.simulate(t, e.target, S.event.fix(e))
-                    };
-                    S.event.special[t] = {
-                        setup: function() {
-                            var r = this.ownerDocument || this.document || this,
-                                i = K.access(r, t);
-                            i || r.addEventListener(e, n, !0), K.access(r, t, (i || 0) + 1)
-                        },
-                        teardown: function() {
-                            var r = this.ownerDocument || this.document || this,
-                                i = K.access(r, t) - 1;
-                            i ? K.access(r, t, i) : (r.removeEventListener(e, n, !0), K.remove(r, t))
-                        }
-                    }
-                }));
-                var Et = r.location,
-                    kt = {
-                        guid: Date.now()
-                    },
-                    At = /\?/;
-                S.parseXML = function(e) {
-                    var t, n;
-                    if (!e || "string" != typeof e) return null;
-                    try {
-                        t = (new r.DOMParser).parseFromString(e, "text/xml")
-                    } catch (e) {}
-                    return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, (function(e) {
-                        return e.textContent
-                    })).join("\n") : e)), t
-                };
-                var jt = /\[\]$/,
-                    Nt = /\r?\n/g,
-                    Dt = /^(?:submit|button|image|reset|file)$/i,
-                    qt = /^(?:input|select|textarea|keygen)/i;
+                });
+                var Ot = /\[\]$/,
+                    Pt = /\r?\n/g,
+                    Rt = /^(?:submit|button|image|reset|file)$/i,
+                    Mt = /^(?:input|select|textarea|keygen)/i;
 
-                function Lt(e, t, n, r) {
+                function It(e, t, n, r) {
                     var i;
                     if (Array.isArray(t)) S.each(t, (function(t, i) {
-                        n || jt.test(e) ? r(e, i) : Lt(e + "[" + ("object" == typeof i && null != i ? t : "") + "]", i, n, r)
+                        n || Ot.test(e) ? r(e, i) : It(e + "[" + ("object" == typeof i && null != i ? t : "") + "]", i, n, r)
                     }));
                     else if (n || "object" !== T(t)) r(e, t);
                     else
-                        for (i in t) Lt(e + "[" + i + "]", t[i], n, r)
+                        for (i in t) It(e + "[" + i + "]", t[i], n, r)
                 }
                 S.param = function(e, t) {
                     var n, r = [],
                         i = function(e, t) {
                             var n = y(t) ? t() : t;
                             r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
                         };
                     if (null == e) return "";
                     if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, (function() {
                         i(this.name, this.value)
                     }));
                     else
-                        for (n in e) Lt(n, e[n], t, i);
+                        for (n in e) It(n, e[n], t, i);
                     return r.join("&")
                 }, S.fn.extend({
                     serialize: function() {
                         return S.param(this.serializeArray())
                     },
                     serializeArray: function() {
                         return this.map((function() {
                             var e = S.prop(this, "elements");
                             return e ? S.makeArray(e) : this
                         })).filter((function() {
                             var e = this.type;
-                            return this.name && !S(this).is(":disabled") && qt.test(this.nodeName) && !Dt.test(e) && (this.checked || !ve.test(e))
+                            return this.name && !S(this).is(":disabled") && Mt.test(this.nodeName) && !Rt.test(e) && (this.checked || !Se.test(e))
                         })).map((function(e, t) {
                             var n = S(this).val();
                             return null == n ? null : Array.isArray(n) ? S.map(n, (function(e) {
                                 return {
                                     name: t.name,
-                                    value: e.replace(Nt, "\r\n")
+                                    value: e.replace(Pt, "\r\n")
                                 }
                             })) : {
                                 name: t.name,
-                                value: n.replace(Nt, "\r\n")
+                                value: n.replace(Pt, "\r\n")
                             }
                         })).get()
                     }
                 });
-                var Ht = /%20/g,
-                    Ot = /#.*$/,
-                    Pt = /([?&])_=[^&]*/,
-                    Rt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-                    Mt = /^(?:GET|HEAD)$/,
-                    It = /^\/\//,
-                    Wt = {},
-                    Ft = {},
-                    $t = "*/".concat("*"),
-                    Bt = x.createElement("a");
+                var Wt = /%20/g,
+                    Ft = /#.*$/,
+                    $t = /([?&])_=[^&]*/,
+                    _t = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+                    Bt = /^(?:GET|HEAD)$/,
+                    Xt = /^\/\//,
+                    Ut = {},
+                    zt = {},
+                    Vt = "*/".concat("*"),
+                    Gt = x.createElement("a");
 
-                function _t(e) {
+                function Yt(e) {
                     return function(t, n) {
                         "string" != typeof t && (n = t, t = "*");
                         var r, i = 0,
-                            o = t.toLowerCase().match(I) || [];
+                            o = t.toLowerCase().match(V) || [];
                         if (y(n))
                             for (; r = o[i++];) "+" === r[0] ? (r = r.slice(1) || "*", (e[r] = e[r] || []).unshift(n)) : (e[r] = e[r] || []).push(n)
                     }
                 }
 
-                function zt(e, t, n, r) {
+                function Qt(e, t, n, r) {
                     var i = {},
-                        o = e === Ft;
+                        o = e === zt;
 
                     function a(s) {
                         var u;
                         return i[s] = !0, S.each(e[s] || [], (function(e, s) {
                             var l = s(t, n, r);
                             return "string" != typeof l || o || i[l] ? o ? !(u = l) : void 0 : (t.dataTypes.unshift(l), a(l), !1)
                         })), u
                     }
                     return a(t.dataTypes[0]) || !i["*"] && a("*")
                 }
 
-                function Ut(e, t) {
+                function Jt(e, t) {
                     var n, r, i = S.ajaxSettings.flatOptions || {};
                     for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
                     return r && S.extend(!0, e, r), e
                 }
-                Bt.href = Et.href, S.extend({
+                Gt.href = Dt.href, S.extend({
                     active: 0,
                     lastModified: {},
                     etag: {},
                     ajaxSettings: {
-                        url: Et.href,
+                        url: Dt.href,
                         type: "GET",
-                        isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Et.protocol),
+                        isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Dt.protocol),
                         global: !0,
                         processData: !0,
                         async: !0,
                         contentType: "application/x-www-form-urlencoded; charset=UTF-8",
                         accepts: {
-                            "*": $t,
+                            "*": Vt,
                             text: "text/plain",
                             html: "text/html",
                             xml: "application/xml, text/xml",
                             json: "application/json, text/javascript"
                         },
                         contents: {
                             xml: /\bxml\b/,
@@ -2776,18 +2725,18 @@
                         },
                         flatOptions: {
                             url: !0,
                             context: !0
                         }
                     },
                     ajaxSetup: function(e, t) {
-                        return t ? Ut(Ut(e, S.ajaxSettings), t) : Ut(S.ajaxSettings, e)
+                        return t ? Jt(Jt(e, S.ajaxSettings), t) : Jt(S.ajaxSettings, e)
                     },
-                    ajaxPrefilter: _t(Wt),
-                    ajaxTransport: _t(Ft),
+                    ajaxPrefilter: Yt(Ut),
+                    ajaxTransport: Yt(zt),
                     ajax: function(e, t) {
                         "object" == typeof e && (t = e, e = void 0), t = t || {};
                         var n, i, o, a, s, u, l, c, f, p, d = S.ajaxSetup({}, t),
                             h = d.context || d,
                             g = d.context && (h.nodeType || h.jquery) ? S(h) : S.event,
                             v = S.Deferred(),
                             y = S.Callbacks("once memory"),
@@ -2797,15 +2746,15 @@
                             T = "canceled",
                             C = {
                                 readyState: 0,
                                 getResponseHeader: function(e) {
                                     var t;
                                     if (l) {
                                         if (!a)
-                                            for (a = {}; t = Rt.exec(o);) a[t[1].toLowerCase() + " "] = (a[t[1].toLowerCase() + " "] || []).concat(t[2]);
+                                            for (a = {}; t = _t.exec(o);) a[t[1].toLowerCase() + " "] = (a[t[1].toLowerCase() + " "] || []).concat(t[2]);
                                         t = a[e.toLowerCase() + " "]
                                     }
                                     return null == t ? null : t.join(", ")
                                 },
                                 getAllResponseHeaders: function() {
                                     return l ? o : null
                                 },
@@ -2821,42 +2770,42 @@
                                         if (l) C.always(e[C.status]);
                                         else
                                             for (t in e) m[t] = [m[t], e[t]];
                                     return this
                                 },
                                 abort: function(e) {
                                     var t = e || T;
-                                    return n && n.abort(t), E(0, t), this
+                                    return n && n.abort(t), k(0, t), this
                                 }
                             };
-                        if (v.promise(C), d.url = ((e || d.url || Et.href) + "").replace(It, Et.protocol + "//"), d.type = t.method || t.type || d.method || d.type, d.dataTypes = (d.dataType || "*").toLowerCase().match(I) || [""], null == d.crossDomain) {
+                        if (v.promise(C), d.url = ((e || d.url || Dt.href) + "").replace(Xt, Dt.protocol + "//"), d.type = t.method || t.type || d.method || d.type, d.dataTypes = (d.dataType || "*").toLowerCase().match(V) || [""], null == d.crossDomain) {
                             u = x.createElement("a");
                             try {
-                                u.href = d.url, u.href = u.href, d.crossDomain = Bt.protocol + "//" + Bt.host != u.protocol + "//" + u.host
+                                u.href = d.url, u.href = u.href, d.crossDomain = Gt.protocol + "//" + Gt.host != u.protocol + "//" + u.host
                             } catch (e) {
                                 d.crossDomain = !0
                             }
                         }
-                        if (d.data && d.processData && "string" != typeof d.data && (d.data = S.param(d.data, d.traditional)), zt(Wt, d, t, C), l) return C;
-                        for (f in (c = S.event && d.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), d.type = d.type.toUpperCase(), d.hasContent = !Mt.test(d.type), i = d.url.replace(Ot, ""), d.hasContent ? d.data && d.processData && 0 === (d.contentType || "").indexOf("application/x-www-form-urlencoded") && (d.data = d.data.replace(Ht, "+")) : (p = d.url.slice(i.length), d.data && (d.processData || "string" == typeof d.data) && (i += (At.test(i) ? "&" : "?") + d.data, delete d.data), !1 === d.cache && (i = i.replace(Pt, "$1"), p = (At.test(i) ? "&" : "?") + "_=" + kt.guid++ + p), d.url = i + p), d.ifModified && (S.lastModified[i] && C.setRequestHeader("If-Modified-Since", S.lastModified[i]), S.etag[i] && C.setRequestHeader("If-None-Match", S.etag[i])), (d.data && d.hasContent && !1 !== d.contentType || t.contentType) && C.setRequestHeader("Content-Type", d.contentType), C.setRequestHeader("Accept", d.dataTypes[0] && d.accepts[d.dataTypes[0]] ? d.accepts[d.dataTypes[0]] + ("*" !== d.dataTypes[0] ? ", " + $t + "; q=0.01" : "") : d.accepts["*"]), d.headers) C.setRequestHeader(f, d.headers[f]);
+                        if (d.data && d.processData && "string" != typeof d.data && (d.data = S.param(d.data, d.traditional)), Qt(Ut, d, t, C), l) return C;
+                        for (f in (c = S.event && d.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), d.type = d.type.toUpperCase(), d.hasContent = !Bt.test(d.type), i = d.url.replace(Ft, ""), d.hasContent ? d.data && d.processData && 0 === (d.contentType || "").indexOf("application/x-www-form-urlencoded") && (d.data = d.data.replace(Wt, "+")) : (p = d.url.slice(i.length), d.data && (d.processData || "string" == typeof d.data) && (i += (qt.test(i) ? "&" : "?") + d.data, delete d.data), !1 === d.cache && (i = i.replace($t, "$1"), p = (qt.test(i) ? "&" : "?") + "_=" + Nt.guid++ + p), d.url = i + p), d.ifModified && (S.lastModified[i] && C.setRequestHeader("If-Modified-Since", S.lastModified[i]), S.etag[i] && C.setRequestHeader("If-None-Match", S.etag[i])), (d.data && d.hasContent && !1 !== d.contentType || t.contentType) && C.setRequestHeader("Content-Type", d.contentType), C.setRequestHeader("Accept", d.dataTypes[0] && d.accepts[d.dataTypes[0]] ? d.accepts[d.dataTypes[0]] + ("*" !== d.dataTypes[0] ? ", " + Vt + "; q=0.01" : "") : d.accepts["*"]), d.headers) C.setRequestHeader(f, d.headers[f]);
                         if (d.beforeSend && (!1 === d.beforeSend.call(h, C, d) || l)) return C.abort();
-                        if (T = "abort", y.add(d.complete), C.done(d.success), C.fail(d.error), n = zt(Ft, d, t, C)) {
+                        if (T = "abort", y.add(d.complete), C.done(d.success), C.fail(d.error), n = Qt(zt, d, t, C)) {
                             if (C.readyState = 1, c && g.trigger("ajaxSend", [C, d]), l) return C;
                             d.async && d.timeout > 0 && (s = r.setTimeout((function() {
                                 C.abort("timeout")
                             }), d.timeout));
                             try {
-                                l = !1, n.send(b, E)
+                                l = !1, n.send(b, k)
                             } catch (e) {
                                 if (l) throw e;
-                                E(-1, e)
+                                k(-1, e)
                             }
-                        } else E(-1, "No Transport");
+                        } else k(-1, "No Transport");
 
-                        function E(e, t, a, u) {
+                        function k(e, t, a, u) {
                             var f, p, x, b, w, T = t;
                             l || (l = !0, s && r.clearTimeout(s), n = void 0, o = u || "", C.readyState = e > 0 ? 4 : 0, f = e >= 200 && e < 300 || 304 === e, a && (b = function(e, t, n) {
                                 for (var r, i, o, a, s = e.contents, u = e.dataTypes;
                                     "*" === u[0];) u.shift(), void 0 === r && (r = e.mimeType || t.getResponseHeader("Content-Type"));
                                 if (r)
                                     for (i in s)
                                         if (s[i] && s[i].test(r)) {
@@ -2974,30 +2923,30 @@
                 }, S.expr.pseudos.visible = function(e) {
                     return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
                 }, S.ajaxSettings.xhr = function() {
                     try {
                         return new r.XMLHttpRequest
                     } catch (e) {}
                 };
-                var Xt = {
+                var Kt = {
                         0: 200,
                         1223: 204
                     },
-                    Vt = S.ajaxSettings.xhr();
-                v.cors = !!Vt && "withCredentials" in Vt, v.ajax = Vt = !!Vt, S.ajaxTransport((function(e) {
+                    Zt = S.ajaxSettings.xhr();
+                v.cors = !!Zt && "withCredentials" in Zt, v.ajax = Zt = !!Zt, S.ajaxTransport((function(e) {
                     var t, n;
-                    if (v.cors || Vt && !e.crossDomain) return {
+                    if (v.cors || Zt && !e.crossDomain) return {
                         send: function(i, o) {
                             var a, s = e.xhr();
                             if (s.open(e.type, e.url, e.async, e.username, e.password), e.xhrFields)
                                 for (a in e.xhrFields) s[a] = e.xhrFields[a];
                             for (a in e.mimeType && s.overrideMimeType && s.overrideMimeType(e.mimeType), e.crossDomain || i["X-Requested-With"] || (i["X-Requested-With"] = "XMLHttpRequest"), i) s.setRequestHeader(a, i[a]);
                             t = function(e) {
                                 return function() {
-                                    t && (t = n = s.onload = s.onerror = s.onabort = s.ontimeout = s.onreadystatechange = null, "abort" === e ? s.abort() : "error" === e ? "number" != typeof s.status ? o(0, "error") : o(s.status, s.statusText) : o(Xt[s.status] || s.status, s.statusText, "text" !== (s.responseType || "text") || "string" != typeof s.responseText ? {
+                                    t && (t = n = s.onload = s.onerror = s.onabort = s.ontimeout = s.onreadystatechange = null, "abort" === e ? s.abort() : "error" === e ? "number" != typeof s.status ? o(0, "error") : o(s.status, s.statusText) : o(Kt[s.status] || s.status, s.statusText, "text" !== (s.responseType || "text") || "string" != typeof s.responseText ? {
                                         binary: s.response
                                     } : {
                                         text: s.responseText
                                     }, s.getAllResponseHeaders()))
                                 }
                             }, s.onload = t(), n = s.onerror = s.ontimeout = t("error"), void 0 !== s.onabort ? s.onabort = n : s.onreadystatechange = function() {
                                 4 === s.readyState && r.setTimeout((function() {
@@ -3042,38 +2991,38 @@
                             }), x.head.appendChild(t[0])
                         },
                         abort: function() {
                             n && n()
                         }
                     }
                 }));
-                var Gt, Yt = [],
-                    Qt = /(=)\?(?=&|$)|\?\?/;
+                var en, tn = [],
+                    nn = /(=)\?(?=&|$)|\?\?/;
                 S.ajaxSetup({
                     jsonp: "callback",
                     jsonpCallback: function() {
-                        var e = Yt.pop() || S.expando + "_" + kt.guid++;
+                        var e = tn.pop() || S.expando + "_" + Nt.guid++;
                         return this[e] = !0, e
                     }
                 }), S.ajaxPrefilter("json jsonp", (function(e, t, n) {
-                    var i, o, a, s = !1 !== e.jsonp && (Qt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Qt.test(e.data) && "data");
-                    if (s || "jsonp" === e.dataTypes[0]) return i = e.jsonpCallback = y(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, s ? e[s] = e[s].replace(Qt, "$1" + i) : !1 !== e.jsonp && (e.url += (At.test(e.url) ? "&" : "?") + e.jsonp + "=" + i), e.converters["script json"] = function() {
+                    var i, o, a, s = !1 !== e.jsonp && (nn.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && nn.test(e.data) && "data");
+                    if (s || "jsonp" === e.dataTypes[0]) return i = e.jsonpCallback = y(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, s ? e[s] = e[s].replace(nn, "$1" + i) : !1 !== e.jsonp && (e.url += (qt.test(e.url) ? "&" : "?") + e.jsonp + "=" + i), e.converters["script json"] = function() {
                         return a || S.error(i + " was not called"), a[0]
                     }, e.dataTypes[0] = "json", o = r[i], r[i] = function() {
                         a = arguments
                     }, n.always((function() {
-                        void 0 === o ? S(r).removeProp(i) : r[i] = o, e[i] && (e.jsonpCallback = t.jsonpCallback, Yt.push(i)), a && y(o) && o(a[0]), a = o = void 0
+                        void 0 === o ? S(r).removeProp(i) : r[i] = o, e[i] && (e.jsonpCallback = t.jsonpCallback, tn.push(i)), a && y(o) && o(a[0]), a = o = void 0
                     })), "script"
-                })), v.createHTMLDocument = ((Gt = x.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Gt.childNodes.length), S.parseHTML = function(e, t, n) {
-                    return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (v.createHTMLDocument ? ((r = (t = x.implementation.createHTMLDocument("")).createElement("base")).href = x.location.href, t.head.appendChild(r)) : t = x), o = !n && [], (i = q.exec(e)) ? [t.createElement(i[1])] : (i = Ce([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
+                })), v.createHTMLDocument = ((en = x.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === en.childNodes.length), S.parseHTML = function(e, t, n) {
+                    return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (v.createHTMLDocument ? ((r = (t = x.implementation.createHTMLDocument("")).createElement("base")).href = x.location.href, t.head.appendChild(r)) : t = x), o = !n && [], (i = F.exec(e)) ? [t.createElement(i[1])] : (i = Le([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
                     var r, i, o
                 }, S.fn.load = function(e, t, n) {
                     var r, i, o, a = this,
                         s = e.indexOf(" ");
-                    return s > -1 && (r = xt(e.slice(s)), e = e.slice(0, s)), y(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), a.length > 0 && S.ajax({
+                    return s > -1 && (r = St(e.slice(s)), e = e.slice(0, s)), y(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), a.length > 0 && S.ajax({
                         url: e,
                         type: i || "GET",
                         dataType: "html",
                         data: t
                     }).done((function(e) {
                         o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
                     })).always(n && function(e, t) {
@@ -3123,46 +3072,46 @@
                                 left: t.left - i.left - S.css(r, "marginLeft", !0)
                             }
                         }
                     },
                     offsetParent: function() {
                         return this.map((function() {
                             for (var e = this.offsetParent; e && "static" === S.css(e, "position");) e = e.offsetParent;
-                            return e || ae
+                            return e || ge
                         }))
                     }
                 }), S.each({
                     scrollLeft: "pageXOffset",
                     scrollTop: "pageYOffset"
                 }, (function(e, t) {
                     var n = "pageYOffset" === t;
                     S.fn[e] = function(r) {
-                        return U(this, (function(e, r, i) {
+                        return ee(this, (function(e, r, i) {
                             var o;
                             if (m(e) ? o = e : 9 === e.nodeType && (o = e.defaultView), void 0 === i) return o ? o[t] : e[r];
                             o ? o.scrollTo(n ? o.pageXOffset : i, n ? i : o.pageYOffset) : e[r] = i
                         }), e, r, arguments.length)
                     }
                 })), S.each(["top", "left"], (function(e, t) {
-                    S.cssHooks[t] = Ge(v.pixelPosition, (function(e, n) {
-                        if (n) return n = Ve(e, t), Fe.test(n) ? S(e).position()[t] + "px" : n
+                    S.cssHooks[t] = et(v.pixelPosition, (function(e, n) {
+                        if (n) return n = Ze(e, t), Ge.test(n) ? S(e).position()[t] + "px" : n
                     }))
                 })), S.each({
                     Height: "height",
                     Width: "width"
                 }, (function(e, t) {
                     S.each({
                         padding: "inner" + e,
                         content: t,
                         "": "outer" + e
                     }, (function(n, r) {
                         S.fn[r] = function(i, o) {
                             var a = arguments.length && (n || "boolean" != typeof i),
                                 s = n || (!0 === i || !0 === o ? "margin" : "border");
-                            return U(this, (function(t, n, i) {
+                            return ee(this, (function(t, n, i) {
                                 var o;
                                 return m(t) ? 0 === r.indexOf("outer") ? t["inner" + e] : t.document.documentElement["client" + e] : 9 === t.nodeType ? (o = t.documentElement, Math.max(t.body["scroll" + e], o["scroll" + e], t.body["offset" + e], o["offset" + e], o["client" + e])) : void 0 === i ? S.css(t, n, s) : S.style(t, n, i, s)
                             }), t, a ? i : void 0, a)
                         }
                     }))
                 })), S.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], (function(e, t) {
                     S.fn[t] = function(e) {
@@ -3185,32 +3134,32 @@
                         return this.mouseenter(e).mouseleave(t || e)
                     }
                 }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), (function(e, t) {
                     S.fn[t] = function(e, n) {
                         return arguments.length > 0 ? this.on(t, null, e, n) : this.trigger(t)
                     }
                 }));
-                var Jt = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+                var rn = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
                 S.proxy = function(e, t) {
                     var n, r, i;
                     if ("string" == typeof t && (n = e[t], t = e, e = n), y(e)) return r = s.call(arguments, 2), i = function() {
                         return e.apply(t || this, r.concat(s.call(arguments)))
                     }, i.guid = e.guid = e.guid || S.guid++, i
                 }, S.holdReady = function(e) {
                     e ? S.readyWait++ : S.ready(!0)
-                }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = D, S.isFunction = y, S.isWindow = m, S.camelCase = Y, S.type = T, S.now = Date.now, S.isNumeric = function(e) {
+                }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = j, S.isFunction = y, S.isWindow = m, S.camelCase = ie, S.type = T, S.now = Date.now, S.isNumeric = function(e) {
                     var t = S.type(e);
                     return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
                 }, S.trim = function(e) {
-                    return null == e ? "" : (e + "").replace(Jt, "$1")
+                    return null == e ? "" : (e + "").replace(rn, "$1")
                 }, void 0 === (n = function() {
                     return S
                 }.apply(t, [])) || (e.exports = n);
-                var Kt = r.jQuery,
-                    Zt = r.$;
+                var on = r.jQuery,
+                    an = r.$;
                 return S.noConflict = function(e) {
-                    return r.$ === S && (r.$ = Zt), e && r.jQuery === S && (r.jQuery = Kt), S
+                    return r.$ === S && (r.$ = an), e && r.jQuery === S && (r.jQuery = on), S
                 }, void 0 === i && (r.jQuery = r.$ = S), S
             }))
         }
     }
 ]);
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/345.03be96cd091aac4797a5.js` & `jupyterlab_widgets-3.0.8/labextension/static/345.17494fea1ff555b26294.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -186,86 +186,82 @@
 
             function w() {
                 return this.rgb().formatRgb()
             }
 
             function x(t) {
                 var e, r;
-                return t = (t + "").trim().toLowerCase(), (e = h.exec(t)) ? (r = e[1].length, e = parseInt(e[1], 16), 6 === r ? S(e) : 3 === r ? new k(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === r ? E(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === r ? E(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = p.exec(t)) ? new k(e[1], e[2], e[3], 1) : (e = f.exec(t)) ? new k(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = d.exec(t)) ? E(e[1], e[2], e[3], e[4]) : (e = m.exec(t)) ? E(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = g.exec(t)) ? $(e[1], e[2] / 100, e[3] / 100, 1) : (e = v.exec(t)) ? $(e[1], e[2] / 100, e[3] / 100, e[4]) : b.hasOwnProperty(t) ? S(b[t]) : "transparent" === t ? new k(NaN, NaN, NaN, 0) : null
+                return t = (t + "").trim().toLowerCase(), (e = h.exec(t)) ? (r = e[1].length, e = parseInt(e[1], 16), 6 === r ? S(e) : 3 === r ? new N(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === r ? E(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === r ? E(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = p.exec(t)) ? new N(e[1], e[2], e[3], 1) : (e = f.exec(t)) ? new N(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = d.exec(t)) ? E(e[1], e[2], e[3], e[4]) : (e = m.exec(t)) ? E(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = g.exec(t)) ? A(e[1], e[2] / 100, e[3] / 100, 1) : (e = v.exec(t)) ? A(e[1], e[2] / 100, e[3] / 100, e[4]) : b.hasOwnProperty(t) ? S(b[t]) : "transparent" === t ? new N(NaN, NaN, NaN, 0) : null
             }
 
             function S(t) {
-                return new k(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
+                return new N(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
             }
 
             function E(t, e, r, n) {
-                return n <= 0 && (t = e = r = NaN), new k(t, e, r, n)
+                return n <= 0 && (t = e = r = NaN), new N(t, e, r, n)
             }
 
-            function N(t) {
-                return t instanceof o || (t = x(t)), t ? new k((t = t.rgb()).r, t.g, t.b, t.opacity) : new k
-            }
-
-            function k(t, e, r, n) {
+            function N(t, e, r, n) {
                 this.r = +t, this.g = +e, this.b = +r, this.opacity = +n
             }
 
-            function P() {
-                return `#${A(this.r)}${A(this.g)}${A(this.b)}`
+            function k() {
+                return `#${V(this.r)}${V(this.g)}${V(this.b)}`
             }
 
-            function M() {
-                const t = C(this.opacity);
-                return `${1===t?"rgb(":"rgba("}${V(this.r)}, ${V(this.g)}, ${V(this.b)}${1===t?")":`, ${t})`}`
+            function P() {
+                const t = M(this.opacity);
+                return `${1===t?"rgb(":"rgba("}${C(this.r)}, ${C(this.g)}, ${C(this.b)}${1===t?")":`, ${t})`}`
             }
 
-            function C(t) {
+            function M(t) {
                 return isNaN(t) ? 1 : Math.max(0, Math.min(1, t))
             }
 
-            function V(t) {
+            function C(t) {
                 return Math.max(0, Math.min(255, Math.round(t) || 0))
             }
 
-            function A(t) {
-                return ((t = V(t)) < 16 ? "0" : "") + t.toString(16)
+            function V(t) {
+                return ((t = C(t)) < 16 ? "0" : "") + t.toString(16)
             }
 
-            function $(t, e, r, n) {
-                return n <= 0 ? t = e = r = NaN : r <= 0 || r >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new D(t, e, r, n)
+            function A(t, e, r, n) {
+                return n <= 0 ? t = e = r = NaN : r <= 0 || r >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new U(t, e, r, n)
             }
 
-            function U(t) {
-                if (t instanceof D) return new D(t.h, t.s, t.l, t.opacity);
-                if (t instanceof o || (t = x(t)), !t) return new D;
-                if (t instanceof D) return t;
+            function $(t) {
+                if (t instanceof U) return new U(t.h, t.s, t.l, t.opacity);
+                if (t instanceof o || (t = x(t)), !t) return new U;
+                if (t instanceof U) return t;
                 var e = (t = t.rgb()).r / 255,
                     r = t.g / 255,
                     n = t.b / 255,
                     i = Math.min(e, r, n),
                     a = Math.max(e, r, n),
                     s = NaN,
                     l = a - i,
                     u = (a + i) / 2;
-                return l ? (s = e === a ? (r - n) / l + 6 * (r < n) : r === a ? (n - e) / l + 2 : (e - r) / l + 4, l /= u < .5 ? a + i : 2 - a - i, s *= 60) : l = u > 0 && u < 1 ? 0 : s, new D(s, l, u, t.opacity)
+                return l ? (s = e === a ? (r - n) / l + 6 * (r < n) : r === a ? (n - e) / l + 2 : (e - r) / l + 4, l /= u < .5 ? a + i : 2 - a - i, s *= 60) : l = u > 0 && u < 1 ? 0 : s, new U(s, l, u, t.opacity)
             }
 
-            function D(t, e, r, n) {
+            function U(t, e, r, n) {
                 this.h = +t, this.s = +e, this.l = +r, this.opacity = +n
             }
 
-            function O(t) {
+            function D(t) {
                 return (t = (t || 0) % 360) < 0 ? t + 360 : t
             }
 
-            function L(t) {
+            function O(t) {
                 return Math.max(0, Math.min(1, t || 0))
             }
 
-            function j(t, e, r) {
+            function L(t, e, r) {
                 return 255 * (t < 60 ? e + (r - e) * t / 60 : t < 180 ? r : t < 240 ? e + (r - e) * (240 - t) / 60 : e)
             }
             n(o, x, {
                 copy(t) {
                     return Object.assign(new this.constructor, this, t)
                 },
                 displayable() {
@@ -273,69 +269,70 @@
                 },
                 hex: y,
                 formatHex: y,
                 formatHex8: function() {
                     return this.rgb().formatHex8()
                 },
                 formatHsl: function() {
-                    return U(this).formatHsl()
+                    return $(this).formatHsl()
                 },
                 formatRgb: w,
                 toString: w
-            }), n(k, (function(t, e, r, n) {
-                return 1 === arguments.length ? N(t) : new k(t, e, r, null == n ? 1 : n)
+            }), n(N, (function(t, e, r, n) {
+                return 1 === arguments.length ? ((i = t) instanceof o || (i = x(i)), i ? new N((i = i.rgb()).r, i.g, i.b, i.opacity) : new N) : new N(t, e, r, null == n ? 1 : n);
+                var i
             }), i(o, {
                 brighter(t) {
-                    return t = null == t ? s : Math.pow(s, t), new k(this.r * t, this.g * t, this.b * t, this.opacity)
+                    return t = null == t ? s : Math.pow(s, t), new N(this.r * t, this.g * t, this.b * t, this.opacity)
                 },
                 darker(t) {
-                    return t = null == t ? a : Math.pow(a, t), new k(this.r * t, this.g * t, this.b * t, this.opacity)
+                    return t = null == t ? a : Math.pow(a, t), new N(this.r * t, this.g * t, this.b * t, this.opacity)
                 },
                 rgb() {
                     return this
                 },
                 clamp() {
-                    return new k(V(this.r), V(this.g), V(this.b), C(this.opacity))
+                    return new N(C(this.r), C(this.g), C(this.b), M(this.opacity))
                 },
                 displayable() {
                     return -.5 <= this.r && this.r < 255.5 && -.5 <= this.g && this.g < 255.5 && -.5 <= this.b && this.b < 255.5 && 0 <= this.opacity && this.opacity <= 1
                 },
-                hex: P,
-                formatHex: P,
+                hex: k,
+                formatHex: k,
                 formatHex8: function() {
-                    return `#${A(this.r)}${A(this.g)}${A(this.b)}${A(255*(isNaN(this.opacity)?1:this.opacity))}`
+                    return `#${V(this.r)}${V(this.g)}${V(this.b)}${V(255*(isNaN(this.opacity)?1:this.opacity))}`
                 },
-                formatRgb: M,
-                toString: M
-            })), n(D, (function(t, e, r, n) {
-                return 1 === arguments.length ? U(t) : new D(t, e, r, null == n ? 1 : n)
+                formatRgb: P,
+                toString: P
+            })), n(U, (function(t, e, r, n) {
+                return 1 === arguments.length ? $(t) : new U(t, e, r, null == n ? 1 : n)
             }), i(o, {
                 brighter(t) {
-                    return t = null == t ? s : Math.pow(s, t), new D(this.h, this.s, this.l * t, this.opacity)
+                    return t = null == t ? s : Math.pow(s, t), new U(this.h, this.s, this.l * t, this.opacity)
                 },
                 darker(t) {
-                    return t = null == t ? a : Math.pow(a, t), new D(this.h, this.s, this.l * t, this.opacity)
+                    return t = null == t ? a : Math.pow(a, t), new U(this.h, this.s, this.l * t, this.opacity)
                 },
                 rgb() {
                     var t = this.h % 360 + 360 * (this.h < 0),
                         e = isNaN(t) || isNaN(this.s) ? 0 : this.s,
                         r = this.l,
                         n = r + (r < .5 ? r : 1 - r) * e,
                         i = 2 * r - n;
-                    return new k(j(t >= 240 ? t - 240 : t + 120, i, n), j(t, i, n), j(t < 120 ? t + 240 : t - 120, i, n), this.opacity)
+                    return new N(L(t >= 240 ? t - 240 : t + 120, i, n), L(t, i, n), L(t < 120 ? t + 240 : t - 120, i, n), this.opacity)
                 },
                 clamp() {
-                    return new D(O(this.h), L(this.s), L(this.l), C(this.opacity))
+                    return new U(D(this.h), O(this.s), O(this.l), M(this.opacity))
                 },
                 displayable() {
                     return (0 <= this.s && this.s <= 1 || isNaN(this.s)) && 0 <= this.l && this.l <= 1 && 0 <= this.opacity && this.opacity <= 1
                 },
                 formatHsl() {
-                    const t = C(this.opacity);
-                    return `${1===t?"hsl(":"hsla("}${O(this.h)}, ${100*L(this.s)}%, ${100*L(this.l)}%${1===t?")":`, ${t})`}`
+                    const t = M(this.opacity);
+                    return `${1===t?"hsl(":"hsla("}${D(this.h)}, ${100*O(this.s)}%, ${100*O(this.l)}%${1===t?")":`, ${t})`}`
                 }
             }))
         },
         4359: (t, e, r) => {
             "use strict";
 
             function n(t, e) {
@@ -743,306 +740,308 @@
                         value: "value",
                         valueHorizontal: "value-horizontal",
                         valueVertical: "value-vertical",
                         valueNormal: "value-normal",
                         valueLarge: "value-large",
                         valueSub: "value-sub"
                     },
-                    E = ".__tooltips",
-                    N = ".__aria";
+                    E = {
+                        tooltips: ".__tooltips",
+                        aria: ".__aria"
+                    };
 
-                function k(t, e) {
+                function N(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'step' is not numeric.");
                     t.singleStep = e
                 }
 
-                function P(t, e) {
+                function k(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'keyboardPageMultiplier' is not numeric.");
                     t.keyboardPageMultiplier = e
                 }
 
-                function M(t, e) {
+                function P(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'keyboardMultiplier' is not numeric.");
                     t.keyboardMultiplier = e
                 }
 
-                function C(t, e) {
+                function M(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'keyboardDefaultStep' is not numeric.");
                     t.keyboardDefaultStep = e
                 }
 
-                function V(t, e) {
+                function C(t, e) {
                     if ("object" != typeof e || Array.isArray(e)) throw new Error("noUiSlider: 'range' is not an object.");
                     if (void 0 === e.min || void 0 === e.max) throw new Error("noUiSlider: Missing 'min' or 'max' in 'range'.");
                     t.spectrum = new w(e, t.snap || !1, t.singleStep)
                 }
 
-                function A(t, e) {
+                function V(t, e) {
                     if (e = l(e), !Array.isArray(e) || !e.length) throw new Error("noUiSlider: 'start' option is incorrect.");
                     t.handles = e.length, t.start = e
                 }
 
-                function $(t, e) {
+                function A(t, e) {
                     if ("boolean" != typeof e) throw new Error("noUiSlider: 'snap' option must be a boolean.");
                     t.snap = e
                 }
 
-                function U(t, e) {
+                function $(t, e) {
                     if ("boolean" != typeof e) throw new Error("noUiSlider: 'animate' option must be a boolean.");
                     t.animate = e
                 }
 
-                function D(t, e) {
+                function U(t, e) {
                     if ("number" != typeof e) throw new Error("noUiSlider: 'animationDuration' option must be a number.");
                     t.animationDuration = e
                 }
 
-                function O(t, e) {
+                function D(t, e) {
                     var r, n = [!1];
                     if ("lower" === e ? e = [!0, !1] : "upper" === e && (e = [!1, !0]), !0 === e || !1 === e) {
                         for (r = 1; r < t.handles; r++) n.push(e);
                         n.push(!1)
                     } else {
                         if (!Array.isArray(e) || !e.length || e.length !== t.handles + 1) throw new Error("noUiSlider: 'connect' option doesn't match handle count.");
                         n = e
                     }
                     t.connect = n
                 }
 
-                function L(t, e) {
+                function O(t, e) {
                     switch (e) {
                         case "horizontal":
                             t.ort = 0;
                             break;
                         case "vertical":
                             t.ort = 1;
                             break;
                         default:
                             throw new Error("noUiSlider: 'orientation' option is invalid.")
                     }
                 }
 
-                function j(t, e) {
+                function L(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'margin' option must be numeric.");
                     0 !== e && (t.margin = t.spectrum.getDistance(e))
                 }
 
-                function T(t, e) {
+                function j(t, e) {
                     if (!o(e)) throw new Error("noUiSlider: 'limit' option must be numeric.");
                     if (t.limit = t.spectrum.getDistance(e), !t.limit || t.handles < 2) throw new Error("noUiSlider: 'limit' option is only supported on linear sliders with 2 or more handles.")
                 }
 
-                function z(t, e) {
+                function T(t, e) {
                     var r;
                     if (!o(e) && !Array.isArray(e)) throw new Error("noUiSlider: 'padding' option must be numeric or array of exactly 2 numbers.");
                     if (Array.isArray(e) && 2 !== e.length && !o(e[0]) && !o(e[1])) throw new Error("noUiSlider: 'padding' option must be numeric or array of exactly 2 numbers.");
                     if (0 !== e) {
                         for (Array.isArray(e) || (e = [e, e]), t.padding = [t.spectrum.getDistance(e[0]), t.spectrum.getDistance(e[1])], r = 0; r < t.spectrum.xNumSteps.length - 1; r++)
                             if (t.padding[0][r] < 0 || t.padding[1][r] < 0) throw new Error("noUiSlider: 'padding' option must be a positive number(s).");
                         var n = e[0] + e[1],
                             i = t.spectrum.xVal[0];
                         if (n / (t.spectrum.xVal[t.spectrum.xVal.length - 1] - i) > 1) throw new Error("noUiSlider: 'padding' option must not exceed 100% of the range.")
                     }
                 }
 
-                function H(t, e) {
+                function z(t, e) {
                     switch (e) {
                         case "ltr":
                             t.dir = 0;
                             break;
                         case "rtl":
                             t.dir = 1;
                             break;
                         default:
                             throw new Error("noUiSlider: 'direction' option was not recognized.")
                     }
                 }
 
-                function R(t, e) {
+                function H(t, e) {
                     if ("string" != typeof e) throw new Error("noUiSlider: 'behaviour' must be a string containing options.");
                     var r = e.indexOf("tap") >= 0,
                         n = e.indexOf("drag") >= 0,
                         i = e.indexOf("fixed") >= 0,
                         o = e.indexOf("snap") >= 0,
                         a = e.indexOf("hover") >= 0,
                         s = e.indexOf("unconstrained") >= 0,
                         l = e.indexOf("drag-all") >= 0;
                     if (i) {
                         if (2 !== t.handles) throw new Error("noUiSlider: 'fixed' behaviour must be used with 2 handles");
-                        j(t, t.start[1] - t.start[0])
+                        L(t, t.start[1] - t.start[0])
                     }
                     if (s && (t.margin || t.limit)) throw new Error("noUiSlider: 'unconstrained' behaviour cannot be used with margin or limit");
                     t.events = {
                         tap: r || o,
                         drag: n,
                         dragAll: l,
                         fixed: i,
                         snap: o,
                         hover: a,
                         unconstrained: s
                     }
                 }
 
-                function F(t, r) {
+                function R(t, r) {
                     if (!1 !== r)
                         if (!0 === r || e(r)) {
                             t.tooltips = [];
                             for (var n = 0; n < t.handles; n++) t.tooltips.push(r)
                         } else {
                             if ((r = l(r)).length !== t.handles) throw new Error("noUiSlider: must pass a formatter for all handles.");
                             r.forEach((function(t) {
                                 if ("boolean" != typeof t && !e(t)) throw new Error("noUiSlider: 'tooltips' must be passed a formatter or 'false'.")
                             })), t.tooltips = r
                         }
                 }
 
-                function _(t, e) {
+                function F(t, e) {
                     if (e.length !== t.handles) throw new Error("noUiSlider: must pass a attributes for all handles.");
                     t.handleAttributes = e
                 }
 
-                function q(t, r) {
+                function _(t, r) {
                     if (!e(r)) throw new Error("noUiSlider: 'ariaFormat' requires 'to' method.");
                     t.ariaFormat = r
                 }
 
-                function X(t, r) {
+                function q(t, r) {
                     if (! function(t) {
                             return e(t) && "function" == typeof t.from
                         }(r)) throw new Error("noUiSlider: 'format' requires 'to' and 'from' methods.");
                     t.format = r
                 }
 
-                function B(t, e) {
+                function X(t, e) {
                     if ("boolean" != typeof e) throw new Error("noUiSlider: 'keyboardSupport' option must be a boolean.");
                     t.keyboardSupport = e
                 }
 
-                function Y(t, e) {
+                function B(t, e) {
                     t.documentElement = e
                 }
 
-                function I(t, e) {
+                function Y(t, e) {
                     if ("string" != typeof e && !1 !== e) throw new Error("noUiSlider: 'cssPrefix' must be a string or `false`.");
                     t.cssPrefix = e
                 }
 
-                function W(t, e) {
+                function I(t, e) {
                     if ("object" != typeof e) throw new Error("noUiSlider: 'cssClasses' must be an object.");
                     "string" == typeof t.cssPrefix ? (t.cssClasses = {}, Object.keys(e).forEach((function(r) {
                         t.cssClasses[r] = t.cssPrefix + e[r]
                     }))) : t.cssClasses = e
                 }
 
-                function Z(t) {
+                function W(t) {
                     var e = {
                             margin: null,
                             limit: null,
                             padding: null,
                             animate: !0,
                             animationDuration: 300,
                             ariaFormat: x,
                             format: x
                         },
                         r = {
                             step: {
                                 r: !1,
-                                t: k
+                                t: N
                             },
                             keyboardPageMultiplier: {
                                 r: !1,
-                                t: P
+                                t: k
                             },
                             keyboardMultiplier: {
                                 r: !1,
-                                t: M
+                                t: P
                             },
                             keyboardDefaultStep: {
                                 r: !1,
-                                t: C
+                                t: M
                             },
                             start: {
                                 r: !0,
-                                t: A
+                                t: V
                             },
                             connect: {
                                 r: !0,
-                                t: O
+                                t: D
                             },
                             direction: {
                                 r: !0,
-                                t: H
+                                t: z
                             },
                             snap: {
                                 r: !1,
-                                t: $
+                                t: A
                             },
                             animate: {
                                 r: !1,
-                                t: U
+                                t: $
                             },
                             animationDuration: {
                                 r: !1,
-                                t: D
+                                t: U
                             },
                             range: {
                                 r: !0,
-                                t: V
+                                t: C
                             },
                             orientation: {
                                 r: !1,
-                                t: L
+                                t: O
                             },
                             margin: {
                                 r: !1,
-                                t: j
+                                t: L
                             },
                             limit: {
                                 r: !1,
-                                t: T
+                                t: j
                             },
                             padding: {
                                 r: !1,
-                                t: z
+                                t: T
                             },
                             behaviour: {
                                 r: !0,
-                                t: R
+                                t: H
                             },
                             ariaFormat: {
                                 r: !1,
-                                t: q
+                                t: _
                             },
                             format: {
                                 r: !1,
-                                t: X
+                                t: q
                             },
                             tooltips: {
                                 r: !1,
-                                t: F
+                                t: R
                             },
                             keyboardSupport: {
                                 r: !0,
-                                t: B
+                                t: X
                             },
                             documentElement: {
                                 r: !1,
-                                t: Y
+                                t: B
                             },
                             cssPrefix: {
                                 r: !0,
-                                t: I
+                                t: Y
                             },
                             cssClasses: {
                                 r: !0,
-                                t: W
+                                t: I
                             },
                             handleAttributes: {
                                 r: !1,
-                                t: _
+                                t: F
                             }
                         },
                         i = {
                             connect: !1,
                             direction: "ltr",
                             behaviour: "tap",
                             orientation: "horizontal",
@@ -1063,15 +1062,15 @@
                     e.transformRule = s ? "transform" : a ? "msTransform" : "webkitTransform";
                     return e.style = [
                         ["left", "top"],
                         ["right", "bottom"]
                     ][e.dir][e.ort], e
                 }
 
-                function G(e, o, u) {
+                function Z(e, o, u) {
                     var f, d, m, g, v, b, y, w = window.navigator.pointerEnabled ? {
                             start: "pointerdown",
                             move: "pointermove",
                             end: "pointerup"
                         } : window.navigator.msPointerEnabled ? {
                             start: "MSPointerDown",
                             move: "MSPointerMove",
@@ -1090,36 +1089,36 @@
                                     }
                                 });
                                 window.addEventListener("test", null, e)
                             } catch (t) {}
                             return t
                         }(),
                         S = e,
-                        k = o.spectrum,
+                        N = o.spectrum,
+                        k = [],
                         P = [],
                         M = [],
-                        C = [],
-                        V = 0,
-                        A = {},
-                        $ = e.ownerDocument,
-                        U = o.documentElement || $.documentElement,
-                        D = $.body,
-                        O = "rtl" === $.dir || 1 === o.ort ? 0 : 100;
+                        C = 0,
+                        V = {},
+                        A = e.ownerDocument,
+                        $ = o.documentElement || A.documentElement,
+                        U = A.body,
+                        D = "rtl" === A.dir || 1 === o.ort ? 0 : 100;
 
-                    function L(t, e) {
-                        var r = $.createElement("div");
+                    function O(t, e) {
+                        var r = A.createElement("div");
                         return e && c(r, e), t.appendChild(r), r
                     }
 
-                    function j(t, e) {
-                        var r = L(t, o.cssClasses.origin),
-                            n = L(r, o.cssClasses.handle);
-                        if (L(n, o.cssClasses.touchArea), n.setAttribute("data-handle", String(e)), o.keyboardSupport && (n.setAttribute("tabindex", "0"), n.addEventListener("keydown", (function(t) {
+                    function L(t, e) {
+                        var r = O(t, o.cssClasses.origin),
+                            n = O(r, o.cssClasses.handle);
+                        if (O(n, o.cssClasses.touchArea), n.setAttribute("data-handle", String(e)), o.keyboardSupport && (n.setAttribute("tabindex", "0"), n.addEventListener("keydown", (function(t) {
                                 return function(t, e) {
-                                    if (H() || R(e)) return !1;
+                                    if (z() || H(e)) return !1;
                                     var r = ["Left", "Right"],
                                         n = ["Down", "Up"],
                                         i = ["PageDown", "PageUp"],
                                         a = ["Home", "End"];
                                     o.dir && !o.ort ? r.reverse() : o.ort && !o.dir && (n.reverse(), i.reverse());
                                     var s, l = t.key.replace("Arrow", ""),
                                         u = l === i[0],
@@ -1127,144 +1126,144 @@
                                         h = l === n[0] || l === r[0] || u,
                                         p = l === n[1] || l === r[1] || c,
                                         f = l === a[0],
                                         d = l === a[1];
                                     if (!(h || p || f || d)) return !0;
                                     if (t.preventDefault(), p || h) {
                                         var m = h ? 0 : 1,
-                                            g = vt(e)[m];
+                                            g = gt(e)[m];
                                         if (null === g) return !1;
-                                        !1 === g && (g = k.getDefaultStep(M[e], h, o.keyboardDefaultStep)), g *= c || u ? o.keyboardPageMultiplier : o.keyboardMultiplier, g = Math.max(g, 1e-7), g *= h ? -1 : 1, s = P[e] + g
+                                        !1 === g && (g = N.getDefaultStep(P[e], h, o.keyboardDefaultStep)), g *= c || u ? o.keyboardPageMultiplier : o.keyboardMultiplier, g = Math.max(g, 1e-7), g *= h ? -1 : 1, s = k[e] + g
                                     } else s = d ? o.spectrum.xVal[o.spectrum.xVal.length - 1] : o.spectrum.xVal[0];
-                                    return pt(e, k.toStepping(s), !0, !0), at("slide", e), at("update", e), at("change", e), at("set", e), !1
+                                    return ht(e, N.toStepping(s), !0, !0), ot("slide", e), ot("update", e), ot("change", e), ot("set", e), !1
                                 }(t, e)
                             }))), void 0 !== o.handleAttributes) {
                             var i = o.handleAttributes[e];
                             Object.keys(i).forEach((function(t) {
                                 n.setAttribute(t, i[t])
                             }))
                         }
                         return n.setAttribute("role", "slider"), n.setAttribute("aria-orientation", o.ort ? "vertical" : "horizontal"), 0 === e ? c(n, o.cssClasses.handleLower) : e === o.handles - 1 && c(n, o.cssClasses.handleUpper), r
                     }
 
-                    function T(t, e) {
-                        return !!e && L(t, o.cssClasses.connect)
+                    function j(t, e) {
+                        return !!e && O(t, o.cssClasses.connect)
                     }
 
-                    function z(t, e) {
-                        return !(!o.tooltips || !o.tooltips[e]) && L(t.firstChild, o.cssClasses.tooltip)
+                    function T(t, e) {
+                        return !(!o.tooltips || !o.tooltips[e]) && O(t.firstChild, o.cssClasses.tooltip)
                     }
 
-                    function H() {
+                    function z() {
                         return S.hasAttribute("disabled")
                     }
 
-                    function R(t) {
+                    function H(t) {
                         return d[t].hasAttribute("disabled")
                     }
 
-                    function F() {
-                        v && (ot("update" + E), v.forEach((function(t) {
+                    function R() {
+                        v && (it("update" + E.tooltips), v.forEach((function(t) {
                             t && r(t)
                         })), v = null)
                     }
 
-                    function _() {
-                        F(), v = d.map(z), it("update" + E, (function(t, e, r) {
+                    function F() {
+                        R(), v = d.map(T), nt("update" + E.tooltips, (function(t, e, r) {
                             if (v && o.tooltips && !1 !== v[e]) {
                                 var n = t[e];
                                 !0 !== o.tooltips[e] && (n = o.tooltips[e].to(r[e])), v[e].innerHTML = n
                             }
                         }))
                     }
 
-                    function q(t, e) {
+                    function _(t, e) {
                         return t.map((function(t) {
-                            return k.fromStepping(e ? k.getStep(t) : t)
+                            return N.fromStepping(e ? N.getStep(t) : t)
                         }))
                     }
 
-                    function X(e) {
+                    function q(e) {
                         var r, n = function(e) {
-                                if (e.mode === t.PipsMode.Range || e.mode === t.PipsMode.Steps) return k.xVal;
+                                if (e.mode === t.PipsMode.Range || e.mode === t.PipsMode.Steps) return N.xVal;
                                 if (e.mode === t.PipsMode.Count) {
                                     if (e.values < 2) throw new Error("noUiSlider: 'values' (>= 2) required for mode 'count'.");
                                     for (var r = e.values - 1, n = 100 / r, i = []; r--;) i[r] = r * n;
-                                    return i.push(100), q(i, e.stepped)
+                                    return i.push(100), _(i, e.stepped)
                                 }
-                                return e.mode === t.PipsMode.Positions ? q(e.values, e.stepped) : e.mode === t.PipsMode.Values ? e.stepped ? e.values.map((function(t) {
-                                    return k.fromStepping(k.getStep(k.toStepping(t)))
+                                return e.mode === t.PipsMode.Positions ? _(e.values, e.stepped) : e.mode === t.PipsMode.Values ? e.stepped ? e.values.map((function(t) {
+                                    return N.fromStepping(N.getStep(N.toStepping(t)))
                                 })) : e.values : []
                             }(e),
                             i = {},
-                            o = k.xVal[0],
-                            a = k.xVal[k.xVal.length - 1],
+                            o = N.xVal[0],
+                            a = N.xVal[N.xVal.length - 1],
                             s = !1,
                             l = !1,
                             u = 0;
                         return (r = n.slice().sort((function(t, e) {
                             return t - e
                         })), n = r.filter((function(t) {
                             return !this[t] && (this[t] = !0)
                         }), {}))[0] !== o && (n.unshift(o), s = !0), n[n.length - 1] !== a && (n.push(a), l = !0), n.forEach((function(r, o) {
                             var a, c, h, p, f, d, m, g, v, b, y = r,
                                 w = n[o + 1],
                                 x = e.mode === t.PipsMode.Steps;
-                            for (x && (a = k.xNumSteps[o]), a || (a = w - y), void 0 === w && (w = y), a = Math.max(a, 1e-7), c = y; c <= w; c = Number((c + a).toFixed(7))) {
-                                for (g = (f = (p = k.toStepping(c)) - u) / (e.density || 1), b = f / (v = Math.round(g)), h = 1; h <= v; h += 1) i[(d = u + h * b).toFixed(5)] = [k.fromStepping(d), 0];
+                            for (x && (a = N.xNumSteps[o]), a || (a = w - y), void 0 === w && (w = y), a = Math.max(a, 1e-7), c = y; c <= w; c = Number((c + a).toFixed(7))) {
+                                for (g = (f = (p = N.toStepping(c)) - u) / (e.density || 1), b = f / (v = Math.round(g)), h = 1; h <= v; h += 1) i[(d = u + h * b).toFixed(5)] = [N.fromStepping(d), 0];
                                 m = n.indexOf(c) > -1 ? t.PipsType.LargeValue : x ? t.PipsType.SmallValue : t.PipsType.NoValue, !o && s && c !== w && (m = 0), c === w && l || (i[p.toFixed(5)] = [c, m]), u = p
                             }
                         })), i
                     }
 
-                    function B(e, r, n) {
-                        var i, a, s = $.createElement("div"),
+                    function X(e, r, n) {
+                        var i, a, s = A.createElement("div"),
                             l = ((i = {})[t.PipsType.None] = "", i[t.PipsType.NoValue] = o.cssClasses.valueNormal, i[t.PipsType.LargeValue] = o.cssClasses.valueLarge, i[t.PipsType.SmallValue] = o.cssClasses.valueSub, i),
                             u = ((a = {})[t.PipsType.None] = "", a[t.PipsType.NoValue] = o.cssClasses.markerNormal, a[t.PipsType.LargeValue] = o.cssClasses.markerLarge, a[t.PipsType.SmallValue] = o.cssClasses.markerSub, a),
                             h = [o.cssClasses.valueHorizontal, o.cssClasses.valueVertical],
                             p = [o.cssClasses.markerHorizontal, o.cssClasses.markerVertical];
 
                         function f(t, e) {
                             var r = e === o.cssClasses.value,
                                 n = r ? l : u;
                             return e + " " + (r ? h : p)[o.ort] + " " + n[t]
                         }
                         return c(s, o.cssClasses.pips), c(s, 0 === o.ort ? o.cssClasses.pipsHorizontal : o.cssClasses.pipsVertical), Object.keys(e).forEach((function(i) {
                             ! function(e, i, a) {
                                 if ((a = r ? r(i, a) : a) !== t.PipsType.None) {
-                                    var l = L(s, !1);
-                                    l.className = f(a, o.cssClasses.marker), l.style[o.style] = e + "%", a > t.PipsType.NoValue && ((l = L(s, !1)).className = f(a, o.cssClasses.value), l.setAttribute("data-value", String(i)), l.style[o.style] = e + "%", l.innerHTML = String(n.to(i)))
+                                    var l = O(s, !1);
+                                    l.className = f(a, o.cssClasses.marker), l.style[o.style] = e + "%", a > t.PipsType.NoValue && ((l = O(s, !1)).className = f(a, o.cssClasses.value), l.setAttribute("data-value", String(i)), l.style[o.style] = e + "%", l.innerHTML = String(n.to(i)))
                                 }
                             }(i, e[i][0], e[i][1])
                         })), s
                     }
 
-                    function Y() {
+                    function B() {
                         g && (r(g), g = null)
                     }
 
-                    function I(t) {
-                        Y();
-                        var e = X(t),
+                    function Y(t) {
+                        B();
+                        var e = q(t),
                             r = t.filter,
                             n = t.format || {
                                 to: function(t) {
                                     return String(Math.round(t))
                                 }
                             };
-                        return g = S.appendChild(B(e, r, n))
+                        return g = S.appendChild(X(e, r, n))
                     }
 
-                    function W() {
+                    function I() {
                         var t = f.getBoundingClientRect(),
                             e = "offset" + ["Width", "Height"][o.ort];
                         return 0 === o.ort ? t.width || f[e] : t.height || f[e]
                     }
 
-                    function G(t, e, r, n) {
+                    function Z(t, e, r, n) {
                         var i = function(i) {
                                 var a, s, l = function(t, e, r) {
                                     var n = 0 === t.type.indexOf("touch"),
                                         i = 0 === t.type.indexOf("mouse"),
                                         o = 0 === t.type.indexOf("pointer"),
                                         a = 0,
                                         s = 0;
@@ -1280,344 +1279,344 @@
                                             a = u[0].pageX, s = u[0].pageY
                                         } else {
                                             var c = Array.prototype.find.call(t.changedTouches, l);
                                             if (!c) return !1;
                                             a = c.pageX, s = c.pageY
                                         }
                                     }
-                                    return e = e || p($), (i || o) && (a = t.clientX + e.x, s = t.clientY + e.y), t.pageOffset = e, t.points = [a, s], t.cursor = i || o, t
+                                    return e = e || p(A), (i || o) && (a = t.clientX + e.x, s = t.clientY + e.y), t.pageOffset = e, t.points = [a, s], t.cursor = i || o, t
                                 }(i, n.pageOffset, n.target || e);
-                                return !!l && !(H() && !n.doNotReject) && (a = S, s = o.cssClasses.tap, !((a.classList ? a.classList.contains(s) : new RegExp("\\b" + s + "\\b").test(a.className)) && !n.doNotReject)) && !(t === w.start && void 0 !== l.buttons && l.buttons > 1) && (!n.hover || !l.buttons) && (x || l.preventDefault(), l.calcPoint = l.points[o.ort], void r(l, n))
+                                return !!l && !(z() && !n.doNotReject) && (a = S, s = o.cssClasses.tap, !((a.classList ? a.classList.contains(s) : new RegExp("\\b" + s + "\\b").test(a.className)) && !n.doNotReject)) && !(t === w.start && void 0 !== l.buttons && l.buttons > 1) && (!n.hover || !l.buttons) && (x || l.preventDefault(), l.calcPoint = l.points[o.ort], void r(l, n))
                             },
                             a = [];
                         return t.split(" ").forEach((function(t) {
                             e.addEventListener(t, i, !!x && {
                                 passive: !0
                             }), a.push([t, i])
                         })), a
                     }
 
-                    function J(t) {
-                        var e, r, n, i, a, l, u = 100 * (t - (e = f, r = o.ort, n = e.getBoundingClientRect(), i = e.ownerDocument, a = i.documentElement, l = p(i), /webkit.*Chrome.*Mobile/i.test(navigator.userAgent) && (l.x = 0), r ? n.top + l.y - a.clientTop : n.left + l.x - a.clientLeft)) / W();
+                    function G(t) {
+                        var e, r, n, i, a, l, u = 100 * (t - (e = f, r = o.ort, n = e.getBoundingClientRect(), i = e.ownerDocument, a = i.documentElement, l = p(i), /webkit.*Chrome.*Mobile/i.test(navigator.userAgent) && (l.x = 0), r ? n.top + l.y - a.clientTop : n.left + l.x - a.clientLeft)) / I();
                         return u = s(u), o.dir ? 100 - u : u
                     }
 
-                    function K(t, e) {
-                        "mouseout" === t.type && "HTML" === t.target.nodeName && null === t.relatedTarget && tt(t, e)
+                    function J(t, e) {
+                        "mouseout" === t.type && "HTML" === t.target.nodeName && null === t.relatedTarget && Q(t, e)
                     }
 
-                    function Q(t, e) {
-                        if (-1 === navigator.appVersion.indexOf("MSIE 9") && 0 === t.buttons && 0 !== e.buttonsProperty) return tt(t, e);
+                    function K(t, e) {
+                        if (-1 === navigator.appVersion.indexOf("MSIE 9") && 0 === t.buttons && 0 !== e.buttonsProperty) return Q(t, e);
                         var r = (o.dir ? -1 : 1) * (t.calcPoint - e.startCalcPoint);
-                        ut(r > 0, 100 * r / e.baseSize, e.locations, e.handleNumbers, e.connect)
+                        lt(r > 0, 100 * r / e.baseSize, e.locations, e.handleNumbers, e.connect)
                     }
 
-                    function tt(t, e) {
-                        e.handle && (h(e.handle, o.cssClasses.active), V -= 1), e.listeners.forEach((function(t) {
-                            U.removeEventListener(t[0], t[1])
-                        })), 0 === V && (h(S, o.cssClasses.drag), ht(), t.cursor && (D.style.cursor = "", D.removeEventListener("selectstart", i))), e.handleNumbers.forEach((function(t) {
-                            at("change", t), at("set", t), at("end", t)
+                    function Q(t, e) {
+                        e.handle && (h(e.handle, o.cssClasses.active), C -= 1), e.listeners.forEach((function(t) {
+                            $.removeEventListener(t[0], t[1])
+                        })), 0 === C && (h(S, o.cssClasses.drag), ct(), t.cursor && (U.style.cursor = "", U.removeEventListener("selectstart", i))), e.handleNumbers.forEach((function(t) {
+                            ot("change", t), ot("set", t), ot("end", t)
                         }))
                     }
 
-                    function et(t, e) {
-                        if (!e.handleNumbers.some(R)) {
+                    function tt(t, e) {
+                        if (!e.handleNumbers.some(H)) {
                             var r;
-                            1 === e.handleNumbers.length && (r = d[e.handleNumbers[0]].children[0], V += 1, c(r, o.cssClasses.active)), t.stopPropagation();
+                            1 === e.handleNumbers.length && (r = d[e.handleNumbers[0]].children[0], C += 1, c(r, o.cssClasses.active)), t.stopPropagation();
                             var n = [],
-                                a = G(w.move, U, Q, {
+                                a = Z(w.move, $, K, {
                                     target: t.target,
                                     handle: r,
                                     connect: e.connect,
                                     listeners: n,
                                     startCalcPoint: t.calcPoint,
-                                    baseSize: W(),
+                                    baseSize: I(),
                                     pageOffset: t.pageOffset,
                                     handleNumbers: e.handleNumbers,
                                     buttonsProperty: t.buttons,
-                                    locations: M.slice()
+                                    locations: P.slice()
                                 }),
-                                s = G(w.end, U, tt, {
+                                s = Z(w.end, $, Q, {
                                     target: t.target,
                                     handle: r,
                                     listeners: n,
                                     doNotReject: !0,
                                     handleNumbers: e.handleNumbers
                                 }),
-                                l = G("mouseout", U, K, {
+                                l = Z("mouseout", $, J, {
                                     target: t.target,
                                     handle: r,
                                     listeners: n,
                                     doNotReject: !0,
                                     handleNumbers: e.handleNumbers
                                 });
-                            n.push.apply(n, a.concat(s, l)), t.cursor && (D.style.cursor = getComputedStyle(t.target).cursor, d.length > 1 && c(S, o.cssClasses.drag), D.addEventListener("selectstart", i, !1)), e.handleNumbers.forEach((function(t) {
-                                at("start", t)
+                            n.push.apply(n, a.concat(s, l)), t.cursor && (U.style.cursor = getComputedStyle(t.target).cursor, d.length > 1 && c(S, o.cssClasses.drag), U.addEventListener("selectstart", i, !1)), e.handleNumbers.forEach((function(t) {
+                                ot("start", t)
                             }))
                         }
                     }
 
-                    function rt(t) {
+                    function et(t) {
                         t.stopPropagation();
-                        var e = J(t.calcPoint),
+                        var e = G(t.calcPoint),
                             r = function(t) {
                                 var e = 100,
                                     r = !1;
                                 return d.forEach((function(n, i) {
-                                    if (!R(i)) {
-                                        var o = M[i],
+                                    if (!H(i)) {
+                                        var o = P[i],
                                             a = Math.abs(o - t);
                                         (a < e || a <= e && t > o || 100 === a && 100 === e) && (r = i, e = a)
                                     }
                                 })), r
                             }(e);
-                        !1 !== r && (o.events.snap || a(S, o.cssClasses.tap, o.animationDuration), pt(r, e, !0, !0), ht(), at("slide", r, !0), at("update", r, !0), o.events.snap ? et(t, {
+                        !1 !== r && (o.events.snap || a(S, o.cssClasses.tap, o.animationDuration), ht(r, e, !0, !0), ct(), ot("slide", r, !0), ot("update", r, !0), o.events.snap ? tt(t, {
                             handleNumbers: [r]
-                        }) : (at("change", r, !0), at("set", r, !0)))
+                        }) : (ot("change", r, !0), ot("set", r, !0)))
                     }
 
-                    function nt(t) {
-                        var e = J(t.calcPoint),
-                            r = k.getStep(e),
-                            n = k.fromStepping(r);
-                        Object.keys(A).forEach((function(t) {
-                            "hover" === t.split(".")[0] && A[t].forEach((function(t) {
-                                t.call(bt, n)
+                    function rt(t) {
+                        var e = G(t.calcPoint),
+                            r = N.getStep(e),
+                            n = N.fromStepping(r);
+                        Object.keys(V).forEach((function(t) {
+                            "hover" === t.split(".")[0] && V[t].forEach((function(t) {
+                                t.call(vt, n)
                             }))
                         }))
                     }
 
-                    function it(t, e) {
-                        A[t] = A[t] || [], A[t].push(e), "update" === t.split(".")[0] && d.forEach((function(t, e) {
-                            at("update", e)
+                    function nt(t, e) {
+                        V[t] = V[t] || [], V[t].push(e), "update" === t.split(".")[0] && d.forEach((function(t, e) {
+                            ot("update", e)
                         }))
                     }
 
-                    function ot(t) {
+                    function it(t) {
                         var e = t && t.split(".")[0],
                             r = e ? t.substring(e.length) : t;
-                        Object.keys(A).forEach((function(t) {
+                        Object.keys(V).forEach((function(t) {
                             var n = t.split(".")[0],
                                 i = t.substring(n.length);
                             e && e !== n || r && r !== i || function(t) {
-                                return t === N || t === E
-                            }(i) && r !== i || delete A[t]
+                                return t === E.aria || t === E.tooltips
+                            }(i) && r !== i || delete V[t]
                         }))
                     }
 
-                    function at(t, e, r) {
-                        Object.keys(A).forEach((function(n) {
+                    function ot(t, e, r) {
+                        Object.keys(V).forEach((function(n) {
                             var i = n.split(".")[0];
-                            t === i && A[n].forEach((function(t) {
-                                t.call(bt, P.map(o.format.to), e, P.slice(), r || !1, M.slice(), bt)
+                            t === i && V[n].forEach((function(t) {
+                                t.call(vt, k.map(o.format.to), e, k.slice(), r || !1, P.slice(), vt)
                             }))
                         }))
                     }
 
-                    function st(t, e, r, n, i, a) {
+                    function at(t, e, r, n, i, a) {
                         var l;
-                        return d.length > 1 && !o.events.unconstrained && (n && e > 0 && (l = k.getAbsoluteDistance(t[e - 1], o.margin, !1), r = Math.max(r, l)), i && e < d.length - 1 && (l = k.getAbsoluteDistance(t[e + 1], o.margin, !0), r = Math.min(r, l))), d.length > 1 && o.limit && (n && e > 0 && (l = k.getAbsoluteDistance(t[e - 1], o.limit, !1), r = Math.min(r, l)), i && e < d.length - 1 && (l = k.getAbsoluteDistance(t[e + 1], o.limit, !0), r = Math.max(r, l))), o.padding && (0 === e && (l = k.getAbsoluteDistance(0, o.padding[0], !1), r = Math.max(r, l)), e === d.length - 1 && (l = k.getAbsoluteDistance(100, o.padding[1], !0), r = Math.min(r, l))), !((r = s(r = k.getStep(r))) === t[e] && !a) && r
+                        return d.length > 1 && !o.events.unconstrained && (n && e > 0 && (l = N.getAbsoluteDistance(t[e - 1], o.margin, !1), r = Math.max(r, l)), i && e < d.length - 1 && (l = N.getAbsoluteDistance(t[e + 1], o.margin, !0), r = Math.min(r, l))), d.length > 1 && o.limit && (n && e > 0 && (l = N.getAbsoluteDistance(t[e - 1], o.limit, !1), r = Math.min(r, l)), i && e < d.length - 1 && (l = N.getAbsoluteDistance(t[e + 1], o.limit, !0), r = Math.max(r, l))), o.padding && (0 === e && (l = N.getAbsoluteDistance(0, o.padding[0], !1), r = Math.max(r, l)), e === d.length - 1 && (l = N.getAbsoluteDistance(100, o.padding[1], !0), r = Math.min(r, l))), !((r = s(r = N.getStep(r))) === t[e] && !a) && r
                     }
 
-                    function lt(t, e) {
+                    function st(t, e) {
                         var r = o.ort;
                         return (r ? e : t) + ", " + (r ? t : e)
                     }
 
-                    function ut(t, e, r, n, i) {
+                    function lt(t, e, r, n, i) {
                         var o = r.slice(),
                             a = n[0],
                             s = [!t, t],
                             l = [t, !t];
                         n = n.slice(), t && n.reverse(), n.length > 1 ? n.forEach((function(t, r) {
-                            var n = st(o, t, o[t] + e, s[r], l[r], !1);
+                            var n = at(o, t, o[t] + e, s[r], l[r], !1);
                             !1 === n ? e = 0 : (e = n - o[t], o[t] = n)
                         })) : s = l = [!0];
                         var u = !1;
                         n.forEach((function(t, n) {
-                            u = pt(t, r[t] + e, s[n], l[n]) || u
+                            u = ht(t, r[t] + e, s[n], l[n]) || u
                         })), u && (n.forEach((function(t) {
-                            at("update", t), at("slide", t)
-                        })), null != i && at("drag", a))
+                            ot("update", t), ot("slide", t)
+                        })), null != i && ot("drag", a))
                     }
 
-                    function ct(t, e) {
+                    function ut(t, e) {
                         return o.dir ? 100 - t - e : t
                     }
 
-                    function ht() {
-                        C.forEach((function(t) {
-                            var e = M[t] > 50 ? -1 : 1,
+                    function ct() {
+                        M.forEach((function(t) {
+                            var e = P[t] > 50 ? -1 : 1,
                                 r = 3 + (d.length + e * t);
                             d[t].style.zIndex = String(r)
                         }))
                     }
 
-                    function pt(t, e, r, n, i) {
-                        return i || (e = st(M, t, e, r, n, !1)), !1 !== e && (function(t, e) {
-                            M[t] = e, P[t] = k.fromStepping(e);
-                            var r = "translate(" + lt(10 * (ct(e, 0) - O) + "%", "0") + ")";
-                            d[t].style[o.transformRule] = r, ft(t), ft(t + 1)
+                    function ht(t, e, r, n, i) {
+                        return i || (e = at(P, t, e, r, n, !1)), !1 !== e && (function(t, e) {
+                            P[t] = e, k[t] = N.fromStepping(e);
+                            var r = "translate(" + st(10 * (ut(e, 0) - D) + "%", "0") + ")";
+                            d[t].style[o.transformRule] = r, pt(t), pt(t + 1)
                         }(t, e), !0)
                     }
 
-                    function ft(t) {
+                    function pt(t) {
                         if (m[t]) {
                             var e = 0,
                                 r = 100;
-                            0 !== t && (e = M[t - 1]), t !== m.length - 1 && (r = M[t]);
+                            0 !== t && (e = P[t - 1]), t !== m.length - 1 && (r = P[t]);
                             var n = r - e,
-                                i = "translate(" + lt(ct(e, n) + "%", "0") + ")",
-                                a = "scale(" + lt(n / 100, "1") + ")";
+                                i = "translate(" + st(ut(e, n) + "%", "0") + ")",
+                                a = "scale(" + st(n / 100, "1") + ")";
                             m[t].style[o.transformRule] = i + " " + a
                         }
                     }
 
-                    function dt(t, e) {
-                        return null === t || !1 === t || void 0 === t ? M[e] : ("number" == typeof t && (t = String(t)), !1 !== (t = o.format.from(t)) && (t = k.toStepping(t)), !1 === t || isNaN(t) ? M[e] : t)
+                    function ft(t, e) {
+                        return null === t || !1 === t || void 0 === t ? P[e] : ("number" == typeof t && (t = String(t)), !1 !== (t = o.format.from(t)) && (t = N.toStepping(t)), !1 === t || isNaN(t) ? P[e] : t)
                     }
 
-                    function mt(t, e, r) {
+                    function dt(t, e, r) {
                         var n = l(t),
-                            i = void 0 === M[0];
-                        e = void 0 === e || e, o.animate && !i && a(S, o.cssClasses.tap, o.animationDuration), C.forEach((function(t) {
-                            pt(t, dt(n[t], t), !0, !1, r)
+                            i = void 0 === P[0];
+                        e = void 0 === e || e, o.animate && !i && a(S, o.cssClasses.tap, o.animationDuration), M.forEach((function(t) {
+                            ht(t, ft(n[t], t), !0, !1, r)
                         }));
-                        var s = 1 === C.length ? 0 : 1;
-                        if (i && k.hasNoSize() && (r = !0, M[0] = 0, C.length > 1)) {
-                            var u = 100 / (C.length - 1);
-                            C.forEach((function(t) {
-                                M[t] = t * u
+                        var s = 1 === M.length ? 0 : 1;
+                        if (i && N.hasNoSize() && (r = !0, P[0] = 0, M.length > 1)) {
+                            var u = 100 / (M.length - 1);
+                            M.forEach((function(t) {
+                                P[t] = t * u
                             }))
                         }
-                        for (; s < C.length; ++s) C.forEach((function(t) {
-                            pt(t, M[t], !0, !0, r)
+                        for (; s < M.length; ++s) M.forEach((function(t) {
+                            ht(t, P[t], !0, !0, r)
                         }));
-                        ht(), C.forEach((function(t) {
-                            at("update", t), null !== n[t] && e && at("set", t)
+                        ct(), M.forEach((function(t) {
+                            ot("update", t), null !== n[t] && e && ot("set", t)
                         }))
                     }
 
-                    function gt(t) {
-                        if (void 0 === t && (t = !1), t) return 1 === P.length ? P[0] : P.slice(0);
-                        var e = P.map(o.format.to);
+                    function mt(t) {
+                        if (void 0 === t && (t = !1), t) return 1 === k.length ? k[0] : k.slice(0);
+                        var e = k.map(o.format.to);
                         return 1 === e.length ? e[0] : e
                     }
 
-                    function vt(t) {
-                        var e = M[t],
-                            r = k.getNearbySteps(e),
-                            n = P[t],
+                    function gt(t) {
+                        var e = P[t],
+                            r = N.getNearbySteps(e),
+                            n = k[t],
                             i = r.thisStep.step,
                             a = null;
                         if (o.snap) return [n - r.stepBefore.startValue || null, r.stepAfter.startValue - n || null];
                         !1 !== i && n + i > r.stepAfter.startValue && (i = r.stepAfter.startValue - n), a = n > r.thisStep.startValue ? r.thisStep.step : !1 !== r.stepBefore.step && n - r.stepBefore.highestStep, 100 === e ? i = null : 0 === e && (a = null);
-                        var s = k.countStepDecimals();
+                        var s = N.countStepDecimals();
                         return null !== i && !1 !== i && (i = Number(i.toFixed(s))), null !== a && !1 !== a && (a = Number(a.toFixed(s))), [a, i]
                     }
-                    c(y = S, o.cssClasses.target), 0 === o.dir ? c(y, o.cssClasses.ltr) : c(y, o.cssClasses.rtl), 0 === o.ort ? c(y, o.cssClasses.horizontal) : c(y, o.cssClasses.vertical), c(y, "rtl" === getComputedStyle(y).direction ? o.cssClasses.textDirectionRtl : o.cssClasses.textDirectionLtr), f = L(y, o.cssClasses.base),
+                    c(y = S, o.cssClasses.target), 0 === o.dir ? c(y, o.cssClasses.ltr) : c(y, o.cssClasses.rtl), 0 === o.ort ? c(y, o.cssClasses.horizontal) : c(y, o.cssClasses.vertical), c(y, "rtl" === getComputedStyle(y).direction ? o.cssClasses.textDirectionRtl : o.cssClasses.textDirectionLtr), f = O(y, o.cssClasses.base),
                         function(t, e) {
-                            var r = L(e, o.cssClasses.connects);
-                            d = [], (m = []).push(T(r, t[0]));
-                            for (var n = 0; n < o.handles; n++) d.push(j(e, n)), C[n] = n, m.push(T(r, t[n + 1]))
+                            var r = O(e, o.cssClasses.connects);
+                            d = [], (m = []).push(j(r, t[0]));
+                            for (var n = 0; n < o.handles; n++) d.push(L(e, n)), M[n] = n, m.push(j(r, t[n + 1]))
                         }(o.connect, f), (b = o.events).fixed || d.forEach((function(t, e) {
-                            G(w.start, t.children[0], et, {
+                            Z(w.start, t.children[0], tt, {
                                 handleNumbers: [e]
                             })
-                        })), b.tap && G(w.start, f, rt, {}), b.hover && G(w.move, f, nt, {
+                        })), b.tap && Z(w.start, f, et, {}), b.hover && Z(w.move, f, rt, {
                             hover: !0
                         }), b.drag && m.forEach((function(t, e) {
                             if (!1 !== t && 0 !== e && e !== m.length - 1) {
                                 var r = d[e - 1],
                                     n = d[e],
                                     i = [t],
                                     a = [r, n],
                                     s = [e - 1, e];
-                                c(t, o.cssClasses.draggable), b.fixed && (i.push(r.children[0]), i.push(n.children[0])), b.dragAll && (a = d, s = C), i.forEach((function(e) {
-                                    G(w.start, e, et, {
+                                c(t, o.cssClasses.draggable), b.fixed && (i.push(r.children[0]), i.push(n.children[0])), b.dragAll && (a = d, s = M), i.forEach((function(e) {
+                                    Z(w.start, e, tt, {
                                         handles: a,
                                         handleNumbers: s,
                                         connect: t
                                     })
                                 }))
                             }
-                        })), mt(o.start), o.pips && I(o.pips), o.tooltips && _(), ot("update" + N), it("update" + N, (function(t, e, r, n, i) {
-                            C.forEach((function(t) {
+                        })), dt(o.start), o.pips && Y(o.pips), o.tooltips && F(), it("update" + E.aria), nt("update" + E.aria, (function(t, e, r, n, i) {
+                            M.forEach((function(t) {
                                 var e = d[t],
-                                    n = st(M, t, 0, !0, !0, !0),
-                                    a = st(M, t, 100, !0, !0, !0),
+                                    n = at(P, t, 0, !0, !0, !0),
+                                    a = at(P, t, 100, !0, !0, !0),
                                     s = i[t],
                                     l = String(o.ariaFormat.to(r[t]));
-                                n = k.fromStepping(n).toFixed(1), a = k.fromStepping(a).toFixed(1), s = k.fromStepping(s).toFixed(1), e.children[0].setAttribute("aria-valuemin", n), e.children[0].setAttribute("aria-valuemax", a), e.children[0].setAttribute("aria-valuenow", s), e.children[0].setAttribute("aria-valuetext", l)
+                                n = N.fromStepping(n).toFixed(1), a = N.fromStepping(a).toFixed(1), s = N.fromStepping(s).toFixed(1), e.children[0].setAttribute("aria-valuemin", n), e.children[0].setAttribute("aria-valuemax", a), e.children[0].setAttribute("aria-valuenow", s), e.children[0].setAttribute("aria-valuetext", l)
                             }))
                         }));
-                    var bt = {
+                    var vt = {
                         destroy: function() {
-                            for (ot(N), ot(E), Object.keys(o.cssClasses).forEach((function(t) {
+                            for (it(E.aria), it(E.tooltips), Object.keys(o.cssClasses).forEach((function(t) {
                                     h(S, o.cssClasses[t])
                                 })); S.firstChild;) S.removeChild(S.firstChild);
                             delete S.noUiSlider
                         },
                         steps: function() {
-                            return C.map(vt)
+                            return M.map(gt)
                         },
-                        on: it,
-                        off: ot,
-                        get: gt,
-                        set: mt,
+                        on: nt,
+                        off: it,
+                        get: mt,
+                        set: dt,
                         setHandle: function(t, e, r, n) {
-                            if (!((t = Number(t)) >= 0 && t < C.length)) throw new Error("noUiSlider: invalid handle number, got: " + t);
-                            pt(t, dt(e, t), !0, !0, n), at("update", t), r && at("set", t)
+                            if (!((t = Number(t)) >= 0 && t < M.length)) throw new Error("noUiSlider: invalid handle number, got: " + t);
+                            ht(t, ft(e, t), !0, !0, n), ot("update", t), r && ot("set", t)
                         },
                         reset: function(t) {
-                            mt(o.start, t)
+                            dt(o.start, t)
                         },
                         __moveHandles: function(t, e, r) {
-                            ut(t, e, M, r)
+                            lt(t, e, P, r)
                         },
                         options: u,
                         updateOptions: function(t, e) {
-                            var r = gt(),
+                            var r = mt(),
                                 i = ["margin", "limit", "padding", "range", "animate", "snap", "step", "format", "pips", "tooltips"];
                             i.forEach((function(e) {
                                 void 0 !== t[e] && (u[e] = t[e])
                             }));
-                            var a = Z(u);
+                            var a = W(u);
                             i.forEach((function(e) {
                                 void 0 !== t[e] && (o[e] = a[e])
-                            })), k = a.spectrum, o.margin = a.margin, o.limit = a.limit, o.padding = a.padding, o.pips ? I(o.pips) : Y(), o.tooltips ? _() : F(), M = [], mt(n(t.start) ? t.start : r, e)
+                            })), N = a.spectrum, o.margin = a.margin, o.limit = a.limit, o.padding = a.padding, o.pips ? Y(o.pips) : B(), o.tooltips ? F() : R(), P = [], dt(n(t.start) ? t.start : r, e)
                         },
                         target: S,
-                        removePips: Y,
-                        removeTooltips: F,
+                        removePips: B,
+                        removeTooltips: R,
                         getPositions: function() {
-                            return M.slice()
+                            return P.slice()
                         },
                         getTooltips: function() {
                             return v
                         },
                         getOrigins: function() {
                             return d
                         },
-                        pips: I
+                        pips: Y
                     };
-                    return bt
+                    return vt
                 }
 
-                function J(t, e) {
+                function G(t, e) {
                     if (!t || !t.nodeName) throw new Error("noUiSlider: create requires a single element, got: " + t);
                     if (t.noUiSlider) throw new Error("noUiSlider: Slider was already initialized.");
-                    var r = G(t, Z(e), e);
+                    var r = Z(t, W(e), e);
                     return t.noUiSlider = r, r
                 }
-                var K = {
+                var J = {
                     __spectrum: w,
                     cssClasses: S,
-                    create: J
+                    create: G
                 };
-                t.create = J, t.cssClasses = S, t.default = K, Object.defineProperty(t, "__esModule", {
+                t.create = G, t.cssClasses = S, t.default = J, Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
             }(e)
         }
     }
 ]);
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/495.ea5e18a84b54f152ae61.js` & `jupyterlab_widgets-3.0.8/labextension/static/495.b58859516292ffe4bc96.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -151,15 +151,15 @@
                 serialize_naive: () => ge,
                 serialize_time: () => ie,
                 time_serializers: () => le,
                 typeset: () => a,
                 uuid: () => i.uuid,
                 version: () => ws
             });
-            var i = s(7193);
+            var i = s(9890);
 
             function a(e, t) {
                 void 0 !== t && (e.textContent = t), void 0 !== window.MathJax && MathJax.Hub.Queue(["Typeset", MathJax.Hub, e])
             }
 
             function l(e) {
                 const t = document.createElement("div");
@@ -607,17 +607,17 @@
             k.class_map = {
                 primary: ["mod-primary"],
                 success: ["mod-success"],
                 info: ["mod-info"],
                 warning: ["mod-warning"],
                 danger: ["mod-danger"]
             };
-            var L = s(8918),
-                V = s(2720),
-                I = s(3992),
+            var L = s(6697),
+                V = s(5633),
+                I = s(8778),
                 W = s(2994),
                 A = s.n(W);
             class E extends g {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _view_name: "BoxView",
                         _model_name: "BoxModel",
@@ -2588,16 +2588,16 @@
                 updateSliderValue(e, t, s) {
                     if (s.updated_view === this) return;
                     const i = this.$slider.noUiSlider.get().map(Math.round),
                         a = this.model.get("index").map(Math.round);
                     i[0] === a[0] && i[1] === a[1] || this.$slider.noUiSlider.set(a)
                 }
             }
-            var xt = s(1840),
-                ft = s(9520);
+            var xt = s(4901),
+                ft = s(5593);
             class wt extends I.Panel {
                 constructor() {
                     super(...arguments), this._widgetRemoved = new xt.Signal(this)
                 }
                 get widgetRemoved() {
                     return this._widgetRemoved
                 }
@@ -2993,15 +2993,15 @@
                     super.initialize(e), this.childrenViews = new i.ViewList(this.addChildView, (e => {
                         e.remove()
                     }), this), this.listenTo(this.model, "change:children", (() => this.updateTabs())), this.listenTo(this.model, "change:titles", (() => this.updateTitles()))
                 }
                 render() {
                     super.render();
                     const e = this.luminoWidget;
-                    e.addClass("jupyter-widgets"), e.addClass("widget-container"), e.addClass("widget-tab"), e.tabsMovable = !0, e.tabBar.insertBehavior = "none", e.tabBar.currentChanged.connect(this._onTabChanged, this), e.tabBar.tabMoved.connect(this._onTabMoved, this), e.tabBar.addClass("widget-tab-bar"), e.tabContents.addClass("widget-tab-contents"), e.tabBar.tabsMovable = !1, this.updateTabs(), this.update()
+                    e.addClass("jupyter-widgets"), e.addClass("widget-container"), e.addClass("jupyter-widget-tab"), e.addClass("widget-tab"), e.tabsMovable = !0, e.tabBar.insertBehavior = "none", e.tabBar.currentChanged.connect(this._onTabChanged, this), e.tabBar.tabMoved.connect(this._onTabMoved, this), e.tabBar.addClass("widget-tab-bar"), e.tabContents.addClass("widget-tab-contents"), e.tabBar.tabsMovable = !1, this.updateTabs(), this.update()
                 }
                 updateTabs() {
                     var e;
                     this.updatingTabs = !0, this.luminoWidget.currentIndex = null, null === (e = this.childrenViews) || void 0 === e || e.update(this.model.get("children")), this.luminoWidget.currentIndex = this.model.get("selected_index"), this.updatingTabs = !1
                 }
                 addChildView(e, t) {
                     const s = this.model.get("titles")[t] || "",
@@ -3811,12 +3811,12 @@
                 warning: ["mod-warning"],
                 danger: ["mod-danger"]
             };
             const ws = s(7021).i8
         },
         7021: e => {
             e.exports = {
-                i8: "5.0.5"
+                i8: "5.0.6"
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/595.b7741b41fd98f8f3d844.js` & `jupyterlab_widgets-3.0.8/labextension/static/595.942a65706d9bc281d5ca.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
                 reject: () => d,
                 remove_buffers: () => g,
                 resolvePromisesDict: () => h,
                 shims: () => H,
                 unpack_models: () => C,
                 uuid: () => c
             });
-            var i = s(1526),
+            var i = s(7930),
                 n = s(8149),
                 o = s.n(n);
 
             function r(e, t) {
                 return e.filter((e => -1 === t.indexOf(e)))
             }
 
@@ -215,16 +215,16 @@
                             this.el.removeEventListener(e.eventName, e.handler, !1)
                         }
                         this._domEvents.length = 0
                     }
                     return this
                 }
             }
-            var O = s(2720),
-                E = s(3992);
+            var O = s(5633),
+                E = s(8778);
             const x = "2.0.0",
                 S = "2.1.0",
                 M = "IPY_MODEL_",
                 P = e => JSON.parse(JSON.stringify(e)),
                 L = globalThis.structuredClone || P;
 
             function C(e, t) {
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/596.340cb969418e72309eb4.js` & `jupyterlab_widgets-3.0.8/labextension/static/596.1f32fb4ed861227b46e2.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     [596, 965], {
         2965: (e, t, u) => {
             u.r(t), u.d(t, {
                 OUTPUT_WIDGET_VERSION: () => _,
                 OutputModel: () => d,
                 OutputView: () => l
             });
-            var s = u(7193);
+            var s = u(9890);
             const _ = "1.0.0";
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: "OutputModel",
                         _view_name: "OutputView",
                         _model_module: "@jupyter-widgets/output",
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/644.7d1bff49f8e38fac4070.js` & `jupyterlab_widgets-3.0.8/labextension/static/644.52a1098a3a5f3e45abff.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2863,27 +2863,26 @@
                     var a = r ? r[s] : s;
                     o[s] = e(t[a], a, t)
                 }
                 return o
             }
 
             function Ge(t) {
-                var e = function(e, n, r, i) {
-                    var o = !we(e) && at(e),
-                        s = (o || e).length,
-                        a = t > 0 ? 0 : s - 1;
-                    for (i || (r = e[o ? o[a] : a], a += t); a >= 0 && a < s; a += t) {
-                        var u = o ? o[a] : a;
-                        r = n(r, e[u], u, e)
-                    }
-                    return r
-                };
-                return function(t, n, r, i) {
+                return function(e, n, r, i) {
                     var o = arguments.length >= 3;
-                    return e(t, Kt(n, i, 4), r, o)
+                    return function(e, n, r, i) {
+                        var o = !we(e) && at(e),
+                            s = (o || e).length,
+                            a = t > 0 ? 0 : s - 1;
+                        for (i || (r = e[o ? o[a] : a], a += t); a >= 0 && a < s; a += t) {
+                            var u = o ? o[a] : a;
+                            r = n(r, e[u], u, e)
+                        }
+                        return r
+                    }(e, Kt(n, i, 4), r, o)
                 }
             }
             const Xe = Ge(1),
                 Qe = Ge(-1);
 
             function Ye(t, e, n) {
                 var r = [];
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/699.2ea6ecfcddb8f3bb4732.js` & `jupyterlab_widgets-3.0.8/labextension/static/699.e966b1425a7d4e8c3f4e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,65 +5,65 @@
             const s = r(8006),
                 n = Symbol("max"),
                 i = Symbol("length"),
                 o = Symbol("lengthCalculator"),
                 a = Symbol("allowStale"),
                 l = Symbol("maxAge"),
                 h = Symbol("dispose"),
-                p = Symbol("noDisposeOnSet"),
-                u = Symbol("lruList"),
+                u = Symbol("noDisposeOnSet"),
+                p = Symbol("lruList"),
                 c = Symbol("cache"),
-                f = Symbol("updateAgeOnGet"),
-                E = () => 1,
+                E = Symbol("updateAgeOnGet"),
+                f = () => 1,
                 m = (e, t, r) => {
                     const s = e[c].get(t);
                     if (s) {
                         const t = s.value;
                         if (v(e, t)) {
                             if (g(e, s), !e[a]) return
-                        } else r && (e[f] && (s.value.now = Date.now()), e[u].unshiftNode(s));
+                        } else r && (e[E] && (s.value.now = Date.now()), e[p].unshiftNode(s));
                         return t.value
                     }
                 },
                 v = (e, t) => {
                     if (!t || !t.maxAge && !e[l]) return !1;
                     const r = Date.now() - t.now;
                     return t.maxAge ? r > t.maxAge : e[l] && r > e[l]
                 },
                 $ = e => {
                     if (e[i] > e[n])
-                        for (let t = e[u].tail; e[i] > e[n] && null !== t;) {
+                        for (let t = e[p].tail; e[i] > e[n] && null !== t;) {
                             const r = t.prev;
                             g(e, t), t = r
                         }
                 },
                 g = (e, t) => {
                     if (t) {
                         const r = t.value;
-                        e[h] && e[h](r.key, r.value), e[i] -= r.length, e[c].delete(r.key), e[u].removeNode(t)
+                        e[h] && e[h](r.key, r.value), e[i] -= r.length, e[c].delete(r.key), e[p].removeNode(t)
                     }
                 };
-            class I {
+            class R {
                 constructor(e, t, r, s, n) {
                     this.key = e, this.value = t, this.length = r, this.now = s, this.maxAge = n || 0
                 }
             }
-            const R = (e, t, r, s) => {
+            const I = (e, t, r, s) => {
                 let n = r.value;
                 v(e, n) && (g(e, r), e[a] || (n = void 0)), n && t.call(s, n.value, n.key, e)
             };
             e.exports = class {
                 constructor(e) {
                     if ("number" == typeof e && (e = {
                             max: e
                         }), e || (e = {}), e.max && ("number" != typeof e.max || e.max < 0)) throw new TypeError("max must be a non-negative number");
                     this[n] = e.max || 1 / 0;
-                    const t = e.length || E;
-                    if (this[o] = "function" != typeof t ? E : t, this[a] = e.stale || !1, e.maxAge && "number" != typeof e.maxAge) throw new TypeError("maxAge must be a number");
-                    this[l] = e.maxAge || 0, this[h] = e.dispose, this[p] = e.noDisposeOnSet || !1, this[f] = e.updateAgeOnGet || !1, this.reset()
+                    const t = e.length || f;
+                    if (this[o] = "function" != typeof t ? f : t, this[a] = e.stale || !1, e.maxAge && "number" != typeof e.maxAge) throw new TypeError("maxAge must be a number");
+                    this[l] = e.maxAge || 0, this[h] = e.dispose, this[u] = e.noDisposeOnSet || !1, this[E] = e.updateAgeOnGet || !1, this.reset()
                 }
                 set max(e) {
                     if ("number" != typeof e || e < 0) throw new TypeError("max must be a non-negative number");
                     this[n] = e || 1 / 0, $(this)
                 }
                 get max() {
                     return this[n]
@@ -78,85 +78,85 @@
                     if ("number" != typeof e) throw new TypeError("maxAge must be a non-negative number");
                     this[l] = e, $(this)
                 }
                 get maxAge() {
                     return this[l]
                 }
                 set lengthCalculator(e) {
-                    "function" != typeof e && (e = E), e !== this[o] && (this[o] = e, this[i] = 0, this[u].forEach((e => {
+                    "function" != typeof e && (e = f), e !== this[o] && (this[o] = e, this[i] = 0, this[p].forEach((e => {
                         e.length = this[o](e.value, e.key), this[i] += e.length
                     }))), $(this)
                 }
                 get lengthCalculator() {
                     return this[o]
                 }
                 get length() {
                     return this[i]
                 }
                 get itemCount() {
-                    return this[u].length
+                    return this[p].length
                 }
                 rforEach(e, t) {
                     t = t || this;
-                    for (let r = this[u].tail; null !== r;) {
+                    for (let r = this[p].tail; null !== r;) {
                         const s = r.prev;
-                        R(this, e, r, t), r = s
+                        I(this, e, r, t), r = s
                     }
                 }
                 forEach(e, t) {
                     t = t || this;
-                    for (let r = this[u].head; null !== r;) {
+                    for (let r = this[p].head; null !== r;) {
                         const s = r.next;
-                        R(this, e, r, t), r = s
+                        I(this, e, r, t), r = s
                     }
                 }
                 keys() {
-                    return this[u].toArray().map((e => e.key))
+                    return this[p].toArray().map((e => e.key))
                 }
                 values() {
-                    return this[u].toArray().map((e => e.value))
+                    return this[p].toArray().map((e => e.value))
                 }
                 reset() {
-                    this[h] && this[u] && this[u].length && this[u].forEach((e => this[h](e.key, e.value))), this[c] = new Map, this[u] = new s, this[i] = 0
+                    this[h] && this[p] && this[p].length && this[p].forEach((e => this[h](e.key, e.value))), this[c] = new Map, this[p] = new s, this[i] = 0
                 }
                 dump() {
-                    return this[u].map((e => !v(this, e) && {
+                    return this[p].map((e => !v(this, e) && {
                         k: e.key,
                         v: e.value,
                         e: e.now + (e.maxAge || 0)
                     })).toArray().filter((e => e))
                 }
                 dumpLru() {
-                    return this[u]
+                    return this[p]
                 }
                 set(e, t, r) {
                     if ((r = r || this[l]) && "number" != typeof r) throw new TypeError("maxAge must be a number");
                     const s = r ? Date.now() : 0,
                         a = this[o](t, e);
                     if (this[c].has(e)) {
                         if (a > this[n]) return g(this, this[c].get(e)), !1;
                         const o = this[c].get(e).value;
-                        return this[h] && (this[p] || this[h](e, o.value)), o.now = s, o.maxAge = r, o.value = t, this[i] += a - o.length, o.length = a, this.get(e), $(this), !0
+                        return this[h] && (this[u] || this[h](e, o.value)), o.now = s, o.maxAge = r, o.value = t, this[i] += a - o.length, o.length = a, this.get(e), $(this), !0
                     }
-                    const f = new I(e, t, a, s, r);
-                    return f.length > this[n] ? (this[h] && this[h](e, t), !1) : (this[i] += f.length, this[u].unshift(f), this[c].set(e, this[u].head), $(this), !0)
+                    const E = new R(e, t, a, s, r);
+                    return E.length > this[n] ? (this[h] && this[h](e, t), !1) : (this[i] += E.length, this[p].unshift(E), this[c].set(e, this[p].head), $(this), !0)
                 }
                 has(e) {
                     if (!this[c].has(e)) return !1;
                     const t = this[c].get(e).value;
                     return !v(this, t)
                 }
                 get(e) {
                     return m(this, e, !0)
                 }
                 peek(e) {
                     return m(this, e, !1)
                 }
                 pop() {
-                    const e = this[u].tail;
+                    const e = this[p].tail;
                     return e ? (g(this, e), e.value) : null
                 }
                 del(e) {
                     g(this, this[c].get(e))
                 }
                 load(e) {
                     this.reset();
@@ -209,58 +209,58 @@
                     r = "function" == typeof clearTimeout ? clearTimeout : i
                 } catch (e) {
                     r = i
                 }
             }();
             var a, l = [],
                 h = !1,
-                p = -1;
+                u = -1;
 
-            function u() {
-                h && a && (h = !1, a.length ? l = a.concat(l) : p = -1, l.length && c())
+            function p() {
+                h && a && (h = !1, a.length ? l = a.concat(l) : u = -1, l.length && c())
             }
 
             function c() {
                 if (!h) {
-                    var e = o(u);
+                    var e = o(p);
                     h = !0;
                     for (var t = l.length; t;) {
-                        for (a = l, l = []; ++p < t;) a && a[p].run();
-                        p = -1, t = l.length
+                        for (a = l, l = []; ++u < t;) a && a[u].run();
+                        u = -1, t = l.length
                     }
                     a = null, h = !1,
                         function(e) {
                             if (r === clearTimeout) return clearTimeout(e);
                             if ((r === i || !r) && clearTimeout) return r = clearTimeout, clearTimeout(e);
                             try {
-                                r(e)
+                                return r(e)
                             } catch (t) {
                                 try {
                                     return r.call(null, e)
                                 } catch (t) {
                                     return r.call(this, e)
                                 }
                             }
                         }(e)
                 }
             }
 
-            function f(e, t) {
+            function E(e, t) {
                 this.fun = e, this.array = t
             }
 
-            function E() {}
+            function f() {}
             s.nextTick = function(e) {
                 var t = new Array(arguments.length - 1);
                 if (arguments.length > 1)
                     for (var r = 1; r < arguments.length; r++) t[r - 1] = arguments[r];
-                l.push(new f(e, t)), 1 !== l.length || h || o(c)
-            }, f.prototype.run = function() {
+                l.push(new E(e, t)), 1 !== l.length || h || o(c)
+            }, E.prototype.run = function() {
                 this.fun.apply(null, this.array)
-            }, s.title = "browser", s.browser = !0, s.env = {}, s.argv = [], s.version = "", s.versions = {}, s.on = E, s.addListener = E, s.once = E, s.off = E, s.removeListener = E, s.removeAllListeners = E, s.emit = E, s.prependListener = E, s.prependOnceListener = E, s.listeners = function(e) {
+            }, s.title = "browser", s.browser = !0, s.env = {}, s.argv = [], s.version = "", s.versions = {}, s.on = f, s.addListener = f, s.once = f, s.off = f, s.removeListener = f, s.removeAllListeners = f, s.emit = f, s.prependListener = f, s.prependOnceListener = f, s.listeners = function(e) {
                 return []
             }, s.binding = function(e) {
                 throw new Error("process.binding is not supported")
             }, s.cwd = function() {
                 return "/"
             }, s.chdir = function(e) {
                 throw new Error("process.chdir is not supported")
@@ -281,178 +281,171 @@
                     }
                     h("comparator", e, t), this.options = t, this.loose = !!t.loose, this.parse(e), this.semver === s ? this.value = "" : this.value = this.operator + this.semver.version, h("comp", this)
                 }
                 parse(e) {
                     const t = this.options.loose ? o[a.COMPARATORLOOSE] : o[a.COMPARATOR],
                         r = e.match(t);
                     if (!r) throw new TypeError(`Invalid comparator: ${e}`);
-                    this.operator = void 0 !== r[1] ? r[1] : "", "=" === this.operator && (this.operator = ""), r[2] ? this.semver = new p(r[2], this.options.loose) : this.semver = s
+                    this.operator = void 0 !== r[1] ? r[1] : "", "=" === this.operator && (this.operator = ""), r[2] ? this.semver = new u(r[2], this.options.loose) : this.semver = s
                 }
                 toString() {
                     return this.value
                 }
                 test(e) {
                     if (h("Comparator.test", e, this.options.loose), this.semver === s || e === s) return !0;
                     if ("string" == typeof e) try {
-                        e = new p(e, this.options)
+                        e = new u(e, this.options)
                     } catch (e) {
                         return !1
                     }
                     return l(e, this.operator, this.semver, this.options)
                 }
                 intersects(e, t) {
                     if (!(e instanceof n)) throw new TypeError("a Comparator is required");
-                    if (t && "object" == typeof t || (t = {
-                            loose: !!t,
-                            includePrerelease: !1
-                        }), "" === this.operator) return "" === this.value || new u(e.value, t).test(this.value);
-                    if ("" === e.operator) return "" === e.value || new u(this.value, t).test(e.semver);
-                    const r = !(">=" !== this.operator && ">" !== this.operator || ">=" !== e.operator && ">" !== e.operator),
-                        s = !("<=" !== this.operator && "<" !== this.operator || "<=" !== e.operator && "<" !== e.operator),
-                        i = this.semver.version === e.semver.version,
-                        o = !(">=" !== this.operator && "<=" !== this.operator || ">=" !== e.operator && "<=" !== e.operator),
-                        a = l(this.semver, "<", e.semver, t) && (">=" === this.operator || ">" === this.operator) && ("<=" === e.operator || "<" === e.operator),
-                        h = l(this.semver, ">", e.semver, t) && ("<=" === this.operator || "<" === this.operator) && (">=" === e.operator || ">" === e.operator);
-                    return r || s || i && o || a || h
+                    return "" === this.operator ? "" === this.value || new p(e.value, t).test(this.value) : "" === e.operator ? "" === e.value || new p(this.value, t).test(e.semver) : !((t = i(t)).includePrerelease && ("<0.0.0-0" === this.value || "<0.0.0-0" === e.value) || !t.includePrerelease && (this.value.startsWith("<0.0.0") || e.value.startsWith("<0.0.0")) || (!this.operator.startsWith(">") || !e.operator.startsWith(">")) && (!this.operator.startsWith("<") || !e.operator.startsWith("<")) && (this.semver.version !== e.semver.version || !this.operator.includes("=") || !e.operator.includes("=")) && !(l(this.semver, "<", e.semver, t) && this.operator.startsWith(">") && e.operator.startsWith("<")) && !(l(this.semver, ">", e.semver, t) && this.operator.startsWith("<") && e.operator.startsWith(">")))
                 }
             }
             e.exports = n;
             const i = r(1388),
                 {
                     re: o,
                     t: a
                 } = r(4808),
                 l = r(8117),
                 h = r(952),
-                p = r(2435),
-                u = r(6843)
+                u = r(2435),
+                p = r(6843)
         },
         6843: (e, t, r) => {
             class s {
                 constructor(e, t) {
                     if (t = i(t), e instanceof s) return e.loose === !!t.loose && e.includePrerelease === !!t.includePrerelease ? e : new s(e.raw, t);
                     if (e instanceof o) return this.raw = e.value, this.set = [
                         [e]
                     ], this.format(), this;
                     if (this.options = t, this.loose = !!t.loose, this.includePrerelease = !!t.includePrerelease, this.raw = e, this.set = e.split("||").map((e => this.parseRange(e.trim()))).filter((e => e.length)), !this.set.length) throw new TypeError(`Invalid SemVer Range: ${e}`);
                     if (this.set.length > 1) {
                         const e = this.set[0];
-                        if (this.set = this.set.filter((e => !E(e[0]))), 0 === this.set.length) this.set = [e];
+                        if (this.set = this.set.filter((e => !v(e[0]))), 0 === this.set.length) this.set = [e];
                         else if (this.set.length > 1)
                             for (const e of this.set)
-                                if (1 === e.length && m(e[0])) {
+                                if (1 === e.length && $(e[0])) {
                                     this.set = [e];
                                     break
                                 }
                     }
                     this.format()
                 }
                 format() {
                     return this.range = this.set.map((e => e.join(" ").trim())).join("||").trim(), this.range
                 }
                 toString() {
                     return this.range
                 }
                 parseRange(e) {
                     e = e.trim();
-                    const t = `parseRange:${Object.keys(this.options).join(",")}:${e}`,
+                    const t = ((this.options.includePrerelease && f) | (this.options.loose && m)) + ":" + e,
                         r = n.get(t);
                     if (r) return r;
                     const s = this.options.loose,
-                        i = s ? h[p.HYPHENRANGELOOSE] : h[p.HYPHENRANGE];
-                    e = e.replace(i, O(this.options.includePrerelease)), a("hyphen replace", e), e = e.replace(h[p.COMPARATORTRIM], u), a("comparator trim", e);
-                    let l = (e = (e = (e = e.replace(h[p.TILDETRIM], c)).replace(h[p.CARETTRIM], f)).split(/\s+/).join(" ")).split(" ").map((e => $(e, this.options))).join(" ").split(/\s+/).map((e => L(e, this.options)));
-                    s && (l = l.filter((e => (a("loose invalid filter", e, this.options), !!e.match(h[p.COMPARATORLOOSE]))))), a("range list", l);
-                    const m = new Map,
-                        v = l.map((e => new o(e, this.options)));
-                    for (const e of v) {
-                        if (E(e)) return [e];
-                        m.set(e.value, e)
-                    }
-                    m.size > 1 && m.has("") && m.delete("");
-                    const g = [...m.values()];
-                    return n.set(t, g), g
+                        i = s ? h[u.HYPHENRANGELOOSE] : h[u.HYPHENRANGE];
+                    e = e.replace(i, S(this.options.includePrerelease)), a("hyphen replace", e), e = e.replace(h[u.COMPARATORTRIM], p), a("comparator trim", e);
+                    let l = (e = (e = (e = e.replace(h[u.TILDETRIM], c)).replace(h[u.CARETTRIM], E)).split(/\s+/).join(" ")).split(" ").map((e => R(e, this.options))).join(" ").split(/\s+/).map((e => y(e, this.options)));
+                    s && (l = l.filter((e => (a("loose invalid filter", e, this.options), !!e.match(h[u.COMPARATORLOOSE]))))), a("range list", l);
+                    const $ = new Map,
+                        g = l.map((e => new o(e, this.options)));
+                    for (const e of g) {
+                        if (v(e)) return [e];
+                        $.set(e.value, e)
+                    }
+                    $.size > 1 && $.has("") && $.delete("");
+                    const I = [...$.values()];
+                    return n.set(t, I), I
                 }
                 intersects(e, t) {
                     if (!(e instanceof s)) throw new TypeError("a Range is required");
-                    return this.set.some((r => v(r, t) && e.set.some((e => v(e, t) && r.every((r => e.every((e => r.intersects(e, t)))))))))
+                    return this.set.some((r => g(r, t) && e.set.some((e => g(e, t) && r.every((r => e.every((e => r.intersects(e, t)))))))))
                 }
                 test(e) {
                     if (!e) return !1;
                     if ("string" == typeof e) try {
                         e = new l(e, this.options)
                     } catch (e) {
                         return !1
                     }
                     for (let t = 0; t < this.set.length; t++)
-                        if (y(this.set[t], e, this.options)) return !0;
+                        if (x(this.set[t], e, this.options)) return !0;
                     return !1
                 }
             }
             e.exports = s;
             const n = new(r(7105))({
                     max: 1e3
                 }),
                 i = r(1388),
                 o = r(7847),
                 a = r(952),
                 l = r(2435),
                 {
                     re: h,
-                    t: p,
-                    comparatorTrimReplace: u,
+                    t: u,
+                    comparatorTrimReplace: p,
                     tildeTrimReplace: c,
-                    caretTrimReplace: f
+                    caretTrimReplace: E
                 } = r(4808),
-                E = e => "<0.0.0-0" === e.value,
-                m = e => "" === e.value,
-                v = (e, t) => {
+                {
+                    FLAG_INCLUDE_PRERELEASE: f,
+                    FLAG_LOOSE: m
+                } = r(5558),
+                v = e => "<0.0.0-0" === e.value,
+                $ = e => "" === e.value,
+                g = (e, t) => {
                     let r = !0;
                     const s = e.slice();
                     let n = s.pop();
                     for (; r && s.length;) r = s.every((e => n.intersects(e, t))), n = s.pop();
                     return r
                 },
-                $ = (e, t) => (a("comp", e, t), e = d(e, t), a("caret", e), e = I(e, t), a("tildes", e), e = w(e, t), a("xrange", e), e = A(e, t), a("stars", e), e),
-                g = e => !e || "x" === e.toLowerCase() || "*" === e,
-                I = (e, t) => e.trim().split(/\s+/).map((e => R(e, t))).join(" "),
-                R = (e, t) => {
-                    const r = t.loose ? h[p.TILDELOOSE] : h[p.TILDE];
+                R = (e, t) => (a("comp", e, t), e = w(e, t), a("caret", e), e = d(e, t), a("tildes", e), e = L(e, t), a("xrange", e), e = O(e, t), a("stars", e), e),
+                I = e => !e || "x" === e.toLowerCase() || "*" === e,
+                d = (e, t) => e.trim().split(/\s+/).map((e => N(e, t))).join(" "),
+                N = (e, t) => {
+                    const r = t.loose ? h[u.TILDELOOSE] : h[u.TILDE];
                     return e.replace(r, ((t, r, s, n, i) => {
                         let o;
-                        return a("tilde", e, t, r, s, n, i), g(r) ? o = "" : g(s) ? o = `>=${r}.0.0 <${+r+1}.0.0-0` : g(n) ? o = `>=${r}.${s}.0 <${r}.${+s+1}.0-0` : i ? (a("replaceTilde pr", i), o = `>=${r}.${s}.${n}-${i} <${r}.${+s+1}.0-0`) : o = `>=${r}.${s}.${n} <${r}.${+s+1}.0-0`, a("tilde return", o), o
+                        return a("tilde", e, t, r, s, n, i), I(r) ? o = "" : I(s) ? o = `>=${r}.0.0 <${+r+1}.0.0-0` : I(n) ? o = `>=${r}.${s}.0 <${r}.${+s+1}.0-0` : i ? (a("replaceTilde pr", i), o = `>=${r}.${s}.${n}-${i} <${r}.${+s+1}.0-0`) : o = `>=${r}.${s}.${n} <${r}.${+s+1}.0-0`, a("tilde return", o), o
                     }))
                 },
-                d = (e, t) => e.trim().split(/\s+/).map((e => N(e, t))).join(" "),
-                N = (e, t) => {
+                w = (e, t) => e.trim().split(/\s+/).map((e => A(e, t))).join(" "),
+                A = (e, t) => {
                     a("caret", e, t);
-                    const r = t.loose ? h[p.CARETLOOSE] : h[p.CARET],
+                    const r = t.loose ? h[u.CARETLOOSE] : h[u.CARET],
                         s = t.includePrerelease ? "-0" : "";
                     return e.replace(r, ((t, r, n, i, o) => {
                         let l;
-                        return a("caret", e, t, r, n, i, o), g(r) ? l = "" : g(n) ? l = `>=${r}.0.0${s} <${+r+1}.0.0-0` : g(i) ? l = "0" === r ? `>=${r}.${n}.0${s} <${r}.${+n+1}.0-0` : `>=${r}.${n}.0${s} <${+r+1}.0.0-0` : o ? (a("replaceCaret pr", o), l = "0" === r ? "0" === n ? `>=${r}.${n}.${i}-${o} <${r}.${n}.${+i+1}-0` : `>=${r}.${n}.${i}-${o} <${r}.${+n+1}.0-0` : `>=${r}.${n}.${i}-${o} <${+r+1}.0.0-0`) : (a("no pr"), l = "0" === r ? "0" === n ? `>=${r}.${n}.${i}${s} <${r}.${n}.${+i+1}-0` : `>=${r}.${n}.${i}${s} <${r}.${+n+1}.0-0` : `>=${r}.${n}.${i} <${+r+1}.0.0-0`), a("caret return", l), l
+                        return a("caret", e, t, r, n, i, o), I(r) ? l = "" : I(n) ? l = `>=${r}.0.0${s} <${+r+1}.0.0-0` : I(i) ? l = "0" === r ? `>=${r}.${n}.0${s} <${r}.${+n+1}.0-0` : `>=${r}.${n}.0${s} <${+r+1}.0.0-0` : o ? (a("replaceCaret pr", o), l = "0" === r ? "0" === n ? `>=${r}.${n}.${i}-${o} <${r}.${n}.${+i+1}-0` : `>=${r}.${n}.${i}-${o} <${r}.${+n+1}.0-0` : `>=${r}.${n}.${i}-${o} <${+r+1}.0.0-0`) : (a("no pr"), l = "0" === r ? "0" === n ? `>=${r}.${n}.${i}${s} <${r}.${n}.${+i+1}-0` : `>=${r}.${n}.${i}${s} <${r}.${+n+1}.0-0` : `>=${r}.${n}.${i} <${+r+1}.0.0-0`), a("caret return", l), l
                     }))
                 },
-                w = (e, t) => (a("replaceXRanges", e, t), e.split(/\s+/).map((e => T(e, t))).join(" ")),
+                L = (e, t) => (a("replaceXRanges", e, t), e.split(/\s+/).map((e => T(e, t))).join(" ")),
                 T = (e, t) => {
                     e = e.trim();
-                    const r = t.loose ? h[p.XRANGELOOSE] : h[p.XRANGE];
+                    const r = t.loose ? h[u.XRANGELOOSE] : h[u.XRANGE];
                     return e.replace(r, ((r, s, n, i, o, l) => {
                         a("xRange", e, r, s, n, i, o, l);
-                        const h = g(n),
-                            p = h || g(i),
-                            u = p || g(o),
-                            c = u;
-                        return "=" === s && c && (s = ""), l = t.includePrerelease ? "-0" : "", h ? r = ">" === s || "<" === s ? "<0.0.0-0" : "*" : s && c ? (p && (i = 0), o = 0, ">" === s ? (s = ">=", p ? (n = +n + 1, i = 0, o = 0) : (i = +i + 1, o = 0)) : "<=" === s && (s = "<", p ? n = +n + 1 : i = +i + 1), "<" === s && (l = "-0"), r = `${s+n}.${i}.${o}${l}`) : p ? r = `>=${n}.0.0${l} <${+n+1}.0.0-0` : u && (r = `>=${n}.${i}.0${l} <${n}.${+i+1}.0-0`), a("xRange return", r), r
+                        const h = I(n),
+                            u = h || I(i),
+                            p = u || I(o),
+                            c = p;
+                        return "=" === s && c && (s = ""), l = t.includePrerelease ? "-0" : "", h ? r = ">" === s || "<" === s ? "<0.0.0-0" : "*" : s && c ? (u && (i = 0), o = 0, ">" === s ? (s = ">=", u ? (n = +n + 1, i = 0, o = 0) : (i = +i + 1, o = 0)) : "<=" === s && (s = "<", u ? n = +n + 1 : i = +i + 1), "<" === s && (l = "-0"), r = `${s+n}.${i}.${o}${l}`) : u ? r = `>=${n}.0.0${l} <${+n+1}.0.0-0` : p && (r = `>=${n}.${i}.0${l} <${n}.${+i+1}.0-0`), a("xRange return", r), r
                     }))
                 },
-                A = (e, t) => (a("replaceStars", e, t), e.trim().replace(h[p.STAR], "")),
-                L = (e, t) => (a("replaceGTE0", e, t), e.trim().replace(h[t.includePrerelease ? p.GTE0PRE : p.GTE0], "")),
-                O = e => (t, r, s, n, i, o, a, l, h, p, u, c, f) => `${r=g(s)?"":g(n)?`>=${s}.0.0${e?"-0":""}`:g(i)?`>=${s}.${n}.0${e?"-0":""}`:o?`>=${r}`:`>=${r}${e?"-0":""}`} ${l=g(h)?"":g(p)?`<${+h+1}.0.0-0`:g(u)?`<${h}.${+p+1}.0-0`:c?`<=${h}.${p}.${u}-${c}`:e?`<${h}.${p}.${+u+1}-0`:`<=${l}`}`.trim(),
-                y = (e, t, r) => {
+                O = (e, t) => (a("replaceStars", e, t), e.trim().replace(h[u.STAR], "")),
+                y = (e, t) => (a("replaceGTE0", e, t), e.trim().replace(h[t.includePrerelease ? u.GTE0PRE : u.GTE0], "")),
+                S = e => (t, r, s, n, i, o, a, l, h, u, p, c, E) => `${r=I(s)?"":I(n)?`>=${s}.0.0${e?"-0":""}`:I(i)?`>=${s}.${n}.0${e?"-0":""}`:o?`>=${r}`:`>=${r}${e?"-0":""}`} ${l=I(h)?"":I(u)?`<${+h+1}.0.0-0`:I(p)?`<${h}.${+u+1}.0-0`:c?`<=${h}.${u}.${p}-${c}`:e?`<${h}.${u}.${+p+1}-0`:`<=${l}`}`.trim(),
+                x = (e, t, r) => {
                     for (let r = 0; r < e.length; r++)
                         if (!e[r].test(t)) return !1;
                     if (t.prerelease.length && !r.includePrerelease) {
                         for (let r = 0; r < e.length; r++)
                             if (a(e[r].semver), e[r].semver !== o.ANY && e[r].semver.prerelease.length > 0) {
                                 const s = e[r].semver;
                                 if (s.major === t.major && s.minor === t.minor && s.patch === t.patch) return !0
@@ -471,20 +464,20 @@
                     re: o,
                     t: a
                 } = r(4808),
                 l = r(1388),
                 {
                     compareIdentifiers: h
                 } = r(4935);
-            class p {
+            class u {
                 constructor(e, t) {
-                    if (t = l(t), e instanceof p) {
+                    if (t = l(t), e instanceof u) {
                         if (e.loose === !!t.loose && e.includePrerelease === !!t.includePrerelease) return e;
                         e = e.version
-                    } else if ("string" != typeof e) throw new TypeError(`Invalid Version: ${e}`);
+                    } else if ("string" != typeof e) throw new TypeError(`Invalid version. Must be a string. Got type "${typeof e}".`);
                     if (e.length > n) throw new TypeError(`version is longer than ${n} characters`);
                     s("SemVer", e, t), this.options = t, this.loose = !!t.loose, this.includePrerelease = !!t.includePrerelease;
                     const r = e.trim().match(t.loose ? o[a.LOOSE] : o[a.FULL]);
                     if (!r) throw new TypeError(`Invalid Version: ${e}`);
                     if (this.raw = e, this.major = +r[1], this.minor = +r[2], this.patch = +r[3], this.major > i || this.major < 0) throw new TypeError("Invalid major version");
                     if (this.minor > i || this.minor < 0) throw new TypeError("Invalid minor version");
                     if (this.patch > i || this.patch < 0) throw new TypeError("Invalid patch version");
@@ -499,87 +492,97 @@
                 format() {
                     return this.version = `${this.major}.${this.minor}.${this.patch}`, this.prerelease.length && (this.version += `-${this.prerelease.join(".")}`), this.version
                 }
                 toString() {
                     return this.version
                 }
                 compare(e) {
-                    if (s("SemVer.compare", this.version, this.options, e), !(e instanceof p)) {
+                    if (s("SemVer.compare", this.version, this.options, e), !(e instanceof u)) {
                         if ("string" == typeof e && e === this.version) return 0;
-                        e = new p(e, this.options)
+                        e = new u(e, this.options)
                     }
                     return e.version === this.version ? 0 : this.compareMain(e) || this.comparePre(e)
                 }
                 compareMain(e) {
-                    return e instanceof p || (e = new p(e, this.options)), h(this.major, e.major) || h(this.minor, e.minor) || h(this.patch, e.patch)
+                    return e instanceof u || (e = new u(e, this.options)), h(this.major, e.major) || h(this.minor, e.minor) || h(this.patch, e.patch)
                 }
                 comparePre(e) {
-                    if (e instanceof p || (e = new p(e, this.options)), this.prerelease.length && !e.prerelease.length) return -1;
+                    if (e instanceof u || (e = new u(e, this.options)), this.prerelease.length && !e.prerelease.length) return -1;
                     if (!this.prerelease.length && e.prerelease.length) return 1;
                     if (!this.prerelease.length && !e.prerelease.length) return 0;
                     let t = 0;
                     do {
                         const r = this.prerelease[t],
                             n = e.prerelease[t];
                         if (s("prerelease compare", t, r, n), void 0 === r && void 0 === n) return 0;
                         if (void 0 === n) return 1;
                         if (void 0 === r) return -1;
                         if (r !== n) return h(r, n)
                     } while (++t)
                 }
                 compareBuild(e) {
-                    e instanceof p || (e = new p(e, this.options));
+                    e instanceof u || (e = new u(e, this.options));
                     let t = 0;
                     do {
                         const r = this.build[t],
                             n = e.build[t];
                         if (s("prerelease compare", t, r, n), void 0 === r && void 0 === n) return 0;
                         if (void 0 === n) return 1;
                         if (void 0 === r) return -1;
                         if (r !== n) return h(r, n)
                     } while (++t)
                 }
-                inc(e, t) {
+                inc(e, t, r) {
                     switch (e) {
                         case "premajor":
-                            this.prerelease.length = 0, this.patch = 0, this.minor = 0, this.major++, this.inc("pre", t);
+                            this.prerelease.length = 0, this.patch = 0, this.minor = 0, this.major++, this.inc("pre", t, r);
                             break;
                         case "preminor":
-                            this.prerelease.length = 0, this.patch = 0, this.minor++, this.inc("pre", t);
+                            this.prerelease.length = 0, this.patch = 0, this.minor++, this.inc("pre", t, r);
                             break;
                         case "prepatch":
-                            this.prerelease.length = 0, this.inc("patch", t), this.inc("pre", t);
+                            this.prerelease.length = 0, this.inc("patch", t, r), this.inc("pre", t, r);
                             break;
                         case "prerelease":
-                            0 === this.prerelease.length && this.inc("patch", t), this.inc("pre", t);
+                            0 === this.prerelease.length && this.inc("patch", t, r), this.inc("pre", t, r);
                             break;
                         case "major":
                             0 === this.minor && 0 === this.patch && 0 !== this.prerelease.length || this.major++, this.minor = 0, this.patch = 0, this.prerelease = [];
                             break;
                         case "minor":
                             0 === this.patch && 0 !== this.prerelease.length || this.minor++, this.patch = 0, this.prerelease = [];
                             break;
                         case "patch":
                             0 === this.prerelease.length && this.patch++, this.prerelease = [];
                             break;
-                        case "pre":
-                            if (0 === this.prerelease.length) this.prerelease = [0];
+                        case "pre": {
+                            const e = Number(r) ? 1 : 0;
+                            if (!t && !1 === r) throw new Error("invalid increment argument: identifier is empty");
+                            if (0 === this.prerelease.length) this.prerelease = [e];
                             else {
-                                let e = this.prerelease.length;
-                                for (; --e >= 0;) "number" == typeof this.prerelease[e] && (this.prerelease[e]++, e = -2); - 1 === e && this.prerelease.push(0)
+                                let s = this.prerelease.length;
+                                for (; --s >= 0;) "number" == typeof this.prerelease[s] && (this.prerelease[s]++, s = -2);
+                                if (-1 === s) {
+                                    if (t === this.prerelease.join(".") && !1 === r) throw new Error("invalid increment argument: identifier already exists");
+                                    this.prerelease.push(e)
+                                }
                             }
-                            t && (0 === h(this.prerelease[0], t) ? isNaN(this.prerelease[1]) && (this.prerelease = [t, 0]) : this.prerelease = [t, 0]);
-                            break;
+                            if (t) {
+                                let s = [t, e];
+                                !1 === r && (s = [t]), 0 === h(this.prerelease[0], t) ? isNaN(this.prerelease[1]) && (this.prerelease = s) : this.prerelease = s
+                            }
+                            break
+                        }
                         default:
                             throw new Error(`invalid increment argument: ${e}`)
                     }
                     return this.format(), this.raw = this.version, this
                 }
             }
-            e.exports = p
+            e.exports = u
         },
         6694: (e, t, r) => {
             const s = r(9943);
             e.exports = (e, t) => {
                 const r = s(e.trim().replace(/^[=v]+/, ""), t);
                 return r ? r.version : null
             }
@@ -649,27 +652,25 @@
             e.exports = (e, t) => s(e, t, !0)
         },
         2271: (e, t, r) => {
             const s = r(2435);
             e.exports = (e, t, r) => new s(e, r).compare(new s(t, r))
         },
         6007: (e, t, r) => {
-            const s = r(9943),
-                n = r(3276);
+            const s = r(9943);
             e.exports = (e, t) => {
-                if (n(e, t)) return null; {
-                    const r = s(e),
-                        n = s(t),
-                        i = r.prerelease.length || n.prerelease.length,
-                        o = i ? "pre" : "",
-                        a = i ? "prerelease" : "";
-                    for (const e in r)
-                        if (("major" === e || "minor" === e || "patch" === e) && r[e] !== n[e]) return o + e;
-                    return a
-                }
+                const r = s(e, null, !0),
+                    n = s(t, null, !0),
+                    i = r.compare(n);
+                if (0 === i) return null;
+                const o = i > 0,
+                    a = o ? n : r,
+                    l = !!(o ? r : n).prerelease.length,
+                    h = l ? "pre" : "";
+                return r.major !== n.major ? h + "major" : r.minor !== n.minor ? h + "minor" : r.patch !== n.patch ? h + "patch" : l ? "prerelease" : a.patch ? "patch" : a.minor ? "minor" : "major"
             }
         },
         3276: (e, t, r) => {
             const s = r(2271);
             e.exports = (e, t, r) => 0 === s(e, t, r)
         },
         6379: (e, t, r) => {
@@ -678,18 +679,18 @@
         },
         8463: (e, t, r) => {
             const s = r(2271);
             e.exports = (e, t, r) => s(e, t, r) >= 0
         },
         6360: (e, t, r) => {
             const s = r(2435);
-            e.exports = (e, t, r, n) => {
-                "string" == typeof r && (n = r, r = void 0);
+            e.exports = (e, t, r, n, i) => {
+                "string" == typeof r && (i = n, n = r, r = void 0);
                 try {
-                    return new s(e instanceof s ? e.version : e, r).inc(t, n).version
+                    return new s(e instanceof s ? e.version : e, r).inc(t, n, i).version
                 } catch (e) {
                     return null
                 }
             }
         },
         7274: (e, t, r) => {
             const s = r(2271);
@@ -708,29 +709,22 @@
             e.exports = (e, t) => new s(e, t).minor
         },
         7893: (e, t, r) => {
             const s = r(2271);
             e.exports = (e, t, r) => 0 !== s(e, t, r)
         },
         9943: (e, t, r) => {
-            const {
-                MAX_LENGTH: s
-            } = r(5558), {
-                re: n,
-                t: i
-            } = r(4808), o = r(2435), a = r(1388);
-            e.exports = (e, t) => {
-                if (t = a(t), e instanceof o) return e;
-                if ("string" != typeof e) return null;
-                if (e.length > s) return null;
-                if (!(t.loose ? n[i.LOOSE] : n[i.FULL]).test(e)) return null;
+            const s = r(2435);
+            e.exports = (e, t, r = !1) => {
+                if (e instanceof s) return e;
                 try {
-                    return new o(e, t)
+                    return new s(e, t)
                 } catch (e) {
-                    return null
+                    if (!r) return null;
+                    throw e
                 }
             }
         },
         4250: (e, t, r) => {
             const s = r(2435);
             e.exports = (e, t) => new s(e, t).patch
         },
@@ -775,102 +769,106 @@
             const s = r(4808),
                 n = r(5558),
                 i = r(2435),
                 o = r(4935),
                 a = r(9943),
                 l = r(7230),
                 h = r(6694),
-                p = r(6360),
-                u = r(6007),
+                u = r(6360),
+                p = r(6007),
                 c = r(4551),
-                f = r(469),
-                E = r(4250),
+                E = r(469),
+                f = r(4250),
                 m = r(8204),
                 v = r(2271),
                 $ = r(733),
                 g = r(5404),
-                I = r(5914),
-                R = r(1116),
+                R = r(5914),
+                I = r(1116),
                 d = r(2961),
                 N = r(6379),
                 w = r(7274),
-                T = r(3276),
-                A = r(7893),
-                L = r(8463),
+                A = r(3276),
+                L = r(7893),
+                T = r(8463),
                 O = r(506),
                 y = r(8117),
-                x = r(8686),
-                S = r(7847),
+                S = r(8686),
+                x = r(7847),
                 P = r(6843),
                 b = r(9844),
                 C = r(8865),
                 D = r(3727),
                 G = r(4338),
-                M = r(5078),
+                M = r(1542),
                 j = r(6240),
                 F = r(9106),
-                X = r(995),
-                k = r(7805),
-                U = r(2013),
-                _ = r(1338),
+                _ = r(995),
+                X = r(7805),
+                k = r(2013),
+                U = r(1338),
                 V = r(3122);
             e.exports = {
                 parse: a,
                 valid: l,
                 clean: h,
-                inc: p,
-                diff: u,
+                inc: u,
+                diff: p,
                 major: c,
-                minor: f,
-                patch: E,
+                minor: E,
+                patch: f,
                 prerelease: m,
                 compare: v,
                 rcompare: $,
                 compareLoose: g,
-                compareBuild: I,
-                sort: R,
+                compareBuild: R,
+                sort: I,
                 rsort: d,
                 gt: N,
                 lt: w,
-                eq: T,
-                neq: A,
-                gte: L,
+                eq: A,
+                neq: L,
+                gte: T,
                 lte: O,
                 cmp: y,
-                coerce: x,
-                Comparator: S,
+                coerce: S,
+                Comparator: x,
                 Range: P,
                 satisfies: b,
                 toComparators: C,
                 maxSatisfying: D,
                 minSatisfying: G,
                 minVersion: M,
                 validRange: j,
                 outside: F,
-                gtr: X,
-                ltr: k,
-                intersects: U,
-                simplifyRange: _,
+                gtr: _,
+                ltr: X,
+                intersects: k,
+                simplifyRange: U,
                 subset: V,
                 SemVer: i,
                 re: s.re,
                 src: s.src,
                 tokens: s.t,
                 SEMVER_SPEC_VERSION: n.SEMVER_SPEC_VERSION,
+                RELEASE_TYPES: n.RELEASE_TYPES,
                 compareIdentifiers: o.compareIdentifiers,
                 rcompareIdentifiers: o.rcompareIdentifiers
             }
         },
         5558: e => {
             const t = Number.MAX_SAFE_INTEGER || 9007199254740991;
             e.exports = {
-                SEMVER_SPEC_VERSION: "2.0.0",
                 MAX_LENGTH: 256,
+                MAX_SAFE_COMPONENT_LENGTH: 16,
                 MAX_SAFE_INTEGER: t,
-                MAX_SAFE_COMPONENT_LENGTH: 16
+                RELEASE_TYPES: ["major", "premajor", "minor", "preminor", "patch", "prepatch", "prerelease"],
+                SEMVER_SPEC_VERSION: "2.0.0",
+                FLAG_INCLUDE_PRERELEASE: 1,
+                FLAG_LOOSE: 2
             }
         },
         952: (e, t, r) => {
             var s = r(4406);
             const n = "object" == typeof s && s.env && s.env.NODE_DEBUG && /\bsemver\b/i.test(s.env.NODE_DEBUG) ? (...e) => console.error("SEMVER", ...e) : () => {};
             e.exports = n
         },
@@ -883,18 +881,19 @@
                 };
             e.exports = {
                 compareIdentifiers: r,
                 rcompareIdentifiers: (e, t) => r(t, e)
             }
         },
         1388: e => {
-            const t = ["includePrerelease", "loose", "rtl"];
-            e.exports = e => e ? "object" != typeof e ? {
-                loose: !0
-            } : t.filter((t => e[t])).reduce(((e, t) => (e[t] = !0, e)), {}) : {}
+            const t = Object.freeze({
+                    loose: !0
+                }),
+                r = Object.freeze({});
+            e.exports = e => e ? "object" != typeof e ? t : e : r
         },
         4808: (e, t, r) => {
             const {
                 MAX_SAFE_COMPONENT_LENGTH: s
             } = r(5558), n = r(952), i = (t = e.exports = {}).re = [], o = t.src = [], a = t.t = {};
             let l = 0;
             const h = (e, t, r) => {
@@ -905,15 +904,15 @@
         },
         995: (e, t, r) => {
             const s = r(9106);
             e.exports = (e, t, r) => s(e, t, ">", r)
         },
         2013: (e, t, r) => {
             const s = r(6843);
-            e.exports = (e, t, r) => (e = new s(e, r), t = new s(t, r), e.intersects(t))
+            e.exports = (e, t, r) => (e = new s(e, r), t = new s(t, r), e.intersects(t, r))
         },
         7805: (e, t, r) => {
             const s = r(9106);
             e.exports = (e, t, r) => s(e, t, "<", r)
         },
         3727: (e, t, r) => {
             const s = r(2435),
@@ -945,15 +944,15 @@
                     return null
                 }
                 return e.forEach((e => {
                     a.test(e) && (i && 1 !== o.compare(e) || (i = e, o = new s(i, r)))
                 })), i
             }
         },
-        5078: (e, t, r) => {
+        1542: (e, t, r) => {
             const s = r(2435),
                 n = r(6843),
                 i = r(6379);
             e.exports = (e, t) => {
                 e = new n(e, t);
                 let r = new s("0.0.0");
                 if (e.test(r)) return r;
@@ -988,37 +987,37 @@
                 {
                     ANY: i
                 } = n,
                 o = r(6843),
                 a = r(9844),
                 l = r(6379),
                 h = r(7274),
-                p = r(506),
-                u = r(8463);
+                u = r(506),
+                p = r(8463);
             e.exports = (e, t, r, c) => {
-                let f, E, m, v, $;
+                let E, f, m, v, $;
                 switch (e = new s(e, c), t = new o(t, c), r) {
                     case ">":
-                        f = l, E = p, m = h, v = ">", $ = ">=";
+                        E = l, f = u, m = h, v = ">", $ = ">=";
                         break;
                     case "<":
-                        f = h, E = u, m = l, v = "<", $ = "<=";
+                        E = h, f = p, m = l, v = "<", $ = "<=";
                         break;
                     default:
                         throw new TypeError('Must provide a hilo val of "<" or ">"')
                 }
                 if (a(e, t, c)) return !1;
                 for (let r = 0; r < t.set.length; ++r) {
                     const s = t.set[r];
                     let o = null,
                         a = null;
                     if (s.forEach((e => {
-                            e.semver === i && (e = new n(">=0.0.0")), o = o || e, a = a || e, f(e.semver, o.semver, c) ? o = e : m(e.semver, a.semver, c) && (a = e)
+                            e.semver === i && (e = new n(">=0.0.0")), o = o || e, a = a || e, E(e.semver, o.semver, c) ? o = e : m(e.semver, a.semver, c) && (a = e)
                         })), o.operator === v || o.operator === $) return !1;
-                    if ((!a.operator || a.operator === v) && E(e, a.semver)) return !1;
+                    if ((!a.operator || a.operator === v) && f(e, a.semver)) return !1;
                     if (a.operator === $ && m(e, a.semver)) return !1
                 }
                 return !0
             }
         },
         1338: (e, t, r) => {
             const s = r(9844),
@@ -1028,85 +1027,87 @@
                 let o = null,
                     a = null;
                 const l = e.sort(((e, t) => n(e, t, r)));
                 for (const e of l) s(e, t, r) ? (a = e, o || (o = e)) : (a && i.push([o, a]), a = null, o = null);
                 o && i.push([o, null]);
                 const h = [];
                 for (const [e, t] of i) e === t ? h.push(e) : t || e !== l[0] ? t ? e === l[0] ? h.push(`<=${t}`) : h.push(`${e} - ${t}`) : h.push(`>=${e}`) : h.push("*");
-                const p = h.join(" || "),
-                    u = "string" == typeof t.raw ? t.raw : String(t);
-                return p.length < u.length ? p : t
+                const u = h.join(" || "),
+                    p = "string" == typeof t.raw ? t.raw : String(t);
+                return u.length < p.length ? u : t
             }
         },
         3122: (e, t, r) => {
             const s = r(6843),
                 n = r(7847),
                 {
                     ANY: i
                 } = n,
                 o = r(9844),
                 a = r(2271),
-                l = (e, t, r) => {
+                l = [new n(">=0.0.0-0")],
+                h = [new n(">=0.0.0")],
+                u = (e, t, r) => {
                     if (e === t) return !0;
                     if (1 === e.length && e[0].semver === i) {
                         if (1 === t.length && t[0].semver === i) return !0;
-                        e = r.includePrerelease ? [new n(">=0.0.0-0")] : [new n(">=0.0.0")]
+                        e = r.includePrerelease ? l : h
                     }
                     if (1 === t.length && t[0].semver === i) {
                         if (r.includePrerelease) return !0;
-                        t = [new n(">=0.0.0")]
+                        t = h
                     }
                     const s = new Set;
-                    let l, u, c, f, E, m, v;
-                    for (const t of e) ">" === t.operator || ">=" === t.operator ? l = h(l, t, r) : "<" === t.operator || "<=" === t.operator ? u = p(u, t, r) : s.add(t.semver);
+                    let n, u, E, f, m, v, $;
+                    for (const t of e) ">" === t.operator || ">=" === t.operator ? n = p(n, t, r) : "<" === t.operator || "<=" === t.operator ? u = c(u, t, r) : s.add(t.semver);
                     if (s.size > 1) return null;
-                    if (l && u) {
-                        if (c = a(l.semver, u.semver, r), c > 0) return null;
-                        if (0 === c && (">=" !== l.operator || "<=" !== u.operator)) return null
+                    if (n && u) {
+                        if (E = a(n.semver, u.semver, r), E > 0) return null;
+                        if (0 === E && (">=" !== n.operator || "<=" !== u.operator)) return null
                     }
                     for (const e of s) {
-                        if (l && !o(e, String(l), r)) return null;
+                        if (n && !o(e, String(n), r)) return null;
                         if (u && !o(e, String(u), r)) return null;
                         for (const s of t)
                             if (!o(e, String(s), r)) return !1;
                         return !0
                     }
-                    let $ = !(!u || r.includePrerelease || !u.semver.prerelease.length) && u.semver,
-                        g = !(!l || r.includePrerelease || !l.semver.prerelease.length) && l.semver;
-                    $ && 1 === $.prerelease.length && "<" === u.operator && 0 === $.prerelease[0] && ($ = !1);
+                    let g = !(!u || r.includePrerelease || !u.semver.prerelease.length) && u.semver,
+                        R = !(!n || r.includePrerelease || !n.semver.prerelease.length) && n.semver;
+                    g && 1 === g.prerelease.length && "<" === u.operator && 0 === g.prerelease[0] && (g = !1);
                     for (const e of t) {
-                        if (v = v || ">" === e.operator || ">=" === e.operator, m = m || "<" === e.operator || "<=" === e.operator, l)
-                            if (g && e.semver.prerelease && e.semver.prerelease.length && e.semver.major === g.major && e.semver.minor === g.minor && e.semver.patch === g.patch && (g = !1), ">" === e.operator || ">=" === e.operator) {
-                                if (f = h(l, e, r), f === e && f !== l) return !1
-                            } else if (">=" === l.operator && !o(l.semver, String(e), r)) return !1;
+                        if ($ = $ || ">" === e.operator || ">=" === e.operator, v = v || "<" === e.operator || "<=" === e.operator, n)
+                            if (R && e.semver.prerelease && e.semver.prerelease.length && e.semver.major === R.major && e.semver.minor === R.minor && e.semver.patch === R.patch && (R = !1), ">" === e.operator || ">=" === e.operator) {
+                                if (f = p(n, e, r), f === e && f !== n) return !1
+                            } else if (">=" === n.operator && !o(n.semver, String(e), r)) return !1;
                         if (u)
-                            if ($ && e.semver.prerelease && e.semver.prerelease.length && e.semver.major === $.major && e.semver.minor === $.minor && e.semver.patch === $.patch && ($ = !1), "<" === e.operator || "<=" === e.operator) {
-                                if (E = p(u, e, r), E === e && E !== u) return !1
+                            if (g && e.semver.prerelease && e.semver.prerelease.length && e.semver.major === g.major && e.semver.minor === g.minor && e.semver.patch === g.patch && (g = !1), "<" === e.operator || "<=" === e.operator) {
+                                if (m = c(u, e, r), m === e && m !== u) return !1
                             } else if ("<=" === u.operator && !o(u.semver, String(e), r)) return !1;
-                        if (!e.operator && (u || l) && 0 !== c) return !1
+                        if (!e.operator && (u || n) && 0 !== E) return !1
                     }
-                    return !(l && m && !u && 0 !== c || u && v && !l && 0 !== c || g || $)
+                    return !(n && v && !u && 0 !== E || u && $ && !n && 0 !== E || R || g)
                 },
-                h = (e, t, r) => {
+                p = (e, t, r) => {
                     if (!e) return t;
                     const s = a(e.semver, t.semver, r);
                     return s > 0 ? e : s < 0 || ">" === t.operator && ">=" === e.operator ? t : e
                 },
-                p = (e, t, r) => {
+                c = (e, t, r) => {
                     if (!e) return t;
                     const s = a(e.semver, t.semver, r);
                     return s < 0 ? e : s > 0 || "<" === t.operator && "<=" === e.operator ? t : e
                 };
             e.exports = (e, t, r = {}) => {
                 if (e === t) return !0;
                 e = new s(e, r), t = new s(t, r);
                 let n = !1;
                 e: for (const s of e.set) {
                     for (const e of t.set) {
-                        const t = l(s, e, r);
+                        const t = u(s, e, r);
                         if (n = n || null !== t, t) continue e
                     }
                     if (n) return !1
                 }
                 return !0
             }
         },
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/965.b0caf50c6bbde92efb37.js` & `jupyterlab_widgets-3.0.8/labextension/static/965.22fa53da8ad2a8da593a.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     [965, 596], {
         2965: (e, t, u) => {
             u.r(t), u.d(t, {
                 OUTPUT_WIDGET_VERSION: () => _,
                 OutputModel: () => d,
                 OutputView: () => l
             });
-            var s = u(7193);
+            var s = u(9890);
             const _ = "1.0.0";
             class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: "OutputModel",
                         _view_name: "OutputView",
                         _model_module: "@jupyter-widgets/output",
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/remoteEntry.35e76720037cafa02724.js` & `jupyterlab_widgets-3.0.8/labextension/static/remoteEntry.98b8a827bfc5f86e95d2.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, d, u, l, f, s, c, p, h, b, m, g, v, y, j, w, P, S = {
-            2063: (e, r, t) => {
+    var e, r, t, a, n, o, i, u, l, f, d, s, c, p, b, h, m, g, v, y, j, w, P, S, k = {
+            5348: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(193), t.e(306), t.e(526), t.e(99), t.e(134)]).then((() => () => t(134))),
-                        "./extension": () => Promise.all([t.e(193), t.e(306), t.e(526), t.e(99), t.e(134)]).then((() => () => t(134)))
+                        "./index": () => Promise.all([t.e(890), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134))),
+                        "./extension": () => Promise.all([t.e(890), t.e(67), t.e(930), t.e(388), t.e(134)]).then((() => () => t(134)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var a = "default",
@@ -20,331 +20,334 @@
                     };
                 t.d(r, {
                     get: () => n,
                     init: () => o
                 })
             }
         },
-        k = {};
+        E = {};
 
-    function E(e) {
-        var r = k[e];
+    function _(e) {
+        var r = E[e];
         if (void 0 !== r) return r.exports;
-        var t = k[e] = {
+        var t = E[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return S[e].call(t.exports, t, t.exports, E), t.loaded = !0, t.exports
+        return k[e].call(t.exports, t, t.exports, _), t.loaded = !0, t.exports
     }
-    E.m = S, E.c = k, E.n = e => {
+    _.m = k, _.c = E, _.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return E.d(r, {
+        return _.d(r, {
             a: r
         }), r
-    }, E.d = (e, r) => {
-        for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
+    }, _.d = (e, r) => {
+        for (var t in r) _.o(r, t) && !_.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => (863 === e ? "@jupyter-widgets/controls" : e) + "." + {
+    }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => (863 === e ? "@jupyter-widgets/controls" : e) + "." + {
         61: "21f571face17e35076c2",
-        99: "53732494dd69b5e31fd8",
-        113: "270dbb43db912c1b3723",
-        134: "402424ef4079078b2e0e",
-        150: "1a6d6a3a0542a41bec5a",
-        193: "a9aa8b320332ce1c2da5",
-        291: "0b98a9cbc7337e1749ed",
-        306: "2ef7538ea3c5af230801",
-        345: "03be96cd091aac4797a5",
-        495: "ea5e18a84b54f152ae61",
-        526: "0e5eba70673325ef505d",
-        595: "b7741b41fd98f8f3d844",
-        596: "340cb969418e72309eb4",
-        644: "7d1bff49f8e38fac4070",
-        699: "2ea6ecfcddb8f3bb4732",
-        720: "4f52203625c8f270cbd8",
-        863: "3e6de8a3e6f58c6508f7",
-        965: "b0caf50c6bbde92efb37"
+        67: "760f0b2ce7647388b914",
+        113: "6113d19fca7ff66ccc66",
+        134: "b4eddbb09f5fd50a4007",
+        291: "cff5ef71b29e18850479",
+        336: "9f709c2076672b1bfe2b",
+        345: "17494fea1ff555b26294",
+        388: "7b9bc65ab3b0b744fe93",
+        495: "b58859516292ffe4bc96",
+        595: "942a65706d9bc281d5ca",
+        596: "1f32fb4ed861227b46e2",
+        633: "2cbcc5998e25c5521f72",
+        644: "52a1098a3a5f3e45abff",
+        699: "e966b1425a7d4e8c3f4e",
+        863: "f3d34622f50c9be50b4f",
+        890: "147c36e3b30d7baedc95",
+        930: "b32c52301e934bfecc7d",
+        965: "22fa53da8ad2a8da593a"
     } [e] + ".js?v=" + {
         61: "21f571face17e35076c2",
-        99: "53732494dd69b5e31fd8",
-        113: "270dbb43db912c1b3723",
-        134: "402424ef4079078b2e0e",
-        150: "1a6d6a3a0542a41bec5a",
-        193: "a9aa8b320332ce1c2da5",
-        291: "0b98a9cbc7337e1749ed",
-        306: "2ef7538ea3c5af230801",
-        345: "03be96cd091aac4797a5",
-        495: "ea5e18a84b54f152ae61",
-        526: "0e5eba70673325ef505d",
-        595: "b7741b41fd98f8f3d844",
-        596: "340cb969418e72309eb4",
-        644: "7d1bff49f8e38fac4070",
-        699: "2ea6ecfcddb8f3bb4732",
-        720: "4f52203625c8f270cbd8",
-        863: "3e6de8a3e6f58c6508f7",
-        965: "b0caf50c6bbde92efb37"
-    } [e], E.g = function() {
+        67: "760f0b2ce7647388b914",
+        113: "6113d19fca7ff66ccc66",
+        134: "b4eddbb09f5fd50a4007",
+        291: "cff5ef71b29e18850479",
+        336: "9f709c2076672b1bfe2b",
+        345: "17494fea1ff555b26294",
+        388: "7b9bc65ab3b0b744fe93",
+        495: "b58859516292ffe4bc96",
+        595: "942a65706d9bc281d5ca",
+        596: "1f32fb4ed861227b46e2",
+        633: "2cbcc5998e25c5521f72",
+        644: "52a1098a3a5f3e45abff",
+        699: "e966b1425a7d4e8c3f4e",
+        863: "f3d34622f50c9be50b4f",
+        890: "147c36e3b30d7baedc95",
+        930: "b32c52301e934bfecc7d",
+        965: "22fa53da8ad2a8da593a"
+    } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-widgets/jupyterlab-manager:", E.l = (t, a, n, o) => {
+    }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter-widgets/jupyterlab-manager:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
-            var i, d;
+            var i, u;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
-                    var f = u[l];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
-            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
             var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
                 c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), d && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, E.r = e => {
+    }, _.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, E.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
-        E.S = {};
+    }, _.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        _.S = {};
         var e = {},
             r = {};
-        E.I = (t, a) => {
+        _.I = (t, a) => {
             a || (a = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
                 if (a.push(n), e[t]) return e[t];
-                E.o(E.S, t) || (E.S[t] = {});
-                var o = E.S[t],
+                _.o(_.S, t) || (_.S[t] = {});
+                var o = _.S[t],
                     i = "@jupyter-widgets/jupyterlab-manager",
-                    d = (e, r, t, a) => {
+                    u = (e, r, t, a) => {
                         var n = o[e] = o[e] || {},
-                            d = n[r];
-                        (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
+                            u = n[r];
+                        (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (d("@jupyter-widgets/base-manager", "1.0.5", (() => Promise.all([E.e(113), E.e(193), E.e(526), E.e(150)]).then((() => () => E(6110))))), d("@jupyter-widgets/base", "6.0.4", (() => Promise.all([E.e(644), E.e(306), E.e(720), E.e(526), E.e(595)]).then((() => () => E(9185))))), d("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([E.e(345), E.e(193), E.e(306), E.e(720), E.e(495), E.e(99), E.e(61)]).then((() => () => E(2495))))), d("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([E.e(193), E.e(306), E.e(526), E.e(99), E.e(134)]).then((() => () => E(134))))), d("@jupyter-widgets/output", "6.0.4", (() => Promise.all([E.e(193), E.e(965)]).then((() => () => E(2965))))), d("jquery", "3.6.3", (() => E.e(291).then((() => () => E(8291))))), d("semver", "7.3.8", (() => E.e(699).then((() => () => E(7699)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (u("@jupyter-widgets/base-manager", "1.0.6", (() => Promise.all([_.e(113), _.e(890), _.e(930), _.e(336)]).then((() => () => _(6110))))), u("@jupyter-widgets/base", "6.0.5", (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))), u("@jupyter-widgets/controls", "5.0.6", (() => Promise.all([_.e(345), _.e(890), _.e(67), _.e(633), _.e(495), _.e(388), _.e(61)]).then((() => () => _(2495))))), u("@jupyter-widgets/jupyterlab-manager", "5.0.8", (() => Promise.all([_.e(890), _.e(67), _.e(930), _.e(388), _.e(134)]).then((() => () => _(134))))), u("@jupyter-widgets/output", "6.0.5", (() => Promise.all([_.e(890), _.e(965)]).then((() => () => _(2965))))), u("jquery", "3.7.0", (() => _.e(291).then((() => () => _(8291))))), u("semver", "7.5.1", (() => _.e(699).then((() => () => _(7699)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        E.g.importScripts && (e = E.g.location + "");
-        var r = E.g.document;
+        _.g.importScripts && (e = _.g.location + "");
+        var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), _.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             a = t[1] ? r(t[1]) : [];
         return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
     }, a = (e, r) => {
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var n = e[a],
                 o = (typeof n)[0];
             if (a >= r.length) return "u" == o;
             var i = r[a],
-                d = (typeof i)[0];
-            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
+                u = (typeof i)[0];
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
             if ("o" != o && "u" != o && n != i) return n < i;
             a++
         }
     }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
-            var d = e[o];
-            i.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? i.pop() + " " + i.pop() : n(d))
+            var u = e[o];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : n(u))
         }
-        return u();
+        return l();
 
-        function u() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var i = 0, d = 1, u = !0;; d++, i++) {
-                var l, f, s = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !u || ("u" == s ? d > a && !n : "" == s != n);
-                if ("u" == f) {
-                    if (!u || "u" != s) return !1
-                } else if (u)
-                    if (s == f)
-                        if (d <= a) {
-                            if (l != e[d]) return !1
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > a && !n : "" == s != n);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
+                } else if (l)
+                    if (s == d)
+                        if (u <= a) {
+                            if (f != e[u]) return !1
                         } else {
-                            if (n ? l > e[d] : l < e[d]) return !1;
-                            l != e[d] && (u = !1)
+                            if (n ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (n || d <= a) return !1;
-                    u = !1, d--
+                    if (n || u <= a) return !1;
+                    l = !1, u--
                 } else {
-                    if (d <= a || f < s != n) return !1;
-                    u = !1
-                } else "s" != s && "n" != s && (u = !1, d--)
+                    if (u <= a || d < s != n) return !1;
+                    l = !1
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            var b = e[i];
+            c.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
-        var t = E.S[e];
-        if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = _.S[e];
+        if (!t || !_.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, u = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
-        var n = u(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, a)), h(e[t][n])
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
+        var n = l(e, t);
+        return o(a, n) || p(f(e, t, n, a)), h(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, c = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, p = (e, r, t, a) => {
-        "undefined" != typeof console && console.warn && console.warn(c(e, r, t, a))
-    }, h = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, a, n) {
-        var o = E.I(r);
-        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, a, n)) : e(r, E.S[r], t, a, n)
-    })(((e, r, t, a) => r && E.o(r, t) ? h(d(r, t)) : a())), g = b(((e, r, t, a) => (i(e, t), h(s(r, t, a) || p(r, e, t, a) || d(r, t))))), v = b(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), y = b(((e, r, t, a, n) => {
-        var o = r && E.o(r, t) && s(r, t, a);
+    }, p = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, b = (e, r, t, a) => {
+        p(c(e, r, t, a))
+    }, h = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, a, n) {
+        var o = _.I(r);
+        return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
+    })(((e, r, t, a) => r && _.o(r, t) ? h(u(r, t)) : a())), v = m(((e, r, t, a) => (i(e, t), h(s(r, t, a) || b(r, e, t, a) || u(r, t))))), y = m(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), j = m(((e, r, t, a, n) => {
+        var o = r && _.o(r, t) && s(r, t, a);
         return o ? h(o) : n()
-    })), j = {}, w = {
-        7193: () => y("default", "@jupyter-widgets/base", [1, 6, 0, 4], (() => Promise.all([E.e(644), E.e(306), E.e(720), E.e(526), E.e(595)]).then((() => () => E(9185))))),
-        2994: () => y("default", "jquery", [1, 3, 1, 1], (() => E.e(291).then((() => () => E(8291))))),
-        3992: () => v("default", "@lumino/widgets", [1, 1, 33, 0]),
-        1526: () => v("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        1840: () => v("default", "@lumino/signaling", [1, 1, 10, 0]),
-        8918: () => v("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        183: () => y("default", "@jupyter-widgets/base-manager", [1, 1, 0, 5], (() => Promise.all([E.e(113), E.e(150)]).then((() => () => E(6110))))),
-        2634: () => v("default", "@jupyterlab/mainmenu", [1, 3, 5, 0]),
-        2856: () => v("default", "@jupyterlab/translation", [1, 3, 5, 0]),
-        4411: () => v("default", "@jupyterlab/settingregistry", [1, 3, 5, 0]),
-        4579: () => v("default", "@jupyterlab/services", [1, 6, 5, 0]),
-        5658: () => v("default", "@lumino/properties", [1, 1, 8, 0]),
-        5923: () => v("default", "@lumino/disposable", [1, 1, 10, 0]),
-        6165: () => v("default", "@jupyterlab/notebook", [1, 3, 5, 0]),
-        7787: () => y("default", "@jupyter-widgets/output", [1, 6, 0, 4], (() => E.e(596).then((() => () => E(2965))))),
-        8097: () => g("default", "@jupyterlab/outputarea", [1, 3, 5, 0]),
-        8714: () => v("default", "@jupyterlab/logconsole", [1, 3, 5, 0]),
-        9e3: () => y("default", "semver", [1, 7, 3, 5], (() => E.e(699).then((() => () => E(7699))))),
-        9101: () => v("default", "@jupyterlab/rendermime", [1, 3, 5, 0]),
-        2720: () => v("default", "@lumino/messaging", [1, 1, 10, 0]),
-        8830: () => m("default", "jquery", (() => E.e(291).then((() => () => E(8291))))),
-        9520: () => v("default", "@lumino/domutils", [1, 1, 8, 0]),
-        2534: () => y("default", "@jupyter-widgets/controls", [1, 5, 0, 5], (() => Promise.all([E.e(345), E.e(720), E.e(495)]).then((() => () => E(2495)))))
-    }, P = {
-        99: [1840, 8918],
-        134: [183, 2634, 2856, 4411, 4579, 5658, 5923, 6165, 7787, 8097, 8714, 9e3, 9101],
-        193: [7193],
-        306: [2994, 3992],
-        495: [9520],
-        526: [1526],
+    })), w = {}, P = {
+        9890: () => j("default", "@jupyter-widgets/base", [1, 6, 0, 5], (() => Promise.all([_.e(644), _.e(67), _.e(633), _.e(930), _.e(595)]).then((() => () => _(9185))))),
+        2994: () => j("default", "jquery", [1, 3, 1, 1], (() => _.e(291).then((() => () => _(8291))))),
+        8778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
+        7930: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        4901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
+        6697: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        56: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 2]),
+        926: () => y("default", "@jupyterlab/translation", [1, 4, 0, 2]),
+        1919: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 2]),
+        3004: () => y("default", "@lumino/properties", [1, 2, 0, 0]),
+        3363: () => v("default", "@jupyterlab/outputarea", [1, 4, 0, 2]),
+        4238: () => y("default", "@jupyterlab/services", [1, 7, 0, 2]),
+        4470: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 2]),
+        4826: () => y("default", "@jupyterlab/mainmenu", [1, 4, 0, 2]),
+        7482: () => j("default", "@jupyter-widgets/base-manager", [1, 1, 0, 6], (() => Promise.all([_.e(113), _.e(336)]).then((() => () => _(6110))))),
+        7717: () => y("default", "@lumino/disposable", [1, 2, 0, 0]),
+        8409: () => j("default", "@jupyter-widgets/output", [1, 6, 0, 5], (() => _.e(596).then((() => () => _(2965))))),
+        9e3: () => j("default", "semver", [1, 7, 3, 5], (() => _.e(699).then((() => () => _(7699))))),
+        9350: () => y("default", "@jupyterlab/logconsole", [1, 4, 0, 2]),
+        5633: () => y("default", "@lumino/messaging", [1, 2, 0, 0]),
+        8830: () => g("default", "jquery", (() => _.e(291).then((() => () => _(8291))))),
+        5593: () => y("default", "@lumino/domutils", [1, 2, 0, 0]),
+        6530: () => j("default", "@jupyter-widgets/controls", [1, 5, 0, 6], (() => Promise.all([_.e(345), _.e(633), _.e(495)]).then((() => () => _(2495)))))
+    }, S = {
+        67: [2994, 8778],
+        134: [56, 926, 1919, 3004, 3363, 4238, 4470, 4826, 7482, 7717, 8409, 9e3, 9350],
+        388: [4901, 6697],
+        495: [5593],
         595: [8830],
-        720: [2720],
-        863: [2534]
-    }, E.f.consumes = (e, r) => {
-        E.o(P, e) && P[e].forEach((e => {
-            if (E.o(j, e)) return r.push(j[e]);
+        633: [5633],
+        863: [6530],
+        890: [9890],
+        930: [7930]
+    }, _.f.consumes = (e, r) => {
+        _.o(S, e) && S[e].forEach((e => {
+            if (_.o(w, e)) return r.push(w[e]);
             var t = r => {
-                    j[e] = 0, E.m[e] = t => {
-                        delete E.c[e], t.exports = r()
+                    w[e] = 0, _.m[e] = t => {
+                        delete _.c[e], t.exports = r()
                     }
                 },
                 a = r => {
-                    delete j[e], E.m[e] = t => {
-                        throw delete E.c[e], r
+                    delete w[e], _.m[e] = t => {
+                        throw delete _.c[e], r
                     }
                 };
             try {
-                var n = w[e]();
-                n.then ? r.push(j[e] = n.then(t).catch(a)) : t(n)
+                var n = P[e]();
+                n.then ? r.push(w[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
                 a(e)
             }
         }))
     }, (() => {
-        E.b = document.baseURI || self.location.href;
+        _.b = document.baseURI || self.location.href;
         var e = {
             513: 0
         };
-        E.f.j = (r, t) => {
-            var a = E.o(e, r) ? e[r] : void 0;
+        _.f.j = (r, t) => {
+            var a = _.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(193|306|526|720|863|99)$/.test(r)) e[r] = 0;
+                else if (/^(388|633|67|863|890|930)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
-                var o = E.p + E.u(r),
+                var o = _.p + _.u(r),
                     i = new Error;
-                E.l(o, (t => {
-                    if (E.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                _.l(o, (t => {
+                    if (_.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
                             o = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, n, [o, i, d] = t,
-                    u = 0;
+                var a, n, [o, i, u] = t,
+                    l = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (a in i) E.o(i, a) && (E.m[a] = i[a]);
-                    d && d(E)
+                    for (a in i) _.o(i, a) && (_.m[a] = i[a]);
+                    u && u(_)
                 }
-                for (r && r(t); u < o.length; u++) n = o[u], E.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); l < o.length; l++) n = o[l], _.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jupyter_widgets_jupyterlab_manager = self.webpackChunk_jupyter_widgets_jupyterlab_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), E.nc = void 0;
-    var _ = E(2063);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-widgets/jupyterlab-manager"] = _
+    })(), _.nc = void 0;
+    var x = _(5348);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-widgets/jupyterlab-manager"] = x
 })();
```

### Comparing `jupyterlab_widgets-3.0.7/labextension/static/third-party-licenses.json` & `jupyterlab_widgets-3.0.8/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.0.5'}, 1: {'versionInfo': '1.0.6'}, 2: {'versionInfo': "*

 * *               "'5.0.6'}, 3: {'versionInfo': '6.0.5'}, 9: {'versionInfo': '4.3.1'}, 10: "*

 * *               "{'versionInfo': '2.0.0'}, 12: {'versionInfo': '5.0.3'}, 13: {'versionInfo': "*

 * *               "'3.1.0'}, 14: {'versionInfo': '4.5.0'}, 16: {'versionInfo': '8.0.2'}, 18: "*

 * *               "{'versionInfo': '3.7.0'}, 21: {'versionInfo': '3.3.6'}, 25: {'versionInfo': "*

 * *               "'8.4.23'}, 27: {'versionInfo': […]*

```diff
@@ -1,32 +1,32 @@
 {
     "packages": [
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/base",
-            "versionInfo": "6.0.4"
+            "versionInfo": "6.0.5"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/base-manager",
-            "versionInfo": "1.0.5"
+            "versionInfo": "1.0.6"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/controls",
-            "versionInfo": "5.0.5"
+            "versionInfo": "5.0.6"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/output",
-            "versionInfo": "6.0.4"
+            "versionInfo": "6.0.5"
         },
         {
             "extractedText": "Copyright (c) 2010-2019 Jeremy Ashkenas, DocumentCloud\n\nPermission is hereby granted, free of charge, to any person\nobtaining a copy of this software and associated documentation\nfiles (the \"Software\"), to deal in the Software without\nrestriction, including without limitation the rights to use,\ncopy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the\nSoftware is furnished to do so, subject to the following\nconditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES\nOF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT\nHOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR\nOTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "backbone",
             "versionInfo": "1.4.0"
         },
@@ -54,69 +54,69 @@
             "name": "d3-format",
             "versionInfo": "3.1.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2012 James Halliday, Josh Duff, and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "deepmerge",
-            "versionInfo": "4.2.2"
+            "versionInfo": "4.3.1"
         },
         {
             "extractedText": "License\n\n(The MIT License)\n\nCopyright (c) 2014 The cheeriojs contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "dom-serializer",
-            "versionInfo": "1.4.1"
+            "versionInfo": "2.0.0"
         },
         {
             "extractedText": "Copyright (c) Felix B\u00f6hm\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\nRedistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n\nRedistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS,\nEVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-2-Clause",
             "name": "domelementtype",
             "versionInfo": "2.3.0"
         },
         {
             "extractedText": "Copyright (c) Felix B\u00f6hm\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\nRedistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n\nRedistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS,\nEVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-2-Clause",
             "name": "domhandler",
-            "versionInfo": "4.3.1"
+            "versionInfo": "5.0.3"
         },
         {
             "extractedText": "Copyright (c) Felix B\u00f6hm\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\nRedistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n\nRedistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS,\nEVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-2-Clause",
             "name": "domutils",
-            "versionInfo": "2.8.0"
+            "versionInfo": "3.1.0"
         },
         {
             "extractedText": "Copyright (c) Felix B\u00f6hm\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\nRedistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n\nRedistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS,\nEVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-2-Clause",
             "name": "entities",
-            "versionInfo": "2.2.0"
+            "versionInfo": "4.5.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Sindre Sorhus <sindresorhus@gmail.com> (https://sindresorhus.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "escape-string-regexp",
             "versionInfo": "4.0.0"
         },
         {
             "extractedText": "Copyright 2010, 2011, Chris Winberry <chris@winberry.net>. All rights reserved.\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to\ndeal in the Software without restriction, including without limitation the\nrights to use, copy, modify, merge, publish, distribute, sublicense, and/or\nsell copies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n \nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n \nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS\nIN THE SOFTWARE.",
             "licenseId": "MIT",
             "name": "htmlparser2",
-            "versionInfo": "6.1.0"
+            "versionInfo": "8.0.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-2017, Jon Schlinkert.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "is-plain-object",
             "versionInfo": "5.0.0"
         },
         {
             "extractedText": "Copyright OpenJS Foundation and other contributors, https://openjsf.org/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "jquery",
-            "versionInfo": "3.6.3"
+            "versionInfo": "3.7.0"
         },
         {
             "extractedText": "Copyright OpenJS Foundation and other contributors <https://openjsf.org/>\n\nBased on Underscore.js, copyright Jeremy Ashkenas,\nDocumentCloud and Investigative Reporters & Editors <http://underscorejs.org/>\n\nThis software consists of voluntary contributions made by many\nindividuals. For exact contribution history, see the revision history\navailable at https://github.com/lodash/lodash\n\nThe following license applies to all parts of this software except as\ndocumented below:\n\n====\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n====\n\nCopyright and related rights for sample code are waived via CC0. Sample\ncode is defined as all source code displayed within the prose of the\ndocumentation.\n\nCC0: http://creativecommons.org/publicdomain/zero/1.0/\n\n====\n\nFiles located in the node_modules and vendor directories are externally\nmaintained libraries used by this software which have their own\nlicenses; we recommend you read them, as their terms may differ from the\nterms above.\n",
             "licenseId": "MIT",
             "name": "lodash",
             "versionInfo": "4.17.21"
         },
@@ -126,15 +126,15 @@
             "name": "lru-cache",
             "versionInfo": "6.0.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright 2017 Andrey Sitnik <andrey@sitnik.ru>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of\nthe Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "nanoid",
-            "versionInfo": "3.3.4"
+            "versionInfo": "3.3.6"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2019 L\u00e9on Gersen\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "nouislider",
             "versionInfo": "15.4.0"
         },
@@ -150,39 +150,39 @@
             "name": "picocolors",
             "versionInfo": "1.0.0"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright 2013 Andrey Sitnik <andrey@sitnik.ru>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of\nthe Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "postcss",
-            "versionInfo": "8.4.21"
+            "versionInfo": "8.4.23"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "process",
             "versionInfo": "0.11.10"
         },
         {
             "extractedText": "Copyright (c) 2013, 2014, 2015 P'unk Avenue LLC\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "sanitize-html",
-            "versionInfo": "2.7.3"
+            "versionInfo": "2.10.0"
         },
         {
             "extractedText": "The ISC License\n\nCopyright (c) Isaac Z. Schlueter and Contributors\n\nPermission to use, copy, modify, and/or distribute this software for any\npurpose with or without fee is hereby granted, provided that the above\ncopyright notice and this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES\nWITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF\nMERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR\nANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES\nWHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN\nACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR\nIN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.\n",
             "licenseId": "ISC",
             "name": "semver",
-            "versionInfo": "7.3.8"
+            "versionInfo": "7.5.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "3.3.1"
+            "versionInfo": "3.3.2"
         },
         {
             "extractedText": "Copyright (c) 2009-2022 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors\n\nPermission is hereby granted, free of charge, to any person\nobtaining a copy of this software and associated documentation\nfiles (the \"Software\"), to deal in the Software without\nrestriction, including without limitation the rights to use,\ncopy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the\nSoftware is furnished to do so, subject to the following\nconditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES\nOF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT\nHOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR\nOTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "underscore",
             "versionInfo": "1.13.6"
         },
```

### Comparing `jupyterlab_widgets-3.0.7/package.json` & `jupyterlab_widgets-3.0.8/labextension/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8915476190476189%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^6.0.5', '@jupyter-widgets/base-manager': '^1.0.6', "*

 * *                   "'@jupyter-widgets/controls': '^5.0.6', '@jupyter-widgets/output': '^6.0.5', "*

 * *                   "'@jupyterlab/application': '^3.0.0 || ^4.0.0', '@jupyterlab/docregistry': "*

 * *                   "'^3.0.0 || ^4.0.0', '@jupyterlab/logconsole': '^3.0.0 || ^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.0.0 || ^4.0.0', '@jupyterlab/nbformat': '^3.0.0 || "*

 * *                   "^4.0.0', […]*

```diff
@@ -1,62 +1,69 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter-widgets/ipywidgets/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^6.0.4",
-        "@jupyter-widgets/base-manager": "^1.0.5",
-        "@jupyter-widgets/controls": "^5.0.5",
-        "@jupyter-widgets/output": "^6.0.4",
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/docregistry": "^3.0.0",
-        "@jupyterlab/logconsole": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/outputarea": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/rendermime-interfaces": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/translation": "^3.0.0",
-        "@lumino/algorithm": "^1.9.1",
-        "@lumino/coreutils": "^1.11.1",
-        "@lumino/disposable": "^1.10.1",
-        "@lumino/properties": "^1.8.1",
-        "@lumino/signaling": "^1.10.1",
-        "@lumino/widgets": "^1.30.0",
+        "@jupyter-widgets/base": "^6.0.5",
+        "@jupyter-widgets/base-manager": "^1.0.6",
+        "@jupyter-widgets/controls": "^5.0.6",
+        "@jupyter-widgets/output": "^6.0.5",
+        "@jupyterlab/application": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/docregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/logconsole": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/mainmenu": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/nbformat": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/notebook": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/outputarea": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime-interfaces": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/services": "^6.0.0 || ^7.0.0",
+        "@jupyterlab/settingregistry": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/translation": "^3.0.0 || ^4.0.0",
+        "@lumino/algorithm": "^1.11.1 || ^2.0.0",
+        "@lumino/coreutils": "^1.11.1 || ^2.1",
+        "@lumino/disposable": "^1.10.1 || ^2.1",
+        "@lumino/properties": "^1.8.1 || ^2.1",
+        "@lumino/signaling": "^1.10.1 || ^2.1",
+        "@lumino/widgets": "^1.30.0 || ^2.1",
         "@types/backbone": "1.4.14",
         "jquery": "^3.1.1",
         "semver": "^7.3.5"
     },
     "description": "The JupyterLab extension providing Jupyter widgets.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@jupyterlab/cells": "^3.0.0",
+        "@jupyterlab/builder": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/cells": "^3.0.0 || ^4.0.0",
+        "@types/jquery": "^3.5.16",
         "@types/semver": "^7.3.6",
         "@typescript-eslint/eslint-plugin": "^5.8.0",
         "@typescript-eslint/parser": "^5.8.0",
         "eslint": "^8.5.0",
         "eslint-config-prettier": "^8.3.0",
         "eslint-plugin-prettier": "^4.0.0",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.3.2",
         "rimraf": "^3.0.2",
+        "source-map-loader": "^4.0.1",
         "typescript": "~4.9.4"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "dist/*.js",
         "schema/*.json"
     ],
+    "gitHead": "5e86a96c0138b837a1b0e609f02dd79de71f5bd6",
     "homepage": "https://github.com/jupyter-widgets/ipywidgets",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.98b8a827bfc5f86e95d2.js"
+        },
         "extension": true,
         "outputDir": "labextension",
         "schemaDir": "./schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -86,9 +93,9 @@
         "prepare": "jlpm clean && jlpm build:prod",
         "watch": "jupyter labextension watch ."
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "5.0.7"
+    "version": "5.0.8"
 }
```

### Comparing `jupyterlab_widgets-3.0.7/setup.cfg` & `jupyterlab_widgets-3.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_widgets-3.0.7/setup.py` & `jupyterlab_widgets-3.0.8/setup.py`

 * *Files identical despite different names*

