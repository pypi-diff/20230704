# Comparing `tmp/python-aternos-3.0.1.tar.gz` & `tmp/python-aternos-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aternos-3.0.1.tar", last modified: Fri Jun 30 06:55:05 2023, max compression
+gzip compressed data, was "python-aternos-3.0.2.tar", last modified: Tue Jul  4 10:29:52 2023, max compression
```

## Comparing `python-aternos-3.0.1.tar` & `python-aternos-3.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.1/LICENSE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.1/NOTICE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7161 2023-06-30 06:55:05.988202 python-aternos-3.0.1/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5925 2023-06-30 05:54:30.000000 python-aternos-3.0.1/README.md
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.1/pyproject.toml
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/python_aternos/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.1/python_aternos/__init__.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.1/python_aternos/ataccount.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.1/python_aternos/atclient.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.1/python_aternos/atconf.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-06-30 06:02:26.000000 python-aternos-3.0.1/python_aternos/atconnect.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.1/python_aternos/aterrors.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.1/python_aternos/atfile.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.1/python_aternos/atfm.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5849 2023-06-30 06:20:51.000000 python-aternos-3.0.1/python_aternos/atjsparse.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.1/python_aternos/atlog.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.1/python_aternos/atmd5.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3311 2023-05-24 15:57:21.000000 python-aternos-3.0.1/python_aternos/atplayers.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.1/python_aternos/atserver.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.1/python_aternos/atwss.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/python_aternos.egg-info/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7161 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/SOURCES.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/dependency_links.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      254 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/requires.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/top_level.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-06-30 06:55:05.988202 python-aternos-3.0.1/setup.cfg
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2043 2023-06-30 06:54:38.000000 python-aternos-3.0.1/setup.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/tests/
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.1/tests/test_http.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.1/tests/test_js2py.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.1/tests/test_jsnode.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.1/tests/test_login.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.116984 python-aternos-3.0.2/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.2/LICENSE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.2/NOTICE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7217 2023-07-04 10:29:52.116984 python-aternos-3.0.2/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5930 2023-07-04 10:24:44.000000 python-aternos-3.0.2/README.md
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.2/pyproject.toml
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/python_aternos/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.2/python_aternos/__init__.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.2/python_aternos/ataccount.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.2/python_aternos/atclient.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.2/python_aternos/atconf.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-06-30 06:02:26.000000 python-aternos-3.0.2/python_aternos/atconnect.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.2/python_aternos/aterrors.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.2/python_aternos/atfile.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.2/python_aternos/atfm.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5849 2023-06-30 06:20:51.000000 python-aternos-3.0.2/python_aternos/atjsparse.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.2/python_aternos/atlog.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.2/python_aternos/atmd5.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3329 2023-07-04 10:14:56.000000 python-aternos-3.0.2/python_aternos/atplayers.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.2/python_aternos/atserver.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.2/python_aternos/atwss.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/python_aternos.egg-info/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7217 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/SOURCES.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/dependency_links.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      283 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/requires.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/top_level.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-07-04 10:29:52.116984 python-aternos-3.0.2/setup.cfg
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2139 2023-07-04 10:23:41.000000 python-aternos-3.0.2/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/tests/
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.2/tests/test_http.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.2/tests/test_js2py.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.2/tests/test_jsnode.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.2/tests/test_login.py
```

### Comparing `python-aternos-3.0.1/LICENSE` & `python-aternos-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/NOTICE` & `python-aternos-3.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/PKG-INFO` & `python-aternos-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.1
+Version: 3.0.2
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
@@ -90,15 +91,15 @@
 > if you have problems with it, and then execute:  
 > `pip install --no-deps python-aternos`
 
 ### Development
 ```bash
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
-$ pip install -e .
+$ pip install -e .[dev]
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
 and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.1 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.2 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-:: Linux Classifier: Operating System :: MacOS Classifier: Intended Audience ::
-Developers Classifier: Topic :: Internet Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: pypi Provides-Extra: docs License-File: LICENSE License-File:
-NOTICE
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Classifier: Operating System :: Microsoft ::
+Windows Classifier: Operating System :: POSIX :: Linux Classifier: Operating
+System :: MacOS Classifier: Intended Audience :: Developers Classifier: Topic
+:: Internet Classifier: Typing :: Typed Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: pypi Provides-
+Extra: docs License-File: LICENSE License-File: NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
 aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
@@ -36,21 +36,21 @@
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
-``` ## Usage To use Aternos API in your Python script, import it and login with
-your username and password or its MD5 hash. Then request the servers list using
-`list_servers()`. You can start/stop your Aternos server, calling `start()` or
-`stop()`. Here is an example how to use the API: ```python # Import from
-python_aternos import Client # Create object atclient = Client() # Log in #
-with username and password atclient.login('example', 'test123') # ----OR---- #
-with username and MD5 hashed password atclient.login_hashed('example',
+[dev] ``` ## Usage To use Aternos API in your Python script, import it and
+login with your username and password or its MD5 hash. Then request the servers
+list using `list_servers()`. You can start/stop your Aternos server, calling
+`start()` or `stop()`. Here is an example how to use the API: ```python #
+Import from python_aternos import Client # Create object atclient = Client() #
+Log in # with username and password atclient.login('example', 'test123') # ----
+OR---- # with username and MD5 hashed password atclient.login_hashed('example',
 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
 atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
 AternosAccount object aternos = atclient.account # Get servers list servs =
 aternos.list_servers() # Get the first server myserv = servs[0] # Start
 myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
 None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
 if testserv is not None: # Prints the server software and its version # (for
```

