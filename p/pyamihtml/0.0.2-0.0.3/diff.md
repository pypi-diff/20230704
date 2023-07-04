# Comparing `tmp/pyamihtml-0.0.2.tar.gz` & `tmp/pyamihtml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyamihtml-0.0.2.tar", last modified: Tue Jul  4 08:29:10 2023, max compression
+gzip compressed data, was "dist/pyamihtml-0.0.3.tar", last modified: Tue Jul  4 09:55:25 2023, max compression
```

## Comparing `pyamihtml-0.0.2.tar` & `pyamihtml-0.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 08:29:10.164841 pyamihtml-0.0.2/
--rw-r--r--   0 pm286      (503) staff       (20)     5420 2022-09-21 21:52:33.000000 pyamihtml-0.0.2/CONFIG.md
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2021-08-20 16:43:32.000000 pyamihtml-0.0.2/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      159 2022-09-21 21:52:33.000000 pyamihtml-0.0.2/MANIFEST.in
--rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 08:29:10.164727 pyamihtml-0.0.2/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)     8963 2023-05-24 09:30:50.000000 pyamihtml-0.0.2/README.md
--rw-r--r--   0 pm286      (503) staff       (20)     1800 2021-09-04 09:10:40.000000 pyamihtml-0.0.2/config.ini.master
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 08:29:10.159155 pyamihtml-0.0.2/pyamihtml/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2021-08-20 16:43:32.000000 pyamihtml-0.0.2/pyamihtml/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5168 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)    10020 2023-07-03 08:18:38.000000 pyamihtml-0.0.2/pyamihtml/ami_config.py
--rw-r--r--   0 pm286      (503) staff       (20)   156540 2023-07-01 22:53:26.000000 pyamihtml-0.0.2/pyamihtml/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    10529 2023-07-01 20:43:25.000000 pyamihtml-0.0.2/pyamihtml/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     1734 2023-07-03 12:48:26.000000 pyamihtml-0.0.2/pyamihtml/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)   103045 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/ami_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     3192 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10585 2023-06-27 08:49:50.000000 pyamihtml-0.0.2/pyamihtml/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    19684 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/bbox_copy.py
--rw-r--r--   0 pm286      (503) staff       (20)    15305 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    52982 2023-07-01 19:02:25.000000 pyamihtml-0.0.2/pyamihtml/ipcc.py
--rw-r--r--   0 pm286      (503) staff       (20)    44047 2023-07-04 08:28:27.000000 pyamihtml-0.0.2/pyamihtml/pyamix.py
--rw-r--r--   0 pm286      (503) staff       (20)    25940 2023-07-01 12:42:42.000000 pyamihtml-0.0.2/pyamihtml/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33890 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    27429 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/pyamihtml/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 08:29:10.160255 pyamihtml-0.0.2/pyamihtml.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      942 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       53 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-06-30 07:44:44.000000 pyamihtml-0.0.2/pyamihtml.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)       51 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)       10 2023-07-04 08:29:10.000000 pyamihtml-0.0.2/pyamihtml.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)      511 2023-01-08 16:25:37.000000 pyamihtml-0.0.2/requirements.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2023-07-04 08:29:10.164875 pyamihtml-0.0.2/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     2260 2023-07-04 08:28:27.000000 pyamihtml-0.0.2/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 08:29:10.164467 pyamihtml-0.0.2/test/
--rw-r--r--   0 pm286      (503) staff       (20)     7530 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)      775 2022-10-29 09:43:23.000000 pyamihtml-0.0.2/test/test_experiment.py
--rw-r--r--   0 pm286      (503) staff       (20)     4194 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)     8874 2021-11-24 22:01:19.000000 pyamihtml-0.0.2/test/test_gui.py
--rw-r--r--   0 pm286      (503) staff       (20)   106191 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    14315 2023-07-03 18:38:37.000000 pyamihtml-0.0.2/test/test_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-01 20:28:05.000000 pyamihtml-0.0.2/test/test_ipcc.py
--rw-r--r--   0 pm286      (503) staff       (20)      439 2023-07-01 20:50:25.000000 pyamihtml-0.0.2/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    79214 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     8530 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_pyamix.py
--rw-r--r--   0 pm286      (503) staff       (20)     1071 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)      299 2022-08-26 08:16:11.000000 pyamihtml-0.0.2/test/test_text.py
--rw-r--r--   0 pm286      (503) staff       (20)     7591 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    34807 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)      663 2023-06-30 07:32:29.000000 pyamihtml-0.0.2/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 09:55:25.450094 pyamihtml-0.0.3/
+-rw-r--r--   0 pm286      (503) staff       (20)     5420 2022-09-21 21:52:33.000000 pyamihtml-0.0.3/CONFIG.md
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2021-08-20 16:43:32.000000 pyamihtml-0.0.3/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      159 2022-09-21 21:52:33.000000 pyamihtml-0.0.3/MANIFEST.in
+-rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 09:55:25.449941 pyamihtml-0.0.3/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)     8963 2023-05-24 09:30:50.000000 pyamihtml-0.0.3/README.md
+-rw-r--r--   0 pm286      (503) staff       (20)     1800 2021-09-04 09:10:40.000000 pyamihtml-0.0.3/config.ini.master
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 09:55:25.447388 pyamihtml-0.0.3/pyamihtml/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2021-08-20 16:43:32.000000 pyamihtml-0.0.3/pyamihtml/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5168 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10020 2023-07-03 08:18:38.000000 pyamihtml-0.0.3/pyamihtml/ami_config.py
+-rw-r--r--   0 pm286      (503) staff       (20)   156540 2023-07-01 22:53:26.000000 pyamihtml-0.0.3/pyamihtml/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10529 2023-07-01 20:43:25.000000 pyamihtml-0.0.3/pyamihtml/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     2516 2023-07-04 08:55:36.000000 pyamihtml-0.0.3/pyamihtml/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)   103045 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/ami_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3192 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10585 2023-06-27 08:49:50.000000 pyamihtml-0.0.3/pyamihtml/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19684 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/bbox_copy.py
+-rw-r--r--   0 pm286      (503) staff       (20)    15305 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    52982 2023-07-01 19:02:25.000000 pyamihtml-0.0.3/pyamihtml/ipcc.py
+-rw-r--r--   0 pm286      (503) staff       (20)    44047 2023-07-04 09:54:59.000000 pyamihtml-0.0.3/pyamihtml/pyamix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    25940 2023-07-01 12:42:42.000000 pyamihtml-0.0.3/pyamihtml/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33890 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27429 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/pyamihtml/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 09:55:25.448154 pyamihtml-0.0.3/pyamihtml.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)     9708 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      942 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       53 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-06-30 07:44:44.000000 pyamihtml-0.0.3/pyamihtml.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)       57 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       10 2023-07-04 09:55:25.000000 pyamihtml-0.0.3/pyamihtml.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)      511 2023-01-08 16:25:37.000000 pyamihtml-0.0.3/requirements.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2023-07-04 09:55:25.450132 pyamihtml-0.0.3/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     2271 2023-07-04 09:54:39.000000 pyamihtml-0.0.3/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2023-07-04 09:55:25.449768 pyamihtml-0.0.3/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     7530 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)      775 2022-10-29 09:43:23.000000 pyamihtml-0.0.3/test/test_experiment.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4194 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8874 2021-11-24 22:01:19.000000 pyamihtml-0.0.3/test/test_gui.py
+-rw-r--r--   0 pm286      (503) staff       (20)   106191 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    13720 2023-07-04 08:59:56.000000 pyamihtml-0.0.3/test/test_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2023-07-01 20:28:05.000000 pyamihtml-0.0.3/test/test_ipcc.py
+-rw-r--r--   0 pm286      (503) staff       (20)      439 2023-07-01 20:50:25.000000 pyamihtml-0.0.3/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    79214 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8530 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_pyamix.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1071 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)      299 2022-08-26 08:16:11.000000 pyamihtml-0.0.3/test/test_text.py
+-rw-r--r--   0 pm286      (503) staff       (20)     7591 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    34807 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)      663 2023-06-30 07:32:29.000000 pyamihtml-0.0.3/test/test_xml.py
```

### Comparing `pyamihtml-0.0.2/CONFIG.md` & `pyamihtml-0.0.3/CONFIG.md`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/LICENSE` & `pyamihtml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/PKG-INFO` & `pyamihtml-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamihtml
-Version: 0.0.2
+Version: 0.0.3
 Summary: pdf2html converter
 Home-page: https://github.com/petermr/pyamihtml
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Platform: UNKNOWN
```

