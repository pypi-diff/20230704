# Comparing `tmp/dolphie-2.0.5.tar.gz` & `tmp/dolphie-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-2.0.5.tar", max compression
+gzip compressed data, was "dolphie-2.0.6.tar", max compression
```

## Comparing `dolphie-2.0.5.tar` & `dolphie-2.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.5/LICENSE
--rw-r--r--   0        0        0     7199 2023-07-03 09:15:41.538676 dolphie-2.0.5/README.md
--rw-r--r--   0        0        0     1347 2023-07-03 06:44:11.377308 dolphie-2.0.5/dolphie/Database.py
--rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.5/dolphie/Functions.py
--rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.5/dolphie/KBHit.py
--rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.5/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.5/dolphie/Panels/innodb_io_panel.py
--rw-r--r--   0        0        0     5323 2023-07-03 01:29:41.157031 dolphie-2.0.5/dolphie/Panels/innodb_locks_panel.py
--rw-r--r--   0        0        0    10063 2023-07-03 01:37:34.898441 dolphie-2.0.5/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    11947 2023-07-03 06:53:31.927002 dolphie-2.0.5/dolphie/Panels/replica_panel.py
--rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.5/dolphie/Queries.py
--rw-r--r--   0        0        0    51459 2023-07-03 10:22:51.305863 dolphie-2.0.5/dolphie/__init__.py
--rwxr-xr-x   0        0        0    16046 2023-07-03 10:23:55.259836 dolphie-2.0.5/dolphie/app.py
--rw-r--r--   0        0        0      521 2023-07-03 10:24:46.555236 dolphie-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 dolphie-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-2.0.6/LICENSE
+-rw-r--r--   0        0        0     7199 2023-07-03 09:15:41.538676 dolphie-2.0.6/README.md
+-rw-r--r--   0        0        0     1347 2023-07-03 06:44:11.377308 dolphie-2.0.6/dolphie/Database.py
+-rw-r--r--   0        0        0     2826 2023-07-03 06:21:35.269967 dolphie-2.0.6/dolphie/Functions.py
+-rw-r--r--   0        0        0     2002 2023-07-02 09:17:46.754079 dolphie-2.0.6/dolphie/KBHit.py
+-rw-r--r--   0        0        0    16417 2023-07-03 06:53:04.526750 dolphie-2.0.6/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0    11491 2023-07-03 01:59:19.386574 dolphie-2.0.6/dolphie/Panels/innodb_io_panel.py
+-rw-r--r--   0        0        0     5323 2023-07-03 01:29:41.157031 dolphie-2.0.6/dolphie/Panels/innodb_locks_panel.py
+-rw-r--r--   0        0        0    10063 2023-07-03 01:37:34.898441 dolphie-2.0.6/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0    11948 2023-07-04 03:00:00.226598 dolphie-2.0.6/dolphie/Panels/replica_panel.py
+-rw-r--r--   0        0        0     8209 2023-07-03 06:52:07.577508 dolphie-2.0.6/dolphie/Queries.py
+-rw-r--r--   0        0        0    51459 2023-07-03 10:22:51.305863 dolphie-2.0.6/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    15807 2023-07-04 03:02:02.732373 dolphie-2.0.6/dolphie/app.py
+-rw-r--r--   0        0        0      521 2023-07-04 03:03:29.621625 dolphie-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 dolphie-2.0.6/PKG-INFO
```

### Comparing `dolphie-2.0.5/LICENSE` & `dolphie-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/README.md` & `dolphie-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Database.py` & `dolphie-2.0.6/dolphie/Database.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Functions.py` & `dolphie-2.0.6/dolphie/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/KBHit.py` & `dolphie-2.0.6/dolphie/KBHit.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Panels/dashboard_panel.py` & `dolphie-2.0.6/dolphie/Panels/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Panels/innodb_io_panel.py` & `dolphie-2.0.6/dolphie/Panels/innodb_io_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Panels/innodb_locks_panel.py` & `dolphie-2.0.6/dolphie/Panels/innodb_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Panels/processlist_panel.py` & `dolphie-2.0.6/dolphie/Panels/processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/Panels/replica_panel.py` & `dolphie-2.0.6/dolphie/Panels/replica_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         table.add_column(overflow="fold")
 
     if list_replica_thread_id is not None:
         table.add_row(
             "[grey78]Host", "[grey93]%s" % dolphie.replica_connections[list_replica_thread_id]["host"], style=row_style
         )
     else:
-        table.add_row("[grey78]Master", "[grey93]%s" % data["Master_Host"], style=row_style)
+        table.add_row("[grey78]Primary", "[grey93]%s" % data["Master_Host"], style=row_style)
 
     table.add_row("[grey78]User", "[grey93]%s" % data["Master_User"], style=row_style)
     table.add_row(
         "[grey78]Thread",
         "[grey78]IO [grey93]%s [grey78]SQL [grey93]%s" % (data["Slave_IO_Running"], data["Slave_SQL_Running"]),
         style=row_style,
     )
```

### Comparing `dolphie-2.0.5/dolphie/Queries.py` & `dolphie-2.0.6/dolphie/Queries.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/__init__.py` & `dolphie-2.0.6/dolphie/__init__.py`

 * *Files identical despite different names*

### Comparing `dolphie-2.0.5/dolphie/app.py` & `dolphie-2.0.6/dolphie/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,28 +209,21 @@
         help="Start with additional columns in processlist panel",
     )
     parser.add_argument(
         "--use-processlist",
         dest="use_processlist",
         action="store_true",
         default=False,
-        help="Start with using Processlist instead of Performance Schema for listing queries.",
-    )
-    parser.add_argument(
-        "--use-processlist",
-        dest="use_processlist",
-        action="store_true",
-        default=False,
-        help="Start with using Processlist instead of Performance Schema for listing queries.",
+        help="Start with using Processlist instead of Performance Schema for listing queries",
     )
     parser.add_argument(
         "--debug",
         action="store_true",
         default=False,
-        help="Print tracebacks on errors. Useful for debugging.",
+        help="Print tracebacks on errors for more verbose debugging",
     )
     parser.add_argument(
         "-V", "--version", action="version", version=dolphie.app_version, help="Display version and exit"
     )
 
     parameter_options = vars(parser.parse_args())  # Convert object to dict
     basic_options = ["user", "password", "host", "port", "socket"]
@@ -275,15 +268,15 @@
     # Use login path for login credentials
     if parameter_options["login_path"]:
         try:
             login_path_data = myloginpath.parse(parameter_options["login_path"])
 
             for option in basic_options:
                 if option in login_path_data:
-                    setattr(dolphie, option, cfg.get("client", option))
+                    setattr(dolphie, option, login_path_data[option])
         except Exception as e:
             # Don't error out for default login path
             if parameter_options["login_path"] != "client":
                 raise Exception(f"Problem reading login path file Reason: {e}")
 
     # Use environment variables for basic options if specified
     for option in basic_options:
```

### Comparing `dolphie-2.0.5/pyproject.toml` & `dolphie-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolphie"
-version = "2.0.5"
+version = "2.0.6"
 description = "An intuitive feature-rich top tool for monitoring MySQL in real time"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.4.2"
```

### Comparing `dolphie-2.0.5/PKG-INFO` & `dolphie-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 2.0.5
+Version: 2.0.6
 Summary: An intuitive feature-rich top tool for monitoring MySQL in real time
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

