# Comparing `tmp/sopel-remind-0.1.0.tar.gz` & `tmp/sopel-remind-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-remind-0.1.0.tar", last modified: Sun Jun 25 10:39:32 2023, max compression
+gzip compressed data, was "sopel-remind-0.2.0.tar", last modified: Mon Jul  3 22:35:28 2023, max compression
```

## Comparing `sopel-remind-0.1.0.tar` & `sopel-remind-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2020-08-04 11:49:52.000000 sopel-remind-0.1.0/LICENSE.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2702 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1511 2023-06-25 10:35:55.000000 sopel-remind-0.1.0/README.rst
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1561 2023-06-25 10:37:36.000000 sopel-remind-0.1.0/pyproject.toml
--rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      338 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/setup.cfg
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/sopel_remind/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2021-01-07 16:28:44.000000 sopel-remind-0.1.0/sopel_remind/__init__.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)    10605 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/sopel_remind/backend.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      594 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/sopel_remind/config.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     5509 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/sopel_remind/plugin.py
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/sopel_remind.egg-info/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2702 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      442 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/SOURCES.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/dependency_links.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       45 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/entry_points.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       16 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/requires.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       13 2023-06-25 10:39:32.000000 sopel-remind-0.1.0/sopel_remind.egg-info/top_level.txt
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-06-25 10:39:32.919111 sopel-remind-0.1.0/tests/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     4426 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/tests/test_at.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     8219 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/tests/test_backend.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6776 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/tests/test_in.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6073 2023-06-25 09:37:22.000000 sopel-remind-0.1.0/tests/test_integration.py
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2020-08-04 11:49:52.000000 sopel-remind-0.2.0/LICENSE.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     3210 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2019 2023-07-03 22:34:55.000000 sopel-remind-0.2.0/README.rst
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1561 2023-07-03 22:34:09.000000 sopel-remind-0.2.0/pyproject.toml
+-rw-r--r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      338 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/setup.cfg
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/sopel_remind/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2021-01-07 16:28:44.000000 sopel-remind-0.2.0/sopel_remind/__init__.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)    10605 2023-06-26 16:21:03.000000 sopel-remind-0.2.0/sopel_remind/backend.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      594 2023-06-26 16:43:31.000000 sopel-remind-0.2.0/sopel_remind/config.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     7312 2023-07-03 22:25:53.000000 sopel-remind-0.2.0/sopel_remind/plugin.py
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/sopel_remind.egg-info/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     3210 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      442 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/SOURCES.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/dependency_links.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       45 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/entry_points.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       16 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/requires.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       13 2023-07-03 22:35:28.000000 sopel-remind-0.2.0/sopel_remind.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-07-03 22:35:28.624550 sopel-remind-0.2.0/tests/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     4426 2023-06-25 09:37:22.000000 sopel-remind-0.2.0/tests/test_at.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     8219 2023-06-25 09:37:22.000000 sopel-remind-0.2.0/tests/test_backend.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6776 2023-06-25 09:37:22.000000 sopel-remind-0.2.0/tests/test_in.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     8789 2023-07-03 22:25:25.000000 sopel-remind-0.2.0/tests/test_integration.py
```

### Comparing `sopel-remind-0.1.0/LICENSE.txt` & `sopel-remind-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sopel-remind-0.1.0/PKG-INFO` & `sopel-remind-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-remind
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reminder plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>, Florian Strzelecki <florian.strzelecki@gmail.com>
 Maintainer-email: Florian Strzelecki <florian.strzelecki@gmail.com>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/sopel-irc/sopel-remind
 Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel-remind/issues
 Keywords: sopel,plugin,reminder,calendar,bot,irc
@@ -69,8 +69,18 @@
 Install
 =======
 
 The recommended way to install this plugin is to use ``pip``::
 
     $ pip install sopel-remind
 
-Note that this plugin requires Python 3.7+ and Sopel 7.1+.
+Note that this plugin requires Python 3.7+ and Sopel 7.1+. It won't work on
+Python versions that are not supported by the version of Sopel you are using.
+
+Migration from built-in
+=======================
+
+If you used Sopel 7.1 (or any previous version) and its built-in "remind"
+plugin, you may want to migrate your reminders to the new plugin. To do that,
+you can run the ``sopel-plugins configure remind`` command and allow the script
+to perform the migration. This will import the reminders from the original file
+before renaming it (by adding the ``.bk`` suffix).
```

### Comparing `sopel-remind-0.1.0/README.rst` & `sopel-remind-0.2.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -42,8 +42,18 @@
 Install
 =======
 
 The recommended way to install this plugin is to use ``pip``::
 
     $ pip install sopel-remind
 
-Note that this plugin requires Python 3.7+ and Sopel 7.1+.
+Note that this plugin requires Python 3.7+ and Sopel 7.1+. It won't work on
+Python versions that are not supported by the version of Sopel you are using.
+
+Migration from built-in
+=======================
+
+If you used Sopel 7.1 (or any previous version) and its built-in "remind"
+plugin, you may want to migrate your reminders to the new plugin. To do that,
+you can run the ``sopel-plugins configure remind`` command and allow the script
+to perform the migration. This will import the reminders from the original file
+before renaming it (by adding the ``.bk`` suffix).
```

### Comparing `sopel-remind-0.1.0/pyproject.toml` & `sopel-remind-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["sopel_remind", "sopel_remind.*"]
 namespaces = false
 
 [project]
 name = "sopel-remind"