### Comparing `pyamihtml-0.0.2/README.md` & `pyamihtml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/config.ini.master` & `pyamihtml-0.0.3/config.ini.master`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_bib.py` & `pyamihtml-0.0.3/pyamihtml/ami_bib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_config.py` & `pyamihtml-0.0.3/pyamihtml/ami_config.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_html.py` & `pyamihtml-0.0.3/pyamihtml/ami_html.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_integrate.py` & `pyamihtml-0.0.3/pyamihtml/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_pdf.py` & `pyamihtml-0.0.3/pyamihtml/ami_pdf.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_svg.py` & `pyamihtml-0.0.3/pyamihtml/ami_svg.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ami_util.py` & `pyamihtml-0.0.3/pyamihtml/ami_util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/bbox_copy.py` & `pyamihtml-0.0.3/pyamihtml/bbox_copy.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/file_lib.py` & `pyamihtml-0.0.3/pyamihtml/file_lib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/ipcc.py` & `pyamihtml-0.0.3/pyamihtml/ipcc.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/pyamix.py` & `pyamihtml-0.0.3/pyamihtml/pyamix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1129,15 +1129,15 @@
 
     def version(self):
         """
         reads setup.py and extracts line of form version='0.0.29'
         This is still a mess. We need to set the version once somewhere.
         """
 
