# Comparing `tmp/envoxy-0.2.6.tar.gz` & `tmp/envoxy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envoxy-0.2.6.tar", last modified: Thu Jun 29 19:40:05 2023, max compression
+gzip compressed data, was "dist/envoxy-0.2.7.tar", last modified: Tue Jul  4 19:25:06 2023, max compression
```

## Comparing `envoxy-0.2.6.tar` & `envoxy-0.2.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1427 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     5091 2023-06-29 19:40:05.000000 envoxy-0.2.6/envoxy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/views/
--rw-rw-r--   0 root         (0) root         (0)     1896 2023-06-28 15:54:54.000000 envoxy-0.2.6/src/envoxy/views/containers.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2023-06-29 19:06:05.000000 envoxy-0.2.6/src/envoxy/views/views.py
--rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/http/
--rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/http/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/http/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.6/src/envoxy/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/mqtt/
--rw-rw-r--   0 root         (0) root         (0)    14000 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/mqtt/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/mqtt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/redis/
--rw-rw-r--   0 root         (0) root         (0)     1865 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/redis/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/postgresql/
--rw-rw-r--   0 root         (0) root         (0)     5690 2022-09-06 19:19:17.000000 envoxy-0.2.6/src/envoxy/postgresql/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/postgresql/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.6/src/envoxy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/zeromq/
--rw-rw-r--   0 root         (0) root         (0)    18421 2023-06-27 14:55:49.000000 envoxy-0.2.6/src/envoxy/zeromq/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/zeromq/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     3115 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/decorators.py
--rw-rw-r--   0 root         (0) root         (0)    17561 2023-06-28 15:43:03.000000 envoxy-0.2.6/src/envoxy/asserts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/couchdb/
--rw-rw-r--   0 root         (0) root         (0)     3271 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/couchdb/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/couchdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/cache/
--rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/cache/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1856 2023-06-27 09:44:39.000000 envoxy-0.2.6/src/envoxy/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/utils/
--rw-rw-r--   0 root         (0) root         (0)      825 2023-06-26 16:48:30.000000 envoxy-0.2.6/src/envoxy/utils/encoders.py
--rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/utils/watchdog.py
--rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/utils/datetime.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/utils/cache.py
--rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/utils/logs.py
--rw-rw-r--   0 root         (0) root         (0)     1397 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/utils/throttle.py
--rw-rw-r--   0 root         (0) root         (0)     1846 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/utils/singleton.py
--rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.6/src/envoxy/utils/config.py
--rw-rw-r--   0 root         (0) root         (0)     1237 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/utils/handlers.py
--rw-rw-r--   0 root         (0) root         (0)     1394 2023-06-29 19:35:18.000000 envoxy-0.2.6/src/envoxy/utils/profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/db/
--rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/db/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/db/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.6/src/envoxy/tests/test_asserts.py
--rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:40:05.000000 envoxy-0.2.6/src/envoxy/auth/
--rw-rw-r--   0 root         (0) root         (0)     2619 2023-06-26 16:39:14.000000 envoxy-0.2.6/src/envoxy/auth/backends.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.6/src/envoxy/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      230 2023-06-28 15:53:20.000000 envoxy-0.2.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 19:40:05.000000 envoxy-0.2.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.6/README.md
--rw-rw-r--   0 root         (0) root         (0)       64 2023-06-26 16:39:14.000000 envoxy-0.2.6/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1202 2023-06-29 19:35:34.000000 envoxy-0.2.6/setup.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-06-29 19:40:05.000000 envoxy-0.2.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-07-04 19:25:06.000000 envoxy-0.2.7/envoxy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.7/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/views/
+-rw-rw-r--   0 root         (0) root         (0)     1896 2023-06-28 15:54:54.000000 envoxy-0.2.7/src/envoxy/views/containers.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2023-06-29 19:06:05.000000 envoxy-0.2.7/src/envoxy/views/views.py
+-rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/http/
+-rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/http/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/http/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.7/src/envoxy/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/mqtt/
+-rw-rw-r--   0 root         (0) root         (0)    14000 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/mqtt/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/mqtt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/redis/
+-rw-rw-r--   0 root         (0) root         (0)     1865 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/redis/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/postgresql/
+-rw-rw-r--   0 root         (0) root         (0)     5690 2022-09-06 19:19:17.000000 envoxy-0.2.7/src/envoxy/postgresql/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/postgresql/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.7/src/envoxy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/zeromq/
+-rw-rw-r--   0 root         (0) root         (0)    18641 2023-07-04 18:43:43.000000 envoxy-0.2.7/src/envoxy/zeromq/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/zeromq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     3115 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)    17561 2023-06-28 15:43:03.000000 envoxy-0.2.7/src/envoxy/asserts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/couchdb/
+-rw-rw-r--   0 root         (0) root         (0)     3271 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/couchdb/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/couchdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/cache/
+-rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/cache/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1856 2023-06-27 09:44:39.000000 envoxy-0.2.7/src/envoxy/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/utils/
+-rw-rw-r--   0 root         (0) root         (0)      825 2023-06-26 16:48:30.000000 envoxy-0.2.7/src/envoxy/utils/encoders.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/utils/watchdog.py
+-rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/utils/datetime.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/utils/logs.py
+-rw-rw-r--   0 root         (0) root         (0)     1397 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/utils/throttle.py
+-rw-rw-r--   0 root         (0) root         (0)     1846 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/utils/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.7/src/envoxy/utils/config.py
+-rw-rw-r--   0 root         (0) root         (0)     1237 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/utils/handlers.py
+-rw-rw-r--   0 root         (0) root         (0)     1394 2023-06-29 19:35:18.000000 envoxy-0.2.7/src/envoxy/utils/profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/db/
+-rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/db/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/db/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.7/src/envoxy/tests/test_asserts.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 19:25:06.000000 envoxy-0.2.7/src/envoxy/auth/
+-rw-rw-r--   0 root         (0) root         (0)     2619 2023-06-26 16:39:14.000000 envoxy-0.2.7/src/envoxy/auth/backends.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.7/src/envoxy/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      230 2023-06-28 15:53:20.000000 envoxy-0.2.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 19:25:06.000000 envoxy-0.2.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-06-26 16:39:14.000000 envoxy-0.2.7/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1202 2023-07-04 18:48:02.000000 envoxy-0.2.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-07-04 19:25:06.000000 envoxy-0.2.7/PKG-INFO
```

### Comparing `envoxy-0.2.6/envoxy.egg-info/SOURCES.txt` & `envoxy-0.2.7/envoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/envoxy.egg-info/PKG-INFO` & `envoxy-0.2.7/envoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.6
+Version: 0.2.7
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `envoxy-0.2.6/LICENSE` & `envoxy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/views/containers.py` & `envoxy-0.2.7/src/envoxy/views/containers.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/views/views.py` & `envoxy-0.2.7/src/envoxy/views/views.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/http/dispatcher.py` & `envoxy-0.2.7/src/envoxy/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/constants.py` & `envoxy-0.2.7/src/envoxy/constants.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/mqtt/dispatcher.py` & `envoxy-0.2.7/src/envoxy/mqtt/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/redis/client.py` & `envoxy-0.2.7/src/envoxy/redis/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/postgresql/client.py` & `envoxy-0.2.7/src/envoxy/postgresql/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/__init__.py` & `envoxy-0.2.7/src/envoxy/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/zeromq/dispatcher.py` & `envoxy-0.2.7/src/envoxy/zeromq/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class ZMQ(Singleton):
 
     _cache = None
     _instances = {}
     _contexts = {}
     _workers = {}
-    _available_workers = queue.Queue()
+    _available_workers = {}
     _executor = None
     _lock = threading.Lock()
 
     def __init__(self):
 
         try:
             _workers_conf = Config.get('zmq_workers')
@@ -69,38 +69,40 @@
 
             self._instances[_server_key] = {
                 'server_key': _server_key,
                 'conf': _conf,
                 'url': f"tcp://{_conf.get('host')}:{_conf.get('port')}"
             }
 
+            self._available_workers[_server_key] = queue.Queue()
+
+            for _i in range(self._max_workers):
+                self.add_worker(_server_key, f'zmqc-poller-{_server_key}-{_i}')
+
         # Cached Routes
         if Config.get('cache'):
             _cache_instance = Cache()
             self._cache = _cache_instance.get_backend()
 
-        for _i in range(self._max_workers):
-            self.add_worker(f'zmqc-poller-{_i}')
-
         self._executor = ThreadPoolExecutor(
             max_workers=self._thread_poll_executor_max_workers, thread_name_prefix='zmqc-worker')
 
-    def get_available_worker(self):
-        return self._available_workers.get()
+    def get_available_worker(self, server_key):
+        return self._available_workers[server_key].get()
 
-    def add_worker(self, worker_id):
+    def add_worker(self, server_key, worker_id):
 
         with self._lock:
 
             self._workers[worker_id] = {
                 'poller': zmq.Poller(),
                 'socket': None
             }
 
-        self.free_worker(worker_id)
+        self.free_worker(server_key, worker_id)
 
     def get_or_create_socket(self, server_key, worker_id):
 
         with self._lock:
 
             _worker = self._workers[worker_id]
 
@@ -148,20 +150,20 @@
                 try:
                     _socket.close(linger=0)
                 except Exception:
                     pass
                 
                 _worker['socket'] = None
 
-    def free_worker(self, worker_id, close_socket=False):
+    def free_worker(self, server_key, worker_id, close_socket=False):
 
         if close_socket:
             self.close_and_unregister_socket(worker_id)
 
-        self._available_workers.put(worker_id)
+        self._available_workers[server_key].put(worker_id)
 
     def remove_header(self, response, header):
 
         if 'headers' in response and header in response['headers']:
             response['headers'].pop(header, None)
 
     def remove_keys(self, response, keys):
@@ -222,15 +224,15 @@
 
                             return _cached_response
 
         try:
 
             while True:
 
-                _worker_id = self.get_available_worker()
+                _worker_id = self.get_available_worker(server_key)
 
                 with self._lock:
                     _worker = self._workers[_worker_id]
 
                 _socket = self.get_or_create_socket(server_key, _worker_id)
 
                 _socket.send_multipart(
@@ -255,15 +257,15 @@
                                 raise NoSocketException(
                                     f'No events received in {(ZEROMQ_POLLIN_TIMEOUT/1000)*ZEROMQ_POLLER_RETRIES} secs on {_instance["url"]}')
 
                         if _socks.get(_socket) == zmq.POLLIN:
 
                             _recv = _socket.recv_multipart()
 
-                            self.free_worker(_worker_id)
+                            self.free_worker(server_key, _worker_id)
 
                             _recv.pop(0)  # discard delimiter
                             _response = envoxy_json_loads(_recv.pop(0))  # actual message
 
                             self.remove_header(_response, 'X-Cid')
 
                             self.remove_keys(_response, ['protocol', 'performative'])
@@ -321,37 +323,37 @@
                             return _response
 
                 except IOError:
 
                     Log.error(
                         f"ZMQ::send_and_recv : Could not connect to ZeroMQ machine: {_instance['url']}")
 
-                    self.free_worker(_worker_id, close_socket=True)
+                    self.free_worker(server_key, _worker_id, close_socket=True)
 
                     time.sleep(ZEROMQ_RETRY_TIMEOUT)
 
                     return self.send_and_recv(server_key, message)
 
         except NoSocketException as e:
 
             Log.warning(
                 f"ZMQ::send_and_recv : It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
 
-            self.free_worker(_worker_id, close_socket=True)
+            self.free_worker(server_key, _worker_id, close_socket=True)
 
             time.sleep(ZEROMQ_RETRY_TIMEOUT)
 
             return self.send_and_recv(server_key, message)
 
         except Exception as e:
 
             Log.warning(
                 f"ZMQ::send_and_recv : Unexpected error. It is not possible to send message using the ZMQ server \"{_instance['url']}\". Error: {e}")
 
-            self.free_worker(_worker_id, close_socket=True)
+            self.free_worker(server_key, _worker_id, close_socket=True)
 
             time.sleep(ZEROMQ_RETRY_TIMEOUT)
 
             return self.send_and_recv(server_key, message)
 
 
 class Dispatcher():
```

