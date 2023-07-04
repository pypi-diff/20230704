# Comparing `tmp/cnextb-1.0.0.tar.gz` & `tmp/cnextb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnextb-1.0.0.tar", last modified: Tue Jul  4 07:20:09 2023, max compression
+gzip compressed data, was "dist/cnextb-1.0.1.tar", last modified: Tue Jul  4 08:24:11 2023, max compression
```

## Comparing `cnextb-1.0.0.tar` & `cnextb-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/
--rwxr--r--   0 root         (0) root         (0)      241 2023-07-04 07:19:58.000000 cnextb-1.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 07:20:09.000000 cnextb-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1837 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-04 07:20:09.000000 cnextb-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/
--rwxr--r--   0 root         (0) root         (0)      316 2023-07-04 06:05:38.000000 cnextb-1.0.0/cnextb/smoke.py
--rwxr--r--   0 root         (0) root         (0)      795 2023-07-04 06:04:28.000000 cnextb-1.0.0/cnextb/connection.py
--rwxr--r--   0 root         (0) root         (0)      312 2023-07-04 06:59:16.000000 cnextb-1.0.0/cnextb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/connection_specific/
--rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/connection_specific/serial/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/
--rwxr--r--   0 root         (0) root         (0)     1993 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_alt.py
--rwxr--r--   0 root         (0) root         (0)    14130 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_socket.py
--rwxr--r--   0 root         (0) root         (0)    10119 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_loop.py
--rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/__init__.py
--rwxr--r--   0 root         (0) root         (0)     3119 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_hwgrep.py
--rwxr--r--   0 root         (0) root         (0)      277 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_rfc2217.py
--rwxr--r--   0 root         (0) root         (0)     9024 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/urlhandler/protocol_spy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/connection_specific/serial/threaded/
--rwxr--r--   0 root         (0) root         (0)     9272 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/threaded/__init__.py
--rwxr--r--   0 root         (0) root         (0)     9104 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/serialcli.py
--rwxr--r--   0 root         (0) root         (0)    21692 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/serialutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/
--rwxr--r--   0 root         (0) root         (0)    11336 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports_windows.py
--rwxr--r--   0 root         (0) root         (0)     3349 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports.py
--rwxr--r--   0 root         (0) root         (0)     3637 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/hexlify_codec.py
--rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/__init__.py
--rwxr--r--   0 root         (0) root         (0)    35085 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/miniterm.py
--rwxr--r--   0 root         (0) root         (0)     4495 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports_posix.py
--rwxr--r--   0 root         (0) root         (0)     4382 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports_linux.py
--rwxr--r--   0 root         (0) root         (0)     3354 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports_common.py
--rwxr--r--   0 root         (0) root         (0)     9302 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/tools/list_ports_osx.py
--rwxr--r--   0 root         (0) root         (0)     3168 2023-07-04 07:14:11.000000 cnextb-1.0.0/cnextb/connection_specific/serial/__init__.py
--rwxr--r--   0 root         (0) root         (0)    32032 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/serialposix.py
--rwxr--r--   0 root         (0) root         (0)    10853 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/win32.py
--rwxr--r--   0 root         (0) root         (0)     3265 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/rs485.py
--rwxr--r--   0 root         (0) root         (0)    20087 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/serialwin32.py
--rwxr--r--   0 root         (0) root         (0)    59444 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/rfc2217.py
--rwxr--r--   0 root         (0) root         (0)     8414 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/serial/serialjava.py
--rwxr--r--   0 root         (0) root         (0)     1670 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/connection_specific/connection_Serial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/device/
--rwxr--r--   0 root         (0) root         (0)     7901 2023-07-04 06:03:52.000000 cnextb-1.0.0/cnextb/device/scanDevices.py
--rwxr--r--   0 root         (0) root         (0)       93 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/device/__init__.py
--rwxr--r--   0 root         (0) root         (0)     3964 2023-07-04 06:02:45.000000 cnextb-1.0.0/cnextb/device/device.py
--rwxr--r--   0 root         (0) root         (0)     1755 2023-07-04 06:05:01.000000 cnextb-1.0.0/cnextb/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:20:09.000000 cnextb-1.0.0/cnextb/debug/
--rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.0/cnextb/debug/__init__.py
--rwxr--r--   0 root         (0) root         (0)      775 2023-07-04 06:00:56.000000 cnextb-1.0.0/cnextb/debug/terminal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/
+-rwxr--r--   0 root         (0) root         (0)      509 2023-07-04 08:23:44.000000 cnextb-1.0.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 08:24:12.000000 cnextb-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      554 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb.egg-info/SOURCES.txt
+-rwxr--r--   0 root         (0) root         (0)      357 2023-07-04 08:22:56.000000 cnextb-1.0.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)      554 2023-07-04 08:24:12.000000 cnextb-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb/
+-rwxr--r--   0 root         (0) root         (0)      316 2023-07-04 06:05:38.000000 cnextb-1.0.1/cnextb/smoke.py
+-rwxr--r--   0 root         (0) root         (0)      795 2023-07-04 06:04:28.000000 cnextb-1.0.1/cnextb/connection.py
+-rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 08:05:14.000000 cnextb-1.0.1/cnextb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb/connection_specific/
+-rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.1/cnextb/connection_specific/__init__.py
+-rwxr--r--   0 root         (0) root         (0)     1670 2023-07-04 05:58:30.000000 cnextb-1.0.1/cnextb/connection_specific/connection_Serial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb/device/
+-rwxr--r--   0 root         (0) root         (0)     7874 2023-07-04 08:04:50.000000 cnextb-1.0.1/cnextb/device/scanDevices.py
+-rwxr--r--   0 root         (0) root         (0)       93 2023-07-04 05:58:30.000000 cnextb-1.0.1/cnextb/device/__init__.py
+-rwxr--r--   0 root         (0) root         (0)     3964 2023-07-04 06:02:45.000000 cnextb-1.0.1/cnextb/device/device.py
+-rwxr--r--   0 root         (0) root         (0)     1755 2023-07-04 06:05:01.000000 cnextb-1.0.1/cnextb/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 08:24:12.000000 cnextb-1.0.1/cnextb/debug/
+-rwxr--r--   0 root         (0) root         (0)        0 2023-07-04 05:58:30.000000 cnextb-1.0.1/cnextb/debug/__init__.py
+-rwxr--r--   0 root         (0) root         (0)      775 2023-07-04 06:00:56.000000 cnextb-1.0.1/cnextb/debug/terminal.py
```

### Comparing `cnextb-1.0.0/cnextb/connection.py` & `cnextb-1.0.1/cnextb/connection.py`

 * *Files identical despite different names*

### Comparing `cnextb-1.0.0/cnextb/connection_specific/connection_Serial.py` & `cnextb-1.0.1/cnextb/connection_specific/connection_Serial.py`

 * *Files identical despite different names*

### Comparing `cnextb-1.0.0/cnextb/device/scanDevices.py` & `cnextb-1.0.1/cnextb/device/scanDevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import serial
 import math
-import cnextb.connection_specific.serial.tools.list_ports as serial_list
+import serial.tools.list_ports as serial_list
 
 
 def list_serial():
     serial_ports = serial_list.comports()
     serial_modules = dict()
 
     for i in serial_ports:
```

### Comparing `cnextb-1.0.0/cnextb/device/device.py` & `cnextb-1.0.1/cnextb/device/device.py`

 * *Files identical despite different names*

### Comparing `cnextb-1.0.0/cnextb/run.py` & `cnextb-1.0.1/cnextb/run.py`

 * *Files identical despite different names*

### Comparing `cnextb-1.0.0/cnextb/debug/terminal.py` & `cnextb-1.0.1/cnextb/debug/terminal.py`

 * *Files identical despite different names*

