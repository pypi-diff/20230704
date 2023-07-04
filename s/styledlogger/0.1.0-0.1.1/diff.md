# Comparing `tmp/styledlogger-0.1.0.tar.gz` & `tmp/styledlogger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.1.0.tar", last modified: Wed Jun 21 13:19:32 2023, max compression
+gzip compressed data, was "styledlogger-0.1.1.tar", last modified: Tue Jul  4 09:17:11 2023, max compression
```

## Comparing `styledlogger-0.1.0.tar` & `styledlogger-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.535569 styledlogger-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-21 13:19:20.000000 styledlogger-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 13:19:32.535569 styledlogger-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-21 13:19:20.000000 styledlogger-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:19:32.535569 styledlogger-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 13:19:20.000000 styledlogger-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.531569 styledlogger-0.1.0/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.535569 styledlogger-0.1.0/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 13:19:20.000000 styledlogger-0.1.0/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:19:32.531569 styledlogger-0.1.0/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 13:19:32.000000 styledlogger-0.1.0/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.591174 styledlogger-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 09:16:56.000000 styledlogger-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-04 09:17:11.591174 styledlogger-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 09:16:56.000000 styledlogger-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:17:11.591174 styledlogger-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 09:16:56.000000 styledlogger-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.587174 styledlogger-0.1.1/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.591174 styledlogger-0.1.1/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-04 09:16:56.000000 styledlogger-0.1.1/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:17:11.587174 styledlogger-0.1.1/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 09:17:11.000000 styledlogger-0.1.1/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.1.0/LICENSE` & `styledlogger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.0/PKG-INFO` & `styledlogger-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -16,15 +16,15 @@
 
 # StyledLogger
 
 ### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+Then you can import the `StyledLogger` class from the `styledlogger` package, and initialize it with a name.
 
 ---
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
@@ -42,9 +42,11 @@
 
 >>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
 22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+There's much more you can do with this library, and I encourage you to play around. Some features include file logging, custom callbacks and more.
+
+Check out the GitHub: https://github.com/BareAlek/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.1.0/README.md` & `styledlogger-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # StyledLogger
 
 ### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+Then you can import the `StyledLogger` class from the `styledlogger` package, and initialize it with a name.
 
 ---
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
@@ -26,9 +26,11 @@
 
 >>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
 22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+There's much more you can do with this library, and I encourage you to play around. Some features include file logging, custom callbacks and more.
+
+Check out the GitHub: https://github.com/BareAlek/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.1.0/styledlogger/classes/printcolors.py` & `styledlogger-0.1.1/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.1.0/styledlogger/classes/styleconfig.py` & `styledlogger-0.1.1/styledlogger/classes/styleconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,17 @@
         fatal_color: str = "purple",
         system_color: str = "cyan",
     ) -> None:
         self.text_format = text_format
         self.time_format = time_format
         self.time_color = self._validate_color(time_color)
         self.name_color = self._validate_color(name_color)
-        self.text_color = self._validate_color(
-            text_color) if text_color else Colors.RESET
+        self.text_color = (
+            self._validate_color(text_color) if text_color else Colors.RESET
+        )
 
         self.debug_color = self._validate_color(debug_color)
         self.info_color = self._validate_color(info_color)
         self.warn_color = self._validate_color(warn_color)
         self.error_color = self._validate_color(error_color)
         self.fatal_color = self._validate_color(fatal_color)
         self.system_color = self._validate_color(system_color)
@@ -86,15 +87,17 @@
             "%msg%": self.text_color + text + self.reset,
         }
 
         for k, v in replacemap.items():
             format_blueprint = format_blueprint.replace(k, v)
         return format_blueprint
 
-    def style_text_uncolored(self, logger_name: str, print_type: PrintType, text: str) -> str:
+    def style_text_uncolored(
+        self, logger_name: str, print_type: PrintType, text: str
+    ) -> str:
         """
         Style the text according to the style config.
         """
         format_blueprint = self.text_format
 
         replacemap = {
             "%name%": logger_name,
```

### Comparing `styledlogger-0.1.0/styledlogger/logger.py` & `styledlogger-0.1.1/styledlogger/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from colorama import (
     just_fix_windows_console,
 )
 
 from .classes.styleconfig import StyleConfig
-from .classes.printtypes import PrintType, \
-    Debug, Info, Warn, Error, Fatal, System
+from .classes.printtypes import PrintType, Debug, Info, Warn, Error, Fatal, System
+from .classes.callback import Callback
 
 just_fix_windows_console()
 
 
 class Logger:
     """
     The main object for logging.
@@ -20,21 +20,40 @@
 
     def __init__(self, name: str, *, file: str = None, level: int = 1) -> None:
         self.name = name
         self.level = level
         self.is_muted = False
         self.style_config = StyleConfig()
         self.file_path = file
+        self.callbacks = []
 
     def set_level(self, level):
         """
         Set the log level. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
         """
         self.level = level
 
+    def add_callback(self, name: str, activation_level, callback: callable):
+        """
+        Add a callback to the logger. The callback will be called with the message as the first argument.
+        """
+        self.callbacks.append(
+            Callback(name=name, activation_level=activation_level, callback=callback)
+        )
+    
+    def remove_callback(self, name: str):
+        """
+        Remove a callback from the logger.
+        """
+        for callback in self.callbacks:
+            if callback.name == name:
+                self.callbacks.remove(callback)
+                return True
+        return False
+
     def debug(self, message):
         """
         Log a debug message
         """
         if self.level <= 0:
             self._log(message, Debug)
 
@@ -69,21 +88,30 @@
     def system(self, message):
         """
         Log a system message
         """
         self._log(message, System)
 
     def _log(self, message, print_type: PrintType):
+
+        for callback in self.callbacks:
+            if callback.activation_level <= print_type.level:
+                callback.run_callback(level=print_type.level, message=message)
+
         if self.is_muted:
             return
 
         if self.file_path:
-            with open(self.file_path, "a+", encoding='utf-8') as file:
-                file.write(self.style_config.style_text_uncolored(
-                    self.name, print_type, message) + "\n")
+            with open(self.file_path, "a+", encoding="utf-8") as file:
+                file.write(
+                    self.style_config.style_text_uncolored(
+                        self.name, print_type, message
+                    )
+                    + "\n"
+                )
 
         print(self.style_config.style_text(self.name, print_type, message))
 
     def set_style(self, style_config: StyleConfig):
         """
         Change the style config of the logger.
         """
```

### Comparing `styledlogger-0.1.0/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.1.1/styledlogger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -16,15 +16,15 @@
 
 # StyledLogger
 
 ### A simple, yet beautiful logging library for Python 🐍 > 3.7
 
 To use, simply install via `pip install styledlogger`
 
-Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
+Then you can import the `StyledLogger` class from the `styledlogger` package, and initialize it with a name.
 
 ---
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
@@ -42,9 +42,11 @@
 
 >>> logger.set_style(StyleConfig( text_format="%time% | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
 
 >>> logger.warn("CPU usage exceeding 90%")
 22/04/2023 10:01 | WARN - CPU usage exceeding 90%
 ```
 
-Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
+There's much more you can do with this library, and I encourage you to play around. Some features include file logging, custom callbacks and more.
+
+Check out the GitHub: https://github.com/BareAlek/StyledLogger
 Contact me at mail: alek@imalek.me
```

