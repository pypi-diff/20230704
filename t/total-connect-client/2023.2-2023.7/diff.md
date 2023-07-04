# Comparing `tmp/total_connect_client-2023.2.tar.gz` & `tmp/total_connect_client-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total_connect_client-2023.2.tar", last modified: Fri Feb 24 23:45:05 2023, max compression
+gzip compressed data, was "total_connect_client-2023.7.tar", last modified: Tue Jul  4 15:10:41 2023, max compression
```

## Comparing `total_connect_client-2023.2.tar` & `total_connect_client-2023.7.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-24 23:45:05.373998 total_connect_client-2023.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2023.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6682 2023-02-24 23:45:05.373998 total_connect_client-2023.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6070 2023-02-24 21:24:49.000000 total_connect_client-2023.2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3229 2023-02-24 22:18:56.000000 total_connect_client-2023.2/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-02-24 23:45:05.373998 total_connect_client-2023.2/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-24 23:45:05.371998 total_connect_client-2023.2/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_authenticate.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_get_panel_meta_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_init.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_misc.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_client_validate_usercode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2191 2023-02-24 22:05:12.000000 total_connect_client-2023.2/tests/test_client_zone_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7192 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2176 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_location_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13454 2023-02-24 21:24:49.000000 total_connect_client-2023.2/tests/test_zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-24 23:45:05.372998 total_connect_client-2023.2/total_connect_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/arm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15022 2023-02-24 22:00:19.000000 total_connect_client-2023.2/total_connect_client/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5486 2023-02-24 21:44:26.000000 total_connect_client-2023.2/total_connect_client/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2023.2/total_connect_client/exceptions.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-24 23:45:05.372998 total_connect_client-2023.2/total_connect_client/live/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/live/auto_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/live/zwave.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13263 2023-02-24 23:41:11.000000 total_connect_client-2023.2/total_connect_client/location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9393 2023-02-24 21:24:49.000000 total_connect_client-2023.2/total_connect_client/zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-24 23:45:05.372998 total_connect_client-2023.2/total_connect_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6682 2023-02-24 23:45:05.000000 total_connect_client-2023.2/total_connect_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1104 2023-02-24 23:45:05.000000 total_connect_client-2023.2/total_connect_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-24 23:45:05.000000 total_connect_client-2023.2/total_connect_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2023-02-24 23:45:05.000000 total_connect_client-2023.2/total_connect_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-02-24 23:45:05.000000 total_connect_client-2023.2/total_connect_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2023.7/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7505 2023-07-04 15:10:41.722420 total_connect_client-2023.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6893 2023-06-25 20:47:34.000000 total_connect_client-2023.7/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3229 2023-07-04 15:10:00.000000 total_connect_client-2023.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-04 15:10:41.722420 total_connect_client-2023.7/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.721420 total_connect_client-2023.7/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_authenticate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_get_panel_meta_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_init.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2481 2023-04-29 22:02:21.000000 total_connect_client-2023.7/tests/test_client_misc.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_validate_usercode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3332 2023-06-29 00:24:58.000000 total_connect_client-2023.7/tests/test_client_zone_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7373 2023-04-29 21:52:35.000000 total_connect_client-2023.7/tests/test_location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1996 2023-06-28 23:58:46.000000 total_connect_client-2023.7/tests/test_location_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14210 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/arm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1219 2023-06-24 19:33:36.000000 total_connect_client-2023.7/total_connect_client/bypass_all.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15022 2023-02-24 22:00:19.000000 total_connect_client-2023.7/total_connect_client/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5608 2023-05-06 15:50:27.000000 total_connect_client-2023.7/total_connect_client/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2023.7/total_connect_client/exceptions.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client/live/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/live/auto_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/live/zwave.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15559 2023-06-24 19:33:41.000000 total_connect_client-2023.7/total_connect_client/location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      889 2023-05-06 16:48:15.000000 total_connect_client-2023.7/total_connect_client/sync.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9604 2023-06-22 02:49:55.000000 total_connect_client-2023.7/total_connect_client/zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7505 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1168 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/top_level.txt
```

### Comparing `total_connect_client-2023.2/LICENSE` & `total_connect_client-2023.7/LICENSE`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/PKG-INFO` & `total_connect_client-2023.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-Metadata-Version: 2.1
-Name: total_connect_client
-Version: 2023.2
-Summary: Interact with Total Connect 2 alarm systems
-Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
-Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
-Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
-Keywords: alarm,TotalConnect
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Total-Connect-Client
-Total-Connect-Client is a python client for interacting with the TotalConnect2 alarm system.
+Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
 
 Started by @craigjmidwinter to add alarm support for his personal HomeAssistant set-up, with later contributions from others.
 
-The package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
+To use with Home Assistant, follow the instructions to set up [Total Connect](https://www.home-assistant.io/integrations/totalconnect/).
+
+For command line or other uses, the package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
 
 The code currently supports:
  - Arming (away, stay, night)
  - Disarming
  - Getting panel status (armed, bypassed, etc)
  - Getting zone status (normal, fault, trouble, low battery, etc)
 
+## Zone Status
+
+To see zones that are faulted (open), your Total Connect account must have “Sensor Activities” enabled. Your alarm monitoring company may charge an extra fee to enable this. If available, these can be found in the Total Connect 2 web portal at **Notifications -> Sensor Activities**. Alternately, they can be found in the Total Connect mobile app at **More -> Settings -> Notifications -> Sensor Activities**. 
+
 ## Troubleshooting
 
 If you're having trouble with your system, or find an error message, we may ask you to submit information about your alarm system.  
 
 ### From Home Assistant
 
 - Go to https://<your_home_assistant>/config/integrations
@@ -150,10 +141,10 @@
 similar methods on the values of self.locations.
 
 ## Likely Future Interface Changes
 
 * Previously if the usercodes dictionary was invalid, the DEFAULT_USERCODE
 was silently used. In a future release, we will raise an exception on an invalid dictionary.
 
-If there's something about the interface you don't understand, check out the (Home Assistant integration)[https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/] that uses this package, or submit an issue here.
+If there's something about the interface you don't understand, check out the [Home Assistant integration](https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/) that uses this package, or [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues).
 
-During development, if you discover new status codes or other information not handled, please submit an issue to let us know, or even better submit a pull request.
+During development, if you discover new status codes or other information not handled, please [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues) to let us know, or even better submit a [pull request](https://github.com/craigjmidwinter/total-connect-client/pulls).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `total_connect_client-2023.2/README.md` & `total_connect_client-2023.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,41 @@
+Metadata-Version: 2.1
+Name: total_connect_client
+Version: 2023.7
+Summary: Interact with Total Connect 2 alarm systems
+Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
+Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
+Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
+Keywords: alarm,TotalConnect
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Total-Connect-Client
-Total-Connect-Client is a python client for interacting with the TotalConnect2 alarm system.
+Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
 
 Started by @craigjmidwinter to add alarm support for his personal HomeAssistant set-up, with later contributions from others.
 
