# Comparing `tmp/pyHB-0.3.tar.gz` & `tmp/pyHB-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHB-0.3.tar", last modified: Sun Jul  2 05:33:25 2023, max compression
+gzip compressed data, was "pyHB-0.4.tar", last modified: Tue Jul  4 05:35:17 2023, max compression
```

## Comparing `pyHB-0.3.tar` & `pyHB-0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.471655 pyHB-0.3/
-drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.442114 pyHB-0.3/HB/
--rw-rw-rw-   0        0        0       45 2023-07-02 05:23:02.000000 pyHB-0.3/HB/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-07-02 05:23:02.000000 pyHB-0.3/HB/data.py
--rw-rw-rw-   0        0        0    18587 2023-07-02 05:23:02.000000 pyHB-0.3/HB/functions.py
--rw-rw-rw-   0        0        0       20 2023-07-02 05:23:02.000000 pyHB-0.3/HB/version.py
--rw-rw-rw-   0        0        0    35149 2023-07-02 05:23:01.000000 pyHB-0.3/LICENSE
--rw-rw-rw-   0        0        0      981 2023-07-02 05:33:25.469656 pyHB-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-02 05:23:01.000000 pyHB-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 05:33:25.466649 pyHB-0.3/pyHB.egg-info/
--rw-rw-rw-   0        0        0      981 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-07-02 05:33:25.000000 pyHB-0.3/pyHB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 05:33:25.471655 pyHB-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1555 2023-07-02 05:23:01.000000 pyHB-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/HB/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 05:35:06.000000 pyHB-0.4/HB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-04 05:35:06.000000 pyHB-0.4/HB/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-07-04 05:35:06.000000 pyHB-0.4/HB/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-04 05:35:06.000000 pyHB-0.4/HB/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 05:35:06.000000 pyHB-0.4/HB/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 05:35:06.000000 pyHB-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-04 05:35:17.605628 pyHB-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 05:35:06.000000 pyHB-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/pyHB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:35:17.609628 pyHB-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-04 05:35:06.000000 pyHB-0.4/setup.py
```

### Comparing `pyHB-0.3/HB/data.py` & `pyHB-0.4/HB/data.py`

 * *Files identical despite different names*

### Comparing `pyHB-0.3/HB/functions.py` & `pyHB-0.4/HB/functions.py`

 * *Files identical despite different names*

### Comparing `pyHB-0.3/LICENSE` & `pyHB-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHB-0.3/PKG-INFO` & `pyHB-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: pyHB
-Version: 0.3
-Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
-Home-page: https://github.com/LEGEND-AI/pyHB
-Author: LegendBoy
-Author-email: krishna045jaiswal@gmail.com
-License: GNU General Public License v3.0
-Keywords: pyHB,HB
-Classifier: Framework :: AsyncIO
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyHB
-
-Credit to LegendBoy_OP
+Metadata-Version: 2.1
+Name: pyHB
+Version: 0.4
+Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
+Home-page: https://github.com/LEGEND-AI/pyHB
+Author: LegendBoy
+Author-email: krishna045jaiswal@gmail.com
+License: GNU General Public License v3.0
+Keywords: pyHB,HB
+Classifier: Framework :: AsyncIO
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyHB
+
+Credit to LegendBoy_OP
```

### Comparing `pyHB-0.3/pyHB.egg-info/PKG-INFO` & `pyHB-0.4/pyHB.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: pyHB
-Version: 0.3
-Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
-Home-page: https://github.com/LEGEND-AI/pyHB
-Author: LegendBoy
-Author-email: krishna045jaiswal@gmail.com
-License: GNU General Public License v3.0
-Keywords: pyHB,HB
-Classifier: Framework :: AsyncIO
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyHB
-
-Credit to LegendBoy_OP
+Metadata-Version: 2.1
+Name: pyHB
+Version: 0.4
+Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
+Home-page: https://github.com/LEGEND-AI/pyHB
+Author: LegendBoy
+Author-email: krishna045jaiswal@gmail.com
+License: GNU General Public License v3.0
+Keywords: pyHB,HB
+Classifier: Framework :: AsyncIO
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyHB
+
+Credit to LegendBoy_OP
```

### Comparing `pyHB-0.3/setup.py` & `pyHB-0.4/setup.py`

 * *Files identical despite different names*

