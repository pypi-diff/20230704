# Comparing `tmp/pyauthenticator-0.1.0.tar.gz` & `tmp/pyauthenticator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauthenticator-0.1.0.tar", last modified: Sun Jul  2 20:04:18 2023, max compression
+gzip compressed data, was "pyauthenticator-0.2.0.tar", last modified: Tue Jul  4 17:42:50 2023, max compression
```

## Comparing `pyauthenticator-0.1.0.tar` & `pyauthenticator-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/pyauthenticator/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/pyauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/pyauthenticator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/pyauthenticator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/pyauthenticator/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/pyauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/pyauthenticator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-02 20:04:18.000000 pyauthenticator-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:04:18.860426 pyauthenticator-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/tests/test_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/tests/test_user_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-02 20:04:15.000000 pyauthenticator-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/pyauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/pyauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/pyauthenticator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/pyauthenticator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/pyauthenticator/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/pyauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/pyauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-04 17:42:50.000000 pyauthenticator-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:42:50.856705 pyauthenticator-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/tests/test_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/tests/test_user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-04 17:42:47.000000 pyauthenticator-0.2.0/versioneer.py
```

### Comparing `pyauthenticator-0.1.0/LICENSE` & `pyauthenticator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.1.0/PKG-INFO` & `pyauthenticator-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthenticator
-Version: 0.1.0
+Version: 0.2.0
 Summary: Similar to the Google authenticator just written in python.
 Home-page: https://github.com/jan-janssen/pyauthenticator
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyauthenticator-0.1.0/README.md` & `pyauthenticator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.1.0/pyauthenticator/__init__.py` & `pyauthenticator-0.2.0/pyauthenticator/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Generate two factor authentication codes on the command line
 """
-from pyauthenticator.share import (
-    load_config,
-    generate_qrcode,
-    get_two_factor_code as get_two_factor_code_internal,
-)
+from pyauthenticator.share import generate_qrcode
+from pyauthenticator.share import get_two_factor_code as get_two_factor_code_internal
+from pyauthenticator.share import load_config
 
 
 def write_qrcode_to_file(service, file_name=None):
     """
     Write qrcode to file to scan it with a mobile application
 
     Args:
```

### Comparing `pyauthenticator-0.1.0/pyauthenticator/__main__.py` & `pyauthenticator-0.2.0/pyauthenticator/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Generate two factor authentication codes on the command line
 """
 import argparse
 import sys
+
 from pyauthenticator.share import (
-    list_services,
-    load_config,
-    generate_qrcode,
     add_service,
+    generate_qrcode,
     get_two_factor_code,
+    list_services,
+    load_config,
 )
 
 
 def command_line_parser(cmd_args=None):
     """
     Main function primarly used for the command line interface
     """
```

### Comparing `pyauthenticator-0.1.0/pyauthenticator/share.py` & `pyauthenticator-0.2.0/pyauthenticator/share.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Shared functionality to generate two factor authentication codes
 """
-import base64
 import json
 import os
-import otpauth
+from inspect import signature
+
+import pyotp
+import qrcode
 from PIL import Image
 from pyzbar.pyzbar import decode
-import qrcode
-
 
 # default configuration file
 config_file = "~/.pyauthenticator"
 
 
 def expand_path(path):
     """
@@ -71,36 +71,14 @@
         kv[0]: kv[1]
         for kv in [
             otpvar.split("=") for otpvar in otpauth_str.replace("?", "&").split("&")[1:]
         ]
     }
 
 
-def add_padding(main_str, padding_str, padding_length, inverse_padding=False):
-    """
-    Add padding to a string either in the beginning or at the end
-
-    Args:
-        main_str (str): string to add padding to
-        padding_str (str): padding character as string
-        padding_length (int): the length of the final string should be a multiple of the padding length
-        inverse_padding (bool): add padding in the beginning rather than the end
-
-    Returns:
-        str: resulting string with padding
-    """
-    missing_padding = len(main_str) % padding_length
-    if missing_padding:
-        if inverse_padding:
-            main_str = padding_str * (padding_length - missing_padding) + main_str
-        else:
-            main_str += padding_str * (padding_length - missing_padding)
-    return main_str
-
-
 def check_if_key_in_config(key, config_dict):
     """
     Check if a given key is included in a dictionary, raise an ValueError if it is not.
 
     Args:
         key (str): key as string
         config_dict (dict): configuration dictionary
