# Comparing `tmp/python-aternos-3.0.2.tar.gz` & `tmp/python-aternos-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aternos-3.0.2.tar", last modified: Tue Jul  4 10:29:52 2023, max compression
+gzip compressed data, was "python-aternos-3.0.3.tar", last modified: Tue Jul  4 10:57:30 2023, max compression
```

## Comparing `python-aternos-3.0.2.tar` & `python-aternos-3.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.116984 python-aternos-3.0.2/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.2/LICENSE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.2/NOTICE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7217 2023-07-04 10:29:52.116984 python-aternos-3.0.2/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5930 2023-07-04 10:24:44.000000 python-aternos-3.0.2/README.md
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.2/pyproject.toml
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/python_aternos/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.2/python_aternos/__init__.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.2/python_aternos/ataccount.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.2/python_aternos/atclient.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.2/python_aternos/atconf.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-06-30 06:02:26.000000 python-aternos-3.0.2/python_aternos/atconnect.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.2/python_aternos/aterrors.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.2/python_aternos/atfile.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.2/python_aternos/atfm.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5849 2023-06-30 06:20:51.000000 python-aternos-3.0.2/python_aternos/atjsparse.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.2/python_aternos/atlog.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.2/python_aternos/atmd5.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3329 2023-07-04 10:14:56.000000 python-aternos-3.0.2/python_aternos/atplayers.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.2/python_aternos/atserver.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.2/python_aternos/atwss.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/python_aternos.egg-info/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7217 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/SOURCES.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/dependency_links.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      283 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/requires.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-07-04 10:29:52.000000 python-aternos-3.0.2/python_aternos.egg-info/top_level.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-07-04 10:29:52.116984 python-aternos-3.0.2/setup.cfg
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2139 2023-07-04 10:23:41.000000 python-aternos-3.0.2/setup.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:29:52.113650 python-aternos-3.0.2/tests/
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.2/tests/test_http.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.2/tests/test_js2py.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.2/tests/test_jsnode.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.2/tests/test_login.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.3/LICENSE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.3/NOTICE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-04 10:57:30.170874 python-aternos-3.0.3/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5818 2023-07-04 10:56:37.000000 python-aternos-3.0.3/README.md
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.3/pyproject.toml
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/python_aternos/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.3/python_aternos/__init__.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.3/python_aternos/ataccount.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.3/python_aternos/atclient.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.3/python_aternos/atconf.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-07-04 10:42:47.000000 python-aternos-3.0.3/python_aternos/atconnect.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.3/python_aternos/aterrors.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.3/python_aternos/atfile.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.3/python_aternos/atfm.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5888 2023-07-04 10:44:31.000000 python-aternos-3.0.3/python_aternos/atjsparse.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      579 2023-07-04 10:47:12.000000 python-aternos-3.0.3/python_aternos/atlog.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.3/python_aternos/atmd5.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3329 2023-07-04 10:42:58.000000 python-aternos-3.0.3/python_aternos/atplayers.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.3/python_aternos/atserver.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.3/python_aternos/atwss.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/python_aternos.egg-info/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7105 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/SOURCES.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/dependency_links.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      283 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/requires.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-07-04 10:57:30.000000 python-aternos-3.0.3/python_aternos.egg-info/top_level.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-07-04 10:57:30.170874 python-aternos-3.0.3/setup.cfg
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2139 2023-07-04 10:47:42.000000 python-aternos-3.0.3/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-07-04 10:57:30.170874 python-aternos-3.0.3/tests/
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.3/tests/test_http.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.3/tests/test_js2py.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.3/tests/test_jsnode.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.3/tests/test_login.py
```

### Comparing `python-aternos-3.0.2/LICENSE` & `python-aternos-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/NOTICE` & `python-aternos-3.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/PKG-INFO` & `python-aternos-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.2
+Version: 3.0.3
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -53,23 +53,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 > **WARNING**
 >
-> Recently, Aternos started somehow detecting
-> API requests from this library.
-> Any automated access is prohibited according
-> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**.
+> Aternos now trying to detect python-aternos requests
+> by finding bugs in custom JavaScript parser.
 >
-> **USE AT YOUR OWN RISK**
+> Please, always keep the library up-to-date.
 >
