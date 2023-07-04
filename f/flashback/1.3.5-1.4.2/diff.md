# Comparing `tmp/flashback-1.3.5.tar.gz` & `tmp/flashback-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashback-1.3.5.tar", last modified: Mon Feb 27 13:17:32 2023, max compression
+gzip compressed data, was "flashback-1.4.2.tar", last modified: Tue Jul  4 15:12:43 2023, max compression
```

## Comparing `flashback-1.3.5.tar` & `flashback-1.4.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.826811 flashback-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-02-27 13:17:19.000000 flashback-1.3.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-27 13:17:19.000000 flashback-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-27 13:17:19.000000 flashback-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-02-27 13:17:32.826811 flashback-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-27 13:17:19.000000 flashback-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.814811 flashback-1.3.5/flashback/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.814811 flashback-1.3.5/flashback/accessing/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/accessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/accessing/dig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/borg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.814811 flashback-1.3.5/flashback/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.818812 flashback-1.3.5/flashback/caching/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/disk_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/memcached_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/memory_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/adapters/redis_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/caching/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/classproperty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.818812 flashback-1.3.5/flashback/debugging/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/caller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.818812 flashback-1.3.5/flashback/debugging/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/filters/call_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/filters/decorator_operator_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/filters/type_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/get_call_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/get_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/get_frameinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/profiled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.818812 flashback-1.3.5/flashback/debugging/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/styles/jellybeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/debugging/xp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/encrypted_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.822811 flashback-1.3.5/flashback/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/_inflect.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/adverbize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/camelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/kebabize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.822811 flashback-1.3.5/flashback/formatting/locales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/locales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/locales/de.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/locales/en.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/locales/es.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/locales/fr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/ordinalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/oxford_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/pascalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/pluralize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/singularize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/snakeize.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/transliterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/formatting/truncate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.822811 flashback-1.3.5/flashback/i16g/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/i16g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/i16g/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.822811 flashback-1.3.5/flashback/importing/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/importing/import_class_from_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/importing/import_module_from_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.826811 flashback-1.3.5/flashback/iterating/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/flat_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/renumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/iterating/uniq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.826811 flashback-1.3.5/flashback/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/logging/affixed_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/logging/configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/logging/muted.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/retryable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/sampled.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/timed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-27 13:17:19.000000 flashback-1.3.5/flashback/timeoutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:17:32.814811 flashback-1.3.5/flashback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-02-27 13:17:32.000000 flashback-1.3.5/flashback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-27 13:17:32.000000 flashback-1.3.5/flashback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:17:32.000000 flashback-1.3.5/flashback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-27 13:17:32.000000 flashback-1.3.5/flashback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-27 13:17:32.000000 flashback-1.3.5/flashback.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-27 13:17:19.000000 flashback-1.3.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-27 13:17:19.000000 flashback-1.3.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 13:17:19.000000 flashback-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 13:17:32.826811 flashback-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-02-27 13:17:19.000000 flashback-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-04 15:12:20.000000 flashback-1.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 15:12:20.000000 flashback-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 15:12:20.000000 flashback-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-04 15:12:43.611612 flashback-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-04 15:12:20.000000 flashback-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/accessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/accessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/accessing/dig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/borg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/caching/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/disk_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/memcached_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/memory_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/adapters/redis_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/caching/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/classproperty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/debugging/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/caller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/debugging/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/filters/call_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/filters/decorator_operator_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/filters/type_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/get_call_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/get_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/get_frameinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/profiled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback/debugging/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/styles/jellybeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/debugging/xp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/encrypted_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/_inflect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/adverbize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/camelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/kebabize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/formatting/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/locales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/locales/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/locales/en.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/locales/es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/locales/fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/ordinalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/oxford_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/pascalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/pluralize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/singularize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/snakeize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/formatting/truncate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/i16g/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/i16g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/i16g/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/importing/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/importing/import_class_from_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/importing/import_module_from_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/iterating/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/flat_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/renumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/iterating/uniq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.611612 flashback-1.4.2/flashback/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/logging/affixed_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/logging/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/logging/muted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/retryable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/sampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/timed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 15:12:20.000000 flashback-1.4.2/flashback/timeoutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:12:43.607612 flashback-1.4.2/flashback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-04 15:12:43.000000 flashback-1.4.2/flashback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-04 15:12:43.000000 flashback-1.4.2/flashback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:12:43.000000 flashback-1.4.2/flashback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-04 15:12:43.000000 flashback-1.4.2/flashback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 15:12:43.000000 flashback-1.4.2/flashback.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 15:12:20.000000 flashback-1.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 15:12:20.000000 flashback-1.4.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 15:12:20.000000 flashback-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:12:43.611612 flashback-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-04 15:12:20.000000 flashback-1.4.2/setup.py
```

### Comparing `flashback-1.3.5/CHANGELOG.md` & `flashback-1.4.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 1.4.2 (04/07/2023)
+
+- Updated dependencies
+- Updated github actions
+- Updated pypi upload
+
 ## 1.3.5 (27/02/2023)
 
 - Fix dependencies
 
 ## 1.3.4 (27/02/2023)
 
 - Updated dependencies
