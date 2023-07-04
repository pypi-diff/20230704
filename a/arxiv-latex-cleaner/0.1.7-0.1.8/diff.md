# Comparing `tmp/arxiv_latex_cleaner-0.1.7.tar.gz` & `tmp/arxiv_latex_cleaner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arxiv_latex_cleaner-0.1.7.tar", last modified: Sun Aug  2 18:16:38 2020, max compression
+gzip compressed data, was "dist/arxiv_latex_cleaner-0.1.8.tar", last modified: Mon Aug  3 05:21:56 2020, max compression
```

## Comparing `arxiv_latex_cleaner-0.1.7.tar` & `arxiv_latex_cleaner-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 18:16:38.327220 arxiv_latex_cleaner-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (116)    11358 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6038 2020-08-02 18:16:38.327220 arxiv_latex_cleaner-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4635 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 18:16:38.323220 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/
--rw-r--r--   0 runner    (1001) docker     (116)      607 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2602 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      631 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)    14002 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/arxiv_latex_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-02 18:16:38.323220 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6038 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      454 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       29 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2020-08-02 18:16:38.000000 arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       29 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-02 18:16:38.327220 arxiv_latex_cleaner-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1797 2020-08-02 18:16:30.000000 arxiv_latex_cleaner-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 05:21:56.918133 arxiv_latex_cleaner-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (116)    11358 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     6280 2020-08-03 05:21:56.918133 arxiv_latex_cleaner-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4832 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 05:21:56.914133 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/
+-rw-r--r--   0 runner    (1001) docker     (116)      607 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2602 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      631 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14002 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/arxiv_latex_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-03 05:21:56.914133 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     6280 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      454 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       79 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2020-08-03 05:21:56.000000 arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-03 05:21:56.918133 arxiv_latex_cleaner-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1824 2020-08-03 05:21:47.000000 arxiv_latex_cleaner-0.1.8/setup.py
```

### Comparing `arxiv_latex_cleaner-0.1.7/LICENSE` & `arxiv_latex_cleaner-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-0.1.7/PKG-INFO` & `arxiv_latex_cleaner-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv_latex_cleaner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cleans the LaTeX code of your paper to submit to arXiv.
 Home-page: https://github.com/google-research/arxiv-latex-cleaner
 Author: Google Research Authors
 Author-email: jponttuset@gmail.com
 License: Apache License, Version 2.0
 Description: # `arxiv_latex_cleaner`
         
@@ -21,14 +21,17 @@
         
         ## Installation:
         
         ```console
         pip install arxiv-latex-cleaner
         ```
         
+        | :exclamation:  arxiv_latex_cleaner is only compatible with Python >=3  :exclamation: |
+        |--------------------------------------------------------------------------------------|
+        
         Alternatively, you can download the source code:
         
         ```console
         git clone https://github.com/google-research/arxiv-latex-cleaner
         cd arxiv-latex-cleaner/
         python -m arxiv_latex_cleaner --help
         ```
@@ -42,21 +45,21 @@
         ## Main features:
         
         #### Privacy-oriented
         
         *   Removes all auxiliary files (`.aux`, `.log`, `.out`, etc.).
         *   Removes all comments from your code (yes, those are visible on arXiv and you
             do not want them to be). These also include `\begin{comment}\end{comment}`
-            environments.
+            and `\iffalse\fi` environments.
         *   Optionally removes user-defined commands entered with `commands_to_delete`
-            (such as `\todo{}` that you at the end redefine as the empty string).
+            (such as `\todo{}` that you redefine as the empty string at the end).
         
         #### Size-oriented
         
-        There is a 10MB limit on arXiv submissions, so to make it fit:
+        There is a 50MB limit on arXiv submissions, so to make it fit:
         
         *   Removes all unused `.tex` files (those that are not in the root and not
             included in any other `.tex` file).
         *   Removes all unused images that take up space (those that are not actually
             included in any used `.tex` file).
         *   Optionally resizes all images to `im_size` pixels, to reduce the size of the
             submission. You can whitelist some images to skip the global size using
