# Comparing `tmp/opr-200.tar.gz` & `tmp/opr-210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-200.tar", last modified: Mon Jun 26 13:37:42 2023, max compression
+gzip compressed data, was "opr-210.tar", last modified: Tue Jul  4 00:54:05 2023, max compression
```

## Comparing `opr-200.tar` & `opr-210.tar`

### file list

```diff
@@ -1,56 +1,47 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-26 13:37:42.431785 opr-200/
--rw-r--r--   0 bart      (1000) bart      (1000)     2432 2023-06-26 13:37:42.423785 opr-200/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1882 2023-06-26 13:27:33.000000 opr-200/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-26 13:37:42.419785 opr-200/opr/
--rw-r--r--   0 bart      (1000) bart      (1000)     2666 2023-06-26 13:27:33.000000 opr-200/opr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2492 2023-06-26 13:27:33.000000 opr-200/opr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      600 2023-06-26 13:27:33.000000 opr-200/opr/clients.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1110 2023-06-26 13:27:33.000000 opr-200/opr/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2094 2023-06-26 13:27:33.000000 opr-200/opr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      180 2023-06-26 13:27:33.000000 opr-200/opr/configs.py
--rw-r--r--   0 bart      (1000) bart      (1000)      817 2023-06-26 13:27:33.000000 opr-200/opr/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      399 2023-06-26 13:27:33.000000 opr-200/opr/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)      302 2023-06-26 13:27:33.000000 opr-200/opr/defines.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1344 2023-06-26 13:27:33.000000 opr-200/opr/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      381 2023-06-26 13:27:33.000000 opr-200/opr/errored.py
--rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-06-26 13:27:33.000000 opr-200/opr/evented.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1974 2023-06-26 13:27:33.000000 opr-200/opr/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      954 2023-06-26 13:27:33.000000 opr-200/opr/listens.py
--rw-r--r--   0 bart      (1000) bart      (1000)      466 2023-06-26 13:27:33.000000 opr-200/opr/logging.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-26 13:37:42.423785 opr-200/opr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      488 2023-06-26 13:27:33.000000 opr-200/opr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      596 2023-06-26 13:27:33.000000 opr-200/opr/modules/cfg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      234 2023-06-26 13:27:33.000000 opr-200/opr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      730 2023-06-26 13:27:33.000000 opr-200/opr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      439 2023-06-26 13:27:33.000000 opr-200/opr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      979 2023-06-26 13:27:33.000000 opr-200/opr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20870 2023-06-26 13:27:33.000000 opr-200/opr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      725 2023-06-26 13:27:33.000000 opr-200/opr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3615 2023-06-26 13:27:33.000000 opr-200/opr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2023-06-26 13:27:33.000000 opr-200/opr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-06-26 13:27:33.000000 opr-200/opr/modules/rld.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7741 2023-06-26 13:27:33.000000 opr-200/opr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)      377 2023-06-26 13:27:33.000000 opr-200/opr/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1000)      964 2023-06-26 13:27:33.000000 opr-200/opr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1014 2023-06-26 13:27:33.000000 opr-200/opr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2448 2023-06-26 13:27:33.000000 opr-200/opr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)      236 2023-06-26 13:27:33.000000 opr-200/opr/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2085 2023-06-26 13:27:33.000000 opr-200/opr/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2181 2023-06-26 13:27:33.000000 opr-200/opr/objfunc.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1839 2023-06-26 13:27:33.000000 opr-200/opr/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4739 2023-06-26 13:27:33.000000 opr-200/opr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-06-26 13:27:33.000000 opr-200/opr/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2671 2023-06-26 13:27:33.000000 opr-200/opr/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-06-26 13:27:33.000000 opr-200/opr/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2949 2023-06-26 13:27:33.000000 opr-200/opr/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-26 13:37:42.419785 opr-200/opr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2432 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      895 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       42 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-26 13:37:42.000000 opr-200/opr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      887 2023-06-26 13:27:33.000000 opr-200/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-06-26 13:37:42.431785 opr-200/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-06-26 13:27:33.000000 opr-200/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.379548 opr-210/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2325 2023-07-04 00:54:05.379548 opr-210/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1775 2023-07-01 05:55:02.000000 opr-210/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-07-03 12:59:17.000000 opr-210/opr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8946 2023-07-03 12:53:54.000000 opr-210/opr/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      535 2023-07-03 12:35:01.000000 opr-210/opr/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      460 2023-07-03 19:18:45.000000 opr-210/opr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      221 2023-07-03 00:11:35.000000 opr-210/opr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      704 2023-07-03 00:11:44.000000 opr-210/opr/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-07-03 11:40:39.000000 opr-210/opr/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      937 2023-07-03 11:41:20.000000 opr-210/opr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20759 2023-07-03 12:52:48.000000 opr-210/opr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      826 2023-07-03 00:19:09.000000 opr-210/opr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      330 2023-07-03 11:17:11.000000 opr-210/opr/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8130 2023-07-03 11:42:24.000000 opr-210/opr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1039 2023-07-03 00:19:36.000000 opr-210/opr/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      342 2023-07-03 11:42:39.000000 opr-210/opr/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1065 2023-07-03 00:20:30.000000 opr-210/opr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      995 2023-07-03 00:15:32.000000 opr-210/opr/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      218 2023-07-03 00:15:40.000000 opr-210/opr/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6951 2023-07-03 12:35:39.000000 opr-210/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5121 2023-07-03 14:25:17.000000 opr-210/opr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1429 2023-07-03 12:41:32.000000 opr-210/opr/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4395 2023-07-04 00:48:57.000000 opr-210/opr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2372 2023-07-03 12:33:25.000000 opr-210/opr/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1978 2023-07-03 12:42:29.000000 opr-210/opr/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.375548 opr-210/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2325 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      778 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       41 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-04 00:54:05.000000 opr-210/opr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      886 2023-07-04 00:53:22.000000 opr-210/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-04 00:54:05.379548 opr-210/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-01 10:59:30.000000 opr-210/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-04 00:54:05.379548 opr-210/test/
+-rw-r--r--   0 bart      (1000) bart      (1000)      675 2023-07-01 05:55:02.000000 opr-210/test/test_composite.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      442 2023-07-03 12:00:09.000000 opr-210/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      370 2023-07-03 12:00:20.000000 opr-210/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      935 2023-07-01 05:55:02.000000 opr-210/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4376 2023-07-03 11:59:37.000000 opr-210/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      642 2023-07-03 13:43:53.000000 opr-210/test/test_recursive.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1232 2023-07-03 01:04:57.000000 opr-210/test/test_storage.py
```

### Comparing `opr-200/PKG-INFO` & `opr-210/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 200
+Version: 210
 Summary: Object Programming Runtime
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
@@ -125,26 +125,22 @@
     cfg - irc configuration
     dlt - remove a user
     dpl - sets display items
     ftc - runs a fetching batch
     fnd - find objects 
     flt - instances registered
     log - log some text
