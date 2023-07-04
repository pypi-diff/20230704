# Comparing `tmp/example990420-0.0.4.tar.gz` & `tmp/example990420-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-0.0.4.tar", last modified: Tue Jul  4 07:54:07 2023, max compression
+gzip compressed data, was "example990420-0.0.5.tar", last modified: Tue Jul  4 08:30:24 2023, max compression
```

## Comparing `example990420-0.0.4.tar` & `example990420-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:54:07.815237 example990420-0.0.4/
--rw-rw-rw-   0        0        0    11079 2023-07-04 07:54:07.813241 example990420-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 example990420-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 07:54:07.790900 example990420-0.0.4/example990420.egg-info/
--rw-rw-rw-   0        0        0    11079 2023-07-04 07:54:07.000000 example990420-0.0.4/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-04 07:54:07.000000 example990420-0.0.4/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:54:07.000000 example990420-0.0.4/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 07:54:07.000000 example990420-0.0.4/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 07:54:07.815791 example990420-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1263 2023-07-04 07:54:04.000000 example990420-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:54:07.797158 example990420-0.0.4/taibun/
--rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.4/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:54:07.806288 example990420-0.0.4/taibun/data/
--rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.4/taibun/data/simplified.json
--rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.4/taibun/data/words.json
--rw-rw-rw-   0        0        0    19874 2023-07-04 01:32:21.000000 example990420-0.0.4/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.156697 example990420-0.0.5/
+-rw-rw-rw-   0        0        0    11131 2023-07-04 08:30:24.153702 example990420-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 example990420-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.105594 example990420-0.0.5/example990420.egg-info/
+-rw-rw-rw-   0        0        0    11131 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:30:24.157692 example990420-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2023-07-04 08:30:16.000000 example990420-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.136558 example990420-0.0.5/taibun/
+-rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.5/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.144962 example990420-0.0.5/taibun/data/
+-rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.5/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.5/taibun/data/words.json
+-rw-rw-rw-   0        0        0    19924 2023-07-04 08:29:57.000000 example990420-0.0.5/taibun/taibun.py
```

### Comparing `example990420-0.0.4/PKG-INFO` & `example990420-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
+Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.4 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.5 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
-System :: Microsoft :: Windows Description-Content-Type: text/markdown
+Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Description-Content-Type: text/markdown
    # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
     [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
   **Taiwanese Hokkien transliterator from Chinese characters** It has methods
 that allow to customise transliteration and retrieve any necessary information
                     about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
```

### Comparing `example990420-0.0.4/README.md` & `example990420-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `example990420-0.0.4/example990420.egg-info/PKG-INFO` & `example990420-0.0.5/example990420.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
+Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.4 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.5 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
-System :: Microsoft :: Windows Description-Content-Type: text/markdown
+Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Description-Content-Type: text/markdown
    # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
     [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
   **Taiwanese Hokkien transliterator from Chinese characters** It has methods
 that allow to customise transliteration and retrieve any necessary information
                     about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
```

### Comparing `example990420-0.0.4/setup.py` & `example990420-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
+# build instructions
+#  python3 setup.py sdist
+# twine upload dist/*
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
     LONG_DESCRIPTION = '\n' + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Convert Chinese characters to Taiwanese'
 #LONG_DESCRIPTION = 'Taiwanese Hokkien transliterator from Chinese characters.'
 
 # Setting up
 setup(
     name="example990420",
     version=VERSION,
@@ -24,14 +28,15 @@
     package_dir={'taibun': 'taibun'},
     package_data={'taibun': ['data/*.json']},
     license='MIT',
     url='https://github.com/andreihar/taibun',
     install_requires=[],
     keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization', 'transliteration'],
     classifiers=[
+        'Topic :: Text Processing :: Linguistic',
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

### Comparing `example990420-0.0.4/taibun/data/simplified.json` & `example990420-0.0.5/taibun/data/simplified.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.4/taibun/data/words.json` & `example990420-0.0.5/taibun/data/words.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.4/taibun/taibun.py` & `example990420-0.0.5/taibun/taibun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 import unicodedata
+import os
 
 """
 Description: Converts Chinese characters to phonetic transcription of any
 	 		 of two main pronunciations of Taiwanese Hokkien. Supports both
              Traditional and Simplified characters.
 Invariant: Phonetic transcription depends on the dialect passed into the function.
 	 	   `south` for Zhangzhou (漳州)-leaning pronunciation (set by default).
@@ -17,16 +18,15 @@
            format = mark for diacritical representation
 					number for numeric representation
                     strip for no representation of tones
 """
 
 ## TODO: strip doesn't work for zhuyin and TLPA
 ##       zhuyin conversion incorrect
-
-word_dict = json.load(open("data/words.json", encoding="utf-8"))
+word_dict = json.load(open(os.path.join(os.path.dirname(__file__), "data/words.json"), encoding="utf-8"))
 
 class Converter(object):
 
     suffix_token = '[SFFX_TKN]'
     tone_token = '[TN_TKN]'
     DEFAULT_DELIMITER = object()
     DEFAULT_SANDHI = object()
```

