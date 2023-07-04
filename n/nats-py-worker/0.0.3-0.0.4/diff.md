# Comparing `tmp/nats-py-worker-0.0.3.tar.gz` & `tmp/nats-py-worker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-py-worker-0.0.3.tar", last modified: Mon Jul  3 02:46:47 2023, max compression
+gzip compressed data, was "nats-py-worker-0.0.4.tar", last modified: Mon Jul  3 03:01:47 2023, max compression
```

## Comparing `nats-py-worker-0.0.3.tar` & `nats-py-worker-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.058283 nats-py-worker-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.059284 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.059284 nats-py-worker-0.0.3/src/nats_worker/
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/src/nats_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21798 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/src/nats_worker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/tests/test_nats_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:01:47.032771 nats-py-worker-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 03:01:47.032771 nats-py-worker-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 03:01:47.032771 nats-py-worker-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:01:47.030771 nats-py-worker-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:01:47.031772 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 03:01:47.000000 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-03 03:01:47.000000 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:01:47.000000 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 03:01:47.000000 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-03 03:01:47.000000 nats-py-worker-0.0.4/src/nats_py_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:01:47.031772 nats-py-worker-0.0.4/src/nats_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/src/nats_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22009 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/src/nats_worker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:01:47.032771 nats-py-worker-0.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-03 03:01:35.000000 nats-py-worker-0.0.4/tests/test_nats_worker.py
```

### Comparing `nats-py-worker-0.0.3/LICENSE` & `nats-py-worker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.3/PKG-INFO` & `nats-py-worker-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py-worker
-Version: 0.0.3
+Version: 0.0.4
 Summary: An opinionated utility for using NATS as a worker queue with NATS.py
 License: Copyright (c) 2023 The University of Adelaide
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `nats-py-worker-0.0.3/README.md` & `nats-py-worker-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.3/pyproject.toml` & `nats-py-worker-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.3/src/nats_py_worker.egg-info/PKG-INFO` & `nats-py-worker-0.0.4/src/nats_py_worker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py-worker
-Version: 0.0.3
+Version: 0.0.4
 Summary: An opinionated utility for using NATS as a worker queue with NATS.py
 License: Copyright (c) 2023 The University of Adelaide
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `nats-py-worker-0.0.3/src/nats_worker/core.py` & `nats-py-worker-0.0.4/src/nats_worker/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,21 @@
                 ):
                     key = key_map(msg)
                     state_entry = await get_value(
                         connection=connection, bucket=bucket, key=key
                     )
                     if state_entry is None:
                         state_entry = NatsKeyValue.Entry(
-                            bucket=bucket, key=key, revision=None, value=None
+                            bucket=bucket,
+                            key=key,
+                            revision=None,
+                            value=None,
+                            delta=None,
+                            created=None,
+                            operation=None,
                         )
                     new_state = await f(state_entry, msg, **kwargs)
                     if new_state is not None:
                         await save_value(
                             connection=connection,
                             bucket=bucket,
                             key=key,
```

### Comparing `nats-py-worker-0.0.3/tests/test_nats_worker.py` & `nats-py-worker-0.0.4/tests/test_nats_worker.py`

 * *Files identical despite different names*

