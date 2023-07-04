# Comparing `tmp/swarms-0.4.2.tar.gz` & `tmp/swarms-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.2.tar", last modified: Tue Jul  4 17:40:40 2023, max compression
+gzip compressed data, was "swarms-0.4.3.tar", last modified: Tue Jul  4 17:44:28 2023, max compression
```

## Comparing `swarms-0.4.2.tar` & `swarms-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:40:30.000000 swarms-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:40:40.023820 swarms-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16455 2023-07-04 17:40:30.000000 swarms-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:30.000000 swarms-0.4.2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 17:40:30.000000 swarms-0.4.2/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 17:40:30.000000 swarms-0.4.2/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:40:30.000000 swarms-0.4.2/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:40:40.023820 swarms-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-04 17:40:30.000000 swarms-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.023820 swarms-0.4.2/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 17:40:30.000000 swarms-0.4.2/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:40:40.019820 swarms-0.4.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 17:40:40.000000 swarms-0.4.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.381006 swarms-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 17:44:19.000000 swarms-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:44:28.381006 swarms-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16455 2023-07-04 17:44:19.000000 swarms-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:19.000000 swarms-0.4.3/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-04 17:44:19.000000 swarms-0.4.3/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 17:44:19.000000 swarms-0.4.3/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 17:44:19.000000 swarms-0.4.3/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:44:28.381006 swarms-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 17:44:19.000000 swarms-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34561 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.381006 swarms-0.4.3/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70990 2023-07-04 17:44:19.000000 swarms-0.4.3/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:28.377005 swarms-0.4.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 17:44:28.000000 swarms-0.4.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.2/LICENSE` & `swarms-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/PKG-INFO` & `swarms-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.2
+Version: 0.4.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.2/README.md` & `swarms-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/api/container.py` & `swarms-0.4.3/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/api/main.py` & `swarms-0.4.3/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/api/worker.py` & `swarms-0.4.3/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/swarms.py` & `swarms-0.4.3/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/workers/agents.py` & `swarms-0.4.3/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/workers/auto_agent.py` & `swarms-0.4.3/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.3/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/workers/multi_modal.py` & `swarms-0.4.3/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/agents/workers/omni_agent.py` & `swarms-0.4.3/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms/tools/main.py` & `swarms-0.4.3/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.2/swarms.egg-info/PKG-INFO` & `swarms-0.4.3/swarms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.2
+Version: 0.4.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.2/swarms.egg-info/SOURCES.txt` & `swarms-0.4.3/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

