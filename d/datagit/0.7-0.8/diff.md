# Comparing `tmp/datagit-0.7.tar.gz` & `tmp/datagit-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.7.tar", last modified: Mon Jul  3 17:14:34 2023, max compression
+gzip compressed data, was "datagit-0.8.tar", last modified: Tue Jul  4 09:25:47 2023, max compression
```

## Comparing `datagit-0.7.tar` & `datagit-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.110550 datagit-0.7/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 17:14:34.110393 datagit-0.7/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-03 14:48:50.000000 datagit-0.7/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.109029 datagit-0.7/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.7/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2120 2023-07-03 17:12:23.000000 datagit-0.7/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     9717 2023-07-03 17:07:17.000000 datagit-0.7/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.7/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.110116 datagit-0.7/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 17:14:34.110633 datagit-0.7/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 17:14:31.000000 datagit-0.7/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.755957 datagit-0.8/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-04 09:25:47.755800 datagit-0.8/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-04 08:55:47.000000 datagit-0.8/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.754719 datagit-0.8/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-07-04 08:55:47.000000 datagit-0.8/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2336 2023-07-04 08:55:47.000000 datagit-0.8/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     9804 2023-07-04 09:24:12.000000 datagit-0.8/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-07-04 08:55:47.000000 datagit-0.8/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.755560 datagit-0.8/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-04 09:25:47.756013 datagit-0.8/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-04 09:25:34.000000 datagit-0.8/setup.py
```

### Comparing `datagit-0.7/PKG-INFO` & `datagit-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.7
+Version: 0.8
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.7/README.md` & `datagit-0.8/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.7/datagit/dataset_helpers.py` & `datagit-0.8/datagit/dataset_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,48 @@
     assert_dataset_has_unique_key(df)
 
     sorted_df = df.sort_values(by=['unique_key'])
     return sorted_df
 
 
 def compare_dataframes(initial_df: pd.DataFrame, final_df: pd.DataFrame, unique_key: str):
-    # Get the unique keys for each dataframe
-    initial_keys = set(initial_df[unique_key])
-    final_keys = set(final_df[unique_key])
-
-    intersection_keys = initial_keys.intersection(final_keys)
-
-    # Calculate the additions, modifications, and deletions
-    additions = len(final_keys - intersection_keys)
-    deletions = len(initial_keys - intersection_keys)
-
-    # Get the intersection of the unique keys
-
-    # Filter the rows in df1 and df2 that match the intersection of the unique keys
-    df1_intersection = initial_df[initial_df[unique_key].isin(
-        intersection_keys)].reset_index(drop=True)
-    df2_intersection = final_df[final_df[unique_key].isin(
-        intersection_keys)].reset_index(drop=True)
-
-    diff = df1_intersection.compare(df2_intersection)
-
-    modifications = diff.__len__()
-
-    # Construct the result text
-    result = ""
-    if additions > 0:
-        result += f"- 🆕 {additions} addition{'s' if additions > 1 else ''}\n"
-    else:
-        result += f"- ~~🆕 0 addition~~\n"
-    if modifications > 0:
-        result += f"- ♻️ {modifications} modification{'s' if modifications > 1 else ''}\n"
-    else:
-        result += f"- ~~♻️ 0 modification~~\n"
-    if deletions > 0:
-        result += f"- 🗑️ {deletions} deletion{'s' if deletions > 1 else ''}\n"
-    else:
-        result += f"- ~~🗑️ 0 deletion~~\n"
-
-    return result.strip()
+    try:
+        # Get the unique keys for each dataframe
+        initial_keys = set(initial_df[unique_key])
+        final_keys = set(final_df[unique_key])
+
+        intersection_keys = initial_keys.intersection(final_keys)
+
+        # Calculate the additions, modifications, and deletions
+        additions = len(final_keys - intersection_keys)
+        deletions = len(initial_keys - intersection_keys)
+
+        # Get the intersection of the unique keys
+
+        # Filter the rows in df1 and df2 that match the intersection of the unique keys
+        df1_intersection = initial_df[initial_df[unique_key].isin(
+            intersection_keys)].reset_index(drop=True)
+        df2_intersection = final_df[final_df[unique_key].isin(
+            intersection_keys)].reset_index(drop=True)
+
+        diff = df1_intersection.compare(df2_intersection)
+
+        modifications = diff.__len__()
+
+        # Construct the result text
+        result = ""
+        if additions > 0:
+            result += f"- 🆕 {additions} addition{'s' if additions > 1 else ''}\n"
+        else:
+            result += f"- ~~🆕 0 addition~~\n"
+        if modifications > 0:
+            result += f"- ♻️ {modifications} modification{'s' if modifications > 1 else ''}\n"
+        else:
+            result += f"- ~~♻️ 0 modification~~\n"
+        if deletions > 0:
+            result += f"- 🗑️ {deletions} deletion{'s' if deletions > 1 else ''}\n"
+        else:
+            result += f"- ~~🗑️ 0 deletion~~\n"
+
+        return result.strip()
+    except Exception as e:
+        return f"Could not generate drift description: {e}"
```

### Comparing `datagit-0.7/datagit/github_connector.py` & `datagit-0.8/datagit/github_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,28 +40,31 @@
             except KeyError:
                 old_dates = []
             new_dates = set(dataframe[date_column])
             already_stored_dates = new_dates.intersection(old_dates)
             new_dataframe = dataframe[~dataframe[date_column].isin(
                 already_stored_dates)]
             old_data_with_freshdata = pd.concat(
-                [old_dataframe, new_dataframe])
+                [old_dataframe, new_dataframe]).reset_index(drop=True)
             if len(new_dataframe) > 0:
                 print("New data found")
                 push_new_lines(
                     file_path, repo, reported_branch, old_data_with_freshdata, store_json)
             checkout_branch_from_default_branch(repo, computed_branch)
-            if not old_data_with_freshdata.equals(dataframe):
+
+            if not old_data_with_freshdata.equals(dataframe.reset_index(drop=True)):
                 print("Drift detected")
+
                 push_drift_lines(file_path, repo, computed_branch,
                                  dataframe, store_json)
                 print("Drift pushed")
                 print("Creating pull request")
                 description_body = f"Drift detected:\n" + \
-                    compare_dataframes(old_data_with_freshdata, dataframe, "unique_key")
+                    compare_dataframes(old_data_with_freshdata,
+                                       dataframe, "unique_key")
                 create_pullrequest(repo, computed_branch,
                                    assignees, file_path, description_body)
 
     pass
 
 
 def assert_file_exists(repo: Repository.Repository, file_path: str, ref: str) -> Optional[ContentFile.ContentFile]:
```

### Comparing `datagit-0.7/datagit/query_builder.py` & `datagit-0.8/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.7/datagit.egg-info/PKG-INFO` & `datagit-0.8/datagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.7
+Version: 0.8
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.7/setup.py` & `datagit-0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.7",
+    version="0.8",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/data-drift/datagit",
```