@@ -77,15 +80,15 @@
         *   Only replaces environments with preceding `\tikzsetnextfilename{picture_name}` command
             (as in `\tikzsetnextfilename{picture_name}\begin{tikzpicture} ... \end{tikzpicture}`) where
             the externalized `picture_name.pdf` filename matches `picture_name`.
         
         ## Usage:
         
         ```
-        usage: arxiv_latex_cleaner@v0.1.4 [-h] [--resize_images] [--im_size IM_SIZE]
+        usage: arxiv_latex_cleaner@v0.1.8 [-h] [--resize_images] [--im_size IM_SIZE]
                                           [--compress_pdf]
                                           [--pdf_im_resolution PDF_IM_RESOLUTION]
                                           [--images_whitelist IMAGES_WHITELIST]
                                           [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                           input_folder
         
         Clean the LaTeX code of your paper to submit to arXiv. Check the README for
@@ -121,8 +124,9 @@
         ## Note
         
         This is not an officially supported Google product.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `arxiv_latex_cleaner-0.1.7/README.md` & `arxiv_latex_cleaner-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 ## Installation:
 
 ```console
 pip install arxiv-latex-cleaner
 ```
 
+| :exclamation:  arxiv_latex_cleaner is only compatible with Python >=3  :exclamation: |
+|--------------------------------------------------------------------------------------|
+
 Alternatively, you can download the source code:
 
 ```console
 git clone https://github.com/google-research/arxiv-latex-cleaner
 cd arxiv-latex-cleaner/
 python -m arxiv_latex_cleaner --help
 ```
@@ -34,21 +37,21 @@
 ## Main features:
 
 #### Privacy-oriented
 
 *   Removes all auxiliary files (`.aux`, `.log`, `.out`, etc.).
 *   Removes all comments from your code (yes, those are visible on arXiv and you
     do not want them to be). These also include `\begin{comment}\end{comment}`
-    environments.
+    and `\iffalse\fi` environments.
 *   Optionally removes user-defined commands entered with `commands_to_delete`
-    (such as `\todo{}` that you at the end redefine as the empty string).
+    (such as `\todo{}` that you redefine as the empty string at the end).
 
 #### Size-oriented
 
-There is a 10MB limit on arXiv submissions, so to make it fit:
+There is a 50MB limit on arXiv submissions, so to make it fit:
 
 *   Removes all unused `.tex` files (those that are not in the root and not
     included in any other `.tex` file).
 *   Removes all unused images that take up space (those that are not actually
     included in any used `.tex` file).
 *   Optionally resizes all images to `im_size` pixels, to reduce the size of the
     submission. You can whitelist some images to skip the global size using
@@ -69,15 +72,15 @@
 *   Only replaces environments with preceding `\tikzsetnextfilename{picture_name}` command
     (as in `\tikzsetnextfilename{picture_name}\begin{tikzpicture} ... \end{tikzpicture}`) where
     the externalized `picture_name.pdf` filename matches `picture_name`.
 
 ## Usage:
 
 ```
-usage: arxiv_latex_cleaner@v0.1.4 [-h] [--resize_images] [--im_size IM_SIZE]
+usage: arxiv_latex_cleaner@v0.1.8 [-h] [--resize_images] [--im_size IM_SIZE]
                                   [--compress_pdf]
                                   [--pdf_im_resolution PDF_IM_RESOLUTION]
                                   [--images_whitelist IMAGES_WHITELIST]
                                   [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                   input_folder
 
 Clean the LaTeX code of your paper to submit to arXiv. Check the README for
```

