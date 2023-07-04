# Comparing `tmp/arxiv_latex_cleaner-1.0.0.tar.gz` & `tmp/arxiv_latex_cleaner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv_latex_cleaner-1.0.0.tar", last modified: Tue Jul  4 08:23:06 2023, max compression
+gzip compressed data, was "arxiv_latex_cleaner-1.0.1.tar", last modified: Tue Jul  4 08:25:40 2023, max compression
```

## Comparing `arxiv_latex_cleaner-1.0.0.tar` & `arxiv_latex_cleaner-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:23:06.348103 arxiv_latex_cleaner-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-04 08:23:06.348103 arxiv_latex_cleaner-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:23:06.344103 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22323 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/arxiv_latex_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:23:06.348103 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:23:06.000000 arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:23:06.348103 arxiv_latex_cleaner-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-04 08:22:50.000000 arxiv_latex_cleaner-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:25:40.633304 arxiv_latex_cleaner-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-04 08:25:40.633304 arxiv_latex_cleaner-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:25:40.633304 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22323 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/arxiv_latex_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:25:40.633304 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:25:40.000000 arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:25:40.633304 arxiv_latex_cleaner-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-04 08:25:31.000000 arxiv_latex_cleaner-1.0.1/setup.py
```

### Comparing `arxiv_latex_cleaner-1.0.0/LICENSE` & `arxiv_latex_cleaner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-1.0.0/PKG-INFO` & `arxiv_latex_cleaner-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv_latex_cleaner
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cleans the LaTeX code of your paper to submit to arXiv.
 Home-page: https://github.com/google-research/arxiv-latex-cleaner
 Author: Google Research Authors
 Author-email: jponttuset@gmail.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
@@ -130,15 +130,15 @@
 copied, making sure all figure files are copied to the cleaned version. See also
 [cleaner_config.yaml](cleaner_config.yaml) for details on how to specify the
 patterns.
 
 ## Usage:
 
 ```
-usage: arxiv_latex_cleaner@v0.1.30 [-h] [--resize_images] [--im_size IM_SIZE]
+usage: arxiv_latex_cleaner@v1.0.1 [-h] [--resize_images] [--im_size IM_SIZE]
                                    [--compress_pdf]
                                    [--pdf_im_resolution PDF_IM_RESOLUTION]
                                    [--images_allowlist IMAGES_ALLOWLIST]
                                    [--keep_bib]
                                    [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                    [--use_external_tikz USE_EXTERNAL_TIKZ]
                                    [--config CONFIG] [--verbose]
```

### Comparing `arxiv_latex_cleaner-1.0.0/README.md` & `arxiv_latex_cleaner-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 copied, making sure all figure files are copied to the cleaned version. See also
 [cleaner_config.yaml](cleaner_config.yaml) for details on how to specify the
 patterns.
 
 ## Usage:
 
 ```
-usage: arxiv_latex_cleaner@v0.1.30 [-h] [--resize_images] [--im_size IM_SIZE]
+usage: arxiv_latex_cleaner@v1.0.1 [-h] [--resize_images] [--im_size IM_SIZE]
                                    [--compress_pdf]
                                    [--pdf_im_resolution PDF_IM_RESOLUTION]
                                    [--images_allowlist IMAGES_ALLOWLIST]
                                    [--keep_bib]
                                    [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                    [--use_external_tikz USE_EXTERNAL_TIKZ]
                                    [--config CONFIG] [--verbose]
```

### Comparing `arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/__init__.py` & `arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/__main__.py` & `arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/__main__.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/_version.py` & `arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "v1.0.0"
+__version__ = "v1.0.1"
```

### Comparing `arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner/arxiv_latex_cleaner.py` & `arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner/arxiv_latex_cleaner.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-1.0.0/arxiv_latex_cleaner.egg-info/PKG-INFO` & `arxiv_latex_cleaner-1.0.1/arxiv_latex_cleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-latex-cleaner
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cleans the LaTeX code of your paper to submit to arXiv.
 Home-page: https://github.com/google-research/arxiv-latex-cleaner
 Author: Google Research Authors
 Author-email: jponttuset@gmail.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
@@ -130,15 +130,15 @@
 copied, making sure all figure files are copied to the cleaned version. See also
 [cleaner_config.yaml](cleaner_config.yaml) for details on how to specify the
 patterns.
 
 ## Usage:
 
 ```
-usage: arxiv_latex_cleaner@v0.1.30 [-h] [--resize_images] [--im_size IM_SIZE]
+usage: arxiv_latex_cleaner@v1.0.1 [-h] [--resize_images] [--im_size IM_SIZE]
                                    [--compress_pdf]
                                    [--pdf_im_resolution PDF_IM_RESOLUTION]
                                    [--images_allowlist IMAGES_ALLOWLIST]
                                    [--keep_bib]
                                    [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                    [--use_external_tikz USE_EXTERNAL_TIKZ]
                                    [--config CONFIG] [--verbose]
```

### Comparing `arxiv_latex_cleaner-1.0.0/setup.py` & `arxiv_latex_cleaner-1.0.1/setup.py`

 * *Files identical despite different names*

