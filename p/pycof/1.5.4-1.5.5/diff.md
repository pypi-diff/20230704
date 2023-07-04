# Comparing `tmp/pycof-1.5.4.tar.gz` & `tmp/pycof-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycof-1.5.4.tar", last modified: Tue May  2 11:43:45 2023, max compression
+gzip compressed data, was "pycof-1.5.5.tar", last modified: Tue Jul  4 10:03:35 2023, max compression
```

## Comparing `pycof-1.5.4.tar` & `pycof-1.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.906039 pycof-1.5.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.4/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-05-02 11:43:45.906039 pycof-1.5.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.895205 pycof-1.5.4/pycof/
--rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.4/pycof/data.py
--rw-r--r--   0 florian   (1000) florian   (1000)    30739 2023-01-01 14:48:35.000000 pycof-1.5.4/pycof/format.py
--rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.4/pycof/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11316 2022-09-11 09:44:36.000000 pycof-1.5.4/pycof/misc.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.4/pycof/sql.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14352 2022-09-25 17:15:48.000000 pycof-1.5.4/pycof/sqlhelper.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.895205 pycof-1.5.4/pycof.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      313 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-02 11:43:45.906039 pycof-1.5.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1170 2023-03-12 10:48:27.000000 pycof-1.5.4/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1216 2023-05-02 11:43:45.000000 pycof-1.5.4/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.5/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 10:03:35.128156 pycof-1.5.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/pycof/
+-rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-07-04 10:03:34.000000 pycof-1.5.5/pycof/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.5/pycof/data.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    30792 2023-07-04 10:03:08.000000 pycof-1.5.5/pycof/format.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.5/pycof/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15161 2023-07-04 09:14:03.000000 pycof-1.5.5/pycof/misc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.5/pycof/sql.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14117 2023-07-04 08:44:49.000000 pycof-1.5.5/pycof/sqlhelper.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-04 10:03:35.128156 pycof-1.5.5/pycof.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      313 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-04 10:03:35.000000 pycof-1.5.5/pycof.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-07-04 10:03:35.128156 pycof-1.5.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1170 2023-03-12 10:48:27.000000 pycof-1.5.5/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1216 2023-07-04 10:03:34.000000 pycof-1.5.5/setup_new.py
```

### Comparing `pycof-1.5.4/LICENSE` & `pycof-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycof-1.5.4/PKG-INFO` & `pycof-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.4
+Version: 1.5.5
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.4/README.md` & `pycof-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pycof-1.5.4/pycof/data.py` & `pycof-1.5.5/pycof/data.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.4/pycof/format.py` & `pycof-1.5.5/pycof/format.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 from email.mime.multipart import MIMEMultipart
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from .sqlhelper import _get_config, _get_credentials
-from .misc import file_age, verbose_display, _pycof_folders
+from .misc import file_age, verbose_display, _pycof_folders, EmailSSHTunnel
 
 # Define default Google API scopes
 default_scopes = ['https://mail.google.com/', 'https://www.googleapis.com/auth/calendar.readonly']
 
 
 #######################################################################################################################
 
 # Send an Email
-def send_email(to, subject, body, cc='', credentials={}):
+def send_email(to, subject, body, cc='', credentials={}, connection='auto'):
     """Simplified function to send emails.
     Will look at the credentials at :obj:`/etc/.pycof/config.json`. User can also pass a dictionnary for credentials.
 
     :Parameters:
         * **to** (:obj:`str`): Recipient of the email.
         * **subject** (:obj:`str`): Subject of the email.
         * **body** (:obj:`str`): Content of the email to be send.
@@ -73,38 +73,34 @@
 
 
     :Example:
         >>> content = "This is a test"
         >>> pycof.send_email(to="test@domain.com", body=content, subject="Hello world!")
     """
     config = _get_config(credentials)
+
+    if connection.lower() == 'auto':
+        pattern = re.compile("^([0-9]+.[0-9]+.[0-9]+.[0-9]+)+$")
+        connection = 'direct' if pattern.match(config.get('EMAIL_SMTP')) else 'ssh'
     msg = MIMEMultipart()
