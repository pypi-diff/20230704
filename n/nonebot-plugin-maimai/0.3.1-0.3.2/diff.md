# Comparing `tmp/nonebot_plugin_maimai-0.3.1.tar.gz` & `tmp/nonebot_plugin_maimai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.3.1.tar` & `nonebot_plugin_maimai-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/LICENSE
--rw-r--r--   0        0        0     3693 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/README.md
--rw-r--r--   0        0        0    15337 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1556 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17432 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17520 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5353 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      385 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     7873 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1059 2023-07-03 16:30:55.657049 nonebot_plugin_maimai-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3693 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/README.md
+-rw-r--r--   0        0        0    15337 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17432 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17520 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5353 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      385 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     8990 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1059 2023-07-04 10:15:04.983081 nonebot_plugin_maimai-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.3.1/LICENSE` & `nonebot_plugin_maimai-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/README.md` & `nonebot_plugin_maimai-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/__init__.py` & `nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
 
-__version__ = "0.3.0"
+__version__ = "0.3.2"
 __plugin_meta__ = PluginMetadata(
     name="舞萌maimai",
     description='指令：舞萌帮助',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_maimai",
     supported_adapters={"~onebot.v11"},
```

### Comparing `nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.3.2/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.3.1/pyproject.toml` & `nonebot_plugin_maimai-0.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_maimai"
-version = "0.3.1"
+version = "0.3.2"
 description= "Maimai DX plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 repository = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 keywords = ["maimai", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_maimai-0.3.1/PKG-INFO` & `nonebot_plugin_maimai-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimai
-Version: 0.3.1
+Version: 0.3.2
 Summary: Maimai DX plugin for NoneBot
 Home-page: https://github.com/Agnes4m/nonebot_plugin_maimai
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.3.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.3.2 Summary:
 Maimai DX plugin for NoneBot Home-page: https://github.com/Agnes4m/
 nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

