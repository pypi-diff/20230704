# Comparing `tmp/pedurma-0.1.98.tar.gz` & `tmp/pedurma-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedurma-0.1.98.tar", last modified: Fri May  6 06:55:44 2022, max compression
+gzip compressed data, was "pedurma-0.1.99.tar", last modified: Thu May 12 12:25:49 2022, max compression
```

## Comparing `pedurma-0.1.98.tar` & `pedurma-0.1.99.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 06:55:44.081890 pedurma-0.1.98/
--rw-r--r--   0 root         (0) root         (0)     1064 2022-05-06 06:55:40.000000 pedurma-0.1.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)      546 2022-05-06 06:55:44.081890 pedurma-0.1.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       48 2022-05-06 06:55:40.000000 pedurma-0.1.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 06:55:44.081890 pedurma-0.1.98/pedurma/
--rw-r--r--   0 root         (0) root         (0)      338 2022-05-06 06:55:41.000000 pedurma-0.1.98/pedurma/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1395 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/config.py
--rw-r--r--   0 root         (0) root         (0)     6395 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/docx_serializer.py
--rw-r--r--   0 root         (0) root         (0)      367 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3690 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/nalanda_text.py
--rw-r--r--   0 root         (0) root         (0)     4781 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/notes.py
--rw-r--r--   0 root         (0) root         (0)     5376 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/pagination_update.py
--rw-r--r--   0 root         (0) root         (0)     1584 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/pecha.py
--rw-r--r--   0 root         (0) root         (0)    11537 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/preprocess.py
--rw-r--r--   0 root         (0) root         (0)     1629 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/preview.py
--rw-r--r--   0 root         (0) root         (0)     4766 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/preview_note_layer.py
--rw-r--r--   0 root         (0) root         (0)     1611 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/proofreading.py
--rw-r--r--   0 root         (0) root         (0)    37102 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/reconstruction.py
--rw-r--r--   0 root         (0) root         (0)      505 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/reinsertion.py
--rw-r--r--   0 root         (0) root         (0)    14163 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/save_text.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/text_report.py
--rw-r--r--   0 root         (0) root         (0)    20765 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/texts.py
--rw-r--r--   0 root         (0) root         (0)     7181 2022-05-06 06:55:40.000000 pedurma-0.1.98/pedurma/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-06 06:55:44.081890 pedurma-0.1.98/pedurma.egg-info/
--rw-r--r--   0 root         (0) root         (0)      546 2022-05-06 06:55:44.000000 pedurma-0.1.98/pedurma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      586 2022-05-06 06:55:44.000000 pedurma-0.1.98/pedurma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-06 06:55:44.000000 pedurma-0.1.98/pedurma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-05-06 06:55:44.000000 pedurma-0.1.98/pedurma.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-05-06 06:55:44.000000 pedurma-0.1.98/pedurma.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      298 2022-05-06 06:55:44.081890 pedurma-0.1.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1294 2022-05-06 06:55:40.000000 pedurma-0.1.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:25:49.326137 pedurma-0.1.99/
+-rw-r--r--   0 root         (0) root         (0)     1064 2022-05-12 12:25:46.000000 pedurma-0.1.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      546 2022-05-12 12:25:49.326137 pedurma-0.1.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       48 2022-05-12 12:25:46.000000 pedurma-0.1.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:25:49.322137 pedurma-0.1.99/pedurma/
+-rw-r--r--   0 root         (0) root         (0)      338 2022-05-12 12:25:47.000000 pedurma-0.1.99/pedurma/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/config.py
+-rw-r--r--   0 root         (0) root         (0)     6395 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/docx_serializer.py
+-rw-r--r--   0 root         (0) root         (0)      367 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/nalanda_text.py
+-rw-r--r--   0 root         (0) root         (0)     4781 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/notes.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/pagination_update.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/pecha.py
+-rw-r--r--   0 root         (0) root         (0)    11537 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/preprocess.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/preview.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/preview_note_layer.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/proofreading.py
+-rw-r--r--   0 root         (0) root         (0)    37203 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/reconstruction.py
+-rw-r--r--   0 root         (0) root         (0)      505 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/reinsertion.py
+-rw-r--r--   0 root         (0) root         (0)    14163 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/save_text.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/text_report.py
+-rw-r--r--   0 root         (0) root         (0)    20765 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/texts.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2022-05-12 12:25:46.000000 pedurma-0.1.99/pedurma/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-12 12:25:49.326137 pedurma-0.1.99/pedurma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      546 2022-05-12 12:25:49.000000 pedurma-0.1.99/pedurma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      586 2022-05-12 12:25:49.000000 pedurma-0.1.99/pedurma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-12 12:25:49.000000 pedurma-0.1.99/pedurma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-05-12 12:25:49.000000 pedurma-0.1.99/pedurma.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-05-12 12:25:49.000000 pedurma-0.1.99/pedurma.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2022-05-12 12:25:49.326137 pedurma-0.1.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-05-12 12:25:46.000000 pedurma-0.1.99/setup.py
```

### Comparing `pedurma-0.1.98/LICENSE` & `pedurma-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/PKG-INFO` & `pedurma-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedurma
-Version: 0.1.98
+Version: 0.1.99
 Summary: Pedurma Reconstruction functionalities
 Home-page: https://github.com/Esukhia/pedurma
 Author: Ngawang Thrinley, Tenzin, Tenzin Kaldan
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pedurma-0.1.98/pedurma/config.py` & `pedurma-0.1.99/pedurma/config.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/docx_serializer.py` & `pedurma-0.1.99/pedurma/docx_serializer.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/nalanda_text.py` & `pedurma-0.1.99/pedurma/nalanda_text.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/notes.py` & `pedurma-0.1.99/pedurma/notes.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/pagination_update.py` & `pedurma-0.1.99/pedurma/pagination_update.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/pecha.py` & `pedurma-0.1.99/pedurma/pecha.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/preprocess.py` & `pedurma-0.1.99/pedurma/preprocess.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/preview.py` & `pedurma-0.1.99/pedurma/preview.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/preview_note_layer.py` & `pedurma-0.1.99/pedurma/preview_note_layer.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/proofreading.py` & `pedurma-0.1.99/pedurma/proofreading.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/reconstruction.py` & `pedurma-0.1.99/pedurma/reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1048,15 +1048,18 @@
     left_context = chunks[0]
     for chunk_walker, chunk in enumerate(chunks):
         if re.search(r"\(\d+\) \<.+?\>", chunk):
             try:
                 right_context = chunks[chunk_walker + 1]
             except Exception:
                 right_context = ""
