# Comparing `tmp/django_cloud_storages-1.1.6.tar.gz` & `tmp/django_cloud_storages-1.1.7.tar.gz`

## Comparing `django_cloud_storages-1.1.6.tar` & `django_cloud_storages-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/.readthedocs.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/cloud_storages/__init__.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/README.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/.readthedocs.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0    10464 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/README.md
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.6/.readthedocs.yaml` & `django_cloud_storages-1.1.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.6/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.7/cloud_storages/backends/appwrite.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,22 +49,15 @@
         folder, filename = self.extract_folder_and_filename(name)
         try:
             response = self.storage.get_file_view(folder, filename)
             file_content = BytesIO(response)
             response_file = File(file_content, name=name)
             return response_file
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
     
     def save(self, name, content, max_length=None):
         """
         Save new content to the file specified by name. The content should be
         a proper File object or any Python file-like object, ready to be read
         from the beginning.
         """
@@ -186,23 +179,17 @@
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.delete_file(folder, filename)
+            return result
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
 
     def exists(self, name):
         """
         Return True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
         """
         folder, filename = self.extract_folder_and_filename(name)
@@ -227,22 +214,15 @@
         Return the total size, in bytes, of the file specified by name.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.get_file(folder, filename)
             return result.sizeOriginal
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
     
     def url(self, name, permanent_link=None):
         """
         Return an absolute URL where the file's contents can be accessed directly by a web browser.
         """
         folder, filename = self.extract_folder_and_filename(name)
         file_url = f"{self.APPWRITE_API_ENDPOINT}/storage/buckets/{folder}/files/{filename}/view?project={self.APPWRITE_PROJECT_ID}"
@@ -254,53 +234,32 @@
         The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.get_file(folder, filename)
             return result.updatedAt
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
 
     def get_created_time(self, name):
         """
         Return the creation time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.get_file(folder, filename)
             return result.createdAt
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
     
     def get_modified_time(self, name):
         """
         Return the last modified time (as a datetime) of the file specified by
         name. The datetime will be timezone-aware if USE_TZ=True.
         """
         folder, filename = self.extract_folder_and_filename(name)
         try:
             result = self.storage.get_file(folder, filename)
             return result.updatedAt
         except AppwriteException as e:
-            if str(e) == "Storage bucket with the requested ID could not be found.":
-                error_msg = f"The folder does not exists on the cloud storage.\nFolder Name: {folder}."
-                raise ContentDoesNotExistsError(error_msg)
-            elif str(e) == "The requested file could not be found.":
-                error_msg = f"The file does not exists on the cloud storage.\nFile Name: {filename}."
-                raise ContentDoesNotExistsError(error_msg)
-            else:
-                raise e
+            throwAppwriteException(e, folder, filename)
```

### Comparing `django_cloud_storages-1.1.6/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.7/cloud_storages/backends/dropbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,20 +54,15 @@
         full_name = self._full_path(name)
         try:
             file_metadata, response = self.dbx.files_download(full_name)
             file_content = BytesIO(response.content)
             response_file = File(file_content, name=name)
             return response_file
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
            
         
     def save(self, name, content, max_length=None):
         """
         Save new content to the file specified by name. The content should be
         a proper File object or any Python file-like object, ready to be read
         from the beginning.
@@ -152,29 +147,25 @@
         """
         Delete the specified file from the storage system.
         """
         full_name = self._full_path(name)
         try:
             self.dbx.files_delete_v2(full_name)
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
                 
     def exists(self, name):
         """
         Return True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
         """
         full_name = self._full_path(name)
         try:
-            return bool(self.dbx.files_get_metadata(full_name))
+            self.dbx.files_get_metadata(full_name)
+            return True
         except ApiError as e:
             err = e.error
             if err.is_path_lookup():
                 # lookUpError = err.get_path_lookup()
                 # error_msg = dropBoxErrorMsg(lookUpError._tag)
                 return False
             raise e
@@ -198,20 +189,15 @@
         Return the total size, in bytes, of the file specified by name.
         """
         full_name = self._full_path(name)
         try:
             metadata = self.dbx.files_get_metadata(full_name)
             return metadata.size
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
 
     def url(self, name, permanent_link=DROPBOX_PERMANENT_LINK):
         """
         Return an absolute URL where the file's contents can be accessed directly by a web browser.
         """
         full_name = self._full_path(name)
         try:
@@ -232,54 +218,39 @@
         The datetime will be timezone-aware if USE_TZ=True.
         """
         full_name = self._full_path(name)
         try:
             last_accessed = self.dbx.files_get_metadata(full_name).client_modified
             return last_accessed
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
 
     def get_created_time(self, name):
         """
         Return the creation time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         full_name = self._full_path(name)
         try:
             created_at = self.dbx.files_get_metadata(full_name).client_modified
             return created_at
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
 
     def get_modified_time(self, name):
         """
         Return the last modified time (as a datetime) of the file specified by
         name. The datetime will be timezone-aware if USE_TZ=True.
         """
         full_name = self._full_path(name)
         try:
             last_modified = self.dbx.files_get_metadata(full_name).server_modified
             return last_modified
         except ApiError as e:
-            err = e.error
-            if err.is_path_lookup():
-                lookUpError = err.get_path_lookup()
-                error_msg = dropBoxErrorMsg(lookUpError._tag)
-                raise ContentDoesNotExistsError(error_msg)
-            raise e
+            throwDropboxException(e)
                 
     def _chunked_upload(self, content, dest_path):
         upload_session = self.dbx.files_upload_session_start(content.read(self.CHUNK_SIZE))
         cursor = UploadSessionCursor(session_id=upload_session.session_id, offset=content.tell())
         commit = CommitInfo(path=dest_path, mode=WriteMode(self.write_mode))
         while content.tell() < content.size:
             if (content.size - content.tell()) <= self.CHUNK_SIZE:
```

### Comparing `django_cloud_storages-1.1.6/.gitignore` & `django_cloud_storages-1.1.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -153,8 +153,9 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
+.vscode/
```

### Comparing `django_cloud_storages-1.1.6/LICENSE` & `django_cloud_storages-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.6/README.md` & `django_cloud_storages-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.6/pyproject.toml` & `django_cloud_storages-1.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 [project]
 name = "django-cloud-storages"
 dynamic = ["version"]
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
+maintainers = [
+  { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
+]
+keywords = ["django", "python", "django-storages", "django-file-storages", "cloud storage", "file storage", "django dropbox"]
 description = "Cloud file storages for django."
 dependencies = ["django", "requests", "dropbox", "appwrite"]
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django_cloud_storages-1.1.6/PKG-INFO` & `django_cloud_storages-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.1.6
+Version: 1.1.7
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://pypi.org/project/django-cloud-storages
 Project-URL: Source code, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
+Maintainer-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: cloud storage,django,django dropbox,django-file-storages,django-storages,file storage,python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

