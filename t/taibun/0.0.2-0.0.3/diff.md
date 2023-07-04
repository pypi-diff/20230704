# Comparing `tmp/taibun-0.0.2.tar.gz` & `tmp/taibun-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-0.0.2.tar", last modified: Tue Jul  4 05:04:22 2023, max compression
+gzip compressed data, was "taibun-0.0.3.tar", last modified: Tue Jul  4 09:13:01 2023, max compression
```

## Comparing `taibun-0.0.2.tar` & `taibun-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.388658 taibun-0.0.2/
--rw-rw-rw-   0        0        0    10993 2023-07-04 05:04:22.387689 taibun-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10125 2023-07-04 04:42:52.000000 taibun-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 05:04:22.389642 taibun-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-07-04 05:04:01.000000 taibun-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.356731 taibun-0.0.2/taibun/
--rw-rw-rw-   0        0        0       20 2023-06-15 08:41:22.000000 taibun-0.0.2/taibun/__init__.py
--rw-rw-rw-   0        0        0    19874 2023-07-04 01:32:21.000000 taibun-0.0.2/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:04:22.382660 taibun-0.0.2/taibun.egg-info/
--rw-rw-rw-   0        0        0    10993 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 05:04:22.000000 taibun-0.0.2/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 09:13:01.776962 taibun-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-07-04 08:45:02.000000 taibun-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10946 2023-07-04 09:13:01.772279 taibun-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9927 2023-07-04 09:04:02.000000 taibun-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:13:01.780490 taibun-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2023-07-04 09:12:12.000000 taibun-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:13:01.667192 taibun-0.0.3/taibun/
+-rw-rw-rw-   0        0        0       46 2023-07-04 07:50:30.000000 taibun-0.0.3/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:13:01.762353 taibun-0.0.3/taibun/data/
+-rw-rw-rw-   0        0        0    17141 2023-06-17 08:58:24.000000 taibun-0.0.3/taibun/data/simplified.json
+-rw-rw-rw-   0        0        0   645595 2023-07-03 18:29:04.000000 taibun-0.0.3/taibun/data/words.json
+-rw-rw-rw-   0        0        0    19967 2023-07-04 08:47:50.000000 taibun-0.0.3/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:13:01.751652 taibun-0.0.3/taibun.egg-info/
+-rw-rw-rw-   0        0        0    10946 2023-07-04 09:13:01.000000 taibun-0.0.3/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-04 09:13:01.000000 taibun-0.0.3/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:13:01.000000 taibun-0.0.3/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 09:13:01.000000 taibun-0.0.3/taibun.egg-info/top_level.txt
```

### Comparing `taibun-0.0.2/PKG-INFO` & `taibun-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: taibun
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
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Development Status :: 2 - Pre-Alpha
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
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
 [Report Bug][bug] •
@@ -202,15 +205,15 @@
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
@@ -294,16 +297,14 @@
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
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: taibun Version: 0.0.2 Summary: Convert Chinese
-characters to Taiwanese Author: Andrei Harbachov Author-email:
-harbachov@gmail.com> Keywords:
-python,taiwan,taiwanese,taigi,hokkien,romanization Classifier: Development
-Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+Metadata-Version: 2.1 Name: taibun Version: 0.0.3 Summary: Convert Chinese
+characters to Taiwanese Home-page: https://github.com/andreihar/taibun Author:
+Andrei Harbachov Author-email:
+harbachov@gmail.com> License: MIT Keywords:
+python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
+Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Description-Content-Type: text/markdown License-File: LICENSE
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
@@ -79,15 +80,15 @@
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
@@ -116,25 +117,23 @@
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

### Comparing `taibun-0.0.2/README.md` & `taibun-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 <!-- PROJECT LOGO -->
 <div align="center">
 
-# <ruby>台文<rt>Tâi-bûn</rt></ruby>
+# 台文 | Tâi-bûn
 
 <!-- PROJECT SHIELDS -->
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
 [Report Bug][bug] •
@@ -186,15 +185,15 @@
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
@@ -278,16 +277,14 @@
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
@@ -1,13 +1,12 @@
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
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

### Comparing `taibun-0.0.2/setup.py` & `taibun-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
+# python setup.py sdist
+# twine upload dist/*
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding='utf-8') as fh:
     LONG_DESCRIPTION = '\n' + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Convert Chinese characters to Taiwanese'