-    mdl - genocide model
     met - add a user
     mre - displays cached output
     nck - changes nick on irc
-    now - genocide stats
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
-    req - reconsider
     rss - add a feed
     slg - slogan
     thr - show the running threads
-    tpc - genocide stats into topic
 
 
 FILES
 
 ::
 
     ~/.local/bin/opr
```

### Comparing `opr-200/README.rst` & `opr-210/opr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: opr
+Version: 210
+Summary: Object Programming Runtime
+Author-email: Bart Thate <bthate@dds.nl>
+License: Public Domain
+Project-URL: home, https://pypi.org/project/opr
+Project-URL: bugs, https://github.com/bthate/opr/issues
+Project-URL: source, https://github.com/bthate/opr
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: Public Domain
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+
 NAME
 
 ::
 
     OPR - Object Programming Runtime
 
 
@@ -108,26 +125,22 @@
     cfg - irc configuration
     dlt - remove a user
     dpl - sets display items
     ftc - runs a fetching batch
     fnd - find objects 
     flt - instances registered
     log - log some text
-    mdl - genocide model
     met - add a user
     mre - displays cached output
     nck - changes nick on irc
-    now - genocide stats
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
-    req - reconsider
     rss - add a feed
     slg - slogan
     thr - show the running threads
-    tpc - genocide stats into topic
 
 
 FILES
 
 ::
 
     ~/.local/bin/opr
```

### Comparing `opr-200/opr/__main__.py` & `opr-210/opr/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,106 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=E0012,C0114,C0115,C0116,C0413,E0401,W0212,W0611,W1514,R1732
-# pylint: disable=E0611
-# flake8: noqa: E402
-# pylama: ignore=W0611,E402
-
-import os
-import readline
-import sys
-import termios
-import time
-
-
-from .clients import Client
-from .command import Commands
-from .logging import Logging
-from .persist import Persist
-from .runtime import DATE, NAME, Cfg, command, parse_cli
-from .runtime import scanstr, waiter
-
-
-from . import  modules
-Commands.modules = modules
-
-
-__VERSION__ = "200"
 
 
-NAME = "opr"
+"utility"
 
 
-Persist.workdir = os.path.expanduser(f"~/.{NAME}")
+# IMPORTS
 
 
-class CLI(Client):
-
-    def announce(self, txt):
-        pass
-
-    def raw(self, txt):
-        print(txt)
-
-
-class Console(CLI):
+import os
+import pathlib
 
-    def handle(self, evt):
-        CLI.handle(self, evt)
-        evt.wait()
 
-    def poll(self):
-        return self.event(input("> "))
+# DEFINES
 
 
-def banner():
-    print(f"{NAME.upper()} started {DATE}")
-    sys.stdout.flush()
+def __dir__():
+    return (
+            'cdir',
+            'doskip',
+            'elapsed',
+            'fnclass',
+            'fntime',
+            'spl',
+            'strip',
+            'touch'
+           )
+
+
+# UTILITY
+
+
+def cdir(pth) -> None:
+    "Create directory"
+    if not pth.endswith(os.sep):
+        pth = os.path.dirname(pth)
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
+def doskip(txt, skipping) -> bool:
+    "check if text needs to be skipped"
+    for skip in spl(skipping):
+        if skip in txt:
+            return True
+    return False
+
+
+def elapsed(seconds, short=True) -> str:
+    "return elapsed time string"
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    year = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    years = int(nsec/year)
+    nsec -= years*year
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if years:
+        txt += f"{years}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if years and short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
 
 
-def daemon():
-    pid = os.fork()
-    if pid != 0:
-        os._exit(0)
-    os.setsid()
-    os.umask(0)
-    sis = open('/dev/null', 'r')
-    os.dup2(sis.fileno(), sys.stdin.fileno())
-    sos = open('/dev/null', 'a+')
-    ses = open('/dev/null', 'a+')
-    os.dup2(sos.fileno(), sys.stdout.fileno())
-    os.dup2(ses.fileno(), sys.stderr.fileno())
+def spl(txt) -> []:
+    "split comma seperated string" 
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
 
 
-def wrap(func):
-    fds = sys.stdin.fileno()
-    gotterm = True
-    try:
-        old = termios.tcgetattr(fds)
-    except termios.error:
-        gotterm = False
-    try:
-        func()
-    except (EOFError, KeyboardInterrupt):
-        pass
-    finally:
-        if gotterm:
-            termios.tcsetattr(fds, termios.TCSADRAIN, old)
-        waiter()
-
-
-def ver(event):
-    event.reply(f"{NAME.upper()} version {__VERSION__}")
-
-
-def main():
-    parse_cli(' '.join(sys.argv[1:]))
-    if "v" in Cfg.opts and "d" not in Cfg.opts:
-        Logging.verbose = True
-        Logging.raw = print
-    Commands.add(ver)
-    dowait = False
-    if Cfg.txt:
-        scanstr(modules, Cfg.mod, doall=True)
-        cli = CLI()
-        command(cli, Cfg.otxt)
-    elif 'd' in Cfg.opts:
-        daemon()
-        dowait = True
-    if "c" in Cfg.opts:
-        dowait = True
-    if dowait:
-        banner()
-        if 'c' in Cfg.opts and "d" not in Cfg.opts:
-            csl = Console()
-            csl.start()
-        scanstr(modules, Cfg.mod)
-        scanstr(modules, Cfg.mod, True, wait=True)
-        while 1:
-            time.sleep(1.0)
-            waiter()
+def strip(pth) -> str:
+    "strip path to ident part"
+    return os.sep.join(pth.split(os.sep)[-4:])
 
 
-if __name__ == "__main__":
-    wrap(main)
+def touch(fname) -> None:
+    "touch a file"
+    fds = os.open(fname, os.O_WRONLY | os.O_CREAT)
+    os.close(fds)
```

### Comparing `opr-200/opr/modules/fnd.py` & `opr-210/opr/modules/fnd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C0116
 
 
-"locate objects"
+"find"
 
 
 import time
 
 
-from ..objects import keys
-from ..objfunc import prt
-from ..persist import Persist
-from ..utility import elapsed, fntime
+from opr.objects import keys, prt
+from opr.persist import files, find, fntime
+from opr.utility import elapsed
 
 
 def fnd(event):