-> I will try to fix that as soon as possible.
+> I'm going to use Selenium in this library later
+> (but you'll still be able to choose between
+> lightweight HTML parsing and running a browser).
 
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.2 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.3 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -17,27 +17,25 @@
 Extra: docs License-File: LICENSE License-File: NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
-Aternos started somehow detecting > API requests from this library. > Any
-automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
-/aternos.gmbh/en/aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
-to fix that as soon as possible. Python Aternos supports: - Logging in to
-account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
-Saving session to the file and restoring - Changing username, email and
-password - Parsing Minecraft servers list - Parsing server info by its ID -
-Starting/stoping server, restarting, confirming/cancelling launch - Updating
-server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
-websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+aternos.org/)' private API and html parsing. > **WARNING** > > Aternos now
+trying to detect python-aternos requests > by finding bugs in custom JavaScript
+parser. > > Please, always keep the library up-to-date. > > I'm going to use
+Selenium in this library later > (but you'll still be able to choose between >
+lightweight HTML parsing and running a browser). Python Aternos supports: -
+Logging in to account with password (plain or hashed) or `ATERNOS_SESSION`
+cookie value - Saving session to the file and restoring - Changing username,
+email and password - Parsing Minecraft servers list - Parsing server info by
+its ID - Starting/stoping server, restarting, confirming/cancelling launch -
+Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/
+howto/websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
 [dev] ``` ## Usage To use Aternos API in your Python script, import it and
```

### Comparing `python-aternos-3.0.2/README.md` & `python-aternos-3.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 > **WARNING**
 >
-> Recently, Aternos started somehow detecting
-> API requests from this library.
-> Any automated access is prohibited according
-> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**.
+> Aternos now trying to detect python-aternos requests
+> by finding bugs in custom JavaScript parser.
 >
-> **USE AT YOUR OWN RISK**
+> Please, always keep the library up-to-date.
 >
-> I will try to fix that as soon as possible.
+> I'm going to use Selenium in this library later
+> (but you'll still be able to choose between
+> lightweight HTML parsing and running a browser).
 
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,26 +1,24 @@
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
-Aternos started somehow detecting > API requests from this library. > Any
-automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
-/aternos.gmbh/en/aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
-to fix that as soon as possible. Python Aternos supports: - Logging in to
-account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
-Saving session to the file and restoring - Changing username, email and
-password - Parsing Minecraft servers list - Parsing server info by its ID -
-Starting/stoping server, restarting, confirming/cancelling launch - Updating
-server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
-websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+aternos.org/)' private API and html parsing. > **WARNING** > > Aternos now
+trying to detect python-aternos requests > by finding bugs in custom JavaScript
+parser. > > Please, always keep the library up-to-date. > > I'm going to use
+Selenium in this library later > (but you'll still be able to choose between >
+lightweight HTML parsing and running a browser). Python Aternos supports: -
+Logging in to account with password (plain or hashed) or `ATERNOS_SESSION`
+cookie value - Saving session to the file and restoring - Changing username,
+email and password - Parsing Minecraft servers list - Parsing server info by
+its ID - Starting/stoping server, restarting, confirming/cancelling launch -
+Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/
+howto/websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
 [dev] ``` ## Usage To use Aternos API in your Python script, import it and
```

### Comparing `python-aternos-3.0.2/python_aternos/ataccount.py` & `python-aternos-3.0.3/python_aternos/ataccount.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atclient.py` & `python-aternos-3.0.3/python_aternos/atclient.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atconf.py` & `python-aternos-3.0.3/python_aternos/atconf.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atconnect.py` & `python-aternos-3.0.3/python_aternos/atconnect.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/aterrors.py` & `python-aternos-3.0.3/python_aternos/aterrors.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atfile.py` & `python-aternos-3.0.3/python_aternos/atfile.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atfm.py` & `python-aternos-3.0.3/python_aternos/atfm.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atjsparse.py` & `python-aternos-3.0.3/python_aternos/atjsparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
         ctx.execute('''
         window.Map = function(_i){ };
         window.setTimeout = function(_f,_t){ };
         window.setInterval = function(_f,_t){ };
         window.encodeURIComponent = function(_s){ };
         window.document = { };
         document.doctype = { };
+        document.currentScript = { };
         document.getElementById = function(_s){ };
         ''')
 
         self.ctx = ctx
 
     def exec_js(self, func: str) -> None:
         self.ctx.execute(self.to_ecma5(func))