-#LONG_DESCRIPTION = 'Taiwanese Hokkien transliterator from Chinese characters.'
 
 # Setting up
 setup(
     name="taibun",
     version=VERSION,
     author="Andrei Harbachov",
     author_email="<andrei.harbachov@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
+    package_dir={'taibun': 'taibun'},
+    package_data={'taibun': ['data/*.json']},
+    license='MIT',
+    url='https://github.com/andreihar/taibun',
     install_requires=[],
-    keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization'],
+    keywords=['python', 'taiwan', 'taiwanese', 'taigi', 'hokkien', 'romanization', 'transliteration'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        'Topic :: Text Processing :: Linguistic',
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `taibun-0.0.2/taibun/taibun.py` & `taibun-0.0.3/taibun/taibun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 import re
 import unicodedata
 
 """
 Description: Converts Chinese characters to phonetic transcription of any
 	 		 of two main pronunciations of Taiwanese Hokkien. Supports both
@@ -18,15 +19,15 @@
 					number for numeric representation
                     strip for no representation of tones
 """
 
 ## TODO: strip doesn't work for zhuyin and TLPA
 ##       zhuyin conversion incorrect
 
-word_dict = json.load(open("data/words.json", encoding="utf-8"))
+word_dict = json.load(open(os.path.join(os.path.dirname(__file__), "data/words.json"), encoding="utf-8"))
 
 class Converter(object):
 
     suffix_token = '[SFFX_TKN]'
     tone_token = '[TN_TKN]'
     DEFAULT_DELIMITER = object()
     DEFAULT_SANDHI = object()
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

### Comparing `taibun-0.0.2/taibun.egg-info/PKG-INFO` & `taibun-0.0.3/taibun.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: taibun
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
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Development Status :: 2 - Pre-Alpha
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
 [![Contributors][contributors-badge]][contributors]
 [![Release][release-badge]][release]
 [![Licence][licence-badge]][licence]
 [![LinkedIn][linkedin-badge]][linkedin]
-[![GitHub][github-badge]][github]
 
 **Taiwanese Hokkien transliterator from Chinese characters**
 
 It has methods that allow to customise transliteration and retrieve any necessary information about Taiwanese Hokkien pronunciation.<br />
 Includes word tokeniser for Taiwanese Hokkien.
 
 [Report Bug][bug] •
@@ -202,15 +205,15 @@
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
@@ -294,16 +297,14 @@
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
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: taibun Version: 0.0.2 Summary: Convert Chinese
-characters to Taiwanese Author: Andrei Harbachov Author-email:
-harbachov@gmail.com> Keywords:
-python,taiwan,taiwanese,taigi,hokkien,romanization Classifier: Development
-Status :: 1 - Planning Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Description-Content-Type: text/markdown
-   # å°æTÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
+Metadata-Version: 2.1 Name: taibun Version: 0.0.3 Summary: Convert Chinese
+characters to Taiwanese Home-page: https://github.com/andreihar/taibun Author:
+Andrei Harbachov Author-email:
+harbachov@gmail.com> License: MIT Keywords:
+python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration Classifier:
+Topic :: Text Processing :: Linguistic Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Description-Content-Type: text/markdown License-File: LICENSE
+ # å°æ | TÃ¢i-bÃ»n  [![Contributors][contributors-badge]][contributors] [!
   [Release][release-badge]][release] [![Licence][licence-badge]][licence] [!
-    [LinkedIn][linkedin-badge]][linkedin] [![GitHub][github-badge]][github]
-  **Taiwanese Hokkien transliterator from Chinese characters** It has methods
-that allow to customise transliteration and retrieve any necessary information
-                    about Taiwanese Hokkien pronunciation.
+ [LinkedIn][linkedin-badge]][linkedin] **Taiwanese Hokkien transliterator from
+Chinese characters** It has methods that allow to customise transliteration and
+   retrieve any necessary information about Taiwanese Hokkien pronunciation.
   Includes word tokeniser for Taiwanese Hokkien. [Report Bug][bug] â¢ [PyPI]
                                     [pypi]
 ---   Table of Contents
    1. Install
    2. Usage
           o Converter
                 # System
@@ -79,15 +80,15 @@
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
@@ -116,25 +117,23 @@
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