+    "locate objects"
     if not event.args:
-        res = sorted([x.split('.')[-1].lower() for x in Persist.files()])
+        res = sorted([x.split('.')[-1].lower() for x in files()])
         if res:
             event.reply(",".join(res))
         else:
             event.reply('no types yet.')
         return
     otype = event.args[0]
     nmr = 0
     keyz = None
     if event.gets:
         keyz = ','.join(keys(event.gets))
     if len(event.args) > 1:
         keyz += ',' + ','.join(event.args[1:])
-    for obj in Persist.find(otype, event.gets):
+    for obj in find(otype, event.gets):
         if not keyz:
             keyz = ',' + ','.join(keys(obj))
         prnt = prt(obj, keyz)
         lap = elapsed(time.time()-fntime(obj.__oid__))
         event.reply(f'{nmr} {prnt} {lap}')
         nmr += 1
     if not nmr:
```

### Comparing `opr-200/opr/modules/irc.py` & `opr-210/opr/modules/irc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
-# flake8:
-# pylama: ignore=C901
 
 
 "internet relay chat"
 
 
 import base64
 import os
@@ -16,50 +12,56 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from ..clients import Client
-from ..command import Commands
-from ..default import Default
-from ..errored import Errors
-from ..evented import Event
-from ..listens import Listens
-from ..logging import Logging
-from ..objects import Object, copy, keys, update
-from ..objfunc import edit, prt
-from ..persist import Persist, last, write
-from ..runtime import NAME, launch
-from ..utility import elapsed, fntime
+from opr.handler import Bus, Commands, Errors, Event, Handler
+from opr.loggers import Logging
+from opr.objects import Default, Object, copy, edit, keys, prt, update
+from opr.persist import find, fntime, last, write
+from opr.threads import launch
+from opr.utility import elapsed
+
+
+NAME = "opr"
 
 
 saylock = _thread.allocate_lock()
 
 
 def start():
+    "start a irc bot"
     irc = IRC()
     irc.start()
-    irc.joined.wait()
+    irc.events.joined.wait()
     return irc
 
 
-class NoUser(Exception):
+def stop():
+    "stop irc bots"
+    for bot in Bus.objs:
+        print(type(bot))
+        if "IRC" in str(type(bot)):
+            bot.stop()
 
-    pass
 
+class NoUser(Exception):
 
-# CONFIG
+    "user is not found"
 
 
 class Config(Default):
 
-    channel = '#%s' % NAME
+    "irc config"
+
+    channel = f'#{NAME}'
     control = '!'
+    edited = time.time()
     nick = NAME
     nocommands = True
     password = ''
     port = 6667
     realname = NAME
     sasl = False
     server = 'localhost'
@@ -67,248 +69,222 @@
     sleep = 60
     username = NAME
     users = False
     verbose = False
 
     def __init__(self):
         Default.__init__(self)
-        self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
-        self.nocommands = Config.nocommands
-        self.password = Config.password
         self.port = Config.port
         self.realname = Config.realname
-        self.sasl = Config.sasl
         self.server = Config.server
-        self.servermodes = Config.servermodes
-        self.sleep = Config.sleep
         self.username = Config.username
-        self.users = Config.users
-        self.verbose = Config.verbose
-
-
-Persist.add(Config)
 
+    def __edited__(self):
+        return Config.edited
 