-    msg['From'] = config.get('EMAIL_SENDER')
+    msg['From'] = config.get('EMAIL_USER')
     msg['To'] = to
-    msg['Cc'] = '' if cc == '' else cc
+    # msg['Cc'] = '' if cc == '' else cc
     msg['Subject'] = subject
 
     mail_type = 'html' if '</' in body else 'plain'
-    msg.attach(MIMEText(body, mail_type))
+    msg.attach(MIMEText(body))
 
     text = msg.as_string()
 
-    # Server login
-    try:
-        port = str(config.get('EMAIL_PORT'))
-    except Exception:
-        port = '587'  # Default Google port number
-    connection = config.get('EMAIL_SMTP') + ':' + port
-    server = smtplib.SMTP(connection)
-    server.starttls()
-    server.login(user=config.get('EMAIL_USER'), password=config.get('EMAIL_PASSWORD'))
-
-    # Send email
-    server.sendmail(config.get('EMAIL_USER'), [to, '', cc], text)
-    server.quit()
+    with EmailSSHTunnel(config=config, connection=connection) as tunnel:
+        conn = tunnel.connector()
+        conn.sendmail(config.get('EMAIL_USER'), [to, '', cc], text)
+        conn.quit()
+        # conn.sendmail('noreply@florianfelice.com','florian@florianfelice.com',msg.as_string())
 
 # Send an email from Gmail
 class google_email:
     def __init__(self, credentials={}, scopes=default_scopes, token_path=None):
         """Simplified class to send email from a Gmail email address with secured connection with developper API.
         The `Google credentials file <https://developers.google.com/calendar/quickstart/python>`_ needs to be saved as :obj:`/etc/.pycof/google.json`.
```

### Comparing `pycof-1.5.4/pycof/misc.py` & `pycof-1.5.5/pycof/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 import pandas as pd
 import numpy as np
 
 from io import StringIO, BytesIO
 
 from tqdm import tqdm
 import datetime
+import sshtunnel
+
+import smtplib
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+
 
 
 ########################################################################################################################
 # Get config file
 
 def _pycof_folders(output=None, verbose=False):
     # Define the root folder depending on the OS
@@ -257,7 +263,88 @@
         return(print(*element, sep=sep, end=end))
     elif (verbose in [1, True]) & (type(element) in [str]) & (return_list is False):
         return(print(element, sep=sep, end=end))
     elif (verbose in [0, False]) & (type(element) in [str, type(None)]):
         disp = 0  # we don't display anything
     else:
         return(element)
+
+
+# #######################################################################################################################
+# Fake SSH tunnel for direct connections
+
+class _fake_tunnel:
+    def __init__():
+        pass
+
+    def close():
+        pass
+
+########################################################################################################################
+# SSHTunnel for email
+class EmailSSHTunnel:
+    def __init__(self, config, connection='direct', engine='default'):
+        self.connection = connection.lower()
+        self.config = config
+        self.engine = engine
+
+    def __enter__(self):
+        if self.connection == 'ssh':
+            try:
+                ssh_port = 22 if self.config.get('SSH_PORT') is None else int(self.config.get('SSH_PORT'))
+                remote_addr = 'localhost' if self.config.get('EMAIL_REMOTE_HOST') is None else self.config.get('EMAIL_REMOTE_HOST')
+                remote_port = 1025 if self.config.get('EMAIL_REMOTE_PORT') is None else int(self.config.get('EMAIL_REMOTE_PORT'))
+                hostname = '127.0.0.1' if self.config.get('EMAIL_LOCAL_HOST') is None else self.config.get('EMAIL_LOCAL_HOST')
+
+                if (self.config.get('SSH_PASSWORD') is None) & (self.config.get('SSH_KEY') is None):
+                    # Try to get the default SSH location if neither a password nor a path is provided
+                    ssh_path = os.path.join(_pycof_folders('home'), '.ssh', 'id_rsa')
+                else:
+                    ssh_path = self.config.get('SSH_KEY')
+
+                self.tunnel = sshtunnel.SSHTunnelForwarder((self.config.get('EMAIL_SMTP'), ssh_port),
+                                                           ssh_username=self.config.get('SSH_USER'),
+                                                           ssh_password=self.config.get('SSH_PASSWORD'),
+                                                           ssh_pkey=ssh_path,
+                                                           remote_bind_address=(remote_addr, remote_port))
+                self.tunnel.daemon_forward_servers = True
+                self.tunnel.connector = self._define_connector
+            except Exception:
+                raise ConnectionError('Failed to establish SSH connection with host')
+        else:
+            self.tunnel = _fake_tunnel
+            self.tunnel.connector = self._define_connector
+
+        return self.tunnel
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.tunnel.close()
+
+    def _define_connector(self):
+        """Define the SQL connector for executing SQL.
+
+        :param config: Credentials file containing authentiation information, defaults to {}.
+        :type config: :obj:`dict`, optional
+        :param engine: SQL engine to use ('Redshift', 'SQLite' or 'MySQL'), defaults to 'default'
+        :type engine: str, optional
+        :param connection: Connextion type. Cqn either be 'direct' or 'SSH', defaults to 'direct'
+        :type connection: str, optional
+
+        :return: Connector, cursor and tunnel
+        """
+        user = self.config.get('EMAIL_USER')
+        password = self.config.get('EMAIL_PASSWORD')
+        hostname = self.config.get('EMAIL_SMTP')
+        port = self.config.get('EMAIL_PORT')
+
+        if self.connection.lower() == 'ssh':
+            hostname = '127.0.0.1' if self.config.get('EMAIL_REMOTE_HOST') is None else self.config.get('EMAIL_REMOTE_HOST')
+            self.tunnel.start()
+            port = self.tunnel.local_bind_port
+
+        try:
+            connector = smtplib.SMTP(hostname, port)
+            connector.login(user, password)
+        except Exception:
+            raise ConnectionError('Failed to connect to the email server')
+
+        return connector
```

### Comparing `pycof-1.5.4/pycof/sql.py` & `pycof-1.5.5/pycof/sql.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.4/pycof/sqlhelper.py` & `pycof-1.5.5/pycof/sqlhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 import datetime
 import hashlib
 import warnings
 import csv
 from types import SimpleNamespace
 
-from .misc import verbose_display, file_age, write, _get_config, _pycof_folders
+from .misc import verbose_display, file_age, write, _get_config, _pycof_folders, _fake_tunnel
 from .data import read
 
 # #######################################################################################################################
 # Cache data from SQL
 
 def _cache(sql, tunnel, query_type="SELECT", cache_time='24h', cache_file_name=None, cache_folder=None, verbose=False):
     # Parse cache_time value
@@ -141,24 +141,14 @@
         config['DB_USER']     = cluster_creds['DbUser']
         config['DB_PASSWORD'] = cluster_creds['DbPassword']
 
     return config
 
 
 # #######################################################################################################################
-# Fake SSH tunnel for direct connections
-
-class _fake_tunnel:
-    def __init__():
-        pass
-
-    def close():
-        pass
-
-# #######################################################################################################################
 # Get SSH tunnel
 
 class SSHTunnel:
     def __init__(self, config, connection='direct', engine='default'):
         self.connection = connection.lower()
         self.config = config
         self.engine = engine
```

### Comparing `pycof-1.5.4/pycof.egg-info/PKG-INFO` & `pycof-1.5.5/pycof.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.4
+Version: 1.5.5
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.4/setup.py` & `pycof-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.4/setup_new.py` & `pycof-1.5.5/setup_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycof",
-    version="1.5.4",
+    version="1.5.5",
     author="Florian Felice",
     author_email="admin@florianfelice.com",
     description="A package for commonly used functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/pycof",
     packages=setuptools.find_packages(),
```

