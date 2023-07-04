# Comparing `tmp/gutenberg2kindle-0.4.0.tar.gz` & `tmp/gutenberg2kindle-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gutenberg2kindle-0.4.0.tar", max compression
+gzip compressed data, was "gutenberg2kindle-0.5.0.tar", max compression
```

## Comparing `gutenberg2kindle-0.4.0.tar` & `gutenberg2kindle-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2023-05-01 05:47:57.287656 gutenberg2kindle-0.4.0/LICENSE
--rw-r--r--   0        0        0     2611 2023-05-01 05:47:57.287842 gutenberg2kindle-0.4.0/README.md
--rw-r--r--   0        0        0      137 2023-05-14 19:15:45.358842 gutenberg2kindle-0.4.0/gutenberg2kindle/__init__.py
--rw-r--r--   0        0        0     4924 2023-05-01 05:47:57.288274 gutenberg2kindle-0.4.0/gutenberg2kindle/cli.py
--rw-r--r--   0        0        0     3241 2023-05-01 05:47:57.288366 gutenberg2kindle-0.4.0/gutenberg2kindle/config.py
--rw-r--r--   0        0        0     2217 2023-05-01 05:47:57.288436 gutenberg2kindle-0.4.0/gutenberg2kindle/email.py
--rw-r--r--   0        0        0     1911 2023-05-01 05:47:57.288508 gutenberg2kindle-0.4.0/gutenberg2kindle/gutenberg.py
--rw-r--r--   0        0        0     1378 2023-05-14 19:15:37.642698 gutenberg2kindle-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4038 1970-01-01 00:00:00.000000 gutenberg2kindle-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-01 05:47:57.287656 gutenberg2kindle-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2611 2023-05-01 05:47:57.287842 gutenberg2kindle-0.5.0/README.md
+-rw-r--r--   0        0        0      137 2023-07-04 01:34:08.206600 gutenberg2kindle-0.5.0/gutenberg2kindle/__init__.py
+-rw-r--r--   0        0        0     5191 2023-07-04 01:22:58.268750 gutenberg2kindle-0.5.0/gutenberg2kindle/cli.py
+-rw-r--r--   0        0        0     3241 2023-05-01 05:47:57.288366 gutenberg2kindle-0.5.0/gutenberg2kindle/config.py
+-rw-r--r--   0        0        0     2217 2023-05-01 05:47:57.288436 gutenberg2kindle-0.5.0/gutenberg2kindle/email.py
+-rw-r--r--   0        0        0     1911 2023-05-01 05:47:57.288508 gutenberg2kindle-0.5.0/gutenberg2kindle/gutenberg.py
+-rw-r--r--   0        0        0     1378 2023-07-04 01:20:15.139031 gutenberg2kindle-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4038 1970-01-01 00:00:00.000000 gutenberg2kindle-0.5.0/PKG-INFO
```

### Comparing `gutenberg2kindle-0.4.0/LICENSE` & `gutenberg2kindle-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.4.0/README.md` & `gutenberg2kindle-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.4.0/gutenberg2kindle/cli.py` & `gutenberg2kindle-0.5.0/gutenberg2kindle/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 
 import argparse
 import getpass
 import socket
 import sys
 from typing import Final, Optional, Union
 
+from gutenberg2kindle import __version__
 from gutenberg2kindle.config import (
     AVAILABLE_SETTINGS,
     get_config,
     interactive_config,
     set_config,
     setup_settings,
 )
 from gutenberg2kindle.email import send_book
 from gutenberg2kindle.gutenberg import download_book
 
 COMMAND_SEND: Final[str] = "send"
 COMMAND_GET_CONFIG: Final[str] = "get-config"
 COMMAND_SET_CONFIG: Final[str] = "set-config"
 COMMAND_INTERACTIVE_CONFIG: Final[str] = "interactive-config"
+COMMAND_VERSION: Final[str] = "version"
 AVAILABLE_COMMANDS: Final[list[str]] = [
     COMMAND_SEND,
     COMMAND_GET_CONFIG,
     COMMAND_SET_CONFIG,
     COMMAND_INTERACTIVE_CONFIG,
+    COMMAND_VERSION,
 ]
 
 
 def get_parser() -> argparse.ArgumentParser:
     """
     Generate and return a parser for the CLI tool
     """
@@ -47,15 +50,16 @@
         "command",
         metavar="COMMAND",
         type=str,
         choices=AVAILABLE_COMMANDS,
         help=(
             "Command to use. Supported options allow the user to "
             "either set the tool's config options, read the current "
-            "config, or send some books using the current config."
+            "config, or send some books using the current config. "
+            f"Supported values are {', '.join(AVAILABLE_COMMANDS)}."
         ),
     )
     parser.add_argument(
         "--book-id",
         "-b",
         metavar="BOOK_ID",
         type=int,
@@ -173,10 +177,13 @@
 
         set_config(name, value)
         print(format_setting(name, value))
 
     elif command == COMMAND_INTERACTIVE_CONFIG:
         interactive_config()
 
+    elif command == COMMAND_VERSION:
+        print(f"gutenberg2kindle version {__version__}")
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `gutenberg2kindle-0.4.0/gutenberg2kindle/config.py` & `gutenberg2kindle-0.5.0/gutenberg2kindle/config.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.4.0/gutenberg2kindle/email.py` & `gutenberg2kindle-0.5.0/gutenberg2kindle/email.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.4.0/gutenberg2kindle/gutenberg.py` & `gutenberg2kindle-0.5.0/gutenberg2kindle/gutenberg.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.4.0/pyproject.toml` & `gutenberg2kindle-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gutenberg2kindle"
-version = "0.4.0"
+version = "0.5.0"
 description = "A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP"
 authors = ["Andrés Ignacio Torres <dev@aitorres.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/aitorres/gutenberg2kindle"
 keywords = [
     "python",
@@ -29,23 +29,23 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/aitorres/gutenberg2kindle/issues"
 "Change Log" = "https://github.com/aitorres/gutenberg2kindle/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 usersettings = "^1.1.5"
-requests = "^2.30.0"
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 pylint = "^2.17.4"
-types-requests = "^2.30.0.0"
+types-requests = "^2.31.0.1"
 
 [tool.poetry.scripts]
 gutenberg2kindle = "gutenberg2kindle.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gutenberg2kindle-0.4.0/PKG-INFO` & `gutenberg2kindle-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gutenberg2kindle
-Version: 0.4.0
+Version: 0.5.0
 Summary: A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP
 Home-page: https://github.com/aitorres/gutenberg2kindle
 License: AGPL-3.0-only
 Keywords: python,cli,ebooks,kindle,gutenberg,project gutenberg
 Author: Andrés Ignacio Torres
 Author-email: dev@aitorres.com
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: usersettings (>=1.1.5,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/aitorres/gutenberg2kindle/issues
 Project-URL: Change Log, https://github.com/aitorres/gutenberg2kindle/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/aitorres/gutenberg2kindle
 Description-Content-Type: text/markdown
 
 # Gutenberg2Kindle
```

