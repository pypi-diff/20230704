# Comparing `tmp/example990420-0.0.5.tar.gz` & `tmp/example990420-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example990420-0.0.5.tar", last modified: Tue Jul  4 08:30:24 2023, max compression
+gzip compressed data, was "example990420-0.0.6.tar", last modified: Tue Jul  4 09:01:51 2023, max compression
```

## Comparing `example990420-0.0.5.tar` & `example990420-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.156697 example990420-0.0.5/
--rw-rw-rw-   0        0        0    11131 2023-07-04 08:30:24.153702 example990420-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 example990420-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.105594 example990420-0.0.5/example990420.egg-info/
--rw-rw-rw-   0        0        0    11131 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 08:30:23.000000 example990420-0.0.5/example990420.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:30:24.157692 example990420-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1383 2023-07-04 08:30:16.000000 example990420-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.136558 example990420-0.0.5/taibun/
--rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.5/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:30:24.144962 example990420-0.0.5/taibun/data/
--rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.5/taibun/data/simplified.json
--rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.5/taibun/data/words.json
--rw-rw-rw-   0        0        0    19924 2023-07-04 08:29:57.000000 example990420-0.0.5/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.558403 example990420-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 example990420-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    11029 2023-07-04 09:01:51.555272 example990420-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9995 2023-07-04 09:00:01.000000 example990420-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.512357 example990420-0.0.6/example990420.egg-info/
+-rw-rw-rw-   0        0        0    11029 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-04 09:01:51.000000 example990420-0.0.6/example990420.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 09:01:50.000000 example990420-0.0.6/example990420.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:01:51.559403 example990420-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-07-04 09:01:35.000000 example990420-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.527562 example990420-0.0.6/taibun/
+-rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 example990420-0.0.6/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:01:51.542139 example990420-0.0.6/taibun/data/
+-rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 example990420-0.0.6/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 example990420-0.0.6/taibun/data/words.json
+-rw-rw-rw-   0        0        0    19924 2023-07-04 08:29:57.000000 example990420-0.0.6/taibun/taibun.py
```

### Comparing `example990420-0.0.5/PKG-INFO` & `example990420-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <!-- PROJECT LOGO -->
 <div align="center">
 
-# <ruby>台文<rt>Tâi-bûn</rt></ruby>
+# 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
+<dev align='center'>
+
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
+
+</dev>
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
+<dev align='center'>
+
 [Report Bug][bug] •
 [PyPI][pypi]
 
+</dev>
+
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
@@ -205,15 +213,15 @@
 ```
 
 
 <!-- EXAMPLE -->
 ## Example
 
 ```python
-from taibun import Converter
+from taibun import Converter, Tokeniser
 
 # System
 c = Converter() # Tailo system default
 c.get('先生講，學生恬恬聽。')
 >> Sian-sinn kóng, ha̍k-sing tiām-tiām thiann.
 
 c = Converter(system='Zhuyin')
@@ -297,16 +305,14 @@
 [contributors]: #usage
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun.svg?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
 [linkedin]: https://www.linkedin.com/in/andrei-harbachov/
