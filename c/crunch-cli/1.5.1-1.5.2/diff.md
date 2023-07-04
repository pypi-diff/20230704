# Comparing `tmp/crunch-cli-1.5.1.tar.gz` & `tmp/crunch-cli-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.5.1.tar", last modified: Fri Jun 30 10:13:20 2023, max compression
+gzip compressed data, was "crunch-cli-1.5.2.tar", last modified: Tue Jul  4 11:12:20 2023, max compression
```

## Comparing `crunch-cli-1.5.1.tar` & `crunch-cli-1.5.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.892974 crunch-cli-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:13:20.888974 crunch-cli-1.5.1/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 10:13:20.000000 crunch-cli-1.5.1/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 10:13:20.892974 crunch-cli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 10:13:15.000000 crunch-cli-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/setup.py
```

### Comparing `crunch-cli-1.5.1/crunch/command/convert.py` & `crunch-cli-1.5.2/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/command/download.py` & `crunch-cli-1.5.2/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/command/push.py` & `crunch-cli-1.5.2/crunch/command/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,29 +81,27 @@
 
             if export_path:
                 print(f"export {export_path}")
 
                 with open(export_path, "wb") as fd:
                     shutil.copyfileobj(tmp, fd)
             else:
-                print(f"export project/{project_name}")
-
                 files = [
                     ("codeFile", ('code.tar', tmp, "application/x-tar"))
                 ]
 
                 for path, name in _list_model_files(model_directory_path):
                     print(f"model {name}")
 
                     fd = open(path, "rb")
                     fds.append(fd)
 
                     files.append(("modelFiles", (name, fd)))
-                    print(f"export project/{project_name}")
 
+                print(f"export project/{project_name}")
                 submission = session.post(
                     f"/v1/projects/{project_name}/submissions",
                     data={
                         "message": message,
                         "mainFilePath": main_file_path,
                         "modelDirectoryPath": model_directory_path,
                         "pushToken": push_token,
```

### Comparing `crunch-cli-1.5.1/crunch/command/setup.py` & `crunch-cli-1.5.2/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/command/test.py` & `crunch-cli-1.5.2/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/constants.py` & `crunch-cli-1.5.2/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/demo-project/.gitignore` & `crunch-cli-1.5.2/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/demo-project/main.py` & `crunch-cli-1.5.2/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/ensure.py` & `crunch-cli-1.5.2/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/inline.py` & `crunch-cli-1.5.2/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/library.py` & `crunch-cli-1.5.2/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/main.py` & `crunch-cli-1.5.2/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/tester.py` & `crunch-cli-1.5.2/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch/utils.py` & `crunch-cli-1.5.2/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.5.2/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.1/setup.py` & `crunch-cli-1.5.2/setup.py`

 * *Files identical despite different names*

