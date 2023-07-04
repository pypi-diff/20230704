# Comparing `tmp/asyncpg-promise-0.1.0.tar.gz` & `tmp/asyncpg-promise-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg-promise-0.1.0.tar", last modified: Tue Jul  4 21:27:26 2023, max compression
+gzip compressed data, was "asyncpg-promise-0.1.1.tar", last modified: Tue Jul  4 21:31:55 2023, max compression
```

## Comparing `asyncpg-promise-0.1.0.tar` & `asyncpg-promise-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:27:26.869090 asyncpg-promise-0.1.0/
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:27:26.867794 asyncpg-promise-0.1.0/AsyncPGPromise/
--rw-r--r--   0 knrs       (501) staff       (20)     1166 2023-07-04 21:19:45.000000 asyncpg-promise-0.1.0/AsyncPGPromise/AsyncPGPromise.py
--rw-r--r--   0 knrs       (501) staff       (20)        0 2023-07-04 21:03:35.000000 asyncpg-promise-0.1.0/AsyncPGPromise/__init__.py
--rw-r--r--   0 knrs       (501) staff       (20)      207 2023-07-04 21:27:26.868951 asyncpg-promise-0.1.0/PKG-INFO
--rw-r--r--   0 knrs       (501) staff       (20)     1985 2023-07-04 21:27:06.000000 asyncpg-promise-0.1.0/README.md
-drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:27:26.868762 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/
--rw-r--r--   0 knrs       (501) staff       (20)      207 2023-07-04 21:27:26.000000 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/PKG-INFO
--rw-r--r--   0 knrs       (501) staff       (20)      272 2023-07-04 21:27:26.000000 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/SOURCES.txt
--rw-r--r--   0 knrs       (501) staff       (20)        1 2023-07-04 21:27:26.000000 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/dependency_links.txt
--rw-r--r--   0 knrs       (501) staff       (20)       16 2023-07-04 21:27:26.000000 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/requires.txt
--rw-r--r--   0 knrs       (501) staff       (20)       15 2023-07-04 21:27:26.000000 asyncpg-promise-0.1.0/asyncpg_promise.egg-info/top_level.txt
--rw-r--r--   0 knrs       (501) staff       (20)       38 2023-07-04 21:27:26.869133 asyncpg-promise-0.1.0/setup.cfg
--rw-r--r--   0 knrs       (501) staff       (20)      355 2023-07-04 21:07:26.000000 asyncpg-promise-0.1.0/setup.py
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:31:55.163609 asyncpg-promise-0.1.1/
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:31:55.162634 asyncpg-promise-0.1.1/AsyncPGPromise/
+-rw-r--r--   0 knrs       (501) staff       (20)     1166 2023-07-04 21:19:45.000000 asyncpg-promise-0.1.1/AsyncPGPromise/AsyncPGPromise.py
+-rw-r--r--   0 knrs       (501) staff       (20)        0 2023-07-04 21:03:35.000000 asyncpg-promise-0.1.1/AsyncPGPromise/__init__.py
+-rw-r--r--   0 knrs       (501) staff       (20)      207 2023-07-04 21:31:55.163476 asyncpg-promise-0.1.1/PKG-INFO
+-rw-r--r--   0 knrs       (501) staff       (20)     1985 2023-07-04 21:27:06.000000 asyncpg-promise-0.1.1/README.md
+drwxr-xr-x   0 knrs       (501) staff       (20)        0 2023-07-04 21:31:55.163291 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/
+-rw-r--r--   0 knrs       (501) staff       (20)      207 2023-07-04 21:31:55.000000 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/PKG-INFO
+-rw-r--r--   0 knrs       (501) staff       (20)      272 2023-07-04 21:31:55.000000 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/SOURCES.txt
+-rw-r--r--   0 knrs       (501) staff       (20)        1 2023-07-04 21:31:55.000000 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/dependency_links.txt
+-rw-r--r--   0 knrs       (501) staff       (20)        8 2023-07-04 21:31:55.000000 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/requires.txt
+-rw-r--r--   0 knrs       (501) staff       (20)       15 2023-07-04 21:31:55.000000 asyncpg-promise-0.1.1/asyncpg_promise.egg-info/top_level.txt
+-rw-r--r--   0 knrs       (501) staff       (20)       38 2023-07-04 21:31:55.163650 asyncpg-promise-0.1.1/setup.cfg
+-rw-r--r--   0 knrs       (501) staff       (20)      341 2023-07-04 21:31:49.000000 asyncpg-promise-0.1.1/setup.py
```

### Comparing `asyncpg-promise-0.1.0/AsyncPGPromise/AsyncPGPromise.py` & `asyncpg-promise-0.1.1/AsyncPGPromise/AsyncPGPromise.py`

 * *Files identical despite different names*

### Comparing `asyncpg-promise-0.1.0/README.md` & `asyncpg-promise-0.1.1/README.md`

 * *Files identical despite different names*

