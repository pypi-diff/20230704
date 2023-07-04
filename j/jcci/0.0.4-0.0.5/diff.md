# Comparing `tmp/jcci-0.0.4.tar.gz` & `tmp/jcci-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.4.tar", last modified: Wed Jun 28 11:10:53 2023, max compression
+gzip compressed data, was "jcci-0.0.5.tar", last modified: Tue Jul  4 10:44:36 2023, max compression
```

## Comparing `jcci-0.0.4.tar` & `jcci-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 11:10:53.264125 jcci-0.0.4/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:06:31.000000 jcci-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1468 2023-06-28 11:10:53.263138 jcci-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      955 2023-06-26 05:36:35.000000 jcci-0.0.4/README.md
--rw-rw-rw-   0        0        0      695 2023-06-28 11:10:41.000000 jcci-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 11:10:53.264125 jcci-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 11:10:53.248137 jcci-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 11:10:53.254125 jcci-0.0.4/src/jcci/
--rw-rw-rw-   0        0        0        0 2022-09-20 03:04:57.000000 jcci-0.0.4/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-25 09:25:01.000000 jcci-0.0.4/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    41682 2023-06-26 05:17:01.000000 jcci-0.0.4/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-06-28 11:10:53.262124 jcci-0.0.4/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     1468 2023-06-28 11:10:53.000000 jcci-0.0.4/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-28 11:10:53.000000 jcci-0.0.4/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 11:10:53.000000 jcci-0.0.4/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-28 11:10:53.000000 jcci-0.0.4/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-28 11:10:53.000000 jcci-0.0.4/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.078792 jcci-0.0.5/
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:06:31.000000 jcci-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1468 2023-07-04 10:44:36.077793 jcci-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      955 2023-06-26 05:36:35.000000 jcci-0.0.5/README.md
+-rw-rw-rw-   0        0        0      695 2023-07-04 10:44:25.000000 jcci-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 10:44:36.078792 jcci-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.064810 jcci-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.070793 jcci-0.0.5/src/jcci/
+-rw-rw-rw-   0        0        0        0 2022-09-20 03:04:57.000000 jcci-0.0.5/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-06-25 09:25:01.000000 jcci-0.0.5/src/jcci/java_analyzer.py
+-rw-rw-rw-   0        0        0    42459 2023-07-04 10:38:53.000000 jcci-0.0.5/src/jcci/jcci.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:44:36.076829 jcci-0.0.5/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0     1468 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-04 10:44:36.000000 jcci-0.0.5/src/jcci.egg-info/top_level.txt
```

### Comparing `jcci-0.0.4/PKG-INFO` & `jcci-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.4
+Version: 0.0.5
 Summary: Java code commit impact in pure Python
 Author-email: Quan Li <441640312@qq.com>
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jcci-0.0.4/README.md` & `jcci-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jcci-0.0.4/pyproject.toml` & `jcci-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Quan Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact in pure Python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `jcci-0.0.4/src/jcci/java_analyzer.py` & `jcci-0.0.5/src/jcci/java_analyzer.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.4/src/jcci/jcci.py` & `jcci-0.0.5/src/jcci/jcci.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,23 @@
                                                 method_annotation_element.name == 'path' or method_annotation_element.name == 'value']
                         if len(method_api_path_list) > 0:
                             method_api_path_obj = method_api_path_list[0]
                             if 'value' in method_api_path_obj.attrs:
                                 method_api_path += [method_api_path_obj.value.replace('"', '')]
                             else:
                                 if 'values' in method_api_path_obj.attrs:
-                                    method_api_path += [method_api_value.value.replace('"', '') for method_api_value in
-                                                        method_api_path_obj.values]
+                                    for method_api_value in method_api_path_obj.values:
+                                        if type(method_api_value).__name__ == "BinaryOperation":
+                                            operandl = method_api_value.operandl
+                                            operandr = method_api_value.operandr
+                                            operandl_str = _get_api_part_route(operandl)
+                                            operandr_str = _get_api_part_route(operandr)
+                                            method_api_path += [operandl_str + operandr_str]
+                                        else:
+                                            method_api_path += [method_api_value.value.replace('"', '')]
                                 else:
                                     method_api_path += [method_name + '/cci-unknown']
             if len(method_api_path) == 0:
                 method_api_path = ['/']
             for method_api_path_obj in method_api_path:
                 if method_api_path_obj.startswith('/'):
                     method_api_path_obj = method_api_path_obj[1:]
@@ -266,14 +273,20 @@
                                 extends_name_path, is_controller)
     file_analyze.imports = imports
     file_analyze.implements = implements_names_list
     file_analyze.declarators = fields_list
     file_analyze.methods = methods_list
     return file_analyze
 
+def _get_api_part_route(part):
+    part_class = type(part).__name__
+    if part_class == 'MemberReference':
+        return part.member
+    elif part_class == 'Literal':
+        return part.value
 
 def _get_method_end_line(method_obj):
     method_end_line = method_obj.position.line
     if method_obj.body is not None and len(method_obj.body) > 0:
         method_end_line = method_obj.body[-1].position.line
         method_body = method_obj.body[-1]
         while True:
@@ -706,7 +719,9 @@
     t2 = datetime.datetime.now()
     try:
         print(datetime.datetime.now(), ':', 'Analyze done, remove occupy, others can analyze now', flush=True)
         os.remove(folder_name + sep + 'Occupy.ing')
     except:
         pass
     print(datetime.datetime.now(), ':', 'Analyze done, spend: ', t2 - t1, flush=True)
+
+
```

### Comparing `jcci-0.0.4/src/jcci.egg-info/PKG-INFO` & `jcci-0.0.5/src/jcci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.4
+Version: 0.0.5
 Summary: Java code commit impact in pure Python
 Author-email: Quan Li <441640312@qq.com>
 Project-URL: Homepage, https://github.com/baikaishuipp/jcci
 Project-URL: Bug Tracker, https://github.com/baikaishuipp/jcci/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