### Comparing `arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/__init__.py` & `arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/__main__.py` & `arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/__main__.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/_version.py` & `arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "v0.1.7"
+__version__ = "v0.1.8"
```

### Comparing `arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner/arxiv_latex_cleaner.py` & `arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner/arxiv_latex_cleaner.py`

 * *Files identical despite different names*

### Comparing `arxiv_latex_cleaner-0.1.7/arxiv_latex_cleaner.egg-info/PKG-INFO` & `arxiv_latex_cleaner-0.1.8/arxiv_latex_cleaner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-latex-cleaner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cleans the LaTeX code of your paper to submit to arXiv.
 Home-page: https://github.com/google-research/arxiv-latex-cleaner
 Author: Google Research Authors
 Author-email: jponttuset@gmail.com
 License: Apache License, Version 2.0
 Description: # `arxiv_latex_cleaner`
         
@@ -21,14 +21,17 @@
         
         ## Installation:
         
         ```console
         pip install arxiv-latex-cleaner
         ```
         
+        | :exclamation:  arxiv_latex_cleaner is only compatible with Python >=3  :exclamation: |
+        |--------------------------------------------------------------------------------------|
+        
         Alternatively, you can download the source code:
         
         ```console
         git clone https://github.com/google-research/arxiv-latex-cleaner
         cd arxiv-latex-cleaner/
         python -m arxiv_latex_cleaner --help
         ```
@@ -42,21 +45,21 @@
         ## Main features:
         
         #### Privacy-oriented
         
         *   Removes all auxiliary files (`.aux`, `.log`, `.out`, etc.).
         *   Removes all comments from your code (yes, those are visible on arXiv and you
             do not want them to be). These also include `\begin{comment}\end{comment}`
-            environments.
+            and `\iffalse\fi` environments.
         *   Optionally removes user-defined commands entered with `commands_to_delete`
-            (such as `\todo{}` that you at the end redefine as the empty string).
+            (such as `\todo{}` that you redefine as the empty string at the end).
         
         #### Size-oriented
         
-        There is a 10MB limit on arXiv submissions, so to make it fit:
+        There is a 50MB limit on arXiv submissions, so to make it fit:
         
         *   Removes all unused `.tex` files (those that are not in the root and not
             included in any other `.tex` file).
         *   Removes all unused images that take up space (those that are not actually
             included in any used `.tex` file).
         *   Optionally resizes all images to `im_size` pixels, to reduce the size of the
             submission. You can whitelist some images to skip the global size using
@@ -77,15 +80,15 @@
         *   Only replaces environments with preceding `\tikzsetnextfilename{picture_name}` command
             (as in `\tikzsetnextfilename{picture_name}\begin{tikzpicture} ... \end{tikzpicture}`) where
             the externalized `picture_name.pdf` filename matches `picture_name`.
         
         ## Usage:
         
         ```
-        usage: arxiv_latex_cleaner@v0.1.4 [-h] [--resize_images] [--im_size IM_SIZE]
+        usage: arxiv_latex_cleaner@v0.1.8 [-h] [--resize_images] [--im_size IM_SIZE]
                                           [--compress_pdf]
                                           [--pdf_im_resolution PDF_IM_RESOLUTION]
                                           [--images_whitelist IMAGES_WHITELIST]
                                           [--commands_to_delete COMMANDS_TO_DELETE [COMMANDS_TO_DELETE ...]]
                                           input_folder
         
         Clean the LaTeX code of your paper to submit to arXiv. Check the README for
@@ -121,8 +124,9 @@
         ## Note
         
         This is not an officially supported Google product.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `arxiv_latex_cleaner-0.1.7/setup.py` & `arxiv_latex_cleaner-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         if l_c and not l_c.startswith('#'):
             install_requires.append(l_c)
 
 setup(
     name="arxiv_latex_cleaner",
     version=__version__,
     packages=find_packages(exclude=["*.tests"]),
+    python_requires='>=3',
     url="https://github.com/google-research/arxiv-latex-cleaner",
     license="Apache License, Version 2.0",
     author="Google Research Authors",
     author_email="jponttuset@gmail.com",
     description="Cleans the LaTeX code of your paper to submit to arXiv.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