-# OUTPUT
+    def __size__(self):
+        return len(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
+    "text wrapper"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
         self.width = 450
 
 
 class Output(Object):
 
+    "output cache"
+
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
-        self.state = Default()
-        self.state.starttime = time.time()
 
     def dosay(self, channel, txt):
+        "echo text to channel"
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
+        "add to channel cache"
         if channel not in self.cache:
             setattr(self.cache, channel, [])
         cache = getattr(self.cache, channel, None)
         cache.extend(txtlist)
 
     def gettxt(self, channel):
+        "return text from chanel cache"
         txt = None
         try:
             cache = getattr(self.cache, channel, None)
             txt = cache.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "send channel/txt to queue"
         if channel not in self.cache:
             setattr(self.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def output(self):
+        "output loop"
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             wrapper = TextWrap()
             try:
                 txtlist = wrapper.wrap(txt)
             except AttributeError:
                 continue
             if len(txtlist) > 3:
                 self.extend(channel, txtlist)
+                length = len(txtlist)
                 self.dosay(
                            channel,
-                           'use !mre to show more (+%s)' % len(txtlist)
+                           f"use !mre to show more (+{length})"
                           )
                 continue
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     def size(self, chan):
+        "show size of channel cache"
         if chan in self.cache:
             return len(getattr(self.cache, chan, []))
         return 0
 
     def start(self):
+        "start output loop"
         self.dostop.clear()
         launch(self.output)
         return self
 
     def stop(self):
+        "stop output loop"
         self.dostop.set()
         self.oqueue.put_nowait((None, None))
 
 
-# IRC
-
+class IRC(Handler, Output):
 
-class IRC(Client, Output):
+    "internet relay chat"
 
     def __init__(self):
-        Client.__init__(self)
+        Handler.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.authed = threading.Event()
-        self.connected = threading.Event()
+        self.events = Default()
+        self.events.authed = threading.Event()
+        self.events.connected = threading.Event()
+        self.events.joined = threading.Event()
         self.channels = []
-        self.joined = threading.Event()
-        self.keeprunning = False
-        self.outqueue = queue.Queue()
         self.sock = None
-        self.speed = 'slow'
-        self.state = Object()
-        self.state.needconnect = False
-        self.state.errors = []
-        self.state.last = 0
-        self.state.lastline = ''
+        self.state = Default()
+        self.state.keeprunning = False
         self.state.nrconnect = 0
-        self.state.nrerror = 0
         self.state.nrsend = 0
-        self.state.pongcheck = False
-        self.state.starttime = time.time()
-        self.threaded = False
         self.zelf = ''
-        self.register('903', self.h903)
-        self.register('904', self.h903)
-        self.register('AUTHENTICATE', self.auth)
-        self.register('CAP', self.cap)
-        self.register('ERROR', self.error)
-        self.register('LOG', self.log)
-        self.register('NOTICE', self.notice)
-        self.register('PRIVMSG', self.privmsg)
-        self.register('QUIT', self.quit)
-        self.register("command", self.docommand)
-        self.target = 'type'
+        self.register('903', cb_h903)
+        self.register('904', cb_h903)
+        self.register('AUTHENTICATE', cb_auth)
+        self.register('CAP', cb_cap)
+        self.register('ERROR', cb_error)
+        self.register('LOG', cb_log)
+        self.register('NOTICE', cb_notice)
+        self.register('PRIVMSG', cb_privmsg)
+        self.register('QUIT', cb_quit)
+        self.register("command", cb_command)
 
     def announce(self, txt):
+        "annouce text on channels"
         for channel in self.channels:
             self.say(channel, txt)
 
-    def auth(self, event):
-        assert self.cfg.password
-        self.direct('AUTHENTICATE %s' % self.cfg.password)
-
-    def cap(self, event):
-        if self.cfg.password and 'ACK' in event.arguments:
-            self.direct('AUTHENTICATE PLAIN')
-        else:
-            self.direct('CAP REQ :sasl')
-
     def command(self, cmd, *args):
+        "send command to server"
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
-                self.raw('%s %s' % (cmd.upper(), args[0]))
+                self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
-                self.raw(
-                         '%s %s :%s' % (
-                                        cmd.upper(),
-                                        args[0],
-                                        ' '.join(args[1:])
-                                       )
-                        )
+                txt = ' '.join(args[1:])
+                self.raw(f'{cmd.upper()} {args[0]} :{txt}')
             elif len(args) >= 3:
-                self.raw(
-                         '%s %s %s :%s' % (
-                                           cmd.upper(),
-                                           args[0],
-                                           args[1],
-                                           ' '.join(args[2:])
-                                           )
-                        )
+                txt = ' '.join(args[2:])
+                self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server"
         self.state.nrconnect += 1
-        self.connected.clear()
+        self.events.connected.clear()
         Logging.debug(f"connecting to {server}:{port}")
         if self.cfg.password:
             Logging.debug("using SASL")
             self.cfg.sasl = True
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.check_hostname = False
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
-            self.authed.set()
+            self.events.authed.set()
         if self.sock:
-            os.set_inheritable(self.fileno(), os.O_RDWR)
+            os.set_inheritable(self.sock.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
-            self.connected.set()
+            self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send direct text"
         Logging.debug(txt)
         self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
+        "disconnect from server"
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
             Errors.errors.append(ex)
 
-    def docommand(self, evt):
-        evt.orig = repr(self)
-        Commands.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
+        "connect loop"
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
@@ -317,114 +293,80 @@
                 self.state.errors = str(ex)
                 Logging.debug(str(ex))
             Logging.debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
-        self.joined.wait()
+        "called from output cache"
+        self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
-    def error(self, event):
-        self.state.nrerror += 1
-        self.state.errors.append(event.txt)
-        Logging.debug(event.txt)
-
     def event(self, txt):
+        "return a event"
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.command(
-                             'MODE %s %s' % (
-                                             self.cfg.nick,
-                                             self.cfg.servermodes
-                                            )
-                            )
+                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
             self.state.errors = []
-            self.joined.set()
+            self.events.joined.set()
         elif cmd == '433':
             self.state.errors = txt
             nck = self.cfg.nick + '_' + str(random.randint(1, 10))
             self.command('NICK', nck)
         return evt
 
-    def fileno(self):
-        return self.sock.fileno()
-
-    def h903(self, event):
-        self.command('CAP END')
-        self.authed.set()
-
-    def h904(self, event):
-        self.command('CAP END')
-        self.authed.set()
-
     def joinall(self):
+        "join all channels"
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
+        "keep alive loop"
         while 1:
-            self.connected.wait()
-            self.keeprunning = True
+            self.events.connected.wait()
+            self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 Logging.debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
-                self.keeprunning = False
-                self.connected.clear()
+                self.state.keeprunning = False
+                self.events.connected.clear()
                 self.stop()
                 start()
                 break
 
     def logon(self, server, nck):
-        self.connected.wait()
-        self.authed.wait()
-        self.direct('NICK %s' % nck)
-        self.direct(
-                    'USER %s %s %s :%s' % (
-                                           self.cfg.username or nck,
-                                           server,
-                                           server,
-                                           self.cfg.realname or nck
-                                          )
-                   )
+        "logon to server"
+        self.events.connected.wait()
+        self.events.authed.wait()
+        nck = self.cfg.username
+        self.direct(f'NICK {nck}')
+        self.direct(f'USER {nck} {server} {server} {nck}')
 
-    def kill(self, event):
-        pass
-
-    def log(self, event):
-        pass
-
-    def notice(self, event):
-        if event.txt.startswith('VERSION'):
-            txt = '\001VERSION %s %s - %s\001' % (
-                'op',
-                self.cfg.version,
-                self.cfg.username,
-            )
-            self.command('NOTICE', event.channel, txt)
 
     def parsing(self, txt):
+        # pylint: disable=R0912,R0915
+        "parse text"
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         Logging.debug(txt)
         obj = Event()
         obj.rawstr = rawstr
         obj.command = ''
@@ -475,15 +417,16 @@
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        self.connected.wait()
+        "poll input buffer for event"
+        self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
             except (
@@ -499,39 +442,16 @@
                 Logging.debug("handler stopped")
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
-    def privmsg(self, event):
-        if self.cfg.nocommands:
-            return
-        if event.txt:
-            if event.txt[0] in [self.cfg.control, '!']:
-                event.txt = event.txt[1:]
-            elif event.txt.startswith('%s:' % self.cfg.nick):
-                event.txt = event.txt[len(self.cfg.nick)+1:]
-            else:
-                return
-            if self.cfg.users and not Users.allowed(event.origin, 'USER'):
-                return
-            Logging.debug(f"command from {event.origin}: {event.txt}")
-            msg = Event()
-            copy(msg, event)
-            msg.type = 'command'
-            msg.parse(event.txt)
-            self.handle(msg)
-
-    def quit(self, event):
-        Logging.debug(f"quit from {self.cfg.server}")
-        if event.orig and event.orig in self.zelf:
-            self.stop()
-
     def raw(self, txt):
+        "send raw text"
         txt = txt.rstrip()
         Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
@@ -548,131 +468,236 @@
                 Errors.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
+        "reconnect to server"
         Logging.debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
-        self.connected.clear()
-        self.joined.clear()
+        self.events.connected.clear()
+        self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def say(self, channel, txt):
+        "sat text of channel"
         self.oput(channel, txt)
 
     def some(self):
-        self.connected.wait()
+        "check input cache"
+        self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start irc loop"
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
-        self.connected.clear()
-        self.joined.clear()
-        launch(Client.start, self)
+        self.events.connected.clear()
+        self.events.joined.clear()
+        launch(Handler.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
-        if not self.keeprunning:
+        if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        Listens.remove(self)
-        Client.stop(self)
+        "stop irc loop"
+        Bus.remove(self)
+        Handler.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
-# USERS
+def cb_auth(evt):
+    "authenticate to server"
+    bot = evt.bot()
+    assert evt
+    assert bot.cfg.password
+    bot.direct(f'AUTHENTICATE {bot.cfg.password}')
+
+def cb_cap(evt):
+    "ask capabilities from server"
+    bot = evt.bot()
+    if bot.cfg.password and 'ACK' in evt.arguments:
+        bot.direct('AUTHENTICATE PLAIN')
+    else:
+        bot.direct('CAP REQ :sasl')
+
+
+def cb_command(evt):
+    "execute an command"
+    Commands.handle(evt)
+
+
+def cb_error(evt):
+    "handle error"
+    bot = evt.bot()
+    bot.state.nrerror += 1
+    bot.state.errors.append(evt.txt)
+    Logging.debug(evt.txt)
+
+
+def cb_h903(evt):
+    "capabilities end"
+    assert evt
+    bot = evt.bot()
+    bot.command('CAP END')
+    bot.events.authed.set()
+
+
+def cb_h904(evt):
+    "capabilities end"
+    assert evt
+    bot = evt.bot()
+    bot.command('CAP END')
+    bot.events.authed.set()
+
+
+def cb_kill(evt):
+    "got killed"
+
+
+def cb_log(evt):
+    "log event"
+
+
+def cb_notice(evt):
+    "handle notice"
+    bot = evt.bot()
+    if evt.txt.startswith('VERSION'):
+        txt = f'\001VERSION {NAME} {bot.cfg.version} - {bot.cfg.username}\001'
+        bot.command('NOTICE', evt.channel, txt)
+
+
+def cb_privmsg(evt):
+    "handle privmsg"
+    bot = evt.bot()
+    if bot.cfg.nocommands:
+        return
+    if evt.txt:
+        if evt.txt[0] in ['!',]:
+            evt.txt = evt.txt[1:]
+        elif evt.txt.startswith(f'{bot.cfg.nick}:'):
+            evt.txt = evt.txt[len(bot.cfg.nick)+1:]
+        else:
+            return
+        if bot.cfg.users and not Users.allowed(evt.origin, 'USER'):
+            return
+        Logging.debug(f"command from {evt.origin}: {evt.txt}")
+        msg = Event()
+        copy(msg, evt)
+        msg.type = 'command'
+        msg.parse(evt.txt)
+        bot.handle(msg)
+
+
+def cb_quit(evt):
+    "handle quit"
+    bot = evt.bot()
+    Logging.debug(f"quit from {bot.cfg.server}")
+    if evt.orig and evt.orig in bot.zelf:
+        bot.stop()
 
 
 class User(Object):
 
+    "an irc user"
+
     def __init__(self, val=None):
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
-
-Persist.add(User)
+    def isok(self):
+        "verify user"
+        return True
+
+    def isthere(self):
+        "verify presence"
+        return True
 
 
 class Users(Object):
 
+    "manages all irc users"
+
     @staticmethod
     def allowed(origin, perm):
+        "check whether user has permissions"
         perm = perm.upper()
         user = Users.get_user(origin)
         val = False
         if user and perm in user.perms:
             val = True
         return val
 
     @staticmethod
     def delete(origin, perm):
+        "delete an user"
         res = False
         for user in Users.get_users(origin):
             try:
                 user.perms.remove(perm)
                 write(user)
                 res = True
             except ValueError:
                 pass
         return res
 
     @staticmethod
     def get_users(origin=''):
+        "find all users"
         selector = {'user': origin}
-        return Persist.find('user', selector)
+        return find('user', selector)
 
     @staticmethod
     def get_user(origin):
+        "select specific user"
         users = list(Users.get_users(origin))
         res = None
         if len(users) > 0:
             res = users[-1]
         return res
 
     @staticmethod
     def perm(origin, permission):
+        "set permission of an user"
         user = Users.get_user(origin)
         if not user:
             raise NoUser(origin)
         if permission.upper() not in user.perms:
             user.perms.append(permission.upper())
             write(user)
         return user
 
 
-# COMMANDS
-
-
 def cfg(event):
+    "edit irc config"
     config = Config()
     last(config)
     if not event.sets:
         event.reply(
                     prt(
                         config,
                         keys(config),
@@ -682,63 +707,68 @@
     else:
         edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def dlt(event):
+    "delete an user"
     if not event.args:
         event.reply('dlt <username>')
         return
     selector = {'user': event.args[0]}
-    for obj in Persist.find('user', selector):
+    for obj in find('user', selector):
         obj.__deleted__ = True
         write(obj)
         event.reply('ok')
         break
 
 
 def met(event):
+    "add an user"
     if not event.args:
         nmr = 0
-        for obj in Persist.find('user'):
+        for obj in find('user'):
             lap = elapsed(time.time() - fntime(obj.__fnm__))
             event.reply(f'{nmr} {obj.user} {obj.perms} {lap}s')
             nmr += 1
         if not nmr:
             event.reply('no user')
         return
     user = User()
     user.user = event.rest
     user.perms = ['USER']
     write(user)
     event.reply('ok')
 
 
 def mre(event):
+    "pull from output cache"
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
     if event.channel not in bot.cache:
-        event.reply('no output in %s cache.' % event.channel)
+        event.reply(f'no output in {event.channel} cache.')
         return
     for _x in range(3):
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
-    event.reply('%s more in cache' % size)
-
+    event.reply(f'{size} more in cache')
 
 def pwd(event):
+    "create pasword from nickserv user/pass pair"
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
-    txt = '\x00%s\x00%s' % (event.args[0], event.args[1])
+    arg1 = event.args[0]
+    arg2 = event.args[1]
+    txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
```

### Comparing `opr-200/opr/modules/rss.py` & `opr-210/opr/modules/rss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=E0012,R,C0114,C0115,C0116,C0209,W0613,E1101
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -15,73 +13,95 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from ..listens import Listens
-from ..objects import Object, update
-from ..objfunc import prt
-from ..persist import Persist, last, write
-from ..repeats import Repeater
-from ..runtime import Cfg, launch, threaded
-from ..utility import elapsed, fntime, spl
+from opr.handler import Bus, Cfg
+from opr.objects import Default, Object, prt, update
+from opr.persist import find, fntime, last, write
+from opr.repeats import Repeater
+from opr.threads import launch, threaded
+from opr.utility import elapsed, spl
 
 
 def start():
+    "start a fetcher"
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 fetchlock = _thread.allocate_lock()
 
 
-class Feed(Object):
+class Feed(Default):
 
-    pass
+    "represent a rss feed"
+
+    def len(self):
+        "length"
+        return len(self.__dict__)
+
+    def size(self):
+        "size"
+        return len(self.__dict__)
 
 
 class Rss(Object):
 
+    "save rss item"
+
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
-
-Persist.add(Rss)
+    def len(self):
+        "length"
+        return len(self.__dict__)
+
+    def size(self):
+        "size"
+        return len(self.__dict__)
 
 
 class Seen(Object):
 
+    "list of seen urls"
+
     def __init__(self):
         super().__init__()
         self.urls = []
 
-
-Persist.add(Seen)
+    def len(self):
+        "length" 
+        return len(self.__dict__)
+
+    def size(self):
+        "size"
+        return len(self.__dict__)
 
 
 class Fetcher(Object):
 
+    "rss feed fetcher"
+
     dosave = False
     seen = Seen()
 
     def __init__(self):
         super().__init__()
         self.connected = threading.Event()
 
-    def clone(self, other):
-        pass
-
     @staticmethod
     def display(obj):
+        "display rss item"
         result = ''
         displaylist = []
         try:
             displaylist = obj.display_list or 'title,link'
         except AttributeError:
             displaylist = 'title,link,author'
         for key in spl(displaylist):
@@ -94,107 +114,109 @@
             data = striphtml(data.rstrip())
             data = unescape(data)
             result += data.rstrip()
             result += ' - '
         return result[:-2].rstrip()
 
     def fetch(self, feed):
+        "fetch updates"
         with fetchlock:
             counter = 0
             objs = []
             for obj in reversed(list(getfeed(feed.rss, feed.display_list))):
                 fed = Feed()
                 update(fed, obj)
                 update(fed, feed)
                 if 'link' in fed:
                     url = urllib.parse.urlparse(fed.link)
                     if url.path and not url.path == '/':
-                        uurl = '%s://%s/%s' % (
-                                               url.scheme,
-                                               url.netloc,
-                                               url.path
-                                              )
+                        uurl = f'{url.scheme}://{url.netloc}/{url.path}'
                     else:
                         uurl = fed.link
                     if uurl in Fetcher.seen.urls:
                         continue
                     Fetcher.seen.urls.append(uurl)
                 counter += 1
                 if self.dosave:
                     write(fed)
                 objs.append(fed)
         if objs:
             write(Fetcher.seen)
         txt = ''
         feedname = getattr(feed, 'name')
         if feedname:
-            txt = '[%s] ' % feedname
+            txt = f'[{feedname}] '
         for obj in objs:
             txt2 = txt + self.display(obj)
-            Listens.announce(txt2.rstrip())
+            Bus.announce(txt2.rstrip())
         return counter
 
     def run(self):
+        "run fetching updates of all feeds"
         thrs = []
-        for feed in Persist.find('rss'):
+        for feed in find('rss'):
             thrs.append(launch(self.fetch, feed))
         return thrs
 
     def start(self, repeat=True):
+        "start fetcher"
         last(Fetcher.seen)
         if repeat:
             repeater = Repeater(300.0, self.run)
             repeater.start()
 
 
 class Parser(Object):
 
+    "parse rss feed"
+
     @staticmethod
     def getitem(line, item):
+        "return xml items in rss feed"
         lne = ''
         try:
-            index1 = line.index('<%s>' % item) + len(item) + 2
-            index2 = line.index('</%s>' % item)
+            index1 = line.index(f'<{item}>') + len(item) + 2
+            index2 = line.index(f'</{item}>')
             lne = line[index1:index2]
             if 'CDATA' in lne:
                 lne = lne.replace('![CDATA[', '')
                 lne = lne.replace(']]', '')
                 lne = lne[1:-1]
         except ValueError:
             lne = None
         return lne
 
     @staticmethod
     def parse(txt, item='title,link'):
+        "parse text for xml items"
         res = []
         for line in txt.split('<item>'):
             line = line.strip()
             obj = Object()
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
-# UTILITIES
-
-
 def getfeed(url, item):
+    "fetch feed"
     if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
     return Parser.parse(str(result.data, 'utf-8'), item)
 
 
 def gettinyurl(url):
+    "fetch feed using tinyurl"
     postarray = [
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
     req = Request('http://tinyurl.com/create.php',
                   data=bytes(postdata, 'UTF-8'))
@@ -205,109 +227,111 @@
             i = re.search('data-clipboard-text="(.*?)"', line, re.M)
             if i:
                 return i.groups()
     return []
 
 
 def geturl(url):
+    "fetch url"
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
     req.add_header('User-agent', useragent("rss fetcher"))
     with urllib.request.urlopen(req) as response:
         response.data = response.read()
         return response
 
 
 def striphtml(text):
+    "strip html"
     clean = re.compile('<.*?>')
     return re.sub(clean, '', text)
 
 
 def unescape(text):
+    "unescape html"
     txt = re.sub(r'\s+', ' ', text)
     return html.unescape(txt)
 
 
 def useragent(txt):
+    "return useragent string"
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-# COMMANDS
-
-
 def dpl(event):
+    "set items to display"
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
-    for feed in Persist.find('rss', {'rss': event.args[0]}):
+    for feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             write(feed)
     event.reply('ok')
 
 
 @threaded
 def ftc(event):
+    "fetch feeds"
     res = []
     thrs = []
     fetcher = Fetcher()
     fetcher.start(False)
     thrs = fetcher.run()
     for thr in thrs:
         res.append(thr.join())
     if res:
         event.reply(','.join([str(x) for x in res if x]))
         return
 
 
 def nme(event):
+    "give feed an display name"
     if len(event.args) != 2:
         event.reply('name <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
-    for feed in Persist.find('rss', selector):
+    for feed in find('rss', selector):
         if feed:
             feed.name = event.args[1]
             write(feed)
     event.reply('ok')
 
 
 def rem(event):
+    "remove feed"
     if len(event.args) != 1:
         event.reply('rem <stringinurl>')
         return
     selector = {'rss': event.args[0]}
-    for feed in Persist.find('rss', selector):
+    for feed in find('rss', selector):
         if feed:
             feed.__deleted__ = True
             write(feed)
     event.reply('ok')
 
 
 def rss(event):
+    "add feed"
     if not event.rest:
         nrs = 0
-        for feed in Persist.find('rss'):
-            event.reply(
-                        '%s %s %s' % (
-                                      nrs,
-                                      prt(feed),
-                                      elapsed(time.time()-fntime(feed.__oid__))
-                                     )
-                       )
+        for feed in find('rss'):
+            elp = elapsed(time.time()-fntime(feed.__oid__))
+            txt = prt(feed)
+            event.reply(f'{nrs} {txt} {elp}')
             nrs += 1
         if not nrs:
             event.reply('no rss feed found.')
         return
     url = event.args[0]
     if 'http' not in url:
         event.reply('i need an url')
         return
-    for res in Persist.find('rss', {'rss': url}):
+    for res in find('rss', {'rss': url}):
         if res:
-            event.reply('already got %s' % url)
+            event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     write(feed)
     event.reply('ok')
```

### Comparing `opr-200/opr/modules/thr.py` & `opr-210/opr/modules/thr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C0114,C0116,E1101
 
 
-"show running threads"
+"thread"
 
 
 import threading
 import time
 
 
-from ..objects import Object, update
-from ..runtime import STARTTIME
-from ..utility import elapsed
+from opr.objects import Object, update
+from opr.utility import elapsed
+
+
+STARTTIME = time.time()
 
 
 def thr(event):
+    "show list of running threads"
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
             uptime = obj.sleep - int(time.time() - obj.state.latest)
         elif getattr(obj, 'starttime', None):
             uptime = int(time.time() - obj.starttime)
         else:
             uptime = int(time.time() - STARTTIME)
         result.append((uptime, thread.name))
     res = []
-    for uptime, txt in sorted(result, key=lambda x: x[0]):
+    for uptime, txt in sorted(result, key=lambda x: x[1]):
         lap = elapsed(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
```

### Comparing `opr-200/opr/persist.py` & `opr-210/opr/persist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,191 +1,234 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R,C0114,C0115,C0116,W0613,E1101
 
 
-"store to disk"
+"persist"
+
+
+# IMPORTS
 
 
 import os
+import sys
+import time
 import _thread
 
 
-from .decoder import load
-from .default import Default
-from .encoder import dump
-from .objects import Object, ident, items, kind, update
-from .objfunc import search
-from .utility import cdir, fnclass, fntime, strip
+from opr.objects import Object, copy, ident, dump, items, kind, load, update
+from opr.utility import cdir, strip
+
+
+# DEFINES
 
 
 def __dir__():
     return (
             'Persist',
+            'files',
+            'find',
+            'fnclass',
+            'fns',
+            'fntime',
+            'hook',
             'last',
             'read',
+            'readrec',
+            'search',
             'write',
             'writerec'
            )
 
 
 disklock = _thread.allocate_lock()
 
 
+# CLASSES
+
+
 class Persist(Object):
 
-    cls = Default()
+    "directory to persist to"
+
     workdir = ""
 
     @staticmethod
-    def add(clz) -> str:
-        setattr(Persist.cls, f"{clz.__module__}.{clz.__name__}", clz)
+    def path(pth) -> str:
+        "return store path"
+        return os.path.join(Persist.workdir, 'store', pth)
 
     @staticmethod
-    def clz(mtc) -> type:
-        mtc = mtc.lower()
-        for clzz in Persist.cls:
-            if mtc == clzz.split(".")[-1].lower():
-                yield clzz
+    def storedir() -> str:
+        "return storage directory"
+        return os.path.join(Persist.workdir, "store")
 
-    @staticmethod
-    def files() -> []:
-        return os.listdir(os.path.join(Persist.workdir, "store"))
 
-    @staticmethod
-    def find(mtc, selector=None) -> []:
-        if selector is None:
-            selector = {}
-        for fnm in Persist.fns(mtc):
-            obj = Persist.hook(fnm)
-            if '__deleted__' in obj:
-                continue
-            if selector and not search(obj, selector):
-                continue
-            yield obj
+# UTILITY
 
-    @staticmethod
-    def fns(mtc) -> []:
-        assert Persist.workdir
-        dname = ''
-        lst = mtc.lower().split(".")[-1]
-        for rootdir, dirs, _files in os.walk(Persist.workdir, topdown=False):
-            if dirs:
-                dname = sorted(dirs)[-1]
-                if dname.count('-') == 2:
-                    ddd = os.path.join(rootdir, dname)
-                    fls = sorted(os.listdir(ddd))
-                    if fls:
-                        path2 = os.path.join(ddd, fls[-1])
-                        spl = strip(path2).split(os.sep, maxsplit=1)[0]
-                        if lst in spl.lower().split(".")[-1]:
-                            yield strip(path2)
 
-    @staticmethod
-    def get(cmd) -> type:
-        return getattr(Persist.cls, cmd, None)
+def files() -> []:
+    "show all files in store"
+    res = []
+    path = Persist.storedir()
+    if os.path.exists(path):
+        res = os.listdir(path)
+    return res
 
-    @staticmethod
-    def hook(otp) -> type:
-        clz = fnclass(otp)
-        cls = Persist.get(clz)
-        if cls:
-            obj = cls()
-            read(obj, otp)
-            return obj
-        obj = Object()
-        read(obj, otp)
-        return obj
 
-    @staticmethod
-    def logdir() -> str:
-        return os.path.join(Persist.workdir, "logs")
+def find(mtc, selector=None) -> []:
+    "locate specific objects"
+    if selector is None:
+        selector = {}
+    for fnm in fns(mtc):
+        obj = hook(fnm)
+        if '__deleted__' in obj:
+            continue
+        if selector and not search(obj, selector):
+            continue
+        yield obj
 
-    @staticmethod
-    def match(mtc, selector=None) -> []:
-        if selector is None:
-            selector = {}
-        for tpe in Persist.clz(mtc):
-            for fnm in Persist.fns(tpe):
-                obj = Persist.hook(fnm)
-                if '__deleted__' in obj:
-                    continue
-                if selector and not search(obj, selector):
-                    continue
-                yield obj
 
-    @staticmethod
-    def path(pth) -> str:
-        return os.path.join(Persist.workdir, 'store', pth)
+def fnclass(pth) -> str:
+    "return class from filename"
+    try:
+        *_rest, mpth = pth.split("store")
+        splitted = mpth.split(os.sep)
+        return splitted[0]
+    except ValueError:
+        pass
+    return None
+
+
+def fns(mtc) -> []:
+    "return matching filenames"
+    dname = ''
+    lst = mtc.lower().split(".")[-1]
+    for rootdir, dirs, _files in os.walk(Persist.storedir(), topdown=False):
+        if dirs:
+            dname = sorted(dirs)[-1]
+            if dname.count('-') == 2:
+                ddd = os.path.join(rootdir, dname)
+                fls = sorted(os.listdir(ddd))
+                if fls:
+                    path2 = os.path.join(ddd, fls[-1])
+                    splitted = strip(path2).split(os.sep, maxsplit=1)[0]
+                    if lst in splitted.lower().split(".")[-1]:
+                        yield strip(path2)
+
+
+def fntime(daystr) -> float:
+    "return time from filename"
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        tme += float('.' + rest)
+    else:
+        tme = 0
+    return tme
 
-    @staticmethod
-    def remove(clz) -> None:
-        delattr(Persist.cls, f"{clz.__module__}.{clz.__name__}")
 
-    @staticmethod
-    def storedir() -> str:
-        return os.path.join(Persist.workdir, "store")
+def hook(otp) -> type:
+    "return object from filename"
+    clz = fnclass(otp)
+    splitted = clz.split(".")
+    modname = ".".join(splitted[:1])
+    clz = splitted[-1]
+    mod = sys.modules.get(modname, None)
+    if mod:
+        cls = getattr(mod, clz, None)
+    if cls:
+        obj = cls()
+        read(obj, otp)
+        return obj
+    obj = Object()
+    read(obj, otp)
+    return obj
 
 
-# FUNCTIONS
+## METHODS
 
 
 def last(obj, selector=None) -> None:
+    "update with last saved version"
     if selector is None:
         selector = {}
     result = sorted(
-                    Persist.find(kind(obj), selector),
+                    find(kind(obj), selector),
                     key=lambda x: fntime(x.__oid__)
                    )
     if result:
         inp = result[-1]
         update(obj, inp)
         obj.__oid__ = inp.__oid__
     return obj.__oid__
 
 
 def read(obj, pth) -> str:
+    "read object from path"
     pth = Persist.path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
     return obj.__oid__
 
 
 def readrec(obj, pth=None) -> type:
+    "read object recursively"
     ooo = type(obj)()
     if pth:
         read(ooo, pth)
     else:
         update(ooo, obj)
     oooo = type(obj)()
     for key, value in items(ooo):
         if issubclass(type(value), Object):
             setattr(oooo, key, readrec(value))
             continue
-        else:
-            setattr(oooo, key, value)
+        setattr(oooo, key, value)
     return oooo
 
 
+def search(obj, selector) -> bool:
+    "check whether values in selector dict match in the object"
+    res = False
+    select = Object()
+    copy(select, selector)
+    for key, value in items(select):
+        try:
+            val = getattr(obj, key)
+        except AttributeError:
+            continue
+        if str(value) in str(val):
+            res = True
+            break
+    return res
+
+
 def write(obj) -> str:
+    "write object to disk"
     try:
-        pth = Persist.path(obj.__oid__)
+        pth = obj.__oid__
     except TypeError:
-        pth = Persist.path(ident(obj))
+        pth = ident(obj)
+    pth = Persist.path(pth)
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
 
 
 def writerec(obj):
+    "write object recursively"
     ooo = type(obj)()
     for key, value in items(obj):
         if issubclass(type(value), Object):
             setattr(ooo, key, writerec(value))
         else:
             setattr(ooo, key, str(value))
     return write(ooo)
```

### Comparing `opr-200/opr.egg-info/PKG-INFO` & `opr-210/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: opr
-Version: 200
-Summary: Object Programming Runtime
-Author-email: Bart Thate <bthate@dds.nl>
-License: Public Domain
-Project-URL: home, https://pypi.org/project/opr
-Project-URL: bugs, https://github.com/bthate/opr/issues
-Project-URL: source, https://github.com/bthate/opr
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: Public Domain
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Topic :: Utilities
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-
 NAME
 
 ::
 
     OPR - Object Programming Runtime
 
 
@@ -125,26 +108,22 @@
     cfg - irc configuration
     dlt - remove a user
     dpl - sets display items
     ftc - runs a fetching batch
     fnd - find objects 
     flt - instances registered
     log - log some text
-    mdl - genocide model
     met - add a user
     mre - displays cached output
     nck - changes nick on irc
-    now - genocide stats
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
-    req - reconsider
     rss - add a feed
     slg - slogan
     thr - show the running threads
-    tpc - genocide stats into topic
 
 
 FILES
 
 ::
 
     ~/.local/bin/opr
```

### Comparing `opr-200/opr.egg-info/SOURCES.txt` & `opr-210/opr.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 README.rst
 pyproject.toml
 setup.py
-opr/__init__.py
 opr/__main__.py
-opr/clients.py
-opr/clocked.py
-opr/command.py
-opr/configs.py
-opr/decoder.py
-opr/default.py
-opr/defines.py
-opr/encoder.py
-opr/errored.py
-opr/evented.py
 opr/handler.py
-opr/listens.py
-opr/logging.py
+opr/loggers.py
 opr/objects.py
-opr/objfunc.py
-opr/parsers.py
 opr/persist.py
 opr/repeats.py
 opr/runtime.py
 opr/threads.py
 opr/utility.py
 opr.egg-info/PKG-INFO
 opr.egg-info/SOURCES.txt
 opr.egg-info/dependency_links.txt
 opr.egg-info/entry_points.txt
 opr.egg-info/requires.txt
 opr.egg-info/top_level.txt
 opr.egg-info/zip-safe
 opr/modules/__init__.py
-opr/modules/cfg.py
 opr/modules/cmd.py
 opr/modules/err.py
 opr/modules/flt.py
 opr/modules/fnd.py
 opr/modules/irc.py
 opr/modules/log.py
-opr/modules/mbx.py
 opr/modules/mod.py
-opr/modules/rld.py
 opr/modules/rss.py
+opr/modules/shp.py
 opr/modules/sts.py
 opr/modules/tdo.py
 opr/modules/thr.py
-opr/modules/udp.py
-opr/modules/upt.py
+opr/modules/upt.py
+test/test_composite.py
+test/test_decoder.py
+test/test_encoder.py
+test/test_inherit.py
+test/test_objects.py
+test/test_recursive.py
+test/test_storage.py
```

### Comparing `opr-200/pyproject.toml` & `opr-210/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "opr"
 description = "Object Programming Runtime"
-version = "200"
+version = "210"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
              'Development Status :: 3 - Alpha',
@@ -24,15 +24,15 @@
 [project.urls]
 "home" = "https://pypi.org/project/opr"
 "bugs" = "https://github.com/bthate/opr/issues"
 "source" = "https://github.com/bthate/opr"
 
 
 [project.scripts]
-opr = "opr.__main__:main"
+opr = "opr.runtime:main"
 
 
 [project.optional-dependencies]
 dev = []
 
 [tool.setuptools]
 packages = [
```

