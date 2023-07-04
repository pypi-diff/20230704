# Comparing `tmp/bondzai.davinsy-py-0.0.3.tar.gz` & `tmp/bondzai.davinsy-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.3.tar", last modified: Wed Jun 21 10:24:23 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.4.tar", last modified: Tue Jul  4 09:33:29 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.3.tar` & `bondzai.davinsy-py-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:42.056804 bondzai.davinsy-py-0.0.3/
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/NOTICE
--rwxrwxrwx   0 root         (0) root         (0)      491 2023-06-21 10:51:42.056804 bondzai.davinsy-py-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:41.541890 bondzai.davinsy-py-0.0.3/bondzai/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:41.846032 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-06-21 10:51:31.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3989 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/davinsy.py
--rwxrwxrwx   0 root         (0) root         (0)     6243 2023-06-21 10:51:31.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/enums.py
--rwxrwxrwx   0 root         (0) root         (0)      333 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/logger.py
--rwxrwxrwx   0 root         (0) root         (0)    21765 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/model.py
--rwxrwxrwx   0 root         (0) root         (0)    24433 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/operations.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/preproc.py
--rwxrwxrwx   0 root         (0) root         (0)     1034 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 10:51:42.032811 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      491 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      591 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-21 10:51:41.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 10:51:40.000000 bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-21 10:50:10.000000 bondzai.davinsy-py-0.0.3/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-06-21 10:51:42.062380 bondzai.davinsy-py-0.0.3/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.964277 bondzai.davinsy-py-0.0.4/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-04 09:33:29.964376 bondzai.davinsy-py-0.0.4/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)       72 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.958034 bondzai.davinsy-py-0.0.4/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.961634 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/
+-rw-r--r--   0 theo       (501) staff       (20)       24 2023-07-04 09:33:20.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     3989 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/davinsy.py
+-rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 09:33:20.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)    21765 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/model.py
+-rw-r--r--   0 theo       (501) staff       (20)    24433 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/operations.py
+-rw-r--r--   0 theo       (501) staff       (20)     3342 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/preproc.py
+-rw-r--r--   0 theo       (501) staff       (20)     1034 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:33:29.964050 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      591 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       26 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:33:29.000000 bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:30.000000 bondzai.davinsy-py-0.0.4/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-04 09:33:29.964990 bondzai.davinsy-py-0.0.4/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.3/NOTICE` & `bondzai.davinsy-py-0.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,29 @@
 
 
 class EventOperationID(Enum):
     EVT_EXT_EXCEPTION = 0x00
     EVT_EXT_DATA_IN = 0x01
     EVT_EXT_CMD_STATUS = 0x100
     EVT_EXT_LOG = 0x101
-    EVT_EXT_POSTPROC = 0x200
+    EVT_EXT_VM_RESULT = 0x200
+    EVT_EXT_ASL_RESULT = 0x201
+    EVT_EXT_SET_MODE = 0x300
+    EVT_EXT_CORRECTION = 0x301
+    EVT_EXT_TRIGGER = 0x302
     EVT_EXT_CUSTOM_1 = 0xF00
     EVT_EXT_CUSTOM_2 = 0xF01
     EVT_EXT_CUSTOM_3 = 0xF02
     EVT_EXT_CUSTOM_4 = 0xF03
+    EVT_EXT_CUSTOM_5 = 0xF04
+    EVT_EXT_CUSTOM_6 = 0xF05
+    EVT_EXT_CUSTOM_7 = 0xF06
+    EVT_EXT_CUSTOM_8 = 0xF07
+    EVT_EXT_CUSTOM_9 = 0xF08
+    EVT_EXT_CUSTOM_10 = 0xF09
     EVT_INT_EXCEPTION = 0x1000
     EVT_INT_DATA_STORED = 0x1001
     EVT_INT_DISCOVERY = 0x1002
     EVT_INT_TRANSPORT = 0x1003
     EVT_INT_DATA_UPDATED = 0x1100
     EVT_INT_READY_TO_PREPROC_BATCH = 0x1101
     EVT_INT_PREPROC_BATCH_DONE = 0x1102
@@ -59,14 +69,20 @@
 class AgentAIMode(Enum):
     APP_AI_MODE_NOT_INIT = -1
     APP_AI_MODE_STANDBY = 0
     APP_AI_MODE_ENROLLEMENT = 1
     APP_AI_MODE_INFERENCE = 2
 
 
+class AgentAIType(Enum):
+    APP_AI_TYPE_NOT_INIT = -1
+    APP_AI_TYPE_CLASSIFICATION = 0
+    APP_AI_TYPE_REGRESSION = 1
+
+
 class PPOperationUID(Enum):
     OPS_ID_EXT = 0x80000000
     OPS_ID = 0x00000000
     OPS_MISC = 0x00000000
     OPS_MATH = 0x01000000
     OPS_DSP = 0x02000000
     OPS_IMG = 0x03000000
```

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/model.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/operations.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/preproc.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.4/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.4/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.3/setup.cfg` & `bondzai.davinsy-py-0.0.4/setup.cfg`

 * *Files identical despite different names*