```

### Comparing `python-aternos-3.0.2/python_aternos/atlog.py` & `python-aternos-3.0.3/python_aternos/atlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Creates a logger"""
 
 import logging
 
 
 log = logging.getLogger('aternos')
 handler = logging.StreamHandler()
-fmt = logging.Formatter('%(asctime)s %(levelname)s %(message)s')
+fmt = logging.Formatter('%(asctime)s %(levelname)-5s %(message)s')
 
 handler.setFormatter(fmt)
 log.addHandler(handler)
 
 
 def is_debug() -> bool:
     """Is debug logging enabled"""
```

### Comparing `python-aternos-3.0.2/python_aternos/atplayers.py` & `python-aternos-3.0.3/python_aternos/atplayers.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atserver.py` & `python-aternos-3.0.3/python_aternos/atserver.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos/atwss.py` & `python-aternos-3.0.3/python_aternos/atwss.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/python_aternos.egg-info/PKG-INFO` & `python-aternos-3.0.3/python_aternos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.2
+Version: 3.0.3
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -53,23 +53,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 > **WARNING**
 >
-> Recently, Aternos started somehow detecting
-> API requests from this library.
-> Any automated access is prohibited according
-> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**.
+> Aternos now trying to detect python-aternos requests
+> by finding bugs in custom JavaScript parser.
 >
-> **USE AT YOUR OWN RISK**
+> Please, always keep the library up-to-date.
 >
-> I will try to fix that as soon as possible.
+> I'm going to use Selenium in this library later
+> (but you'll still be able to choose between
+> lightweight HTML parsing and running a browser).
 
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.2 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.3 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -17,27 +17,25 @@
 Extra: docs License-File: LICENSE License-File: NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
-Aternos started somehow detecting > API requests from this library. > Any
-automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
-/aternos.gmbh/en/aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
-to fix that as soon as possible. Python Aternos supports: - Logging in to
-account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
-Saving session to the file and restoring - Changing username, email and
-password - Parsing Minecraft servers list - Parsing server info by its ID -
-Starting/stoping server, restarting, confirming/cancelling launch - Updating
-server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
-websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+aternos.org/)' private API and html parsing. > **WARNING** > > Aternos now
+trying to detect python-aternos requests > by finding bugs in custom JavaScript
+parser. > > Please, always keep the library up-to-date. > > I'm going to use
+Selenium in this library later > (but you'll still be able to choose between >
+lightweight HTML parsing and running a browser). Python Aternos supports: -
+Logging in to account with password (plain or hashed) or `ATERNOS_SESSION`
+cookie value - Saving session to the file and restoring - Changing username,
+email and password - Parsing Minecraft servers list - Parsing server info by
+its ID - Starting/stoping server, restarting, confirming/cancelling launch -
+Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/
+howto/websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
 Managing files, settings, players (whitelist, operators, etc.) ## Install ###
 Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
 > Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
 pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
 install --no-deps python-aternos` ### Development ```bash $ git clone https://
 github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
 [dev] ``` ## Usage To use Aternos API in your Python script, import it and
```

### Comparing `python-aternos-3.0.2/python_aternos.egg-info/SOURCES.txt` & `python-aternos-3.0.3/python_aternos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/setup.py` & `python-aternos-3.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name='python-aternos',
-    version='3.0.2',
+    version='3.0.3',
     author='Chechkenev Andrey (@DarkCat09)',
     author_email='aacd0709@mail.ru',
     description='An unofficial Aternos API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DarkCat09/python-aternos',
     project_urls={
```

### Comparing `python-aternos-3.0.2/tests/test_http.py` & `python-aternos-3.0.3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/tests/test_js2py.py` & `python-aternos-3.0.3/tests/test_js2py.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/tests/test_jsnode.py` & `python-aternos-3.0.3/tests/test_jsnode.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.2/tests/test_login.py` & `python-aternos-3.0.3/tests/test_login.py`

 * *Files identical despite different names*

