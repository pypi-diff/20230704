# Comparing `tmp/blibs-1.0.0.tar.gz` & `tmp/blibs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blibs-1.0.0.tar", last modified: Fri Dec 16 23:19:32 2022, max compression
+gzip compressed data, was "blibs-1.1.0.tar", last modified: Tue Jul  4 01:28:32 2023, max compression
```

## Comparing `blibs-1.0.0.tar` & `blibs-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 23:19:32.112760 blibs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-16 23:19:32.112760 blibs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2022-12-16 23:19:15.000000 blibs-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2022-12-16 23:19:15.000000 blibs-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 23:19:32.112760 blibs-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 23:19:32.108760 blibs-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 23:19:32.108760 blibs-1.0.0/src/blibs/
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2022-12-16 23:19:15.000000 blibs-1.0.0/src/blibs/Colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-16 23:19:15.000000 blibs-1.0.0/src/blibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2022-12-16 23:19:15.000000 blibs-1.0.0/src/blibs/traverseconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 23:19:32.112760 blibs-1.0.0/src/blibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-16 23:19:32.000000 blibs-1.0.0/src/blibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-16 23:19:32.000000 blibs-1.0.0/src/blibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 23:19:32.000000 blibs-1.0.0/src/blibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-16 23:19:32.000000 blibs-1.0.0/src/blibs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:28:32.178855 blibs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 01:28:32.178855 blibs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-04 01:28:08.000000 blibs-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 01:28:25.000000 blibs-1.1.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-04 01:28:08.000000 blibs-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:28:32.178855 blibs-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:28:32.170855 blibs-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:28:32.174855 blibs-1.1.0/src/blibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-04 01:28:08.000000 blibs-1.1.0/src/blibs/Colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-04 01:28:08.000000 blibs-1.1.0/src/blibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-04 01:28:08.000000 blibs-1.1.0/src/blibs/traverseconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:28:32.174855 blibs-1.1.0/src/blibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 01:28:32.000000 blibs-1.1.0/src/blibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 01:28:32.000000 blibs-1.1.0/src/blibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:28:32.000000 blibs-1.1.0/src/blibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 01:28:32.000000 blibs-1.1.0/src/blibs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:28:32.174855 blibs-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 01:28:08.000000 blibs-1.1.0/tests/test_import.py
```

### Comparing `blibs-1.0.0/pyproject.toml` & `blibs-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blibs-1.0.0/src/blibs/Colorize.py` & `blibs-1.1.0/src/blibs/Colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
             fgc = "yellow"
         else:
             fgc = "red"
         # print dir(self.stream)
         self.stream.write(colorize(self.format(record), fg=fgc, bg=bgc, bold=bold) + "\n")
 
 
-def init_root_logger(format="%(asctime)s %(name)-15s %(levelname)-8s %(message)s", level=1):
+def init_root_logger(format="%(asctime)s %(name)-15s %(levelname)-8s %(message)s", level=1, handler_level=None):
     log = logging.getLogger()
     formatter = logging.Formatter(format)
     sh = ColHandler()
     sh.setFormatter(formatter)
+    if handler_level:
+        sh.setLevel(handler_level)
     log.setLevel(level)
     log.addHandler(sh)
 
 
 def colorize(
     txt,
     fgcol=None,
```

### Comparing `blibs-1.0.0/src/blibs/traverseconf.py` & `blibs-1.1.0/src/blibs/traverseconf.py`

 * *Files identical despite different names*