### Comparing `envoxy-0.2.6/src/envoxy/decorators.py` & `envoxy-0.2.7/src/envoxy/decorators.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/asserts.py` & `envoxy-0.2.7/src/envoxy/asserts.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/couchdb/client.py` & `envoxy-0.2.7/src/envoxy/couchdb/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/cache/__init__.py` & `envoxy-0.2.7/src/envoxy/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/cache/redis.py` & `envoxy-0.2.7/src/envoxy/cache/redis.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/encoders.py` & `envoxy-0.2.7/src/envoxy/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/watchdog.py` & `envoxy-0.2.7/src/envoxy/utils/watchdog.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/datetime.py` & `envoxy-0.2.7/src/envoxy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/cache.py` & `envoxy-0.2.7/src/envoxy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/logs.py` & `envoxy-0.2.7/src/envoxy/utils/logs.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/throttle.py` & `envoxy-0.2.7/src/envoxy/utils/throttle.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/singleton.py` & `envoxy-0.2.7/src/envoxy/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/config.py` & `envoxy-0.2.7/src/envoxy/utils/config.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/handlers.py` & `envoxy-0.2.7/src/envoxy/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/utils/profiling.py` & `envoxy-0.2.7/src/envoxy/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/db/dispatcher.py` & `envoxy-0.2.7/src/envoxy/db/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/tests/test_asserts.py` & `envoxy-0.2.7/src/envoxy/tests/test_asserts.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/tests/fixtures.py` & `envoxy-0.2.7/src/envoxy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/src/envoxy/auth/backends.py` & `envoxy-0.2.7/src/envoxy/auth/backends.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/README.md` & `envoxy-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.6/setup.py` & `envoxy-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return os.path.join(data_dir, path)
 
 with open(find_file('README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='envoxy',
-    version='0.2.6',
+    version='0.2.7',
     description='Envoxy Platform Framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Matheus (vorjdux) Santos',
     author_email='vorj.dux@gmail.com',
     url='https://github.com/habitio/envoxy',
     packages=find_packages(where='src/', exclude=("tests", "templates")),
```

### Comparing `envoxy-0.2.6/PKG-INFO` & `envoxy-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.6
+Version: 0.2.7
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

