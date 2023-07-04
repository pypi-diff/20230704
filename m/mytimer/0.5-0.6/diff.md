# Comparing `tmp/mytimer-0.5.tar.gz` & `tmp/mytimer-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytimer-0.5.tar", last modified: Thu May 25 15:11:52 2023, max compression
+gzip compressed data, was "mytimer-0.6.tar", last modified: Tue Jul  4 19:07:01 2023, max compression
```

## Comparing `mytimer-0.5.tar` & `mytimer-0.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.089664 mytimer-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 15:11:39.000000 mytimer-0.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-25 15:11:39.000000 mytimer-0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-25 15:11:39.000000 mytimer-0.5/FACES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:11:39.000000 mytimer-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 15:11:39.000000 mytimer-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-25 15:11:52.089664 mytimer-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-25 15:11:39.000000 mytimer-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 15:11:39.000000 mytimer-0.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)   602412 2023-05-25 15:11:39.000000 mytimer-0.5/mytimer/sounds/alarm.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:52.085664 mytimer-0.5/mytimer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 15:11:52.000000 mytimer-0.5/mytimer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 15:11:51.000000 mytimer-0.5/mytimer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 15:11:39.000000 mytimer-0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:11:52.089664 mytimer-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-25 15:11:39.000000 mytimer-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:07:01.832521 mytimer-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-04 19:06:51.000000 mytimer-0.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 19:06:51.000000 mytimer-0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-04 19:06:51.000000 mytimer-0.6/FACES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 19:06:51.000000 mytimer-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 19:06:51.000000 mytimer-0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-07-04 19:07:01.832521 mytimer-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-04 19:06:51.000000 mytimer-0.6/PROGRAMS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-04 19:06:51.000000 mytimer-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 19:06:51.000000 mytimer-0.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:07:01.828521 mytimer-0.6/mytimer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:07:01.832521 mytimer-0.6/mytimer/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/sounds/1.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   602412 2023-07-04 19:06:51.000000 mytimer-0.6/mytimer/sounds/2.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:07:01.832521 mytimer-0.6/mytimer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 19:07:01.000000 mytimer-0.6/mytimer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 19:06:51.000000 mytimer-0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:07:01.832521 mytimer-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-04 19:06:51.000000 mytimer-0.6/setup.py
```

### Comparing `mytimer-0.5/CHANGELOG.md` & `mytimer-0.6/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.6] - 2023-07-04
+### Added
+- `--program` argument
+- `PROGRAMS.md`
+- `run_timer` function
+### Changed
+- Inputs type changed to `int`
+- `README.md` updated
+- `WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE`
+- Alarm tone changed
 ## [0.5] - 2023-05-25
 ### Added
 - 5 new faces
 - `--message` argument
 ### Changed
 - `play_sound` function modified
 - `playsound` removed from `requirements.txt`