-version = "0.1.0"
+version = "0.2.0"
 description = "Reminder plugin for Sopel"
 keywords = [
   "sopel",
   "plugin",
   "reminder",
   "calendar",
   "bot",
```

### Comparing `sopel-remind-0.1.0/sopel_remind/backend.py` & `sopel-remind-0.2.0/sopel_remind/backend.py`

 * *Files identical despite different names*

### Comparing `sopel-remind-0.1.0/sopel_remind/config.py` & `sopel-remind-0.2.0/sopel_remind/config.py`

 * *Files identical despite different names*

### Comparing `sopel-remind-0.1.0/sopel_remind/plugin.py` & `sopel-remind-0.2.0/sopel_remind/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Reminder plugin for Sopel."""
 from __future__ import annotations
 
+import io
 import os
 import threading
 from datetime import datetime
 
 import pytz
 from sopel import plugin, tools  # type: ignore
 from sopel.bot import Sopel, SopelWrapper  # type: ignore
 from sopel.config import Config  # type: ignore
+from sopel.config.types import BooleanAttribute  # type: ignore
 from sopel.trigger import Trigger  # type: ignore
 
 from . import backend, config
 
 LOCK = threading.RLock()
 LOGGER = tools.get_logger('remind')
 
@@ -24,28 +26,72 @@
 
 
 def shutdown(bot: Sopel):
     """Shutdown the plugin."""
     backend.shutdown(bot)
 
 
-def configure(settings: Config):
+def configure(settings: Config) -> None:
     """Configure the plugin."""
     settings.define_section('remind', config.RemindSection)
     settings.remind.configure_setting(
         'location',
         'In which folder would you like to store your reminders?',
         default=settings.core.homedir)
     os.makedirs(settings.remind.location, exist_ok=True)
 
+    # manage migration while configuring the plugin
+    migrate: str = input(
+        'Do you want to migrate from the built-in remind plugin? Y/n'
+    ) or 'y'
+    migrate_attr = BooleanAttribute('mock_migrate', default=True)
+    if migrate_attr.parse(migrate):
+        # is there anything to migrate?
+        builtin_filename = os.path.join(
+            settings.core.homedir,
+            settings.basename + '.reminders.db',
+        )
+
+        migrated: int = 0
+        if os.path.isfile(builtin_filename):
+            backup_name = builtin_filename + '.bk'
+            filename = backend.get_reminder_filename(settings)
+            migrated = migrate_builtin(builtin_filename, filename)
+            os.rename(builtin_filename, backup_name)
+            print('Migrated file renamed to "%s".' % backup_name)
+
+        if migrated:
+            print('Migrated %d reminder(s).' % migrated)
+        else:
+            print('There was no reminder to migrate. You are good to go!')
+
+
+def migrate_builtin(from_file: str, to_file: str) -> int:
+    """Migrate reminders from the built-in remind plugin."""
+    return_value: int = 0
+    reminders = backend.load_reminders(to_file)
+
+    with io.open(from_file, 'r', encoding='utf-8') as database:
+        for i, line in enumerate(database, start=1):
+            unixtime, channel, nick, message = line.split('\t', 3)
+            message = message.rstrip('\n')
+            timestamp = int(float(unixtime))  # ignore microseconds
+            reminders.append(
+                backend.Reminder(timestamp, channel, nick, message)
+            )
+            return_value = i
+
+    backend.save_reminders(reminders, to_file)
+    return return_value
+
 
 @plugin.interval(2)
 def reminder_job(bot: Sopel):
     """Check reminders every 2s."""
-    if not bot.backend.connected:
+    if not bot.backend.is_connected() or not bot.connection_registered:
         # Don't run if the bot is not connected.
         LOGGER.debug('No reminders to send while the bot is not connected.')
         return
 
     now = int(pytz.utc.localize(datetime.utcnow()).timestamp())
     kept = []
```

### Comparing `sopel-remind-0.1.0/sopel_remind.egg-info/PKG-INFO` & `sopel-remind-0.2.0/sopel_remind.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-remind
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reminder plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>, Florian Strzelecki <florian.strzelecki@gmail.com>
 Maintainer-email: Florian Strzelecki <florian.strzelecki@gmail.com>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/sopel-irc/sopel-remind
 Project-URL: Bug Tracker, https://github.com/sopel-irc/sopel-remind/issues
 Keywords: sopel,plugin,reminder,calendar,bot,irc
@@ -69,8 +69,18 @@
 Install
 =======
 
 The recommended way to install this plugin is to use ``pip``::
 
     $ pip install sopel-remind
 
-Note that this plugin requires Python 3.7+ and Sopel 7.1+.
+Note that this plugin requires Python 3.7+ and Sopel 7.1+. It won't work on
+Python versions that are not supported by the version of Sopel you are using.
+
+Migration from built-in
+=======================
+
+If you used Sopel 7.1 (or any previous version) and its built-in "remind"
+plugin, you may want to migrate your reminders to the new plugin. To do that,
+you can run the ``sopel-plugins configure remind`` command and allow the script
+to perform the migration. This will import the reminders from the original file
+before renaming it (by adding the ``.bk`` suffix).
```

### Comparing `sopel-remind-0.1.0/tests/test_at.py` & `sopel-remind-0.2.0/tests/test_at.py`

 * *Files identical despite different names*

### Comparing `sopel-remind-0.1.0/tests/test_backend.py` & `sopel-remind-0.2.0/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `sopel-remind-0.1.0/tests/test_in.py` & `sopel-remind-0.2.0/tests/test_in.py`

 * *Files identical despite different names*

