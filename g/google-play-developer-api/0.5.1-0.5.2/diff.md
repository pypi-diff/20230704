# Comparing `tmp/google_play_developer_api-0.5.1.tar.gz` & `tmp/google_play_developer_api-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.5.1.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.5.2.tar", max compression
```

## Comparing `google_play_developer_api-0.5.1.tar` & `google_play_developer_api-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-06-23 10:59:20.657139 google_play_developer_api-0.5.1/LICENSE
--rw-r--r--   0        0        0      858 2023-06-23 10:59:20.657139 google_play_developer_api-0.5.1/README.md
--rw-r--r--   0        0        0       78 2023-06-23 10:59:20.657139 google_play_developer_api-0.5.1/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0    10868 2023-06-23 10:59:20.657139 google_play_developer_api-0.5.1/google_play_developer_api/reporting.py
--rw-r--r--   0        0        0     2697 2023-06-23 10:59:20.661139 google_play_developer_api-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-23 10:59:20.661139 google_play_developer_api-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0     2337 2023-06-23 10:59:20.661139 google_play_developer_api-0.5.1/tests/test_reporting_apis.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/LICENSE
+-rw-r--r--   0        0        0      858 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/README.md
+-rw-r--r--   0        0        0       78 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0    10876 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/google_play_developer_api/reporting.py
+-rw-r--r--   0        0        0     2697 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     2337 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/tests/test_reporting_apis.py
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.5.2/PKG-INFO
```

### Comparing `google_play_developer_api-0.5.1/LICENSE` & `google_play_developer_api-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.5.1/README.md` & `google_play_developer_api-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.5.1/google_play_developer_api/reporting.py` & `google_play_developer_api-0.5.2/google_play_developer_api/reporting.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                     .query(
                         name=f"apps/{app_package_name}/{metric_set}",
                         body=body,
                     )
                     .execute()
                 )
 
-            rows.extend(report["rows"])
+            rows.extend(report.get("rows", []))
             page_token = report.get("nextPageToken", "")
             if not page_token:
                 break
 
         # PARSE DATA
         result_list = []
         for row in rows:
```

### Comparing `google_play_developer_api-0.5.1/pyproject.toml` & `google_play_developer_api-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.5.1"
+version = "0.5.2"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
 description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `google_play_developer_api-0.5.1/tests/test_reporting_apis.py` & `google_play_developer_api-0.5.2/tests/test_reporting_apis.py`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.5.1/PKG-INFO` & `google_play_developer_api-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.5.1
+Version: 0.5.2
 Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