-The package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
+To use with Home Assistant, follow the instructions to set up [Total Connect](https://www.home-assistant.io/integrations/totalconnect/).
+
+For command line or other uses, the package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
 
 The code currently supports:
  - Arming (away, stay, night)
  - Disarming
  - Getting panel status (armed, bypassed, etc)
  - Getting zone status (normal, fault, trouble, low battery, etc)
 
+## Zone Status
+
+To see zones that are faulted (open), your Total Connect account must have “Sensor Activities” enabled. Your alarm monitoring company may charge an extra fee to enable this. If available, these can be found in the Total Connect 2 web portal at **Notifications -> Sensor Activities**. Alternately, they can be found in the Total Connect mobile app at **More -> Settings -> Notifications -> Sensor Activities**. 
+
 ## Troubleshooting
 
 If you're having trouble with your system, or find an error message, we may ask you to submit information about your alarm system.  
 
 ### From Home Assistant
 
 - Go to https://<your_home_assistant>/config/integrations
@@ -135,10 +156,10 @@
 similar methods on the values of self.locations.
 
 ## Likely Future Interface Changes
 
 * Previously if the usercodes dictionary was invalid, the DEFAULT_USERCODE
 was silently used. In a future release, we will raise an exception on an invalid dictionary.
 
-If there's something about the interface you don't understand, check out the (Home Assistant integration)[https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/] that uses this package, or submit an issue here.
+If there's something about the interface you don't understand, check out the [Home Assistant integration](https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/) that uses this package, or [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues).
 
-During development, if you discover new status codes or other information not handled, please submit an issue to let us know, or even better submit a pull request.
+During development, if you discover new status codes or other information not handled, please [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues) to let us know, or even better submit a [pull request](https://github.com/craigjmidwinter/total-connect-client/pulls).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `total_connect_client-2023.2/pyproject.toml` & `total_connect_client-2023.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name="total_connect_client"
-version="2023.2"
+version="2023.7"
 authors = [
   { name="Craig J. Midwinter", email="craig.j.midwinter@gmail.com" },
 ]
 description="Interact with Total Connect 2 alarm systems"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `total_connect_client-2023.2/tests/test_client_arm_disarm.py` & `total_connect_client-2023.7/tests/test_client_arm_disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_client_authenticate.py` & `total_connect_client-2023.7/tests/test_client_authenticate.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_client_get_panel_meta_data.py` & `total_connect_client-2023.7/tests/test_client_get_panel_meta_data.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_client_init.py` & `total_connect_client-2023.7/tests/test_client_init.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_client_misc.py` & `total_connect_client-2023.7/tests/test_client_misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     RESPONSE_UNKNOWN,
 )
 
 from total_connect_client.zone import ZoneStatus
 
 from total_connect_client.exceptions import (
     BadResultCodeError,
-    PartialResponseError,
     TotalConnectError,
 )
 
 
 class TestTotalConnectClient(unittest.TestCase):
     """Test TotalConnectClient."""
 
@@ -73,9 +72,8 @@
             # second response is FEATURE_NOT_SUPPORTED
             self.location.get_zone_details()
             # third response is UNKNOWN
             with pytest.raises(BadResultCodeError):
                 self.location.get_zone_details()
             # third response is SUCCESS but with empty ZoneStatus
             # ...which we've seen before in the wild
-            with pytest.raises(PartialResponseError):
-                self.location.get_zone_details()
+            self.location.get_zone_details()
```

### Comparing `total_connect_client-2023.2/tests/test_client_request.py` & `total_connect_client-2023.7/tests/test_client_request.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_client_validate_usercode.py` & `total_connect_client-2023.7/tests/test_client_validate_usercode.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_location.py` & `total_connect_client-2023.7/tests/test_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,28 +102,31 @@
         del data["PanelMetadataAndStatus"]["Zones"]
         with pytest.raises(TotalConnectError):
             loc._update_zones(data)
         self.assertTrue(loc.arming_state.is_disarmed())
 
     def tests_set_zone_details(self):
         """Test set_zone_details with normal data passed in."""
-        self.location_normal._update_zone_details(RESPONSE_GET_ZONE_DETAILS_SUCCESS)
+        location = TotalConnectLocation(LOCATION_INFO_BASIC_NORMAL, None)
+        location._update_zone_details(RESPONSE_GET_ZONE_DETAILS_SUCCESS)
+        assert len(location.zones) == 1
 
-        # "Zones" is None
+        location = TotalConnectLocation(LOCATION_INFO_BASIC_NORMAL, None)
+        # "Zones" is None, as seen in #112 and #205
         response = deepcopy(RESPONSE_GET_ZONE_DETAILS_SUCCESS)
         response["ZoneStatus"]["Zones"] = None
-        with pytest.raises(PartialResponseError):
-            self.location_normal._update_zone_details(response)
+        location._update_zone_details(response)
+        assert len(location.zones) == 0
 
         # "ZoneStatusInfoWithPartitionId" is None
+        location = TotalConnectLocation(LOCATION_INFO_BASIC_NORMAL, None)
         response = deepcopy(RESPONSE_GET_ZONE_DETAILS_SUCCESS)
         response["ZoneStatus"]["Zones"] = {"ZoneStatusInfoWithPartitionId": None}
-        # now test with "ZoneInfo" is none
-        with pytest.raises(PartialResponseError):
-            self.location_normal._update_zone_details(response)
+        location._update_zone_details(response)
+        assert len(location.zones) == 0
 
     def tests_auto_bypass_low_battery(self):
         """Test auto bypass of low battery zones."""
 
         mock_client = Mock()
         loc = TotalConnectLocation(LOCATION_INFO_BASIC_NORMAL, mock_client)
```

### Comparing `total_connect_client-2023.2/tests/test_location_arm_disarm.py` & `total_connect_client-2023.7/tests/test_location_arm_disarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,32 @@
 
 from unittest.mock import patch
 
 from common import create_client
 from const import (
     LOCATION_INFO_BASIC_NORMAL,
     RESPONSE_ARMED_AWAY,
+    TCC_REQUEST_METHOD,
     # these are tested in test_client_arm_disarm for now
     # RESPONSE_ARMED_STAY,
     # RESPONSE_ARMED_STAY_NIGHT,
     # RESPONSE_DISARMED,
     # RESPONSE_FEATURE_NOT_SUPPORTED,
 )
 
 from total_connect_client.const import _ResultCode
 from total_connect_client.client import ArmingHelper
 
 # from total_connect_client.exceptions import AuthenticationError, BadResultCodeError
 
-TCC_REQUEST_METHOD = "total_connect_client.client.TotalConnectClient.request"
 
 RESPONSE_ARM_SUCCESS = {
     "ResultCode": _ResultCode.ARM_SUCCESS.value,
     "ResultData": "testing arm success",
 }
-RESPONSE_DISARM_SUCCESS = {
-    "ResultCode": _ResultCode.DISARM_SUCCESS.value,
-    "ResultData": "testing disarm success",
-}
 
 # returned when a zone is faulted
 RESPONSE_ARM_FAILED = {
     "ResultCode": _ResultCode.COMMAND_FAILED.value,
     "ResultData": "testing arm failed",
 }
 RESPONSE_DISARM_FAILED = {
```

### Comparing `total_connect_client-2023.2/tests/test_partition.py` & `total_connect_client-2023.7/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_user.py` & `total_connect_client-2023.7/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/tests/test_zone.py` & `total_connect_client-2023.7/tests/test_zone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test total_connect_client."""
 
 import unittest
+from unittest.mock import Mock
 
 import pytest
 from const import (
     ZONE_LOW_BATTERY,
     ZONE_STATUS_LYRIC_CONTACT,
     ZONE_STATUS_LYRIC_LOCAL_ALARM,
     ZONE_STATUS_LYRIC_KEYPAD,
@@ -93,31 +94,31 @@
 
 
 class TestTotalConnectZone(unittest.TestCase):
     """Test TotalConnectZone."""
 
     def setUp(self):
         """Test setup."""
-        self.zone_normal = tcz(ZS_NORMAL)
-        self.zone_bypassed = tcz(ZONE_BYPASSED)
-        self.zone_faulted = tcz(ZONE_FAULTED)
-        self.zone_tampered = tcz(ZONE_TAMPERED)
-        self.zone_low_battery = tcz(ZONE_LOW_BATTERY)
-        self.zone_bypassed_low_battery = tcz(ZONE_BYPASSED_LOW_BATTERY)
-        self.zone_trouble_low_battery = tcz(ZONE_TROUBLE_LOW_BATTERY)
-        self.zone_triggered = tcz(ZONE_TRIGGERED)
-        self.zone_button = tcz(ZONE_BUTTON)
-        self.zone_smoke = tcz(ZONE_SMOKE)
-        self.zone_gas = tcz(ZONE_GAS)
-        self.zone_lyric_contact = tcz(ZONE_STATUS_LYRIC_CONTACT)
-        self.zone_lyric_motion = tcz(ZONE_STATUS_LYRIC_MOTION)
-        self.zone_lyric_police = tcz(ZONE_STATUS_LYRIC_POLICE)
-        self.zone_lyric_temp = tcz(ZONE_STATUS_LYRIC_TEMP)
-        self.zone_lyric_keypad = tcz(ZONE_STATUS_LYRIC_KEYPAD)
-        self.zone_lyric_local_alarm = tcz(ZONE_STATUS_LYRIC_LOCAL_ALARM)
+        self.zone_normal = tcz(ZS_NORMAL, None)
+        self.zone_bypassed = tcz(ZONE_BYPASSED, None)
+        self.zone_faulted = tcz(ZONE_FAULTED, None)
+        self.zone_tampered = tcz(ZONE_TAMPERED, None)
+        self.zone_low_battery = tcz(ZONE_LOW_BATTERY, None)
+        self.zone_bypassed_low_battery = tcz(ZONE_BYPASSED_LOW_BATTERY, None)
+        self.zone_trouble_low_battery = tcz(ZONE_TROUBLE_LOW_BATTERY, None)
+        self.zone_triggered = tcz(ZONE_TRIGGERED, None)
+        self.zone_button = tcz(ZONE_BUTTON, None)
+        self.zone_smoke = tcz(ZONE_SMOKE, None)
+        self.zone_gas = tcz(ZONE_GAS, None)
+        self.zone_lyric_contact = tcz(ZONE_STATUS_LYRIC_CONTACT, None)
+        self.zone_lyric_motion = tcz(ZONE_STATUS_LYRIC_MOTION, None)
+        self.zone_lyric_police = tcz(ZONE_STATUS_LYRIC_POLICE, None)
+        self.zone_lyric_temp = tcz(ZONE_STATUS_LYRIC_TEMP, None)
+        self.zone_lyric_keypad = tcz(ZONE_STATUS_LYRIC_KEYPAD, None)
+        self.zone_lyric_local_alarm = tcz(ZONE_STATUS_LYRIC_LOCAL_ALARM, None)
 
     def tearDown(self):
         """Tear down."""
         self.zone_normal = None
         self.zone_bypassed = None
         self.zone_faulted = None
         self.zone_tampered = None
@@ -132,15 +133,15 @@
         self.zone_lyric_police = None
         self.zone_lyric_temp = None
         self.zone_lyric_keypad = None
         self.zone_lyric_local_alarm = None
 
     def tests_normal(self):
         """Normal zone."""
-        zone = tcz(ZS_NORMAL)
+        zone = tcz(ZS_NORMAL, None)
         assert zone.partition == "1"
         assert zone.is_bypassed() is False
         assert zone.is_faulted() is False
         assert zone.is_tampered() is False
         assert zone.is_low_battery() is False
         assert zone.is_troubled() is False
         assert zone.is_triggered() is False
@@ -315,15 +316,15 @@
         "ZoneDescription": "Gas",
         "PartitionId": "1",
         "ZoneTypeId": ZoneType.PROA7_MEDICAL,
         "CanBeBypassed": 0,
         "ZoneStatus": ZoneStatus.TAMPER,
     }
 
-    zone = tcz(zone_medical)
+    zone = tcz(zone_medical, None)
     assert zone.is_type_medical() is True
     assert zone.is_type_button() is True
     assert zone.is_tampered() is True
 
 
 def test_unknown_type():
     """Test unknown ZoneType."""
@@ -331,15 +332,15 @@
         "ZoneDescription": "Unknown",
         "PartitionId": "1",
         "ZoneTypeId": 12345,
         "CanBeBypassed": 0,
         "ZoneStatus": ZoneStatus.NORMAL,
     }
 
-    zone = tcz(zone_unknown)
+    zone = tcz(zone_unknown, None)
     assert zone.zone_type_id == 12345
     assert zone._unknown_type_reported is True
 
 
 def test_unknown_status():
     """Test unknown ZoneStatus."""
     zone_unknown = {
@@ -347,13 +348,36 @@
         "PartitionId": "1",
         "ZoneTypeId": 12345,
         "CanBeBypassed": 0,
     }
 
     # invalid status (i.e. None or a string) should raise exception
     with pytest.raises(TotalConnectError):
-        tcz(zone_unknown)
+        tcz(zone_unknown, None)
 
     # unknown but valid status provided, should not raise
     zone_unknown["ZoneStatus"] = 255
-    zone = tcz(zone_unknown)
+    zone = tcz(zone_unknown, None)
     assert zone.status == 255
+
+def test_bypass():
+    """Test bypassing a zone."""
+    location = Mock()
+    zone_data = {
+        "ZoneDescription": "MyZone",
+        "PartitionId": "1",
+        "ZoneTypeId": ZoneType.SECURITY,
+        "CanBeBypassed": 0,
+        "ZoneStatus": ZoneStatus.NORMAL,
+    }
+
+    # should do nothing if zone cannot be bypassed
+    zone = tcz(zone_data, location)
+    zone.bypass()
+    location.zone_bypass.assert_not_called()
+
+    # now make zone bypassable
+    zone_data["CanBeBypassed"] = 1
+    zone = tcz(zone_data, location)
+    zone.bypass()
+    location.zone_bypass.assert_called_once()
+
```

### Comparing `total_connect_client-2023.2/total_connect_client/__init__.py` & `total_connect_client-2023.7/total_connect_client/__init__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/__main__.py` & `total_connect_client-2023.7/total_connect_client/__main__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/arm.py` & `total_connect_client-2023.7/total_connect_client/arm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/client.py` & `total_connect_client-2023.7/total_connect_client/client.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/const.py` & `total_connect_client-2023.7/total_connect_client/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,18 @@
     BAD_USER_OR_PASSWORD = -50004
     INVALID_SESSIONID = -30002
     FAILED_TO_BYPASS_ZONE = -4504
     COMMAND_FAILED = -4502
     USER_CODE_UNAVAILABLE = -4114
     USER_CODE_INVALID = -4106
     FAILED_TO_CONNECT = -4104
+
+    # Invalid Parameter returned when requesting SyncPanelStatus using non-existant JobID.
+    INVALID_PARAMETER = -501
+
     BAD_OBJECT_REFERENCE = -400
     FEATURE_NOT_SUPPORTED = -120
     INVALID_SESSION = -102
     AUTHENTICATION_FAILED = -100
     CONNECTION_ERROR = 4101
```

### Comparing `total_connect_client-2023.2/total_connect_client/device.py` & `total_connect_client-2023.7/total_connect_client/device.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/disarm.py` & `total_connect_client-2023.7/total_connect_client/disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/exceptions.py` & `total_connect_client-2023.7/total_connect_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/live/auto_bypass.py` & `total_connect_client-2023.7/total_connect_client/live/auto_bypass.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/live/zwave.py` & `total_connect_client-2023.7/total_connect_client/live/zwave.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/location.py` & `total_connect_client-2023.7/total_connect_client/location.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self.configuration_sequence_number = None
         self.arming_state = None
         self.partitions = {}
         self._partition_list = None
         self.zones = {}
         self.usercode = DEFAULT_USERCODE
         self.auto_bypass_low_battery = False
+        self._sync_job_id = None
+        self._sync_job_state = None
 
         dib = (location_info_basic.get("DeviceList") or {}).get("DeviceInfoBasic")
         tcdevs = [TotalConnectDevice(d) for d in (dib or {})]
         self.devices = {tcdev.deviceid: tcdev for tcdev in tcdevs}
 
     def __str__(self):
         """Return a text string that is printable."""
@@ -206,14 +208,34 @@
         result = self.parent.request("Bypass", (
             self.parent.token, self.location_id, self.security_device_id, zone_id, self.usercode
         ))
         self.parent.raise_for_resultcode(result)
         LOGGER.info(f"BYPASSED {zone_id} at {self.location_id}")
         self.zones[zone_id]._mark_as_bypassed()
 
+    def zone_bypass_all(self):
+        """Bypass all faulted zones."""
+        faulted_zones = []
+        for zone_id, zone in self.zones.items():
+            if zone.is_faulted():
+                faulted_zones.append(zone_id)
+
+        if faulted_zones:
+            zone_list = {"int": faulted_zones}
+
+            result = self.parent.request("BypassAll", (
+                self.parent.token, self.location_id, self.security_device_id, zone_list, self.usercode
+            ))
+            self.parent.raise_for_resultcode(result)
+            LOGGER.info(f"BYPASSED all zones at location {self.location_id}")          
+
+    def clear_bypass(self):
+        """Clear all bypassed zones."""
+        self.disarm()
+
     def zone_status(self, zone_id: int):
         """Get status of a zone."""
         zone = self.zones.get(zone_id)
         if not zone:
             raise TotalConnectError(f"zone {zone_id} does not exist")
         return zone.status
 
@@ -251,18 +273,19 @@
         ZoneStatusInfoWithPartitionId provides additional info for setting up zones.
         If we used TotalConnectZone._update() it would overwrite missing data with None.
         """
         zone_info = ((result.get("ZoneStatus") or {}).get("Zones") or {}).get(
             "ZoneStatusInfoWithPartitionId"
         )
         if not zone_info:
-            raise PartialResponseError("no ZoneStatusInfoWithPartitionId", result)
-
-        for zonedata in zone_info:
-            self.zones[zonedata["ZoneID"]] = TotalConnectZone(zonedata)
+            LOGGER.warning("No zones found when starting TotalConnect. Try to sync your panel using the TotalConnect app or website.")
+            LOGGER.debug(f"_update_zone_details result: {result}")
+        else:
+            for zonedata in zone_info:
+                self.zones[zonedata["ZoneID"]] = TotalConnectZone(zonedata, self)
 
     def _update_status(self, result):
         """Update from result."""
         data = (result or {}).get("PanelMetadataAndStatus")
         if not data:
             raise PartialResponseError("no PanelMetadataAndStatus", result)
 
@@ -319,12 +342,44 @@
             zid = (zonedata or {}).get("ZoneID")
             if not zid:
                 raise PartialResponseError("no ZoneID", result)
             zone = self.zones.get(zid)
             if zone:
                 zone._update(zonedata)
             else:
-                zone = TotalConnectZone(zonedata)
+                zone = TotalConnectZone(zonedata, self)
                 self.zones[zid] = zone
 
             if zone.is_low_battery() and zone.can_be_bypassed and self.auto_bypass_low_battery:
                 self.zone_bypass(zid)
+
+    def sync_panel(self):
+        """Syncronize the panel with the TotalConnect server."""
+        result = self.parent.request(
+            "SynchronizeSecurityPanel",
+            (self.parent.token, None, self.usercode, self.location_id, False)
+        )
+        self.parent.raise_for_resultcode(result)
+        self._sync_job_id = result.get("JobID")
+        # Successful request so assume state is in progress
+        self._sync_job_state = 1
+        LOGGER.info(f"Started sync of panel for location {self.location_id}")
+
+    def get_sync_status(self):
+        """Get panel sync status from the TotalConnect server."""
+        result = self.parent.request(
+            "GetSyncJobStatus", 
+            (self.parent.token, self._sync_job_id, self.location_id)
+        )
+
+        try:
+            self.parent.raise_for_resultcode(result)
+            job_state = result.get("JobState")
+            if job_state == 1:
+                LOGGER.info(f"Panel sync for location {self.location_id} in progress")
+            elif job_state == 2:
+                LOGGER.info(f"Panel sync for location {self.location_id} complete")
+            else:
+                LOGGER.warning(f"Unknown panel sync status for location {self.location_id}")
+        except TotalConnectError:
+            LOGGER.error(f"Could not get status of Sync Job with ID {self._sync_job_id}")
+
```

### Comparing `total_connect_client-2023.2/total_connect_client/partition.py` & `total_connect_client-2023.7/total_connect_client/partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/user.py` & `total_connect_client-2023.7/total_connect_client/user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.2/total_connect_client/zone.py` & `total_connect_client-2023.7/total_connect_client/zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,18 @@
     VISTA_CONFIGURABLE_92 = 92
     VISTA_CONFIGURABLE_93 = 93
 
 
 class TotalConnectZone:
     """Do not create instances of this class yourself."""
 
-    def __init__(self, zone):
+    def __init__(self, zone, parent_location):
         """Initialize."""
         self.zoneid = zone.get("ZoneID")
+        self._parent_location = parent_location
         self.partition = None
         self.status = None
         self.zone_type_id = None
         self.can_be_bypassed = None
         self.battery_level = None
         self.signal_strength = None
         self.sensor_serial_number = None
@@ -247,7 +248,12 @@
             self.supervision_type = info.get("ZoneSupervisionType")
             self.chime_state = info.get("ChimeState")
             self.device_type = info.get("DeviceType")
 
     def _mark_as_bypassed(self):
         """Set is_bypassed status."""
         self.status |= ZoneStatus.BYPASSED
+
+    def bypass(self):
+        """Bypass the zone."""
+        if self.can_be_bypassed:
+            self._parent_location.zone_bypass(self.zoneid)
```

### Comparing `total_connect_client-2023.2/total_connect_client.egg-info/PKG-INFO` & `total_connect_client-2023.7/total_connect_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: total-connect-client
-Version: 2023.2
+Version: 2023.7
 Summary: Interact with Total Connect 2 alarm systems
 Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
 Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
 Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
 Keywords: alarm,TotalConnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Total-Connect-Client
-Total-Connect-Client is a python client for interacting with the TotalConnect2 alarm system.
+Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
 
 Started by @craigjmidwinter to add alarm support for his personal HomeAssistant set-up, with later contributions from others.
 
-The package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
+To use with Home Assistant, follow the instructions to set up [Total Connect](https://www.home-assistant.io/integrations/totalconnect/).
+
+For command line or other uses, the package can be downloaded at [PyPI](https://pypi.org/project/total-connect-client/).
 
 The code currently supports:
  - Arming (away, stay, night)
  - Disarming
  - Getting panel status (armed, bypassed, etc)
  - Getting zone status (normal, fault, trouble, low battery, etc)
 
+## Zone Status
+
+To see zones that are faulted (open), your Total Connect account must have “Sensor Activities” enabled. Your alarm monitoring company may charge an extra fee to enable this. If available, these can be found in the Total Connect 2 web portal at **Notifications -> Sensor Activities**. Alternately, they can be found in the Total Connect mobile app at **More -> Settings -> Notifications -> Sensor Activities**. 
+
 ## Troubleshooting
 
 If you're having trouble with your system, or find an error message, we may ask you to submit information about your alarm system.  
 
 ### From Home Assistant
 
 - Go to https://<your_home_assistant>/config/integrations
@@ -150,10 +156,10 @@
 similar methods on the values of self.locations.
 
 ## Likely Future Interface Changes
 
 * Previously if the usercodes dictionary was invalid, the DEFAULT_USERCODE
 was silently used. In a future release, we will raise an exception on an invalid dictionary.
 
-If there's something about the interface you don't understand, check out the (Home Assistant integration)[https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/] that uses this package, or submit an issue here.
+If there's something about the interface you don't understand, check out the [Home Assistant integration](https://github.com/home-assistant/core/blob/dev/homeassistant/components/totalconnect/) that uses this package, or [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues).
 
-During development, if you discover new status codes or other information not handled, please submit an issue to let us know, or even better submit a pull request.
+During development, if you discover new status codes or other information not handled, please [submit an issue](https://github.com/craigjmidwinter/total-connect-client/issues) to let us know, or even better submit a [pull request](https://github.com/craigjmidwinter/total-connect-client/pulls).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `total_connect_client-2023.2/total_connect_client.egg-info/SOURCES.txt` & `total_connect_client-2023.7/total_connect_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 tests/test_location_arm_disarm.py
 tests/test_partition.py
 tests/test_user.py
 tests/test_zone.py
 total_connect_client/__init__.py
 total_connect_client/__main__.py
 total_connect_client/arm.py
+total_connect_client/bypass_all.py
 total_connect_client/client.py
 total_connect_client/const.py
 total_connect_client/device.py
 total_connect_client/disarm.py
 total_connect_client/exceptions.py
 total_connect_client/location.py
 total_connect_client/partition.py
+total_connect_client/sync.py
 total_connect_client/user.py
 total_connect_client/zone.py
 total_connect_client.egg-info/PKG-INFO
 total_connect_client.egg-info/SOURCES.txt
 total_connect_client.egg-info/dependency_links.txt
 total_connect_client.egg-info/requires.txt
 total_connect_client.egg-info/top_level.txt
```

