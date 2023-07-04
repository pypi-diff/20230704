# Comparing `tmp/error-alerts-5.4.tar.gz` & `tmp/error-alerts-5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-5.4.tar", last modified: Tue Jul  4 14:39:10 2023, max compression
+gzip compressed data, was "error-alerts-5.5.tar", last modified: Tue Jul  4 14:42:01 2023, max compression
```

## Comparing `error-alerts-5.4.tar` & `error-alerts-5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:39:10.551880 error-alerts-5.4/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.4/.gitignore
--rw-rw-rw-   0        0        0     1301 2023-07-04 14:39:10.551880 error-alerts-5.4/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 14:39:10.547883 error-alerts-5.4/error_alerts/
--rw-rw-rw-   0        0        0     4168 2023-07-04 14:39:07.000000 error-alerts-5.4/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:39:10.550881 error-alerts-5.4/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-07-04 14:39:10.000000 error-alerts-5.4/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-04 14:39:10.000000 error-alerts-5.4/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:39:10.000000 error-alerts-5.4/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 14:39:10.000000 error-alerts-5.4/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 14:39:10.000000 error-alerts-5.4/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 14:39:10.552879 error-alerts-5.4/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-04 14:39:03.000000 error-alerts-5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.515481 error-alerts-5.5/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.5/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-07-04 14:42:01.515481 error-alerts-5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.510484 error-alerts-5.5/error_alerts/
+-rw-rw-rw-   0        0        0     4167 2023-07-04 14:41:51.000000 error-alerts-5.5/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 14:42:01.514481 error-alerts-5.5/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-04 14:42:01.000000 error-alerts-5.5/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 14:42:01.516480 error-alerts-5.5/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-04 14:41:56.000000 error-alerts-5.5/setup.py
```

### Comparing `error-alerts-5.4/PKG-INFO` & `error-alerts-5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.4
+Version: 5.5
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-5.4/README.md` & `error-alerts-5.5/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-5.4/error_alerts/__init__.py` & `error-alerts-5.5/error_alerts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                 
         return None
     
     def send_photo(self, photo, *messages, channel=None):
         if not channel:
             channel = self.channel
         caption = ''
-        if messages:
-            for message in messages:
+        for message in messages:
+            if message:
                 caption += message
                 caption += ' '
         try:
             self.telegram_bot.send_photo(channel, photo, caption)
         except Exception as telegram_error:
             self.printer('Error sending photo to Telegram:', telegram_error, level='error')
```

### Comparing `error-alerts-5.4/error_alerts.egg-info/PKG-INFO` & `error-alerts-5.5/error_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.4
+Version: 5.5
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

