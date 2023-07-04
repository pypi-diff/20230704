# Comparing `tmp/notion2medium-1.0.0.tar.gz` & `tmp/notion2medium-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion2medium-1.0.0.tar", max compression
+gzip compressed data, was "notion2medium-1.0.1.tar", max compression
```

## Comparing `notion2medium-1.0.0.tar` & `notion2medium-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0    11337 2022-02-05 04:59:36.124624 notion2medium-1.0.0/LICENSE
--rw-r--r--   0        0        0       42 2022-02-03 14:20:04.528143 notion2medium-1.0.0/medium_sdk_python/.git
--rw-r--r--   0        0        0      702 2022-02-03 14:20:04.546289 notion2medium-1.0.0/medium_sdk_python/.gitignore
--rw-r--r--   0        0        0      138 2022-02-03 14:20:04.546496 notion2medium-1.0.0/medium_sdk_python/.travis.yml
--rw-r--r--   0        0        0    10377 2022-02-03 14:20:04.546858 notion2medium-1.0.0/medium_sdk_python/LICENSE.TXT
--rw-r--r--   0        0        0       81 2022-02-03 14:20:04.547017 notion2medium-1.0.0/medium_sdk_python/MANIFEST
--rw-r--r--   0        0        0     2781 2022-02-03 14:20:04.547241 notion2medium-1.0.0/medium_sdk_python/README.md
--rw-r--r--   0        0        0     8101 2022-02-03 14:20:04.547698 notion2medium-1.0.0/medium_sdk_python/medium/__init__.py
--rw-r--r--   0        0        0     7914 2022-02-03 14:23:07.825593 notion2medium-1.0.0/medium_sdk_python/medium/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     8021 2022-02-14 10:38:53.368151 notion2medium-1.0.0/medium_sdk_python/medium/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       17 2022-02-03 14:20:04.547884 notion2medium-1.0.0/medium_sdk_python/requirements.txt
--rw-r--r--   0        0        0       40 2022-02-03 14:20:04.548075 notion2medium-1.0.0/medium_sdk_python/setup.cfg
--rw-r--r--   0        0        0      464 2022-02-03 14:20:04.548269 notion2medium-1.0.0/medium_sdk_python/setup.py
--rw-r--r--   0        0        0       17 2022-02-03 14:20:04.548602 notion2medium-1.0.0/medium_sdk_python/tests/requirements.txt
--rw-r--r--   0        0        0     3118 2022-02-03 14:20:04.548785 notion2medium-1.0.0/medium_sdk_python/tests/test.png
--rw-r--r--   0        0        0     7774 2022-02-03 14:20:04.548969 notion2medium-1.0.0/medium_sdk_python/tests/test.py
--rw-r--r--   0        0        0       22 2022-02-23 11:30:12.888471 notion2medium-1.0.0/notion2medium/__init__.py
--rw-r--r--   0        0        0      117 2022-02-23 11:30:12.889823 notion2medium-1.0.0/notion2medium/__main__.py
--rw-r--r--   0        0        0      793 2022-02-23 11:30:12.890681 notion2medium-1.0.0/notion2medium/clients/medium.py
--rw-r--r--   0        0        0      546 2022-02-23 11:30:12.891764 notion2medium-1.0.0/notion2medium/clients/notion_client.py
--rw-r--r--   0        0        0        0 2022-02-04 11:54:19.712211 notion2medium-1.0.0/notion2medium/console/__init__.py
--rw-r--r--   0        0        0     1699 2022-02-23 11:30:12.892760 notion2medium-1.0.0/notion2medium/console/application.py
--rw-r--r--   0        0        0        0 2022-02-04 11:54:19.713092 notion2medium-1.0.0/notion2medium/console/commands/__init__.py
--rw-r--r--   0        0        0     2151 2022-02-23 11:30:12.893336 notion2medium-1.0.0/notion2medium/console/commands/command.py
--rw-r--r--   0        0        0     4261 2022-02-23 11:30:12.894044 notion2medium-1.0.0/notion2medium/console/commands/publish.py
--rw-r--r--   0        0        0     2833 2022-02-23 11:30:12.894808 notion2medium-1.0.0/notion2medium/console/commands/select.py
--rw-r--r--   0        0        0      207 2022-02-23 11:30:12.895321 notion2medium-1.0.0/notion2medium/exceptions/__init__.py
--rw-r--r--   0        0        0     1259 2022-02-23 11:30:12.895809 notion2medium-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1055 2022-02-23 11:31:21.662656 notion2medium-1.0.0/setup.py
--rw-r--r--   0        0        0      513 2022-02-23 11:31:21.662963 notion2medium-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-02-14 23:58:16.907373 notion2medium-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1979 2023-02-14 23:58:16.907487 notion2medium-1.0.1/README.md
+-rw-r--r--   0        0        0       42 2023-02-15 00:03:14.800634 notion2medium-1.0.1/medium_sdk_python/.git
+-rw-r--r--   0        0        0      702 2023-02-15 00:03:14.820702 notion2medium-1.0.1/medium_sdk_python/.gitignore
+-rw-r--r--   0        0        0      138 2023-02-15 00:03:14.820844 notion2medium-1.0.1/medium_sdk_python/.travis.yml
+-rw-r--r--   0        0        0    10377 2023-02-15 00:03:14.821012 notion2medium-1.0.1/medium_sdk_python/LICENSE.TXT
+-rw-r--r--   0        0        0       81 2023-02-15 00:03:14.821111 notion2medium-1.0.1/medium_sdk_python/MANIFEST
+-rw-r--r--   0        0        0     2781 2023-02-15 00:03:14.821240 notion2medium-1.0.1/medium_sdk_python/README.md
+-rw-r--r--   0        0        0     8101 2023-02-15 00:03:14.821453 notion2medium-1.0.1/medium_sdk_python/medium/__init__.py
+-rw-r--r--   0        0        0    10081 2023-03-28 00:13:22.859695 notion2medium-1.0.1/medium_sdk_python/medium/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       17 2023-02-15 00:03:14.821539 notion2medium-1.0.1/medium_sdk_python/requirements.txt
+-rw-r--r--   0        0        0       40 2023-02-15 00:03:14.821636 notion2medium-1.0.1/medium_sdk_python/setup.cfg
+-rw-r--r--   0        0        0      464 2023-02-15 00:03:14.821739 notion2medium-1.0.1/medium_sdk_python/setup.py
+-rw-r--r--   0        0        0       17 2023-02-15 00:03:14.821866 notion2medium-1.0.1/medium_sdk_python/tests/requirements.txt
+-rw-r--r--   0        0        0     3118 2023-02-15 00:03:14.821981 notion2medium-1.0.1/medium_sdk_python/tests/test.png
+-rw-r--r--   0        0        0     7774 2023-02-15 00:03:14.822095 notion2medium-1.0.1/medium_sdk_python/tests/test.py
+-rw-r--r--   0        0        0       22 2023-03-28 02:09:42.564202 notion2medium-1.0.1/notion2medium/__init__.py
+-rw-r--r--   0        0        0      117 2023-02-14 23:58:16.907777 notion2medium-1.0.1/notion2medium/__main__.py
+-rw-r--r--   0        0        0      793 2023-02-14 23:58:16.907931 notion2medium-1.0.1/notion2medium/clients/medium.py
+-rw-r--r--   0        0        0      546 2023-02-14 23:58:16.908033 notion2medium-1.0.1/notion2medium/clients/notion_client.py
+-rw-r--r--   0        0        0        0 2023-02-14 23:58:16.908124 notion2medium-1.0.1/notion2medium/console/__init__.py
+-rw-r--r--   0        0        0     1699 2023-02-14 23:58:16.908235 notion2medium-1.0.1/notion2medium/console/application.py
+-rw-r--r--   0        0        0        0 2023-02-14 23:58:16.908325 notion2medium-1.0.1/notion2medium/console/commands/__init__.py
+-rw-r--r--   0        0        0     2151 2023-02-14 23:58:16.908451 notion2medium-1.0.1/notion2medium/console/commands/command.py
+-rw-r--r--   0        0        0     4274 2023-03-28 01:54:51.418317 notion2medium-1.0.1/notion2medium/console/commands/publish.py
+-rw-r--r--   0        0        0     2833 2023-02-14 23:58:16.908676 notion2medium-1.0.1/notion2medium/console/commands/select.py
+-rw-r--r--   0        0        0      207 2023-02-14 23:58:16.908830 notion2medium-1.0.1/notion2medium/exceptions/__init__.py
+-rw-r--r--   0        0        0     1280 2023-03-28 02:44:08.337508 notion2medium-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 notion2medium-1.0.1/PKG-INFO
```

### Comparing `notion2medium-1.0.0/LICENSE` & `notion2medium-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/.gitignore` & `notion2medium-1.0.1/medium_sdk_python/.gitignore`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/LICENSE.TXT` & `notion2medium-1.0.1/medium_sdk_python/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/README.md` & `notion2medium-1.0.1/medium_sdk_python/README.md`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/medium/__init__.py` & `notion2medium-1.0.1/medium_sdk_python/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/tests/test.png` & `notion2medium-1.0.1/medium_sdk_python/tests/test.png`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/medium_sdk_python/tests/test.py` & `notion2medium-1.0.1/medium_sdk_python/tests/test.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/notion2medium/clients/medium.py` & `notion2medium-1.0.1/notion2medium/clients/medium.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/notion2medium/clients/notion_client.py` & `notion2medium-1.0.1/notion2medium/clients/notion_client.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/notion2medium/console/application.py` & `notion2medium-1.0.1/notion2medium/console/application.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/notion2medium/console/commands/command.py` & `notion2medium-1.0.1/notion2medium/console/commands/command.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/notion2medium/console/commands/publish.py` & `notion2medium-1.0.1/notion2medium/console/commands/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from cleo.helpers import option
 from medium_sdk_python.medium import MediumError
-from notion2md.exporter import string_exporter
+from notion2md.exporter.block import StringExporter
 
 from notion2medium.exceptions import ClientTokenException
 
 from .command import CustomCommand
 
 
 class PublishCommand(CustomCommand):
@@ -100,15 +100,15 @@
             start_message=self.output_ongoing(
                 "RETRIEVING", f"{self.info(page_title)}'s content"
             ),
             end_message=self.output_success(
                 "RETRIEVED", f"{self.info(page_title)}'s content"
             ),
         ):
-            content = string_exporter(block_id=page_id, unzipped=True)
+            content = StringExporter(block_id=page_id, unzipped=True).export()
         # - inject title header to content
         content = self.inject_title_to_content(page_title, content)
 
         try:
             with self.indicator(
                 start_message=self.output_ongoing(
                     "PUBLISHING", f"{self.info(page_title)} to Medium"
```

### Comparing `notion2medium-1.0.0/notion2medium/console/commands/select.py` & `notion2medium-1.0.1/notion2medium/console/commands/select.py`

 * *Files identical despite different names*

### Comparing `notion2medium-1.0.0/pyproject.toml` & `notion2medium-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "notion2medium"
-version = "1.0.0"
+version = "1.0.1"
 description = "a Simple command that publishes Notion Page to Medium."
 authors = ["echo724 <eunchan1001@gmail.com>"]
+readme = "README.md"
 
 packages = [
     { include = "notion2medium" },
     { include = "medium_sdk_python" },
 ]
 
 exclude = ["tests"]
```