### Comparing `python-aternos-3.0.1/README.md` & `python-aternos-3.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 > if you have problems with it, and then execute:  
 > `pip install --no-deps python-aternos`
 
 ### Development
 ```bash
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
-$ pip install -e .
+$ pip install -e .[dev]
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
 and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.
```

#### html2text {}

```diff
@@ -19,21 +19,21 @@
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
-``` ## Usage To use Aternos API in your Python script, import it and login with
-your username and password or its MD5 hash. Then request the servers list using
-`list_servers()`. You can start/stop your Aternos server, calling `start()` or
-`stop()`. Here is an example how to use the API: ```python # Import from
-python_aternos import Client # Create object atclient = Client() # Log in #
-with username and password atclient.login('example', 'test123') # ----OR---- #
-with username and MD5 hashed password atclient.login_hashed('example',
+[dev] ``` ## Usage To use Aternos API in your Python script, import it and
+login with your username and password or its MD5 hash. Then request the servers
+list using `list_servers()`. You can start/stop your Aternos server, calling
+`start()` or `stop()`. Here is an example how to use the API: ```python #
+Import from python_aternos import Client # Create object atclient = Client() #
+Log in # with username and password atclient.login('example', 'test123') # ----
+OR---- # with username and MD5 hashed password atclient.login_hashed('example',
 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
 atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
 AternosAccount object aternos = atclient.account # Get servers list servs =
 aternos.list_servers() # Get the first server myserv = servs[0] # Start
 myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
 None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
 if testserv is not None: # Prints the server software and its version # (for
```

