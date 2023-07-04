# Comparing `tmp/konko-0.0.8.tar.gz` & `tmp/konko-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.8.tar", last modified: Mon Jul  3 02:55:57 2023, max compression
+gzip compressed data, was "konko-0.0.9.tar", last modified: Tue Jul  4 00:00:18 2023, max compression
```

## Comparing `konko-0.0.8.tar` & `konko-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:55:57.360305 konko-0.0.8/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-03 02:55:57.360176 konko-0.0.8/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.8/README.md
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-03 02:55:53.000000 konko-0.0.8/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-03 02:55:57.360353 konko-0.0.8/setup.cfg
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:55:57.358566 konko-0.0.8/src/
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:55:57.359299 konko-0.0.8/src/konko/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-03 02:51:16.000000 konko-0.0.8/src/konko/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.8/src/konko/evaluate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     4294 2023-07-03 02:55:25.000000 konko-0.0.8/src/konko/generate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.8/src/konko/models.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:55:57.360022 konko-0.0.8/src/konko/utils/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:54:57.000000 konko-0.0.8/src/konko/utils/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.8/src/konko/utils/constants.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-06-30 22:20:34.000000 konko-0.0.8/src/konko/utils/utils.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 02:55:57.359732 konko-0.0.8/src/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-03 02:55:57.000000 konko-0.0.8/src/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      324 2023-07-03 02:55:57.000000 konko-0.0.8/src/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-03 02:55:57.000000 konko-0.0.8/src/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-03 02:55:57.000000 konko-0.0.8/src/konko.egg-info/top_level.txt
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.031524 konko-0.0.9/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-04 00:00:18.031370 konko-0.0.9/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.9/README.md
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-03 23:59:16.000000 konko-0.0.9/pyproject.toml
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-04 00:00:18.031570 konko-0.0.9/setup.cfg
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.028834 konko-0.0.9/src/
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.029688 konko-0.0.9/src/konko/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-03 23:52:38.000000 konko-0.0.9/src/konko/__init__.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.9/src/konko/evaluate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     4210 2023-07-03 23:58:48.000000 konko-0.0.9/src/konko/generate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.9/src/konko/models.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.031159 konko-0.0.9/src/konko/utils/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        0 2023-07-03 23:40:17.000000 konko-0.0.9/src/konko/utils/__init__.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.9/src/konko/utils/constants.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-07-03 23:40:39.000000 konko-0.0.9/src/konko/utils/logs.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-04 00:00:18.030498 konko-0.0.9/src/konko.egg-info/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      323 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/SOURCES.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/dependency_links.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-04 00:00:18.000000 konko-0.0.9/src/konko.egg-info/top_level.txt
```

### Comparing `konko-0.0.8/src/konko/evaluate.py` & `konko-0.0.9/src/konko/evaluate.py`

 * *Files identical despite different names*

### Comparing `konko-0.0.8/src/konko/generate.py` & `konko-0.0.9/src/konko/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os
 import requests
 import json 
-from utils.constants import TIMEOUT
-from utils.utils import BackendError
+from konko.utils.constants import TIMEOUT
+from konko.utils.logs import BackendError
 from typing import Any, Dict, List, Union, Iterator
 
 
 def generate(prompt: List[str] = None, 
              models: List[str] = ['gpt-4', 'mpt-7b-instruct', 'llama-30b'],
              prompt_file: str = None,
              prompt_file_separator: str = "----",
              stream: bool = False, 
              optimize: Dict = {"cost" : 10} ) -> Union[List[Dict[str, Union[str, float, int]]],Iterator[Dict[str, Union[str, float, int]]]]:
     """
     This method generates a response for a user-specified prompt(s), set of models and an optimization constraint (cost,quality,latency) 
     Args:
-        prompt: The input prompt to generate a response for 
-        models: The list of models to evaluate from 
+        prompt: The input prompt(s) to generate a response for 
+        models: The model(s) to evaluate from         
+        prompt_file: Path to a file containing many prompts 
+        prompt_file_separator: Seprator string 
+        stream: If set to True this returns a handle to the stream object 
         optimize: The cost,quality, and latency constraints
     Examples: 
         >>> import konko
         >>> prompt = ['Summarize the Foundation by Isaac Asimov']
         >>> models = ['gpt-4', 'mpt-7b-instruct', 'llama-30b']
         >>> optimize = {'cost': 10, 'quality': 6}
         >>> konko.generate(prompt = prompt, models = models, optimize = optimize)
@@ -94,12 +97,7 @@
             data = json.loads(chunk)
             if "error" in data:
                 raise BackendError(data["error"], response=response)
             yield data
     except ConnectionError as e:
             raise BackendError(str(e) + "\n" + chunk, response=response) from e    
 
-
-os.environ['KONKO_URL'] = 'http://alb-http-1196840644.us-west-2.elb.amazonaws.com/'
-print(generate(prompt= ["How do you make authentic Thai Mango Salad?", "What are some good ideas for a BBQ menu?"],
-               models=['mosaicml/mpt-7b-instruct'], stream=False
-               ))
```

### Comparing `konko-0.0.8/src/konko/models.py` & `konko-0.0.9/src/konko/models.py`

 * *Files identical despite different names*