```

### Comparing `flashback-1.3.5/LICENSE` & `flashback-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/PKG-INFO` & `flashback-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 1.3.5
+Version: 1.4.2
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/PaulRenvoise/flashback/develop/assets/logo.png" alt="Flashback"></a>
 </p>
 <h3 align="center">Flashback</h3>
```

### Comparing `flashback-1.3.5/README.md` & `flashback-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/__init__.py` & `flashback-1.4.2/flashback/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "deprecated",
     "retryable",
     "sampled",
     "timed",
     "timeoutable",
 )
 
-__version__ = "1.3.5"
+__version__ = "1.4.2"
```

### Comparing `flashback-1.3.5/flashback/accessing/dig.py` & `flashback-1.4.2/flashback/accessing/dig.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/borg.py` & `flashback-1.4.2/flashback/borg.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/adapters/base.py` & `flashback-1.4.2/flashback/caching/adapters/base.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/adapters/disk_adapter.py` & `flashback-1.4.2/flashback/caching/adapters/disk_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/adapters/memcached_adapter.py` & `flashback-1.4.2/flashback/caching/adapters/memcached_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/adapters/memory_adapter.py` & `flashback-1.4.2/flashback/caching/adapters/memory_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/adapters/redis_adapter.py` & `flashback-1.4.2/flashback/caching/adapters/redis_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/cache.py` & `flashback-1.4.2/flashback/caching/cache.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/caching/cached.py` & `flashback-1.4.2/flashback/caching/cached.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/classproperty.py` & `flashback-1.4.2/flashback/classproperty.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/caller.py` & `flashback-1.4.2/flashback/debugging/caller.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/filters/call_highlight_filter.py` & `flashback-1.4.2/flashback/debugging/filters/call_highlight_filter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/filters/decorator_operator_filter.py` & `flashback-1.4.2/flashback/debugging/filters/decorator_operator_filter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/filters/type_highlight_filter.py` & `flashback-1.4.2/flashback/debugging/filters/type_highlight_filter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/formatter.py` & `flashback-1.4.2/flashback/debugging/formatter.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/get_call_context.py` & `flashback-1.4.2/flashback/debugging/get_call_context.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/get_callable.py` & `flashback-1.4.2/flashback/debugging/get_callable.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/get_frameinfo.py` & `flashback-1.4.2/flashback/debugging/get_frameinfo.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/parser.py` & `flashback-1.4.2/flashback/debugging/parser.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/profiled.py` & `flashback-1.4.2/flashback/debugging/profiled.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/styles/jellybeans.py` & `flashback-1.4.2/flashback/debugging/styles/jellybeans.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/debugging/xp.py` & `flashback-1.4.2/flashback/debugging/xp.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/deprecated.py` & `flashback-1.4.2/flashback/deprecated.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/encrypted_file.py` & `flashback-1.4.2/flashback/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/__init__.py` & `flashback-1.4.2/flashback/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/_inflect.py` & `flashback-1.4.2/flashback/formatting/_inflect.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/adverbize.py` & `flashback-1.4.2/flashback/formatting/adverbize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/camelize.py` & `flashback-1.4.2/flashback/formatting/camelize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/kebabize.py` & `flashback-1.4.2/flashback/formatting/kebabize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/locales/de.py` & `flashback-1.4.2/flashback/formatting/locales/de.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/locales/en.py` & `flashback-1.4.2/flashback/formatting/locales/en.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/locales/es.py` & `flashback-1.4.2/flashback/formatting/locales/es.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/locales/fr.py` & `flashback-1.4.2/flashback/formatting/locales/fr.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/ordinalize.py` & `flashback-1.4.2/flashback/formatting/ordinalize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/oxford_join.py` & `flashback-1.4.2/flashback/formatting/oxford_join.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/parameterize.py` & `flashback-1.4.2/flashback/formatting/parameterize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/pascalize.py` & `flashback-1.4.2/flashback/formatting/pascalize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/pluralize.py` & `flashback-1.4.2/flashback/formatting/pluralize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/singularize.py` & `flashback-1.4.2/flashback/formatting/singularize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/snakeize.py` & `flashback-1.4.2/flashback/formatting/snakeize.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/transliterate.py` & `flashback-1.4.2/flashback/formatting/transliterate.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/formatting/truncate.py` & `flashback-1.4.2/flashback/formatting/truncate.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/i16g/locale.py` & `flashback-1.4.2/flashback/i16g/locale.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/importing/import_class_from_path.py` & `flashback-1.4.2/flashback/importing/import_class_from_path.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/importing/import_module_from_path.py` & `flashback-1.4.2/flashback/importing/import_module_from_path.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/chunks.py` & `flashback-1.4.2/flashback/iterating/chunks.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/compact.py` & `flashback-1.4.2/flashback/iterating/compact.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/flat_map.py` & `flashback-1.4.2/flashback/iterating/flat_map.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/flatten.py` & `flashback-1.4.2/flashback/iterating/flatten.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/partition.py` & `flashback-1.4.2/flashback/iterating/partition.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/renumerate.py` & `flashback-1.4.2/flashback/iterating/renumerate.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/iterating/uniq.py` & `flashback-1.4.2/flashback/iterating/uniq.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/logging/__init__.py` & `flashback-1.4.2/flashback/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/logging/affixed_stream_handler.py` & `flashback-1.4.2/flashback/logging/affixed_stream_handler.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/logging/configurations.py` & `flashback-1.4.2/flashback/logging/configurations.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/logging/muted.py` & `flashback-1.4.2/flashback/logging/muted.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/retryable.py` & `flashback-1.4.2/flashback/retryable.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/sampled.py` & `flashback-1.4.2/flashback/sampled.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/sentinel.py` & `flashback-1.4.2/flashback/sentinel.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/singleton.py` & `flashback-1.4.2/flashback/singleton.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/timed.py` & `flashback-1.4.2/flashback/timed.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback/timeoutable.py` & `flashback-1.4.2/flashback/timeoutable.py`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/flashback.egg-info/PKG-INFO` & `flashback-1.4.2/flashback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 1.3.5
+Version: 1.4.2
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/PaulRenvoise/flashback/develop/assets/logo.png" alt="Flashback"></a>
 </p>
 <h3 align="center">Flashback</h3>
```

### Comparing `flashback-1.3.5/flashback.egg-info/SOURCES.txt` & `flashback-1.4.2/flashback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashback-1.3.5/setup.py` & `flashback-1.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         "Topic :: Utilities",
     ],
 
     packages=find_packages(exclude=("tests", "tests.*")),
 
     install_requires=read_requirements_file("requirements.txt"),
     tests_require=read_requirements_file("requirements-test.txt"),
-    python_requires=">=3.7.*",
+    python_requires=">=3.7",
     setup_requires=["pytest-runner"],
 
     test_suite="tests",
 
     entry_points="",
     scripts="",
     data_files=[],
```