-[github-badge]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
-[github]: https://github.com/andreihar/taibun
 
 [pypi]: https://pypi.org/project/taibun
 [bug]: https://github.com/andreihar/taibun/issues
 [dictionary]: https://twblg.dict.edu.tw/holodict_new/
 [dictionary-via]: https://github.com/g0v/moedict-data-twblg
 [distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.5 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.6 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
 Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Description-Content-Type: text/markdown
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+:: Windows Description-Content-Type: text/markdown License-File: LICENSE
+ # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
-  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
+[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
+ Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
@@ -81,15 +80,15 @@
 TÃ¢i-lÃ¢m, kÃ¡n-tshing "lÃ¢m" (PeÌh-uÄ-jÄ«: TÃ¢i-lÃ¢m; tsÃ¹-im hÃ»-hÅ:
 ããË ãã¢Ë, kok-gÃ­: TÃ¡inÃ¡n). | tse sÄ« TÃ¢i-lÃ¢mï¼kÃ¡n-
 tshingãlÃ¢mãï¼PeÌh-uÄ-jÄ«ï¼TÃ¢i-lÃ¢mï¼tsÃ¹-im hÃ»-hÅï¼ããË
 ãã¢Ëï¼kok-gÃ­ï¼TÃ¡inÃ¡nï¼ã | ### Tokeniser `Tokeniser` class performs
 [NLTK wordpunct_tokenize][nltk-tokenize]-like tokenisation of a Taiwanese
 Hokkien sentence. ```python # constructor t = Tokeniser() # tokenise Taiwanese
 Hokkien sentence t.tokenise(input) ```  ## Example ```python from taibun import
-Converter # System c = Converter() # Tailo system default c.get
+Converter, Tokeniser # System c = Converter() # Tailo system default c.get
 ('åçè¬ï¼å­¸çæ¬æ¬è½ã') >> Sian-sinn kÃ³ng, haÌk-sing tiÄm-tiÄm
 thiann. c = Converter(system='Zhuyin') c.get('åçè¬ï¼å­¸çæ¬æ¬è½ã')
 >> ãã§ã¢ ããª ãã²Ë, ããã ãã§ã¥ ãã§ã°Ë« ãã§ã°Ë«
 ãã§ã©. # Dialect c = Converter() # south dialect default c.get
 ("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ beh Ä«ng tÄ« tsiaÌh hÃ® c = Converter
 (dialect='north') c.get("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ bueh Ä«ng tÅ« tsiaÌh hÃ»
 # Format c = Converter() # for Tailo, mark by default c.get("çæ¥å¿«æ¨") >>
@@ -118,25 +117,23 @@
 taibun?style=for-the-badge [contributors]: #usage [release-badge]: https://
 img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-
 badge [release]: https://github.com/andreihar/taibun/releases [licence-badge]:
 https://img.shields.io/github/license/andreihar/
 taibun.svg?color=000000&style=for-the-badge [licence]: LICENSE [linkedin-
 badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
 badge&logo=linkedin&logoColor=white [linkedin]: https://www.linkedin.com/in/
-andrei-harbachov/ [github-badge]: https://img.shields.io/badge/GitHub-
-100000?style=for-the-badge&logo=github&logoColor=white [github]: https://
-github.com/andreihar/taibun [pypi]: https://pypi.org/project/taibun [bug]:
-https://github.com/andreihar/taibun/issues [dictionary]: https://
-twblg.dict.edu.tw/holodict_new/ [dictionary-via]: https://github.com/g0v/
-moedict-data-twblg [distionary-cc]: https://creativecommons.org/licenses/by-nd/
-3.0/tw/deed.en [tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-
-u%C3%A2n_L%C3%B4-m%C3%A1-j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://
-en.wikipedia.org/wiki/Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]:
-https://en.wikipedia.org/wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-
-wiki]: https://en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-
-i%C5%8Dng_p%C4%ABng-im [zhangzhou-wiki]: https://en.wikipedia.org/wiki/
-Zhangzhou_dialects [quanzhou-wiki]: https://en.wikipedia.org/wiki/
-Quanzhou_dialects [nltk-tokenize]: https://nltk.org/api/nltk.tokenize.html
-[sandhi-wiki]: https://en.wikipedia.org/wiki/Taiwanese_Hokkien#Tone%20sandhi:~:
-text=thng%E2%9F%A9%20(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
+andrei-harbachov/ [pypi]: https://pypi.org/project/taibun [bug]: https://
+github.com/andreihar/taibun/issues [dictionary]: https://twblg.dict.edu.tw/
+holodict_new/ [dictionary-via]: https://github.com/g0v/moedict-data-twblg
+[distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
+[tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-u%C3%A2n_L%C3%B4-m%C3%A1-
+j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://en.wikipedia.org/wiki/
+Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]: https://en.wikipedia.org/
+wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-wiki]: https://
+en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-i%C5%8Dng_p%C4%ABng-im
+[zhangzhou-wiki]: https://en.wikipedia.org/wiki/Zhangzhou_dialects [quanzhou-
+wiki]: https://en.wikipedia.org/wiki/Quanzhou_dialects [nltk-tokenize]: https:/
+/nltk.org/api/nltk.tokenize.html [sandhi-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Hokkien#Tone%20sandhi:~:text=thng%E2%9F%A9%20
+(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
```

### Comparing `example990420-0.0.5/README.md` & `example990420-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 <!-- PROJECT LOGO -->
 <div align="center">
 
-# <ruby>台文<rt>Tâi-bûn</rt></ruby>
+# 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
+<dev align='center'>
+
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
+
+</dev>
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
+<dev align='center'>
+
 [Report Bug][bug] •
 [PyPI][pypi]
 
+</dev>
+
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
@@ -186,15 +193,15 @@
 ```
 
 
 <!-- EXAMPLE -->
 ## Example
 
 ```python
-from taibun import Converter
+from taibun import Converter, Tokeniser
 
 # System
 c = Converter() # Tailo system default
 c.get('先生講，學生恬恬聽。')
 >> Sian-sinn kóng, ha̍k-sing tiām-tiām thiann.
 
 c = Converter(system='Zhuyin')
@@ -278,16 +285,14 @@
 [contributors]: #usage
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun.svg?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
 [linkedin]: https://www.linkedin.com/in/andrei-harbachov/
-[github-badge]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
-[github]: https://github.com/andreihar/taibun
 
 [pypi]: https://pypi.org/project/taibun
 [bug]: https://github.com/andreihar/taibun/issues
 [dictionary]: https://twblg.dict.edu.tw/holodict_new/
 [dictionary-via]: https://github.com/g0v/moedict-data-twblg
 [distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+ # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
-  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
+[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
+ Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
@@ -71,15 +70,15 @@
 TÃ¢i-lÃ¢m, kÃ¡n-tshing "lÃ¢m" (PeÌh-uÄ-jÄ«: TÃ¢i-lÃ¢m; tsÃ¹-im hÃ»-hÅ:
 ããË ãã¢Ë, kok-gÃ­: TÃ¡inÃ¡n). | tse sÄ« TÃ¢i-lÃ¢mï¼kÃ¡n-
 tshingãlÃ¢mãï¼PeÌh-uÄ-jÄ«ï¼TÃ¢i-lÃ¢mï¼tsÃ¹-im hÃ»-hÅï¼ããË
 ãã¢Ëï¼kok-gÃ­ï¼TÃ¡inÃ¡nï¼ã | ### Tokeniser `Tokeniser` class performs
 [NLTK wordpunct_tokenize][nltk-tokenize]-like tokenisation of a Taiwanese
 Hokkien sentence. ```python # constructor t = Tokeniser() # tokenise Taiwanese
 Hokkien sentence t.tokenise(input) ```  ## Example ```python from taibun import
-Converter # System c = Converter() # Tailo system default c.get
+Converter, Tokeniser # System c = Converter() # Tailo system default c.get
 ('åçè¬ï¼å­¸çæ¬æ¬è½ã') >> Sian-sinn kÃ³ng, haÌk-sing tiÄm-tiÄm
 thiann. c = Converter(system='Zhuyin') c.get('åçè¬ï¼å­¸çæ¬æ¬è½ã')
 >> ãã§ã¢ ããª ãã²Ë, ããã ãã§ã¥ ãã§ã°Ë« ãã§ã°Ë«
 ãã§ã©. # Dialect c = Converter() # south dialect default c.get
 ("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ beh Ä«ng tÄ« tsiaÌh hÃ® c = Converter
 (dialect='north') c.get("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ bueh Ä«ng tÅ« tsiaÌh hÃ»
 # Format c = Converter() # for Tailo, mark by default c.get("çæ¥å¿«æ¨") >>
@@ -108,25 +107,23 @@
 taibun?style=for-the-badge [contributors]: #usage [release-badge]: https://
 img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-
 badge [release]: https://github.com/andreihar/taibun/releases [licence-badge]:
 https://img.shields.io/github/license/andreihar/
 taibun.svg?color=000000&style=for-the-badge [licence]: LICENSE [linkedin-
 badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
 badge&logo=linkedin&logoColor=white [linkedin]: https://www.linkedin.com/in/
-andrei-harbachov/ [github-badge]: https://img.shields.io/badge/GitHub-
-100000?style=for-the-badge&logo=github&logoColor=white [github]: https://
-github.com/andreihar/taibun [pypi]: https://pypi.org/project/taibun [bug]:
-https://github.com/andreihar/taibun/issues [dictionary]: https://
-twblg.dict.edu.tw/holodict_new/ [dictionary-via]: https://github.com/g0v/
-moedict-data-twblg [distionary-cc]: https://creativecommons.org/licenses/by-nd/
-3.0/tw/deed.en [tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-
-u%C3%A2n_L%C3%B4-m%C3%A1-j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://
-en.wikipedia.org/wiki/Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]:
-https://en.wikipedia.org/wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-
-wiki]: https://en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-
-i%C5%8Dng_p%C4%ABng-im [zhangzhou-wiki]: https://en.wikipedia.org/wiki/
-Zhangzhou_dialects [quanzhou-wiki]: https://en.wikipedia.org/wiki/
-Quanzhou_dialects [nltk-tokenize]: https://nltk.org/api/nltk.tokenize.html
-[sandhi-wiki]: https://en.wikipedia.org/wiki/Taiwanese_Hokkien#Tone%20sandhi:~:
-text=thng%E2%9F%A9%20(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
+andrei-harbachov/ [pypi]: https://pypi.org/project/taibun [bug]: https://
+github.com/andreihar/taibun/issues [dictionary]: https://twblg.dict.edu.tw/
+holodict_new/ [dictionary-via]: https://github.com/g0v/moedict-data-twblg
+[distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
+[tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-u%C3%A2n_L%C3%B4-m%C3%A1-
+j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://en.wikipedia.org/wiki/
+Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]: https://en.wikipedia.org/
+wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-wiki]: https://
+en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-i%C5%8Dng_p%C4%ABng-im
+[zhangzhou-wiki]: https://en.wikipedia.org/wiki/Zhangzhou_dialects [quanzhou-
+wiki]: https://en.wikipedia.org/wiki/Quanzhou_dialects [nltk-tokenize]: https:/
+/nltk.org/api/nltk.tokenize.html [sandhi-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Hokkien#Tone%20sandhi:~:text=thng%E2%9F%A9%20
+(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
```

### Comparing `example990420-0.0.5/example990420.egg-info/PKG-INFO` & `example990420-0.0.6/example990420.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 Metadata-Version: 2.1
 Name: example990420
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert Chinese characters to Taiwanese
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: <andrei.harbachov@gmail.com>
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <!-- PROJECT LOGO -->
 <div align="center">
 
-# <ruby>台文<rt>Tâi-bûn</rt></ruby>
+# 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
+<dev align='center'>
+
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
+
+</dev>
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
+<dev align='center'>
+
 [Report Bug][bug] •
 [PyPI][pypi]
 
+</dev>
+
 </div>
 
 
 ---
 
 
 <!-- TABLE OF CONTENTS -->
@@ -205,15 +213,15 @@
 ```
 
 
 <!-- EXAMPLE -->
 ## Example
 
 ```python
-from taibun import Converter
+from taibun import Converter, Tokeniser
 
 # System
 c = Converter() # Tailo system default
 c.get('先生講，學生恬恬聽。')
 >> Sian-sinn kóng, ha̍k-sing tiām-tiām thiann.
 
 c = Converter(system='Zhuyin')
@@ -297,16 +305,14 @@
 [contributors]: #usage
 [release-badge]: https://img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-badge
 [release]: https://github.com/andreihar/taibun/releases
 [licence-badge]: https://img.shields.io/github/license/andreihar/taibun.svg?color=000000&style=for-the-badge
 [licence]: LICENSE
 [linkedin-badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
 [linkedin]: https://www.linkedin.com/in/andrei-harbachov/
-[github-badge]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white
-[github]: https://github.com/andreihar/taibun
 
 [pypi]: https://pypi.org/project/taibun
 [bug]: https://github.com/andreihar/taibun/issues
 [dictionary]: https://twblg.dict.edu.tw/holodict_new/
 [dictionary-via]: https://github.com/g0v/moedict-data-twblg
 [distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: example990420 Version: 0.0.5 Summary: Convert
+Metadata-Version: 2.1 Name: example990420 Version: 0.0.6 Summary: Convert
 Chinese characters to Taiwanese Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email:
 harbachov@gmail.com> License: MIT Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
 Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Description-Content-Type: text/markdown
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+:: Windows Description-Content-Type: text/markdown License-File: LICENSE
+ # å°æ | TÃ¢i-bÃ»n   [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
-  Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
+[LinkedIn][linkedin-badge]][linkedin]  **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
+ Includes word tokeniser for Taiwanese Hokkien.  [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
                 # Dialect
@@ -81,15 +80,15 @@
 TÃ¢i-lÃ¢m, kÃ¡n-tshing "lÃ¢m" (PeÌh-uÄ-jÄ«: TÃ¢i-lÃ¢m; tsÃ¹-im hÃ»-hÅ:
 ããË ãã¢Ë, kok-gÃ­: TÃ¡inÃ¡n). | tse sÄ« TÃ¢i-lÃ¢mï¼kÃ¡n-
 tshingãlÃ¢mãï¼PeÌh-uÄ-jÄ«ï¼TÃ¢i-lÃ¢mï¼tsÃ¹-im hÃ»-hÅï¼ããË
 ãã¢Ëï¼kok-gÃ­ï¼TÃ¡inÃ¡nï¼ã | ### Tokeniser `Tokeniser` class performs
 [NLTK wordpunct_tokenize][nltk-tokenize]-like tokenisation of a Taiwanese
 Hokkien sentence. ```python # constructor t = Tokeniser() # tokenise Taiwanese
 Hokkien sentence t.tokenise(input) ```  ## Example ```python from taibun import
-Converter # System c = Converter() # Tailo system default c.get
+Converter, Tokeniser # System c = Converter() # Tailo system default c.get
 ('åçè¬ï¼å­¸çæ¬æ¬è½ã') >> Sian-sinn kÃ³ng, haÌk-sing tiÄm-tiÄm
 thiann. c = Converter(system='Zhuyin') c.get('åçè¬ï¼å­¸çæ¬æ¬è½ã')
 >> ãã§ã¢ ããª ãã²Ë, ããã ãã§ã¥ ãã§ã°Ë« ãã§ã°Ë«
 ãã§ã©. # Dialect c = Converter() # south dialect default c.get
 ("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ beh Ä«ng tÄ« tsiaÌh hÃ® c = Converter
 (dialect='north') c.get("ææ¬²ç¨ç®¸é£é­") >> GuÃ¡ bueh Ä«ng tÅ« tsiaÌh hÃ»
 # Format c = Converter() # for Tailo, mark by default c.get("çæ¥å¿«æ¨") >>
@@ -118,25 +117,23 @@
 taibun?style=for-the-badge [contributors]: #usage [release-badge]: https://
 img.shields.io/github/v/release/andreihar/taibun?color=38618c&style=for-the-
 badge [release]: https://github.com/andreihar/taibun/releases [licence-badge]:
 https://img.shields.io/github/license/andreihar/
 taibun.svg?color=000000&style=for-the-badge [licence]: LICENSE [linkedin-
 badge]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
 badge&logo=linkedin&logoColor=white [linkedin]: https://www.linkedin.com/in/
-andrei-harbachov/ [github-badge]: https://img.shields.io/badge/GitHub-
-100000?style=for-the-badge&logo=github&logoColor=white [github]: https://
-github.com/andreihar/taibun [pypi]: https://pypi.org/project/taibun [bug]:
-https://github.com/andreihar/taibun/issues [dictionary]: https://
-twblg.dict.edu.tw/holodict_new/ [dictionary-via]: https://github.com/g0v/
-moedict-data-twblg [distionary-cc]: https://creativecommons.org/licenses/by-nd/
-3.0/tw/deed.en [tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-
-u%C3%A2n_L%C3%B4-m%C3%A1-j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://
-en.wikipedia.org/wiki/Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://
-en.wikipedia.org/wiki/Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]:
-https://en.wikipedia.org/wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-
-wiki]: https://en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-
-i%C5%8Dng_p%C4%ABng-im [zhangzhou-wiki]: https://en.wikipedia.org/wiki/
-Zhangzhou_dialects [quanzhou-wiki]: https://en.wikipedia.org/wiki/
-Quanzhou_dialects [nltk-tokenize]: https://nltk.org/api/nltk.tokenize.html
-[sandhi-wiki]: https://en.wikipedia.org/wiki/Taiwanese_Hokkien#Tone%20sandhi:~:
-text=thng%E2%9F%A9%20(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
+andrei-harbachov/ [pypi]: https://pypi.org/project/taibun [bug]: https://
+github.com/andreihar/taibun/issues [dictionary]: https://twblg.dict.edu.tw/
+holodict_new/ [dictionary-via]: https://github.com/g0v/moedict-data-twblg
+[distionary-cc]: https://creativecommons.org/licenses/by-nd/3.0/tw/deed.en
+[tailo-wiki]: https://en.wikipedia.org/wiki/T%C3%A2i-u%C3%A2n_L%C3%B4-m%C3%A1-
+j%C4%AB_Phing-im_Hong-%C3%A0n [poj-wiki]: https://en.wikipedia.org/wiki/
+Pe%CC%8Dh-%C5%8De-j%C4%AB [zhuyin-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Phonetic_Symbols [tlpa-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Language_Phonetic_Alphabet [pingyim-wiki]: https://en.wikipedia.org/
+wiki/Bb%C3%A1nl%C3%A1m_p%C3%ACngy%C4%ABm [tongiong-wiki]: https://
+en.wikipedia.org/wiki/Da%C4%AB-gh%C3%AE_t%C5%8Dng-i%C5%8Dng_p%C4%ABng-im
+[zhangzhou-wiki]: https://en.wikipedia.org/wiki/Zhangzhou_dialects [quanzhou-
+wiki]: https://en.wikipedia.org/wiki/Quanzhou_dialects [nltk-tokenize]: https:/
+/nltk.org/api/nltk.tokenize.html [sandhi-wiki]: https://en.wikipedia.org/wiki/
+Taiwanese_Hokkien#Tone%20sandhi:~:text=thng%E2%9F%A9%20
+(%22soup%22).-,Tone%20sandhi,-%5Bedit%5D
```

### Comparing `example990420-0.0.5/setup.py` & `example990420-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-# build instructions
-#  python3 setup.py sdist
+# python setup.py sdist
 # twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
     LONG_DESCRIPTION = '\n' + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Convert Chinese characters to Taiwanese'
-#LONG_DESCRIPTION = 'Taiwanese Hokkien transliterator from Chinese characters.'
 
 # Setting up
 setup(
     name="example990420",
     version=VERSION,
     author="Andrei Harbachov",
     author_email="<andrei.harbachov@gmail.com>",
```

### Comparing `example990420-0.0.5/taibun/data/simplified.json` & `example990420-0.0.6/taibun/data/simplified.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.5/taibun/data/words.json` & `example990420-0.0.6/taibun/data/words.json`

 * *Files identical despite different names*

### Comparing `example990420-0.0.5/taibun/taibun.py` & `example990420-0.0.6/taibun/taibun.py`

 * *Files identical despite different names*

