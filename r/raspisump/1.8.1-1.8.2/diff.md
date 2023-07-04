# Comparing `tmp/raspisump-1.8.1.tar.gz` & `tmp/raspisump-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.8.1.tar", last modified: Fri Jun 16 18:15:34 2023, max compression
+gzip compressed data, was "raspisump-1.8.2.tar", last modified: Tue Jul  4 19:20:47 2023, max compression
```

## Comparing `raspisump-1.8.1.tar` & `raspisump-1.8.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8.1/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8.1/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3971 2023-06-16 18:15:34.076269 raspisump-1.8.1/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8.1/README.md
--rw-r--r--   0 al        (1000) users      (984)       13 2023-06-16 18:14:35.000000 raspisump-1.8.1/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8.1/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     6100 2023-06-16 18:14:35.000000 raspisump-1.8.1/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/css/includes.js
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/css/raspi.css
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/web/images/logo.png
--rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8.1/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8.1/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.1/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4788 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8.1/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2090 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4298 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2126 2023-06-15 16:24:24.000000 raspisump-1.8.1/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3971 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      809 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-06-16 18:15:34.076269 raspisump-1.8.1/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2404 2023-06-16 18:14:35.000000 raspisump-1.8.1/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8.1/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.8.1/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8.2/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8.2/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3971 2023-07-04 19:20:47.939979 raspisump-1.8.2/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8.2/README.md
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-07-04 19:19:39.000000 raspisump-1.8.2/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8.2/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      884 2023-07-04 19:19:39.000000 raspisump-1.8.2/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5937 2023-06-28 18:51:37.000000 raspisump-1.8.2/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8.2/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8.2/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.936646 raspisump-1.8.2/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.2/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8.2/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2413 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/config_values.py
+-rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8.2/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3971 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      836 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       18 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-07-04 19:20:47.939979 raspisump-1.8.2/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2409 2023-07-04 19:19:39.000000 raspisump-1.8.2/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8.2/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.8.2/tests/tests_sump.py
```

### Comparing `raspisump-1.8.1/LICENSE` & `raspisump-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/PKG-INFO` & `raspisump-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8.1
+Version: 1.8.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.8.1/README.md` & `raspisump-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/bin/rsumpchart.py` & `raspisump-1.8.2/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/bin/rsumpmonitor.py` & `raspisump-1.8.2/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/bin/rsumpwebchart.py` & `raspisump-1.8.2/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/conf/raspisump.conf` & `raspisump-1.8.2/conf/raspisump.conf`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,14 @@
 # e.g
 # red(ff0000), black(000000), blue(0000ff), default rsumporange(FB921D)
 line_color = FB921D
 
 
 [email]
 
-# ***Important information for Gmail users only.***
-# ***Please read this thread on allowing applications to send
-# ***email from Googles Gmail service which have implemented ouath2.
-# ***https://github.com/alaudet/raspi-sump/issues/6
-
-# ***Raspi-sump does not implement oauth2 for authentication so you will need 
-# ***to use a workaround for gmail to send alerts.
-
 # Set an appropriate interval for alerts.  If you are taking readings at short
 # intervals it is possible to bombard yourself with SMS text messages when the
 # water reaches a critical level.  For example if you are taking a reading
 # every minute or less an SMS Email alert will be sent each time the reading is
 # taken.  By setting the alert_interval this allows you to receive an email
 # alert at a more appropriate time interval.  Readings will continue and will
 # be logged but SMS text alerts will only be sent as you define it.  
@@ -92,51 +84,54 @@
 # If using localhost or possibly your ISP email this value
 # will most likely be 0.  Check your ISP's configuration docs.
 # For Gmail set this to 1 and fill out the corresponding 
 # username and password values in this file.
 smtp_authentication = 0
 
 
-# SMTP Server uses SSL (0=No, 1=Yes)
+# SMTP Server Information
 # Most SMTP servers are now supporting ssl over tls.  However you can
 # explicitely request tls if need to.
 # leaving both tls and ssl to zero will omit encryption entirely.
 # Select 1 for either, but never both.
 # For Gmail set smtp_ssl to 1.  Gmail can also use tls if needed for the time
 # being.
+# Office 365 Mail uses TLS
 
 # SMTP Server uses TLS (0=No, 1=Yes)
 smtp_tls = 0
 # SMTP Server uses SSL (0=No, 1=Yes)
 smtp_ssl = 0
 
 # If server requires authentication enter username and password.
 # For Gmail, activate these values with your gmail username and app password.
 # See https://support.google.com/mail/answer/185833?hl=en for instructions on 
 # setting an app password.
+# Office 365 also uses app password
+# See https://support.microsoft.com/en-us/account-billing/manage-app-passwords-for-two-step-verification-d6dc8c6d-4bf7-4851-ad95-6d07799387e9
 
 username = 
 password = 
 
 # SMTP Server and Port
-# example --  smtp_server = smtp.gmail.com:587  (TLS)
+# example --  smtp_server = smtp.office365.com:587  (TLS)
 # example --  smtp_server = smtp.gmail.com:465  (SSL)
 # if using a SMTP server on the Pi use localhost:25
 smtp_server = localhost:25
 
 # Notifications will be sent to the following address
 # example -- email_to = cellnumber@wireless_carrier (for sms email alerts)
 # You can also use a regular email address
 # To add multiple recipients seperate email addresses with a comma.
 # e.g. Adding a single recipient
 #   email_to = single_email@somewhere.com
 #
 # e.g. Adding multiple recipients
 #   email_to = recipient1@somewhere.com, recipient2@somewhere.com
-#   Don't forget the space after the comma in the line above.
+#   ****Don't forget the space after the comma in the line above***
 # 
 #   To test emails, run the command 'emailtest' from the pi terminal.
 email_to = 
 
 # Notification will be coming from the following address.
 # You can enter your email address here as the sender.
 # example  email_from = Raspi-Sump <youremail@yourprovider.com>
```

