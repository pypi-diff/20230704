# Comparing `tmp/gdsync666-0.0.1.tar.gz` & `tmp/gdsync666-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsync666-0.0.1.tar", last modified: Sat Jun 17 21:29:50 2023, max compression
+gzip compressed data, was "gdsync666-0.0.2.tar", last modified: Tue Jul  4 09:46:12 2023, max compression
```

## Comparing `gdsync666-0.0.1.tar` & `gdsync666-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-06-17 21:29:50.666284 gdsync666-0.0.1/
--rw-r--r--   0 daniil.chalov   (502) staff       (20)     1072 2023-06-17 21:03:56.000000 gdsync666-0.0.1/LICENSE
--rw-r--r--   0 daniil.chalov   (502) staff       (20)     2829 2023-06-17 21:29:50.666002 gdsync666-0.0.1/PKG-INFO
--rw-r--r--   0 daniil.chalov   (502) staff       (20)      863 2023-06-17 21:28:45.000000 gdsync666-0.0.1/README.md
--rw-r--r--   0 daniil.chalov   (502) staff       (20)     1032 2023-06-17 21:29:05.000000 gdsync666-0.0.1/pyproject.toml
--rw-r--r--   0 daniil.chalov   (502) staff       (20)       38 2023-06-17 21:29:50.666356 gdsync666-0.0.1/setup.cfg
-drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-06-17 21:29:50.659640 gdsync666-0.0.1/src/
-drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-06-17 21:29:50.664025 gdsync666-0.0.1/src/gdsync666.egg-info/
--rw-r--r--   0 daniil.chalov   (502) staff       (20)     2829 2023-06-17 21:29:50.000000 gdsync666-0.0.1/src/gdsync666.egg-info/PKG-INFO
--rw-r--r--   0 daniil.chalov   (502) staff       (20)      316 2023-06-17 21:29:50.000000 gdsync666-0.0.1/src/gdsync666.egg-info/SOURCES.txt
--rw-r--r--   0 daniil.chalov   (502) staff       (20)        1 2023-06-17 21:29:50.000000 gdsync666-0.0.1/src/gdsync666.egg-info/dependency_links.txt
--rw-r--r--   0 daniil.chalov   (502) staff       (20)      125 2023-06-17 21:29:50.000000 gdsync666-0.0.1/src/gdsync666.egg-info/requires.txt
--rw-r--r--   0 daniil.chalov   (502) staff       (20)       18 2023-06-17 21:29:50.000000 gdsync666-0.0.1/src/gdsync666.egg-info/top_level.txt
-drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-06-17 21:29:50.665592 gdsync666-0.0.1/src/google_drive_sync/
--rw-r--r--   0 daniil.chalov   (502) staff       (20)       90 2023-06-17 21:03:56.000000 gdsync666-0.0.1/src/google_drive_sync/__init__.py
--rw-r--r--   0 daniil.chalov   (502) staff       (20)    12060 2023-06-17 21:03:56.000000 gdsync666-0.0.1/src/google_drive_sync/download.py
--rw-r--r--   0 daniil.chalov   (502) staff       (20)    13520 2023-06-17 21:03:56.000000 gdsync666-0.0.1/src/google_drive_sync/upload.py
+drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-07-04 09:46:12.184061 gdsync666-0.0.2/
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)     1072 2023-07-04 09:43:58.000000 gdsync666-0.0.2/LICENSE
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)     2829 2023-07-04 09:46:12.183767 gdsync666-0.0.2/PKG-INFO
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)      863 2023-07-04 09:43:58.000000 gdsync666-0.0.2/README.md
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)     1032 2023-07-04 09:45:47.000000 gdsync666-0.0.2/pyproject.toml
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)       38 2023-07-04 09:46:12.184183 gdsync666-0.0.2/setup.cfg
+drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-07-04 09:46:12.178995 gdsync666-0.0.2/src/
+drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-07-04 09:46:12.182149 gdsync666-0.0.2/src/gdsync666.egg-info/
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)     2829 2023-07-04 09:46:12.000000 gdsync666-0.0.2/src/gdsync666.egg-info/PKG-INFO
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)      316 2023-07-04 09:46:12.000000 gdsync666-0.0.2/src/gdsync666.egg-info/SOURCES.txt
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)        1 2023-07-04 09:46:12.000000 gdsync666-0.0.2/src/gdsync666.egg-info/dependency_links.txt
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)      125 2023-07-04 09:46:12.000000 gdsync666-0.0.2/src/gdsync666.egg-info/requires.txt
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)       18 2023-07-04 09:46:12.000000 gdsync666-0.0.2/src/gdsync666.egg-info/top_level.txt
+drwxr-xr-x   0 daniil.chalov   (502) staff       (20)        0 2023-07-04 09:46:12.183359 gdsync666-0.0.2/src/google_drive_sync/
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)       92 2023-07-04 09:44:08.000000 gdsync666-0.0.2/src/google_drive_sync/__init__.py
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)    12171 2023-07-04 09:44:08.000000 gdsync666-0.0.2/src/google_drive_sync/download.py
+-rw-r--r--   0 daniil.chalov   (502) staff       (20)    13353 2023-07-04 09:44:08.000000 gdsync666-0.0.2/src/google_drive_sync/upload.py
```

### Comparing `gdsync666-0.0.1/LICENSE` & `gdsync666-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsync666-0.0.1/PKG-INFO` & `gdsync666-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsync666
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bidirectionally sync your local folder with a one from Google Drive
 Author-email: Daniil Chalov <cyber.barrista@gmail.com>
 License: Copyright (c) 2012-2023 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `gdsync666-0.0.1/README.md` & `gdsync666-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gdsync666-0.0.1/pyproject.toml` & `gdsync666-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdsync666"
-version = "0.0.1"
+version = "0.0.2"
 description = "Bidirectionally sync your local folder with a one from Google Drive"
 readme = "README.md"
 authors = [{ name = "Daniil Chalov", email = "cyber.barrista@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `gdsync666-0.0.1/src/gdsync666.egg-info/PKG-INFO` & `gdsync666-0.0.2/src/gdsync666.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsync666
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bidirectionally sync your local folder with a one from Google Drive
 Author-email: Daniil Chalov <cyber.barrista@gmail.com>
 License: Copyright (c) 2012-2023 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `gdsync666-0.0.1/src/google_drive_sync/download.py` & `gdsync666-0.0.2/src/google_drive_sync/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import os
 import shutil
 import time
 import hashlib
 
 from apiclient import discovery
 from google.oauth2.credentials import Credentials
-from google_auth_httplib2 import Request
+from google.auth.transport.requests import Request
 from google_auth_oauthlib.flow import InstalledAppFlow
-from googleapiclient.http import MediaIoBaseDownload, MediaFileUpload
+from googleapiclient.http import MediaIoBaseDownload
 
 SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly',
           'https://www.googleapis.com/auth/drive.file',
           'https://www.googleapis.com/auth/drive']
 
 GOOGLE_MIME_TYPES = {
     'application/vnd.google-apps.document':
@@ -201,16 +201,17 @@
 
 def download(creds_file: str, local_folder: str, remote_folder: str):
     """Shows basic usage of the Google Drive API.
 
     Creates a Google Drive API service object and outputs the names and IDs
     for up to 10 files.
     """
-    credentials = get_credentials(creds_file, '../../token.json')
+    credentials = get_credentials(creds_file, 'token.json')
     service = discovery.build('drive', 'v3', credentials=credentials)
+    service._http.timeout = 10000  # Set the timeout value (in seconds)
 
     # Get id of Google Drive folder and it's path (from other script)
     # folder_id, full_path = initial_upload.check_upload(service)
     folder_id, full_path = check_upload(service, local_folder, remote_folder)
     folder_name = full_path.split(os.path.sep)[-1]
     tree_list, root, parents_id = [], '', {}
 
@@ -245,15 +246,15 @@
 
     for folder_dir in download_folders:
         variable = var + folder_dir
         last_dir = folder_dir.split(os.path.sep)[-1]
 
         folder_id = parents_id[last_dir]
         results = service.files().list(
-            pageSize=20, q=('%r in parents' % folder_id)).execute()
+            pageSize=20, q=('%r in parents and trashed = false' % folder_id)).execute()
 
         items = results.get('files', [])
         os.makedirs(variable)
         files = [f for f in items
                  if f['mimeType'] != 'application/vnd.google-apps.folder']
 
         for drive_file in files:
@@ -268,15 +269,15 @@
         os_files = [f for f in os.listdir(variable)
                     if os.path.isfile(os.path.join(variable, f))]
         folder_id = parents_id[last_dir]
 
         results = service.files().list(
             pageSize=1000,
             q=('%r in parents and \
-            mimeType!="application/vnd.google-apps.folder"' % folder_id),
+            mimeType!="application/vnd.google-apps.folder" and trashed = false' % folder_id),
             fields="files(id, name, mimeType, \
                 modifiedTime, md5Checksum)").execute()
 
         items = results.get('files', [])
 
         refresh_files = [f for f in items if f['name'] in os_files]
         upload_files = [f for f in items if f['name'] not in os_files]
@@ -307,14 +308,14 @@
         for os_file in remove_files:
             os.remove(os.path.join(variable, os_file))
 
         for drive_file in upload_files:
             download_file_from_gdrive(variable, drive_file, service)
 
     # Delete old and unwanted folders from computer
-    remove_folders = sorted(remove_folders, key=by_lines, reverse=True)
+    # remove_folders = sorted(remove_folders, key=by_lines, reverse=True)
 
-    for folder_dir in remove_folders:
-        # var = '/'.join(full_path.split('/')[0:-1]) + '/'
-        variable = var + folder_dir
-        last_dir = folder_dir.split(os.path.sep)[-1]
-        shutil.rmtree(variable)
+    # for folder_dir in remove_folders:
+    #     # var = '/'.join(full_path.split('/')[0:-1]) + '/'
+    #     variable = var + folder_dir
+    #     last_dir = folder_dir.split(os.path.sep)[-1]
+    #     shutil.rmtree(variable)
```