### Comparing `python-aternos-3.0.1/python_aternos/ataccount.py` & `python-aternos-3.0.2/python_aternos/ataccount.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atclient.py` & `python-aternos-3.0.2/python_aternos/atclient.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atconf.py` & `python-aternos-3.0.2/python_aternos/atconf.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atconnect.py` & `python-aternos-3.0.2/python_aternos/atconnect.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/aterrors.py` & `python-aternos-3.0.2/python_aternos/aterrors.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atfile.py` & `python-aternos-3.0.2/python_aternos/atfile.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atfm.py` & `python-aternos-3.0.2/python_aternos/atfm.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atjsparse.py` & `python-aternos-3.0.2/python_aternos/atjsparse.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atlog.py` & `python-aternos-3.0.2/python_aternos/atlog.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atplayers.py` & `python-aternos-3.0.2/python_aternos/atplayers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         """Appends a player to the list by the nickname
 
         Args:
             name (str): Player's nickname
         """
 
         self.atserv.atserver_request(
-            f'{AJAX_URL}/players/add.php',
+            f'{AJAX_URL}/server/players/lists/add',
             'POST', data={
                 'list': self.lst.value,
                 'name': name
             }, sendtoken=True
         )
 
         self.players.append(name)
@@ -112,15 +112,15 @@
         """Removes a player from the list by the nickname
 
         Args:
             name (str): Player's nickname
         """
 
         self.atserv.atserver_request(
-            f'{AJAX_URL}/players/remove.php',
+            f'{AJAX_URL}/server/players/lists/remove',
             'POST', data={
                 'list': self.lst.value,
                 'name': name
             }, sendtoken=True
         )
 
         for i, j in enumerate(self.players):
```

### Comparing `python-aternos-3.0.1/python_aternos/atserver.py` & `python-aternos-3.0.2/python_aternos/atserver.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos/atwss.py` & `python-aternos-3.0.2/python_aternos/atwss.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/python_aternos.egg-info/PKG-INFO` & `python-aternos-3.0.2/python_aternos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.1
+Version: 3.0.2
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
@@ -90,15 +91,15 @@
 > if you have problems with it, and then execute:  
 > `pip install --no-deps python-aternos`
 
 ### Development
 ```bash
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
-$ pip install -e .
+$ pip install -e .[dev]
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
 and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.1 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.2 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-:: Linux Classifier: Operating System :: MacOS Classifier: Intended Audience ::
-Developers Classifier: Topic :: Internet Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: pypi Provides-Extra: docs License-File: LICENSE License-File:
-NOTICE
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Classifier: Operating System :: Microsoft ::
+Windows Classifier: Operating System :: POSIX :: Linux Classifier: Operating
+System :: MacOS Classifier: Intended Audience :: Developers Classifier: Topic
+:: Internet Classifier: Typing :: Typed Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: pypi Provides-
+Extra: docs License-File: LICENSE License-File: NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
 aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
@@ -36,21 +36,21 @@
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
-``` ## Usage To use Aternos API in your Python script, import it and login with
-your username and password or its MD5 hash. Then request the servers list using
-`list_servers()`. You can start/stop your Aternos server, calling `start()` or
-`stop()`. Here is an example how to use the API: ```python # Import from
-python_aternos import Client # Create object atclient = Client() # Log in #
-with username and password atclient.login('example', 'test123') # ----OR---- #
-with username and MD5 hashed password atclient.login_hashed('example',
+[dev] ``` ## Usage To use Aternos API in your Python script, import it and
+login with your username and password or its MD5 hash. Then request the servers
+list using `list_servers()`. You can start/stop your Aternos server, calling
+`start()` or `stop()`. Here is an example how to use the API: ```python #
+Import from python_aternos import Client # Create object atclient = Client() #
+Log in # with username and password atclient.login('example', 'test123') # ----
+OR---- # with username and MD5 hashed password atclient.login_hashed('example',
 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
 atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
 AternosAccount object aternos = atclient.account # Get servers list servs =
 aternos.list_servers() # Get the first server myserv = servs[0] # Start
 myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
 None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
 if testserv is not None: # Prints the server software and its version # (for
```

### Comparing `python-aternos-3.0.1/python_aternos.egg-info/SOURCES.txt` & `python-aternos-3.0.2/python_aternos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/setup.py` & `python-aternos-3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name='python-aternos',
-    version='3.0.1',
+    version='3.0.2',
     author='Chechkenev Andrey (@DarkCat09)',
     author_email='aacd0709@mail.ru',
     description='An unofficial Aternos API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DarkCat09/python-aternos',
     project_urls={
@@ -20,14 +20,15 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Intended Audience :: Developers',
         'Topic :: Internet',
@@ -51,13 +52,14 @@
         ],
         'pypi': [
             'build==0.10.0',
             'twine==4.0.2',
         ],
         'docs': [
             'mkdocs==1.4.3',
+            'mkdocstrings[python]==0.22.0',
         ]
     },
     packages=['python_aternos'],
     python_requires=">=3.7",
     include_package_data=True,
 )
```

### Comparing `python-aternos-3.0.1/tests/test_http.py` & `python-aternos-3.0.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/tests/test_js2py.py` & `python-aternos-3.0.2/tests/test_js2py.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/tests/test_jsnode.py` & `python-aternos-3.0.2/tests/test_jsnode.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.1/tests/test_login.py` & `python-aternos-3.0.2/tests/test_login.py`

 * *Files identical despite different names*