-            normalized_collated_text += get_normalized_note(chunk, right_context)
+            try:
+                normalized_collated_text += get_normalized_note(chunk, right_context)
+            except Exception:
+                normalized_collated_text += chunk
         else:
             normalized_collated_text += chunk
     return normalized_collated_text
 
 
 def get_vol_preview(dg_body, namsel_body, dg_note_text, namsel_note_text, vol_num):
     preview_text = ""
```

### Comparing `pedurma-0.1.98/pedurma/save_text.py` & `pedurma-0.1.99/pedurma/save_text.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/text_report.py` & `pedurma-0.1.99/pedurma/text_report.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/texts.py` & `pedurma-0.1.99/pedurma/texts.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma/utils.py` & `pedurma-0.1.99/pedurma/utils.py`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/pedurma.egg-info/PKG-INFO` & `pedurma-0.1.99/pedurma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedurma
-Version: 0.1.98
+Version: 0.1.99
 Summary: Pedurma Reconstruction functionalities
 Home-page: https://github.com/Esukhia/pedurma
 Author: Ngawang Thrinley, Tenzin, Tenzin Kaldan
 Author-email: esukhiadev@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pedurma-0.1.98/pedurma.egg-info/SOURCES.txt` & `pedurma-0.1.99/pedurma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedurma-0.1.98/setup.py` & `pedurma-0.1.99/setup.py`

 * *Files identical despite different names*