-        version = '0.0.2' # 2023-07-03
+        version = '0.0.3' # 2023-07-03
         if False: # this fails - it gets the python distrib
             with open(Path(Path(__file__).parent.parent, "setup.py"), "r") as f:
                 setup_lines = f.readlines()
                 for line in setup_lines:
                     match = re.match("\s*version\s*=\s*\'\s*(\d+\.\d+\.\d+)\s*\'\s*,", line)
                     if match:
                         version = match.group(1)
```

### Comparing `pyamihtml-0.0.2/pyamihtml/util.py` & `pyamihtml-0.0.3/pyamihtml/util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/wikimedia.py` & `pyamihtml-0.0.3/pyamihtml/wikimedia.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml/xml_lib.py` & `pyamihtml-0.0.3/pyamihtml/xml_lib.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/pyamihtml.egg-info/PKG-INFO` & `pyamihtml-0.0.3/pyamihtml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyamihtml
-Version: 0.0.2
+Version: 0.0.3
 Summary: pdf2html converter
 Home-page: https://github.com/petermr/pyamihtml
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Platform: UNKNOWN
```

### Comparing `pyamihtml-0.0.2/pyamihtml.egg-info/SOURCES.txt` & `pyamihtml-0.0.3/pyamihtml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/setup.py` & `pyamihtml-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
  # 'future~=0.18.2',
  'pdfplumber',
  # 'requests~=2.27.1',
  'requests',
  # 'pip~=22.2.2',
  # 'pip',
+  'pyvis',
 # 'configparser~=5.0.2',
  #'zlib-state~=1.2.11',
  # 'wheel~=0.35.1',
  # 'openssl-python',
  # 'cryptography~=37.0.2',
  # 'py~=1.9.0',
  # 'keyring~=21.4.0',
@@ -52,15 +53,15 @@
  #'backports',
 
 ]
 
 setup(
     name='pyamihtml',
     url='https://github.com/petermr/pyamihtml',
-    version='0.0.2',
+    version='0.0.3',
     description='pdf2html converter',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `pyamihtml-0.0.2/test/test_all.py` & `pyamihtml-0.0.3/test/test_all.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_experiment.py` & `pyamihtml-0.0.3/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_file.py` & `pyamihtml-0.0.3/test/test_file.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_gui.py` & `pyamihtml-0.0.3/test/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_html.py` & `pyamihtml-0.0.3/test/test_html.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_integrate.py` & `pyamihtml-0.0.3/test/test_integrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -334,26 +334,12 @@
         pyami.run_command(args)
 
     def test_tfidf_on_glossaries(self):
         """
 
         """
         for report in REPORTS:
-            path = Path(AR6_DIR, report, "annexes", "html", "glossary", "links.csv")
-            self.find_text_similarities(path, maxt=1000)
+            csv_path = Path(AR6_DIR, report, "annexes", "html", "glossary", "links.csv")
+            if not(csv_path.exists()):
+                logger.error(f"file does not exist {csv_path}")
+            AmiNLP.find_text_similarities(csv_path, maxt=1000, min_sim=0.25)
 
-    def find_text_similarities(self, path, maxt=10000, min_sim=0.25):
-        print(f"============{path}=============")
-        data = pd.read_csv(str(path))
-        print(f"data before drop {len(data)}")
-        data.drop_duplicates(inplace=True, subset=["a_text"])
-        print(f"data after drop {len(data)}")
-
-        data = data[~str(data['a_text']).str.contains('See |see ')]
-        data = data[~str(data['t_text']).str.contains('See |see ')]
-        a_text = data.get("a_text")
-        a_id= data.get("a_id")
-        # a_id = [ai.lower() for ai in set(table.get("a_id"))]
-        ami_nlp = AmiNLP()
-        simmat = ami_nlp.find_similarities(a_text, maxt=maxt, min_sim=min_sim)
-
-# ski-kit learn pairwise distances
```

### Comparing `pyamihtml-0.0.2/test/test_pdf.py` & `pyamihtml-0.0.3/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_pyamix.py` & `pyamihtml-0.0.3/test/test_pyamix.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_svg.py` & `pyamihtml-0.0.3/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_util.py` & `pyamihtml-0.0.3/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_wikidata.py` & `pyamihtml-0.0.3/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `pyamihtml-0.0.2/test/test_xml.py` & `pyamihtml-0.0.3/test/test_xml.py`

 * *Files identical despite different names*

