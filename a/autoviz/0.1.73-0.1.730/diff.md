# Comparing `tmp/autoviz-0.1.73.tar.gz` & `tmp/autoviz-0.1.730.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.73.tar", last modified: Mon Jun  5 10:23:55 2023, max compression
+gzip compressed data, was "autoviz-0.1.730.tar", last modified: Tue Jul  4 11:05:21 2023, max compression
```

## Comparing `autoviz-0.1.73.tar` & `autoviz-0.1.730.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-05 10:23:55.126366 autoviz-0.1.73/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14488 2023-06-05 10:23:55.126366 autoviz-0.1.73/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12488 2023-06-04 21:56:05.000000 autoviz-0.1.73/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-05 10:23:54.995810 autoviz-0.1.73/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    34170 2023-06-04 16:19:08.000000 autoviz-0.1.73/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    60800 2023-05-15 13:55:02.000000 autoviz-0.1.73/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.73/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117952 2023-06-04 16:41:05.000000 autoviz-0.1.73/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      782 2023-06-04 15:27:11.000000 autoviz-0.1.73/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      403 2023-06-04 17:06:30.000000 autoviz-0.1.73/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18331 2023-06-04 15:27:51.000000 autoviz-0.1.73/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-06-05 10:23:55.110740 autoviz-0.1.73/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14488 2023-06-05 10:23:54.000000 autoviz-0.1.73/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-06-05 10:23:54.000000 autoviz-0.1.73/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-06-05 10:23:54.000000 autoviz-0.1.73/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      257 2023-06-05 10:23:54.000000 autoviz-0.1.73/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-06-05 10:23:54.000000 autoviz-0.1.73/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-06-05 10:23:55.126366 autoviz-0.1.73/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1231 2023-06-05 10:22:28.000000 autoviz-0.1.73/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-07-04 11:05:21.611830 autoviz-0.1.730/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14489 2023-07-04 11:05:21.611830 autoviz-0.1.730/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12488 2023-06-04 21:56:05.000000 autoviz-0.1.730/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-07-04 11:05:21.477299 autoviz-0.1.730/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    34170 2023-06-04 16:19:08.000000 autoviz-0.1.730/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    60831 2023-07-04 10:42:44.000000 autoviz-0.1.730/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.730/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117952 2023-06-04 16:41:05.000000 autoviz-0.1.730/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      782 2023-06-04 15:27:11.000000 autoviz-0.1.730/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-07-04 11:00:46.000000 autoviz-0.1.730/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18331 2023-06-04 15:27:51.000000 autoviz-0.1.730/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-07-04 11:05:21.589694 autoviz-0.1.730/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14489 2023-07-04 11:05:20.000000 autoviz-0.1.730/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-07-04 11:05:20.000000 autoviz-0.1.730/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-07-04 11:05:20.000000 autoviz-0.1.730/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      257 2023-07-04 11:05:20.000000 autoviz-0.1.730/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-07-04 11:05:20.000000 autoviz-0.1.730/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-07-04 11:05:21.627466 autoviz-0.1.730/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1232 2023-07-04 11:01:08.000000 autoviz-0.1.730/setup.py
```

### Comparing `autoviz-0.1.73/PKG-INFO` & `autoviz-0.1.730/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.73
+Version: 0.1.730
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.73 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.730 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz Author: Ram Seshadri License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can save
 these interactive charts as HTML files automatically with the `html` setting.
 [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/
```

### Comparing `autoviz-0.1.73/README.md` & `autoviz-0.1.730/README.md`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz/AutoViz_Class.py` & `autoviz-0.1.730/autoviz/AutoViz_Class.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz/AutoViz_Holo.py` & `autoviz-0.1.730/autoviz/AutoViz_Holo.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,14 +665,15 @@
                 dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
                 ###########  This is where you put the Panel Together ############
                 hv_panel = pn.panel(dmap)
                 widgets = hv_panel[0]
                 hv_all = pn.Column(pn.Row(*widgets))
             except:
                 print('Error in Distribution Plot')
+                hv_panel = []
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
         if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
             #server = pn.serve(hv_all, start=True, show=True)
             print('%s can be found in URL below:' %plot_name)
             hv_all.show()
```

### Comparing `autoviz-0.1.73/autoviz/AutoViz_NLP.py` & `autoviz-0.1.730/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz/AutoViz_Utils.py` & `autoviz-0.1.730/autoviz/AutoViz_Utils.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz/__init__.py` & `autoviz-0.1.730/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz/classify_method.py` & `autoviz-0.1.730/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.73/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.730/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.73
+Version: 0.1.730
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.73 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.730 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz Author: Ram Seshadri License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can save
 these interactive charts as HTML files automatically with the `html` setting.
 [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/
```

### Comparing `autoviz-0.1.73/setup.py` & `autoviz-0.1.730/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.73",
+    version="0.1.730",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
```

