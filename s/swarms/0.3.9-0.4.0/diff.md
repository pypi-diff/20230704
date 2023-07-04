# Comparing `tmp/swarms-0.3.9.tar.gz` & `tmp/swarms-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.3.9.tar", last modified: Tue Jul  4 16:53:14 2023, max compression
+gzip compressed data, was "swarms-0.4.0.tar", last modified: Tue Jul  4 17:00:50 2023, max compression
```

## Comparing `swarms-0.3.9.tar` & `swarms-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.554609 swarms-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 16:53:04.000000 swarms-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 16:53:14.554609 swarms-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-04 16:53:04.000000 swarms-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:53:14.554609 swarms-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 16:53:04.000000 swarms-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.550609 swarms-0.3.9/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.550609 swarms-0.3.9/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.550609 swarms-0.3.9/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.550609 swarms-0.3.9/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.554609 swarms-0.3.9/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70592 2023-07-04 16:53:04.000000 swarms-0.3.9/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:53:14.550609 swarms-0.3.9/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 16:53:14.000000 swarms-0.3.9/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 16:53:14.000000 swarms-0.3.9/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:53:14.000000 swarms-0.3.9/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 16:53:14.000000 swarms-0.3.9/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 16:53:14.000000 swarms-0.3.9/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.821565 swarms-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:00:41.000000 swarms-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:00:50.821565 swarms-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-04 17:00:41.000000 swarms-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:00:50.821565 swarms-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-04 17:00:41.000000 swarms-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.817565 swarms-0.4.0/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.817565 swarms-0.4.0/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.817565 swarms-0.4.0/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.817565 swarms-0.4.0/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.821565 swarms-0.4.0/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70592 2023-07-04 17:00:41.000000 swarms-0.4.0/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:00:50.817565 swarms-0.4.0/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:00:50.000000 swarms-0.4.0/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-04 17:00:50.000000 swarms-0.4.0/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:00:50.000000 swarms-0.4.0/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 17:00:50.000000 swarms-0.4.0/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:00:50.000000 swarms-0.4.0/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.3.9/LICENSE` & `swarms-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/PKG-INFO` & `swarms-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.9
+Version: 0.4.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.9/README.md` & `swarms-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/setup.py` & `swarms-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.3.9',
+  version = '0.4.0',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
+       'llama-index',
         "transformers",
         "openai",
         "langchain",
         "torch==1.13.1",
         "torchvision==0.14.1",
         "asyncio",
         "nest_asyncio",
@@ -33,15 +34,14 @@
         "accelerate",
         "addict",
         "albumentations",
         "basicsr",
         "controlnet-aux",
         "diffusers",
         "einops",
-        'llama-index',
         "gradio",
         "imageio",
         "imageio-ffmpeg",
         "invisible-watermark",
         "kornia",
         "numpy",
         "omegaconf",
```

### Comparing `swarms-0.3.9/swarms/agents/swarms.py` & `swarms-0.4.0/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/agents/workers/agents.py` & `swarms-0.4.0/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/agents/workers/auto_agent.py` & `swarms-0.4.0/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.0/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/agents/workers/multi_modal.py` & `swarms-0.4.0/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/agents/workers/omni_agent.py` & `swarms-0.4.0/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms/tools/main.py` & `swarms-0.4.0/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms.egg-info/PKG-INFO` & `swarms-0.4.0/swarms.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.3.9
+Version: 0.4.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.3.9/swarms.egg-info/SOURCES.txt` & `swarms-0.4.0/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.3.9/swarms.egg-info/requires.txt` & `swarms-0.4.0/swarms.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+llama-index
 transformers
 openai
 langchain
 torch==1.13.1
 torchvision==0.14.1
 asyncio
 nest_asyncio
@@ -13,15 +14,14 @@
 accelerate
 addict
 albumentations
 basicsr
 controlnet-aux
 diffusers
 einops
-llama-index
 gradio
 imageio
 imageio-ffmpeg
 invisible-watermark
 kornia
 numpy
 omegaconf
```

