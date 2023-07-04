# Comparing `tmp/example990420-0.0.6.tar.gz` & `tmp/example990420-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-0.0.6.tar", last modified: Tue Jul  4 09:01:51 2023, max compression
+gzip compressed data, was "example990420-0.0.7.tar", last modified: Tue Jul  4 09:07:43 2023, max compression
```

## Comparing `example990420-0.0.6.tar` & `example990420-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.558403 example990420-0.0.6/
--rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    11029 2023-07-04 09:01:51.555272 example990420-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     9995 2023-07-04 09:00:01.000000 example990420-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.512357 example990420-0.0.6/example990420.egg-info/
--rw-rw-rw-   0        0        0    11029 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-04 09:01:51.000000 example990420-0.0.6/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 09:01:51.559403 example990420-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-07-04 09:01:35.000000 example990420-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.527562 example990420-0.0.6/taibun/
--rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.6/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.542139 example990420-0.0.6/taibun/data/
--rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.6/taibun/data/simplified.json
--rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.6/taibun/data/words.json
--rw-rw-rw-   0        0        0    19924 2023-07-04 08:29:57.000000 example990420-0.0.6/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.105015 example990420-0.0.7/
+-rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    10953 2023-07-04 09:07:43.103025 example990420-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9927 2023-07-04 09:04:02.000000 example990420-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.073749 example990420-0.0.7/example990420.egg-info/
+-rw-rw-rw-   0        0        0    10953 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 09:07:42.000000 example990420-0.0.7/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:07:43.106011 example990420-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-07-04 09:07:33.000000 example990420-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.082872 example990420-0.0.7/taibun/
+-rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.7/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:07:43.092714 example990420-0.0.7/taibun/data/
+-rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.7/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.7/taibun/data/words.json
+-rw-rw-rw-   0        0        0    19967 2023-07-04 08:47:50.000000 example990420-0.0.7/taibun/taibun.py
```

### Comparing `example990420-0.0.6/LICENSE` & `example990420-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `example990420-0.0.6/PKG-INFO` & `example990420-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
 Classifier: Topic :: Text Processing :: Linguistic
@@ -20,35 +20,27 @@
 
 <!-- PROJECT LOGO -->
 <div align="center">
 
 # 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
-<dev align='center'>
-
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 
-</dev>
-
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
-<dev align='center'>
-
 [Report Bug][bug] •
 [PyPI][pypi]
 
-</dev>
-
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.6 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.7 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
 Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown License-File: LICENSE
- # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
 Chinese characters** It has methods that allow to customise transliteration and
    retrieve any necessary information about Taiwanese Hokkien pronunciation.
- Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
+  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
```

### Comparing `example990420-0.0.6/README.md` & `example990420-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 <!-- PROJECT LOGO -->
 <div align="center">
 
 # 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
-<dev align='center'>
-
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 
-</dev>
-
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
-<dev align='center'>
-
 [Report Bug][bug] •
 [PyPI][pypi]
 
-</dev>
-
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
- # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
 Chinese characters** It has methods that allow to customise transliteration and
    retrieve any necessary information about Taiwanese Hokkien pronunciation.
- Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
+  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
```

### Comparing `example990420-0.0.6/example990420.egg-info/PKG-INFO` & `example990420-0.0.7/example990420.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.6
+Version: 0.0.7
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
 Classifier: Topic :: Text Processing :: Linguistic
@@ -20,35 +20,27 @@
 
 <!-- PROJECT LOGO -->
 <div align="center">
 
 # 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
-<dev align='center'>
-
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
 
-</dev>
-
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
-<dev align='center'>
-
 [Report Bug][bug] •
 [PyPI][pypi]
 
-</dev>
-
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.6 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.7 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
 Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown License-File: LICENSE
- # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
 Chinese characters** It has methods that allow to customise transliteration and
    retrieve any necessary information about Taiwanese Hokkien pronunciation.
- Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
+  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
```

### Comparing `example990420-0.0.6/setup.py` & `example990420-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
     LONG_DESCRIPTION = '\n' + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Convert Chinese characters to Taiwanese'
 
 # Setting up
 setup(
     name="example990420",
     version=VERSION,
     author="Andrei Harbachov",
```

### Comparing `example990420-0.0.6/taibun/data/simplified.json` & `example990420-0.0.7/taibun/data/simplified.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.6/taibun/data/words.json` & `example990420-0.0.7/taibun/data/words.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.6/taibun/taibun.py` & `example990420-0.0.7/taibun/taibun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import os
 import json
 import re
 import unicodedata
-import os
 
 """
 Description: Converts Chinese characters to phonetic transcription of any
 	 		 of two main pronunciations of Taiwanese Hokkien. Supports both
              Traditional and Simplified characters.
 Invariant: Phonetic transcription depends on the dialect passed into the function.
 	 	   `south` for Zhangzhou (漳州)-leaning pronunciation (set by default).
@@ -18,14 +18,15 @@
            format = mark for diacritical representation
 					number for numeric representation
                     strip for no representation of tones
 """
 
 ## TODO: strip doesn't work for zhuyin and TLPA
 ##       zhuyin conversion incorrect
+
 word_dict = json.load(open(os.path.join(os.path.dirname(__file__), "data/words.json"), encoding="utf-8"))
 
 class Converter(object):
 
     suffix_token = '[SFFX_TKN]'
     tone_token = '[TN_TKN]'
     DEFAULT_DELIMITER = object()
@@ -56,15 +57,15 @@
             converted = converted[0].upper() + converted[1:]
             return self.__format_text(self.__format_punctuation_western(converted.strip()))
         return self.__format_punctuation_cjk(converted.strip())
 
 
     # Convert Simplified to Traditional characters
     def to_traditional(self, input):
-        trad = json.load(open("data/simplified.json", encoding="utf-8"))
+        trad = json.load(open(os.path.join(os.path.dirname(__file__), "data/simplified.json"), encoding="utf-8"))
         for c in trad:
             input = input.replace(c, trad[c])
         return input
 
 
     ### Input formatting
```