@@ -36,15 +46,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...dev
+[0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.5/FACES.md` & `mytimer-0.6/FACES.md`

 * *Files identical despite different names*

### Comparing `mytimer-0.5/LICENSE` & `mytimer-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mytimer-0.5/PKG-INFO` & `mytimer-0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 0.5
+Version: 0.6
 Summary: Simple Timer for Your Terminal
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.5
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.6
 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -111,21 +111,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 0.6](https://github.com/sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.5` (Need root access)							
+- `pip install mytimer==0.6`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -177,14 +177,21 @@
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
 
 
+### Program
+
+```console
+mytimer --program=black-tea
+```
+* [Programs List](https://github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md)
+
 ### Message
 
 
 ```console
 mytimer --minute=7 --second=30 --message="Test message"
 ```
 		
@@ -202,15 +209,20 @@
 Just fill an issue and describe it. We'll check it ASAP!
 
 - Please complete the issue template
  			
 
 ## References
 
-<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a> </blockquote>
+<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a></blockquote>
+
+<blockquote>2- <a href="https://www.online-timers.com/">Online Timer</a></blockquote>
+
+<blockquote>3- <a href="https://www.mediacollege.com/">Media College</a></blockquote>
+
 
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
 
@@ -247,14 +259,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.6] - 2023-07-04
+### Added
+- `--program` argument
+- `PROGRAMS.md`
+- `run_timer` function
+### Changed
+- Inputs type changed to `int`
+- `README.md` updated
+- `WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE`
+- Alarm tone changed
 ## [0.5] - 2023-05-25
 ### Added
 - 5 new faces
 - `--message` argument
 ### Changed
 - `play_sound` function modified
 - `playsound` removed from `requirements.txt`
@@ -282,15 +304,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...dev
+[0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: mytimer Version: 0.5 Summary: Simple Timer for Your
+Metadata-Version: 2.1 Name: mytimer Version: 0.6 Summary: Simple Timer for Your
 Terminal Home-page: https://github.com/sepandhaghighi/mytimer Download-URL:
-https://github.com/sepandhaghighi/mytimer/tarball/v0.5 Author: Sepand Haghighi
+https://github.com/sepandhaghighi/mytimer/tarball/v0.6 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source, https://
 github.com/sepandhaghighi/mytimer Keywords: python3 python timer terminal
 stopwatch Classifier: Development Status :: 4 - Beta Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -48,35 +48,38 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.5](https://github.com/
-sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+## Installation ### Source Code - Download [Version 0.6](https://github.com/
+sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
 Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
-`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
-`mytimer` or `python -m mytimer` to run this program ### Version ```console
-mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
-mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
-```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
-mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
-```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
-mode may not be supported on all systems ```console mytimer --minute=7 --
-second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
-second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
-mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
-second=30 --message="Test message" ```
+`pip install mytimer==0.6` ## Usage â ï¸ You can use `mytimer` or `python -
+m mytimer` to run this program ### Version ```console mytimer --version ``` ###
+Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
+```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
+minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
+mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
+second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
+systems ```console mytimer --minute=7 --second=30 --countdown --alarm ``` ###
+Face ```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List]
+(https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md) ### Program
+```console mytimer --program=black-tea ``` * [Programs List](https://
+github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md) ### Message ```console
+mytimer --minute=7 --second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
+     2- Online_Timer
+     3- Media_College
 ## Show your support
 **** Star this repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to our project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
@@ -100,23 +103,27 @@
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
 [http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
+## [Unreleased] ## [0.6] - 2023-07-04 ### Added - `--program` argument -
+`PROGRAMS.md` - `run_timer` function ### Changed - Inputs type changed to `int`
+- `README.md` updated - `WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE` -
+Alarm tone changed ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
 argument ### Changed - `play_sound` function modified - `playsound` removed
 from `requirements.txt` - `README.md` updated ## [0.4] - 2023-02-10 ### Added -
 4 new faces - Infinite timer mode ### Changed - `README.md` updated -
 Parameters moved to `params.py` ## [0.3] - 2022-11-25 ### Added - `--face`
 argument - `FACES.md` ### Changed - `README.md` updated - Minimum `art` library
 version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03 ### Added - `--
 version` flag ### Changed - Test system modified - `countdown_timer` function
 modified - `countup_timer` function modified ## [0.1] - 2022-10-18 ### Added -
 Countdown mode - Count-up mode - Alarm [Unreleased]: https://github.com/
-sepandhaghighi/mytimer/compare/v0.5...dev [0.5]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.6...dev [0.6]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.5...v0.6 [0.5]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.4...v0.5 [0.4]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.3...v0.4 [0.3]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://github.com/
 sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.5/README.md` & `mytimer-0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -77,21 +77,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 0.6](https://github.com/sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.5` (Need root access)							
+- `pip install mytimer==0.6`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -143,14 +143,21 @@
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
 
 
+### Program
+
+```console
+mytimer --program=black-tea
+```
+* [Programs List](https://github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md)
+
 ### Message
 
 
 ```console
 mytimer --minute=7 --second=30 --message="Test message"
 ```
 		
@@ -168,15 +175,20 @@
 Just fill an issue and describe it. We'll check it ASAP!
 
 - Please complete the issue template
  			
 
 ## References
 
-<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a> </blockquote>
+<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a></blockquote>
+
+<blockquote>2- <a href="https://www.online-timers.com/">Online Timer</a></blockquote>
+
+<blockquote>3- <a href="https://www.mediacollege.com/">Media College</a></blockquote>
+
 
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
```

#### html2text {}

```diff
@@ -30,35 +30,38 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.5](https://github.com/
-sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+## Installation ### Source Code - Download [Version 0.6](https://github.com/
+sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
 Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
-`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
-`mytimer` or `python -m mytimer` to run this program ### Version ```console
-mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
-mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
-```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
-mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
-```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
-mode may not be supported on all systems ```console mytimer --minute=7 --
-second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
-second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
-mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
-second=30 --message="Test message" ```
+`pip install mytimer==0.6` ## Usage â ï¸ You can use `mytimer` or `python -
+m mytimer` to run this program ### Version ```console mytimer --version ``` ###
+Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
+```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
+minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
+mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
+second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
+systems ```console mytimer --minute=7 --second=30 --countdown --alarm ``` ###
+Face ```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List]
+(https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md) ### Program
+```console mytimer --program=black-tea ``` * [Programs List](https://
+github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md) ### Message ```console
+mytimer --minute=7 --second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
+     2- Online_Timer
+     3- Media_College
 ## Show your support
 **** Star this repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to our project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
```

### Comparing `mytimer-0.5/mytimer/sounds/alarm.wav` & `mytimer-0.6/mytimer/sounds/2.wav`

 * *Files identical despite different names*

### Comparing `mytimer-0.5/mytimer.egg-info/PKG-INFO` & `mytimer-0.6/mytimer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 0.5
+Version: 0.6
 Summary: Simple Timer for Your Terminal
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.5
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v0.6
 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
@@ -111,21 +111,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 0.5](https://github.com/sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 0.6](https://github.com/sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==0.5` (Need root access)							
+- `pip install mytimer==0.6`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -177,14 +177,21 @@
 
 ```console
 mytimer --minute=7 --second=30 --face=3
 ```
 * [Faces List](https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md)
 
 
+### Program
+
+```console
+mytimer --program=black-tea
+```
+* [Programs List](https://github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md)
+
 ### Message
 
 
 ```console
 mytimer --minute=7 --second=30 --message="Test message"
 ```
 		
@@ -202,15 +209,20 @@
 Just fill an issue and describe it. We'll check it ASAP!
 
 - Please complete the issue template
  			
 
 ## References
 
-<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a> </blockquote>
+<blockquote>1- <a href="https://mixkit.co/free-sound-effects/alarm/">Mixkit Free Alarm Sound Effects</a></blockquote>
+
+<blockquote>2- <a href="https://www.online-timers.com/">Online Timer</a></blockquote>
+
+<blockquote>3- <a href="https://www.mediacollege.com/">Media College</a></blockquote>
+
 
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
 
@@ -247,14 +259,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.6] - 2023-07-04
+### Added
+- `--program` argument
+- `PROGRAMS.md`
+- `run_timer` function
+### Changed
+- Inputs type changed to `int`
+- `README.md` updated
+- `WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE`
+- Alarm tone changed
 ## [0.5] - 2023-05-25
 ### Added
 - 5 new faces
 - `--message` argument
 ### Changed
 - `play_sound` function modified
 - `playsound` removed from `requirements.txt`
@@ -282,15 +304,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...dev
+[0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
 [0.5]: https://github.com/sepandhaghighi/mytimer/compare/v0.4...v0.5
 [0.4]: https://github.com/sepandhaghighi/mytimer/compare/v0.3...v0.4
 [0.3]: https://github.com/sepandhaghighi/mytimer/compare/v0.2...v0.3
 [0.2]: https://github.com/sepandhaghighi/mytimer/compare/v0.1...v0.2
 [0.1]: https://github.com/sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: mytimer Version: 0.5 Summary: Simple Timer for Your
+Metadata-Version: 2.1 Name: mytimer Version: 0.6 Summary: Simple Timer for Your
 Terminal Home-page: https://github.com/sepandhaghighi/mytimer Download-URL:
-https://github.com/sepandhaghighi/mytimer/tarball/v0.5 Author: Sepand Haghighi
+https://github.com/sepandhaghighi/mytimer/tarball/v0.6 Author: Sepand Haghighi
 Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source, https://
 github.com/sepandhaghighi/mytimer Keywords: python3 python timer terminal
 stopwatch Classifier: Development Status :: 4 - Beta Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -48,35 +48,38 @@
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
    CI         mytimer/workflows/CI/               mytimer/workflows/CI/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           [https://app.codacy.com/project/
 Code Quality [CodeFactor]           badge/Grade/            [codebeat_badge]
                           1bf28500431a498998ac79891cd79cda]
-## Installation ### Source Code - Download [Version 0.5](https://github.com/
-sepandhaghighi/mytimer/archive/v0.5.zip) or [Latest Source ](https://
+## Installation ### Source Code - Download [Version 0.6](https://github.com/
+sepandhaghighi/mytimer/archive/v0.6.zip) or [Latest Source ](https://
 github.com/sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI -
 Check [Python Packaging User Guide](https://packaging.python.org/installing/) -
-`pip install mytimer==0.5` (Need root access) ## Usage â ï¸ You can use
-`mytimer` or `python -m mytimer` to run this program ### Version ```console
-mytimer --version ``` ### Basic â ï¸ Press `Ctrl + C` to exit ```console
-mytimer ``` ### Time Limit ```console mytimer --minute=7 --second=30 ```
-```console mytimer --hour=2 --minute=20 ``` ### Timer Mode â ï¸ The default
-mode is `count-up` ```console mytimer --minute=7 --second=30 --countdown ```
-```console mytimer --minute=7 --second=30 --countup ``` ### Alarm â ï¸ This
-mode may not be supported on all systems ```console mytimer --minute=7 --
-second=30 --countdown --alarm ``` ### Face ```console mytimer --minute=7 --
-second=30 --face=3 ``` * [Faces List](https://github.com/sepandhaghighi/
-mytimer/blob/main/FACES.md) ### Message ```console mytimer --minute=7 --
-second=30 --message="Test message" ```
+`pip install mytimer==0.6` ## Usage â ï¸ You can use `mytimer` or `python -
+m mytimer` to run this program ### Version ```console mytimer --version ``` ###
+Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
+```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
+minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
+mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
+second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
+systems ```console mytimer --minute=7 --second=30 --countdown --alarm ``` ###
+Face ```console mytimer --minute=7 --second=30 --face=3 ``` * [Faces List]
+(https://github.com/sepandhaghighi/mytimer/blob/main/FACES.md) ### Program
+```console mytimer --program=black-tea ``` * [Programs List](https://
+github.com/sepandhaghighi/mytimer/blob/main/PROGRAMS.md) ### Message ```console
+mytimer --minute=7 --second=30 --message="Test message" ```
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/help.gif]
                                  Screen Record
 ## Issues & Bug Reports Just fill an issue and describe it. We'll check it
 ASAP! - Please complete the issue template ## References
      1- Mixkit_Free_Alarm_Sound_Effects
+     2- Online_Timer
+     3- Media_College
 ## Show your support
 **** Star this repo ****
  Give a â­ï¸ if this project helped you!
 **** Donate to our project ****
 *** Bitcoin ***
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 *** Ethereum ***
@@ -100,23 +103,27 @@
 *** Zilliqa ***
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 *** Coffeete ***
 [http://www.coffeete.ir/images/buttons/lemonchiffon.png] # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
+## [Unreleased] ## [0.6] - 2023-07-04 ### Added - `--program` argument -
+`PROGRAMS.md` - `run_timer` function ### Changed - Inputs type changed to `int`
+- `README.md` updated - `WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE` -
+Alarm tone changed ## [0.5] - 2023-05-25 ### Added - 5 new faces - `--message`
 argument ### Changed - `play_sound` function modified - `playsound` removed
 from `requirements.txt` - `README.md` updated ## [0.4] - 2023-02-10 ### Added -
 4 new faces - Infinite timer mode ### Changed - `README.md` updated -
 Parameters moved to `params.py` ## [0.3] - 2022-11-25 ### Added - `--face`
 argument - `FACES.md` ### Changed - `README.md` updated - Minimum `art` library
 version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03 ### Added - `--
 version` flag ### Changed - Test system modified - `countdown_timer` function
 modified - `countup_timer` function modified ## [0.1] - 2022-10-18 ### Added -
 Countdown mode - Count-up mode - Alarm [Unreleased]: https://github.com/
-sepandhaghighi/mytimer/compare/v0.5...dev [0.5]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.6...dev [0.6]: https://github.com/
+sepandhaghighi/mytimer/compare/v0.5...v0.6 [0.5]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.4...v0.5 [0.4]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.3...v0.4 [0.3]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.2...v0.3 [0.2]: https://github.com/
 sepandhaghighi/mytimer/compare/v0.1...v0.2 [0.1]: https://github.com/
 sepandhaghighi/mytimer/compare/daa2be6...v0.1
```

### Comparing `mytimer-0.5/setup.py` & `mytimer-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     except Exception:
         return '''Simple Timer for Your Terminal'''
 
 
 setup(
     name='mytimer',
     packages=['mytimer'],
-    version='0.5',
+    version='0.6',
     description='Simple Timer for Your Terminal',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='Sepand Haghighi',
     author_email='sepand@pyrgg.ir',
     url='https://github.com/sepandhaghighi/mytimer',
-    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v0.5',
+    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v0.6',
     keywords="python3 python timer terminal stopwatch",
     project_urls={
         'Source': 'https://github.com/sepandhaghighi/mytimer'
     },
     install_requires=get_requires(),
     python_requires='>=3.5',
     classifiers=[
```

