# Comparing `tmp/irc_api-1.0.1.tar.gz` & `tmp/irc_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-1.0.1.tar", last modified: Mon Jul  3 15:00:52 2023, max compression
+gzip compressed data, was "irc_api-1.0.2.tar", last modified: Tue Jul  4 20:25:56 2023, max compression
```

## Comparing `irc_api-1.0.1.tar` & `irc_api-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 15:00:41.000000 irc_api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 15:00:52.572323 irc_api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 15:00:41.000000 irc_api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-03 15:00:41.000000 irc_api-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:00:52.572323 irc_api-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.568323 irc_api-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 20:25:43.000000 irc_api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 20:25:56.135182 irc_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 20:25:43.000000 irc_api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 20:25:43.000000 irc_api-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:25:56.135182 irc_api-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 20:25:43.000000 irc_api-1.0.2/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:25:56.135182 irc_api-1.0.2/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:25:56.000000 irc_api-1.0.2/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-1.0.1/LICENSE` & `irc_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/PKG-INFO` & `irc_api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-1.0.1/README.md` & `irc_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/pyproject.toml` & `irc_api-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/src/irc_api/bot.py` & `irc_api-1.0.2/src/irc_api/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         Parameters
         ----------
         nick : str
             The nickname of the bot.
         """
         # Start IRC
-        self.irc.connexion(nick, self.auth)
+        self.irc.connection(nick, self.auth)
 
         # Join channels
         for channel in self.channels:
             self.irc.join(channel)
 
         # mainloop
         while True:
```

### Comparing `irc_api-1.0.1/src/irc_api/commands.py` & `irc_api-1.0.2/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/src/irc_api/history.py` & `irc_api-1.0.2/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/src/irc_api/irc.py` & `irc_api-1.0.2/src/irc_api/irc.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 from queue import Queue
 from threading import Thread
 from irc_api.message import Message
 
 
 class IRC:
-    """Manage connexion to an IRC server, authentication and callbacks.
+    """Manage connection to an IRC server, authentication and callbacks.
 
     Attributes
     ----------
     connected : bool, public
         If the bot is connected to an IRC server or not.
 
     socket : ssl.SSLSocket, private
         The IRC's socket.
     inbox : Queue, private
         Queue of the incomming messages.
     handler : Thread, private
 
     Methods
     -------
-    connexion : NoneType, public
+    connection : NoneType, public
         Starts the IRC layer and manage authentication.
     send : NoneType, public
         Sends a message to a given channel.
     receive : Message, public
         Receive a new raw message and return the processed message. 
     join : NoneType, public
         Allows to join a given channel.
@@ -59,15 +59,15 @@
                 socket.create_connection((host, port)),
                 server_hostname=host
             )
         self.__inbox = Queue()
         self.__handler = Thread(target=self.__handle)
 
     # Public methods
-    def connexion(self, nick: str, auth: tuple=()):
+    def connection(self, nick: str, auth: tuple=()):
         """Start the IRC layer. Manage authentication as well.
 
         Parameters
         ----------
         nick : str
             The nickname used.
         auth : tuple, optionnal
@@ -78,16 +78,14 @@
 
         self.send(f"USER {nick} * * :{nick}")
         self.send(f"NICK {nick}")
         if auth:
             self.waitfor(lambda m: "NOTICE" in m and "/AUTH" in m)
             self.send(f"AUTH {auth[0]}:{auth[1]}")
 
-        self.waitfor(lambda m: "You are now logged in" in m)
-
         self.connected = True
 
     def send(self, raw: str):
         """Wrap and encode raw message to send.
 
         Parameters
         ----------
```

### Comparing `irc_api-1.0.1/src/irc_api/message.py` & `irc_api-1.0.2/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.1/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.2/src/irc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