### Comparing `raspisump-1.8.1/conf/web/images/logo.png` & `raspisump-1.8.2/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/conf/web/index.html` & `raspisump-1.8.2/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/docs/install.md` & `raspisump-1.8.2/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/docs/install.pdf` & `raspisump-1.8.2/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/raspisump/alerts.py` & `raspisump-1.8.2/raspisump/alerts.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,50 +8,22 @@
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import os
 import time
 import smtplib
 from datetime import datetime
 import platform
-import configparser
 from collections import deque
 import csv
-from raspisump import log
+from raspisump import log, config_values
 
 
-config = configparser.RawConfigParser()
 user = os.getlogin()
-config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
-configs = {
-    "email_to": config.get("email", "email_to"),
-    "email_from": config.get("email", "email_from"),
-    "smtp_authentication": config.getint("email", "smtp_authentication"),
-    "smtp_tls": config.getint("email", "smtp_tls"),
-    "smtp_server": config.get("email", "smtp_server"),
-    "username": config.get("email", "username"),
-    "password": config.get("email", "password"),
-    "unit": config.get("pit", "unit"),
-}
-# If item in raspisump.conf add to configs dict above.  If not then provide
-# a default value
-try:
-    configs["alert_interval"] = config.getint("email", "alert_interval")
-except configparser.NoOptionError:
-    configs["alert_interval"] = 5
-
-try:
-    configs["alert_when"] = config.get("pit", "alert_when")
-except configparser.NoOptionError:
-    configs["alert_when"] = "high"
-
-try:
-    configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
-except configparser.NoSectionError:
-    configs["smtp_ssl"] = 0
+configs = config_values.configuration()
 
 
 def current_time():
     """Return the current time as reported by the OS."""
     return time.strftime("%I:%M%P %Z")
```

### Comparing `raspisump-1.8.1/raspisump/checkpid.py` & `raspisump-1.8.2/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/raspisump/heartbeat.py` & `raspisump-1.8.2/raspisump/heartbeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,43 +7,22 @@
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import os
 import time
 import smtplib
 from datetime import datetime, timedelta
-import configparser
 from collections import deque
 import csv
-from raspisump import log, alerts
+from raspisump import log, alerts, config_values
 
 
-config = configparser.RawConfigParser()
 user = os.getlogin()
-config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
-configs = {
-    "email_to": config.get("email", "email_to"),
-    "email_from": config.get("email", "email_from"),
-    "smtp_authentication": config.getint("email", "smtp_authentication"),
-    "smtp_tls": config.getint("email", "smtp_tls"),
-    "smtp_server": config.get("email", "smtp_server"),
-    "username": config.get("email", "username"),
-    "password": config.get("email", "password"),
-}
-
-try:
-    configs["heartbeat_interval"] = config.getint("email", "heartbeat_interval")
-except configparser.NoOptionError:
-    configs["heartbeat_interval"] = 10080
-
-try:
-    configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
-except configparser.NoSectionError:
-    configs["smtp_ssl"] = 0
+configs = config_values.configuration()
 
 
 def get_last_alert_time():
     """Retrieve the last alert time string from logfile"""
     heartbeat_log = "/home/" + user + "/raspi-sump/logs/heartbeat_log"
     with open(heartbeat_log, "rt") as f:
         last_row = deque(csv.reader(f), 1)[0]
```

### Comparing `raspisump-1.8.1/raspisump/log.py` & `raspisump-1.8.2/raspisump/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import time
 import os
 
 user = os.getlogin()
 
 
 def log_event(logfile, notification):
