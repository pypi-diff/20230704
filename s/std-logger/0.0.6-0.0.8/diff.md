# Comparing `tmp/std-logger-0.0.6.tar.gz` & `tmp/std-logger-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std-logger-0.0.6.tar", last modified: Tue May 16 03:56:25 2023, max compression
+gzip compressed data, was "std-logger-0.0.8.tar", last modified: Tue Jul  4 10:39:37 2023, max compression
```

## Comparing `std-logger-0.0.6.tar` & `std-logger-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.014644 std-logger-0.0.6/
--rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-05-16 03:56:25.014477 std-logger-0.0.6/PKG-INFO
--rw-r--r--   0 wei.fu     (502) staff       (20)       38 2023-05-16 03:56:25.014696 std-logger-0.0.6/setup.cfg
--rw-r--r--   0 wei.fu     (502) staff       (20)      745 2023-02-15 09:05:01.000000 std-logger-0.0.6/setup.py
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.012698 std-logger-0.0.6/stdLogger/
--rw-r--r--   0 wei.fu     (502) staff       (20)       32 2023-02-10 09:35:37.000000 std-logger-0.0.6/stdLogger/__init__.py
--rw-r--r--   0 wei.fu     (502) staff       (20)     3923 2023-05-16 03:31:35.000000 std-logger-0.0.6/stdLogger/std_logs.py
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.014207 std-logger-0.0.6/std_logger.egg-info/
--rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/PKG-INFO
--rw-r--r--   0 wei.fu     (502) staff       (20)      221 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/SOURCES.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)        1 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/dependency_links.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)       28 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/requires.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)       10 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/top_level.txt
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-07-04 10:39:37.673439 std-logger-0.0.8/
+-rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-07-04 10:39:37.673282 std-logger-0.0.8/PKG-INFO
+-rw-r--r--   0 wei.fu     (502) staff       (20)       38 2023-07-04 10:39:37.673521 std-logger-0.0.8/setup.cfg
+-rw-r--r--   0 wei.fu     (502) staff       (20)      745 2023-02-15 09:05:01.000000 std-logger-0.0.8/setup.py
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-07-04 10:39:37.671978 std-logger-0.0.8/stdLogger/
+-rw-r--r--   0 wei.fu     (502) staff       (20)       32 2023-02-10 09:35:37.000000 std-logger-0.0.8/stdLogger/__init__.py
+-rw-r--r--   0 wei.fu     (502) staff       (20)     3887 2023-07-04 10:38:20.000000 std-logger-0.0.8/stdLogger/std_logs.py
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-07-04 10:39:37.673064 std-logger-0.0.8/std_logger.egg-info/
+-rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-07-04 10:39:37.000000 std-logger-0.0.8/std_logger.egg-info/PKG-INFO
+-rw-r--r--   0 wei.fu     (502) staff       (20)      221 2023-07-04 10:39:37.000000 std-logger-0.0.8/std_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)        1 2023-07-04 10:39:37.000000 std-logger-0.0.8/std_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)       28 2023-07-04 10:39:37.000000 std-logger-0.0.8/std_logger.egg-info/requires.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)       10 2023-07-04 10:39:37.000000 std-logger-0.0.8/std_logger.egg-info/top_level.txt
```

### Comparing `std-logger-0.0.6/setup.py` & `std-logger-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `std-logger-0.0.6/stdLogger/std_logs.py` & `std-logger-0.0.8/stdLogger/std_logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,17 +89,16 @@
         _logger.trace(msg, *args, **kwargs)
 
     def debug(self, __message: str, *args, **kwargs) -> None:
         """
         level 10
         """
         _msg = self.custom_message_context()
-        print(type(__message))
-        #message = "%s | %s" % (_msg, __message)
-        #_logger.debug(message, *args, **kwargs)
+        message = "%s | %s" % (_msg, __message)
+        _logger.debug(message, *args, **kwargs)
 
     def info(self, __message: str, *args, **kwargs) -> None:
         """
         level 20
         """
 
         _msg = self.custom_message_context()
@@ -128,10 +127,7 @@
         """level 50"""
         _msg = self.custom_message_context()
         message = "%s | %s" % (_msg, __message)
         _logger.exception(message, *args, **kwargs)
 
 
 std_logger=logger = StdLogger()
-
-
-
```