@@ -118,45 +96,33 @@
         config_dict (dict): configuration dictionary
 
     Returns:
         str: two factor authentication code as string
     """
     check_if_key_in_config(key=key, config_dict=config_dict)
     decode_dict_internal = get_otpauth_dict(otpauth_str=config_dict[key])
+    funct_sig = signature(pyotp.TOTP)
+    if "digits" in decode_dict_internal.keys():
+        digits = int(decode_dict_internal["digits"])
+    else:
+        digits = funct_sig.parameters["digits"].default
     if "period" in decode_dict_internal.keys():
-        totp = otpauth.TOTP(
-            secret=base64.b32decode(
-                add_padding(
-                    main_str=decode_dict_internal["secret"],
-                    padding_str="=",
-                    padding_length=8,
-                    inverse_padding=False,
-                ),
-                True,
-            ),
-            period=int(decode_dict_internal["period"]),
-        )
+        interval = int(decode_dict_internal["period"])
+    else:
+        interval = funct_sig.parameters["interval"].default
+    if "issuer" in decode_dict_internal.keys():
+        issuer = decode_dict_internal["issuer"]
     else:
-        totp = otpauth.TOTP(
-            secret=base64.b32decode(
-                add_padding(
-                    main_str=decode_dict_internal["secret"],
-                    padding_str="=",
-                    padding_length=8,
-                    inverse_padding=False,
-                ),
-                True,
-            ),
-        )
-    return add_padding(
-        main_str=str(totp.string_code(totp.generate())),
-        padding_str="0",
-        padding_length=6,
-        inverse_padding=True,
-    )
+        issuer = funct_sig.parameters["issuer"].default
+    return pyotp.TOTP(
+        s=decode_dict_internal["secret"],
+        digits=digits,
+        issuer=issuer,
+        interval=interval,
+    ).now()
 
 
 def add_service(
     key, qrcode_png_file_name, config_dict, config_file_to_write=config_file
 ):
     """
     Add new service to configuration file
```

### Comparing `pyauthenticator-0.1.0/pyauthenticator.egg-info/PKG-INFO` & `pyauthenticator-0.2.0/pyauthenticator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthenticator
-Version: 0.1.0
+Version: 0.2.0
 Summary: Similar to the Google authenticator just written in python.
 Home-page: https://github.com/jan-janssen/pyauthenticator
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyauthenticator-0.1.0/setup.py` & `pyauthenticator-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 Setuptools based setup module
 """
-from setuptools import setup, find_packages
-import versioneer
+from setuptools import find_packages, setup
 
+import versioneer
 
 setup(
     name='pyauthenticator',
     version=versioneer.get_version(),
     description='Similar to the Google authenticator just written in python.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/jan-janssen/pyauthenticator',
     author='Jan Janssen',
     author_email='jan.janssen@outlook.com',
     license='BSD',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        'otpauth>=2.0.0',
+        'pyotp>=2.6.0',
         'qrcode>=7.4.2',
         'pyzbar>=0.1.9',
-        'pillow>=9.5.0',
+        'pillow>=10.0.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
         "console_scripts": [
             'pyauthenticator=pyauthenticator.__main__:command_line_parser'
         ]
     }
```

### Comparing `pyauthenticator-0.1.0/tests/test_cmd.py` & `pyauthenticator-0.2.0/tests/test_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import unittest
+import json
 import os
 import subprocess
-import json
+import unittest
 from contextlib import redirect_stdout
 from io import StringIO
-from pyauthenticator.share import expand_path, write_config, config_file
+
 from pyauthenticator.__main__ import command_line_parser
+from pyauthenticator.share import config_file, expand_path, write_config
 
 
 class CmdSubprocessTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.config_dict = {
             "test": "otpauth://totp/Test%3A%20root%40github.com?secret=6IQXETC4ADOSMMUN&issuer=Test"
```

### Comparing `pyauthenticator-0.1.0/tests/test_core.py` & `pyauthenticator-0.2.0/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """
 Test for core functionality
 """
-import unittest
-from pyauthenticator.share import list_services, load_config, generate_qrcode, add_service, get_two_factor_code
 import os
+import unittest
+
+from pyauthenticator.share import (
+    add_service,
+    generate_qrcode,
+    get_two_factor_code,
+    list_services,
+    load_config
+)
 
 
 class TestCore(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.qr_code_png = "test.png"
         cls.config_dict = {
```

### Comparing `pyauthenticator-0.1.0/tests/test_user_interface.py` & `pyauthenticator-0.2.0/tests/test_user_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import unittest
 import os
+import unittest
+
 from pyauthenticator import get_two_factor_code, write_qrcode_to_file
-from pyauthenticator.share import expand_path, write_config, config_file
+from pyauthenticator.share import config_file, expand_path, write_config
 
 
 class TestUserInterface(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.config_dict = {
             "test": "otpauth://totp/Test%3A%20root%40github.com?secret=6IQXETC4ADOSMMUN&issuer=Test"
```

### Comparing `pyauthenticator-0.1.0/versioneer.py` & `pyauthenticator-0.2.0/versioneer.py`

 * *Files identical despite different names*