+    """Write event notification to a logfile"""
     _logfile = f"/home/{user}/raspi-sump/logs/{logfile}"
     with open(_logfile, "a") as f:
         f.write(f"{time.strftime('%Y-%m-%d %H:%M:%S,')}")
         f.write(f"{notification}\n")
 
 
 def log_reading(logfile, water_depth):
```

### Comparing `raspisump-1.8.1/raspisump/reading.py` & `raspisump-1.8.2/raspisump/reading.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,42 +3,18 @@
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
-import os
-import configparser
 from hcsr04sensor import sensor
-from raspisump import log, alerts, heartbeat
+from raspisump import log, alerts, heartbeat, config_values
 
-config = configparser.RawConfigParser()
-user = os.getlogin()
-config.read("/home/" + user + "/raspi-sump/raspisump.conf")
-
-configs = {
-    "critical_water_level": config.getint("pit", "critical_water_level"),
-    "pit_depth": config.getint("pit", "pit_depth"),
-    "temperature": config.getint("pit", "temperature"),
-    "trig_pin": config.getint("gpio_pins", "trig_pin"),
-    "echo_pin": config.getint("gpio_pins", "echo_pin"),
-    "unit": config.get("pit", "unit"),
-}
-
-# If item in raspisump.conf add to configs dict. If not provide defaults.
-try:
-    configs["alert_when"] = config.get("pit", "alert_when")
-except configparser.NoOptionError:
-    configs["alert_when"] = "high"
-
-try:
-    configs["heartbeat"] = config.getint("email", "heartbeat")
-except configparser.NoOptionError:
-    configs["heartbeat"] = 0
+configs = config_values.configuration()
 
 
 def initiate_heartbeat():
     """Initiate the heartbeat email process if needed"""
     if configs["heartbeat"] == 1:
         heartbeat.determine_if_heartbeat()
     else:
```

### Comparing `raspisump-1.8.1/raspisump/todaychart.py` & `raspisump-1.8.2/raspisump/todaychart.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,35 +4,27 @@
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
-import os
 import numpy as np
 import matplotlib as mpl
 
 mpl.use("Agg")
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib import rcParams
+from raspisump import config_values
 
 rcParams.update({"figure.autolayout": True})
-import configparser
 
-config = configparser.RawConfigParser()
-user = os.getlogin()
-config.read("/home/" + user + "/raspi-sump/raspisump.conf")
-configs = {"unit": config.get("pit", "unit")}
-
-try:
-    configs["line_color"] = config.get("charts", "line_color")
-except configparser.NoSectionError:
-    configs["line_color"] = "FB921D"
+
+configs = config_values.configuration()
 
 
 rcParams["date.autoformatter.minute"] = "%H:%M:%S"
 rcParams["date.autoformatter.hour"] = "%H:%M:%S"
 
 
 def graph(csv_file, filename):
```

### Comparing `raspisump-1.8.1/raspisump/webchart.py` & `raspisump-1.8.2/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.1/raspisump.egg-info/PKG-INFO` & `raspisump-1.8.2/raspisump.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8.1
+Version: 1.8.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.8.1/raspisump.egg-info/SOURCES.txt` & `raspisump-1.8.2/raspisump.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 cron/picrontab
 docs/README.md
 docs/install.md
 docs/install.pdf
 raspisump/__init__.py
 raspisump/alerts.py
 raspisump/checkpid.py
+raspisump/config_values.py
 raspisump/emailtest.py
 raspisump/heartbeat.py
 raspisump/log.py
 raspisump/reading.py
 raspisump/todaychart.py
 raspisump/webchart.py
 raspisump.egg-info/PKG-INFO
```

### Comparing `raspisump-1.8.1/setup.py` & `raspisump-1.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.8.1"
+version = "1.8.2"
 user = os.getlogin()
 
 homedir = "/home/" + user + "/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
@@ -57,15 +57,15 @@
     author_email="alaudet@linuxnorth.org",
     url="https://www.linuxnorth.org/raspi-sump/",
     download_url="https://github.com/alaudet/raspi-sump/releases",
     license="MIT License",
     packages=["raspisump"],
     scripts=raspi_sump_files,
     data_files=add_files,
-    install_requires=["hcsr04sensor"],
+    install_requires=["hcsr04sensor>=1.7"],
 )
 
 if os.path.isdir(homedir):
     cmd = "chown -R " + user + " " + homedir
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "raspisump.conf"
     os.system(cmd)
```

### Comparing `raspisump-1.8.1/tests/tests_logging.py` & `raspisump-1.8.2/tests/tests_logging.py`

 * *Files identical despite different names*

