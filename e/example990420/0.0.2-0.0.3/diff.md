# Comparing `tmp/example990420-0.0.2.tar.gz` & `tmp/example990420-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-0.0.2.tar", last modified: Tue Jul  4 05:56:16 2023, max compression
+gzip compressed data, was "example990420-0.0.3.tar", last modified: Tue Jul  4 07:29:29 2023, max compression
```

## Comparing `example990420-0.0.2.tar` & `example990420-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:56:16.606520 example990420-0.0.2/
--rw-rw-rw-   0        0        0    11000 2023-07-04 05:56:16.605624 example990420-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 example990420-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 05:56:16.596547 example990420-0.0.2/example990420.egg-info/
--rw-rw-rw-   0        0        0    11000 2023-07-04 05:56:16.000000 example990420-0.0.2/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-04 05:56:16.000000 example990420-0.0.2/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:56:16.000000 example990420-0.0.2/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 05:56:16.000000 example990420-0.0.2/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 05:56:16.606520 example990420-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-07-04 05:56:14.000000 example990420-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:56:16.601535 example990420-0.0.2/taibun/
--rw-rw-rw-   0        0        0       20 2023-06-15 08:41:22.000000 example990420-0.0.2/taibun/__init__.py
--rw-rw-rw-   0        0        0    19874 2023-07-04 01:32:21.000000 example990420-0.0.2/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:29:29.862215 example990420-0.0.3/
+-rw-rw-rw-   0        0        0    11079 2023-07-04 07:29:29.859844 example990420-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 example990420-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 07:29:29.842918 example990420-0.0.3/example990420.egg-info/
+-rw-rw-rw-   0        0        0    11079 2023-07-04 07:29:29.000000 example990420-0.0.3/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-04 07:29:29.000000 example990420-0.0.3/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:29:29.000000 example990420-0.0.3/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 07:29:29.000000 example990420-0.0.3/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:29:29.863212 example990420-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2023-07-04 07:25:42.000000 example990420-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:29:29.853815 example990420-0.0.3/taibun/
+-rw-rw-rw-   0        0        0       46 2023-07-04 06:23:16.000000 example990420-0.0.3/taibun/__init__.py
+-rw-rw-rw-   0        0        0    19874 2023-07-04 01:32:21.000000 example990420-0.0.3/taibun/taibun.py
```

### Comparing `example990420-0.0.2/PKG-INFO` & `example990420-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert Chinese characters to Taiwanese
+Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
-Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization
-Classifier: Development Status :: 1 - Planning
+License: MIT
+Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.2 Summary: Convert
-Chinese characters to Taiwanese Author: Andrei Harbachov Author-email:
-harbachov@gmail.com> Keywords:
-python,taiwan,taiwanese,taigi,hokkien,romanization Classifier: Development
-Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.3 Summary: Convert
+Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
+Author: Andrei Harbachov Author-email:
+harbachov@gmail.com> License: MIT Keywords:
+python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
+System :: Microsoft :: Windows Description-Content-Type: text/markdown
    # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
     [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
   **Taiwanese Hokkien transliterator from Chinese characters** It has methods
 that allow to customise transliteration and retrieve any necessary information
                     about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
```

### Comparing `example990420-0.0.2/README.md` & `example990420-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `example990420-0.0.2/example990420.egg-info/PKG-INFO` & `example990420-0.0.3/example990420.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert Chinese characters to Taiwanese
+Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
-Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization
-Classifier: Development Status :: 1 - Planning
+License: MIT
+Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.2 Summary: Convert
-Chinese characters to Taiwanese Author: Andrei Harbachov Author-email:
-harbachov@gmail.com> Keywords:
-python,taiwan,taiwanese,taigi,hokkien,romanization Classifier: Development
-Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.3 Summary: Convert
+Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
+Author: Andrei Harbachov Author-email:
+harbachov@gmail.com> License: MIT Keywords:
+python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
+System :: Microsoft :: Windows Description-Content-Type: text/markdown
    # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
     [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
   **Taiwanese Hokkien transliterator from Chinese characters** It has methods
 that allow to customise transliteration and retrieve any necessary information
                     about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
```

### Comparing `example990420-0.0.2/setup.py` & `example990420-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
     LONG_DESCRIPTION = '\n' + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Convert Chinese characters to Taiwanese'
 #LONG_DESCRIPTION = 'Taiwanese Hokkien transliterator from Chinese characters.'
 
 # Setting up
 setup(
     name="example990420",
     version=VERSION,
     author="Andrei Harbachov",
     author_email="<andrei.harbachov@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
+    license='MIT',
+    url='https://github.com/andreihar/taibun',
     install_requires=[],
-    keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization'],
+    keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization', 'transliteration'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `example990420-0.0.2/taibun/taibun.py` & `example990420-0.0.3/taibun/taibun.py`

 * *Files identical despite different names*