### Comparing `gdsync666-0.0.1/src/google_drive_sync/upload.py` & `gdsync666-0.0.2/src/google_drive_sync/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import hashlib
 import mimetypes
 import time
 import os
 
 from apiclient import discovery
-from google_auth_httplib2 import Request
+from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.http import MediaFileUpload
 
 SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly',
           'https://www.googleapis.com/auth/drive.file',
@@ -78,15 +78,15 @@
     Returns:
         ID of uploaded folder, full path to this folder on computer.
 
     """
 
     results = service.files().list(
         pageSize=100,
-        q="'root' in parents and trashed != True and \
+        q="trashed = false and \
         mimeType='application/vnd.google-apps.folder'").execute()
 
     items = results.get('files', [])
 
     # Check if folder exists, and then create it or get this folder's id.
     if remote_folder in [item['name'] for item in items]:
         folder_id = [item['id'] for item in items
@@ -111,15 +111,15 @@
     # The file token.json stores the user's access and refresh tokens, and is
     # created automatically when the authorization flow completes for the first
     # time.
     if os.path.exists(token_file):
         creds = Credentials.from_authorized_user_file(token_file, SCOPES)
     # If there are no (valid) credentials available, let the user log in.
     if not creds or not creds.valid:
-        if creds and creds.expired and creds.refresh_token:
+        if False:  # creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
             flow = InstalledAppFlow.from_client_secrets_file(
                 creds_file, SCOPES)
             creds = flow.run_local_server(port=0)
         # Save the credentials for the next run
         with open(token_file, 'w') as token:
@@ -180,17 +180,17 @@
 
 def upload(creds_file: str, local_folder: str, remote_folder: str):
     """Syncronizes computer folder with Google Drive folder.
 
     Checks files if they exist, uploads new files and subfolders,
     deletes old files from Google Drive and refreshes existing stuff.
     """
-    credentials = get_credentials()
+    credentials = get_credentials(creds_file, 'token.json')
     service = discovery.build('drive', 'v3', credentials=credentials)
-    service._http.timeout = 500
+    service._http.timeout = 10000  # Set the timeout value (in seconds)
 
     # Get id of Google Drive folder and it's path (from other script)
     # folder_id, full_path = initial_upload.check_upload(service)
     folder_id, full_path = check_upload(service, local_folder, remote_folder)
     folder_name = full_path.split(os.path.sep)[-1]
     tree_list = []
     root = ''
@@ -205,29 +205,29 @@
     for root, dirs, files in os.walk(full_path, topdown=True):
         for name in dirs:
             var_path = (os.path.sep).join(
                 root.split(os.path.sep)[root_len + 1:])
             os_tree_list.append(os.path.join(var_path, name))
 
     # old folders on drive
-    remove_folders = list(set(tree_list).difference(set(os_tree_list)))
+    # remove_folders = list(set(tree_list).difference(set(os_tree_list)))
     # new folders on drive, which you dont have(i suppose hehe)
     upload_folders = list(set(os_tree_list).difference(set(tree_list)))
     # foldes that match
     exact_folders = list(set(os_tree_list).intersection(set(tree_list)))
 
     # Add starting directory
     exact_folders.append(folder_name)
     # Sort uploadable folders
     # so now in can be upload from top to down of tree
     upload_folders = sorted(upload_folders, key=by_lines)
 
     # Here we upload new (abcent on Drive) folders
     for folder_dir in upload_folders:
-        var = os.path.join(full_path.split(os.path.sep)[0:-1]) + os.path.sep
+        var = os.path.join(*full_path.split(os.path.sep)[0:-1]) + os.path.sep
         variable = var + folder_dir
         last_dir = folder_dir.split(os.path.sep)[-1]
         pre_last_dir = folder_dir.split(os.path.sep)[-2]
 
         files = [f for f in os.listdir(variable)
                  if os.path.isfile(os.path.join(variable, f))]
 
@@ -312,37 +312,31 @@
                 # media_body = MediaFileUpload(file_dir, mimetype=filemime)
                 media_body = MediaFileUpload(file_dir, mimetype=file_mime)
                 # print('I am HERE, ', )
                 service.files().update(fileId=file_id,
                                        media_body=media_body,
                                        fields='id').execute()
 
-        # Remove old files from Drive
-        for drive_file in remove_files:
-            file_id = [f['id'] for f in items
-                       if f['name'] == drive_file['name']][0]
-            service.files().delete(fileId=file_id).execute()
-
         # Upload new files on Drive
         for os_file in upload_files:
             file_dir = os.path.join(variable, os_file)
 
             # File's new content.
             filemime = mimetypes.MimeTypes().guess_type(file_dir)[0]
             file_metadata = {'name': os_file,
                              'parents': [parents_id[last_dir]]}
             media_body = MediaFileUpload(file_dir, mimetype=filemime)
 
             service.files().create(body=file_metadata,
                                    media_body=media_body,
                                    fields='id').execute()
 
-    remove_folders = sorted(remove_folders, key=by_lines, reverse=True)
+    # remove_folders = sorted(remove_folders, key=by_lines, reverse=True)
 
     # Delete old folders from Drive
-    for folder_dir in remove_folders:
-        var = (os.path.sep).join(full_path.split(
-            os.path.sep)[0:-1]) + os.path.sep
-        variable = var + folder_dir
-        last_dir = folder_dir.split('/')[-1]
-        folder_id = parents_id[last_dir]
-        service.files().delete(fileId=folder_id).execute()
+    # for folder_dir in remove_folders:
+    #     var = (os.path.sep).join(full_path.split(
+    #         os.path.sep)[0:-1]) + os.path.sep
+    #     variable = var + folder_dir
+    #     last_dir = folder_dir.split('/')[-1]
+    #     folder_id = parents_id[last_dir]
+    #     service.files().delete(fileId=folder_id).execute()
```

