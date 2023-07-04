# Comparing `tmp/sync_dl_ytapi-1.1.0-py3-none-any.whl.zip` & `tmp/sync_dl_ytapi-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9387 bytes, number of entries: 10
--rw-r--r--  2.0 unx       95 b- defN 22-Feb-01 00:29 sync_dl_ytapi/__init__.py
+Zip file size: 9523 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-04 17:23 sync_dl_ytapi/__init__.py
 -rw-r--r--  2.0 unx     2147 b- defN 22-Feb-03 02:14 sync_dl_ytapi/commands.py
 -rw-r--r--  2.0 unx     2970 b- defN 22-Feb-03 02:16 sync_dl_ytapi/credentials.py
--rw-r--r--  2.0 unx     6464 b- defN 22-Feb-03 02:15 sync_dl_ytapi/helpers.py
+-rw-r--r--  2.0 unx     6471 b- defN 23-Jul-04 17:22 sync_dl_ytapi/helpers.py
 -rw-r--r--  2.0 unx     6262 b- defN 22-Feb-03 02:26 sync_dl_ytapi/ytapiWrappers.py
--rw-r--r--  2.0 unx     1072 b- defN 22-Feb-03 10:22 sync_dl_ytapi-1.1.0.dist-info/LICENCE
--rw-r--r--  2.0 unx     2633 b- defN 22-Feb-03 10:22 sync_dl_ytapi-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-03 10:22 sync_dl_ytapi-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-Feb-03 10:22 sync_dl_ytapi-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      831 b- defN 22-Feb-03 10:22 sync_dl_ytapi-1.1.0.dist-info/RECORD
-10 files, 22580 bytes uncompressed, 7963 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/LICENCE
+-rw-r--r--  2.0 unx     2994 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      831 b- defN 23-Jul-04 17:47 sync_dl_ytapi-1.1.1.dist-info/RECORD
+10 files, 22948 bytes uncompressed, 8099 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sync_dl_ytapi/helpers.py
 Comment: 
 
 Filename: sync_dl_ytapi/ytapiWrappers.py
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.0.dist-info/LICENCE
+Filename: sync_dl_ytapi-1.1.1.dist-info/LICENCE
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.0.dist-info/METADATA
+Filename: sync_dl_ytapi-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.0.dist-info/WHEEL
+Filename: sync_dl_ytapi-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.0.dist-info/top_level.txt
+Filename: sync_dl_ytapi-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sync_dl_ytapi-1.1.0.dist-info/RECORD
+Filename: sync_dl_ytapi-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sync_dl_ytapi/__init__.py

```diff
@@ -1,2 +1,2 @@
 # This submodule extends sync_dl with tools for editing remote playlists
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

## sync_dl_ytapi/helpers.py

```diff
@@ -18,16 +18,16 @@
     
     blankingStr = ''
     localIds = [localId for localId in localIds]
     remoteIds = [remoteId for remoteId in remoteIds]
 
 
     # Removes all localIds which arent in remoteIds (we arent going to upload songs)
-    for i,localId in enumerate(localIds):
-        if localId not in remoteIds:
+    for i in reversed(range(len(localIds))):
+        if localIds[i] not in remoteIds:
             del localIds[i]
 
     lenRemote = len(remoteIds)
     oldToNew=[-1]*lenRemote
 
     prevOldIndex = -1
     newIndex = 0
```

## Comparing `sync_dl_ytapi-1.1.0.dist-info/LICENCE` & `sync_dl_ytapi-1.1.1.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `sync_dl_ytapi-1.1.0.dist-info/METADATA` & `sync_dl_ytapi-1.1.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sync-dl-ytapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: An addon for sync-dl, providing commands which utilize the youtube api
 Home-page: https://github.com/PrinceOfPuppers/sync-dl-ytapi
 Author: Joshua McPherson
 Author-email: joshuamcpherson5@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -42,43 +40,53 @@
 ```
 pip install sync-dl
 ```
 Using any commands in sync-dl which require this addon will prompt the user to install this addon.
 
 
 # ABOUT
-Provides the --push-order option to sync-dl (along with potentially more in the future)
+Provides sync-dl the ability to edit remote playlists on youtube through the youtube-api
 
 
 # Usage
+## Push Order Command:
 ```
-sync-dl --push-order PLAYLIST
+sync-dl ytapi --push-order PLAYLIST
 ```
 This will prompt you to install sync-dl-ytapi if you have not already, and will
 print out the url to log in with google. Once you have done this it will
 push the local order of PLAYLIST to youtube, reordering songs to match the local order (songs in remote but not in local will always stay after what they are currently after)
 
 PLAYLIST is simply the name of the directory which contains the playlist. playlist directory will always be in current working directory unless a music directory is specified using the -l, --local-dir option to hard set a music directory.
 
 You can also logout (revoke the access tokens and delete the saved credentials) using
 the following command
 ```
-sync-dl --logout
+sync-dl ytapi --logout
 ```
 
 To see all options use the command:
 ```
-sync-dl -h
+sync-dl ytapi -h
+```
+
+## Transfer Command:
+```
+sync-dl ytapi transfer [OPTINOS] SRC_PLAYLIST DEST_PLAYLIST
+```
+Transfers songs between `SRC_PLAYLIST` and `DEST_PLAYLIST` on both local and remote, moving a single song using `-t SI DI` or a range of songs `-r S1 S2 DI`
+
+To see all options as well as a more indepth description use the command:
+```
+sync-dl ytapi transfer -h
 ```
 
 # DEVLOPMENT
 To build for devlopment run:
 ```
 git clone https://github.com/PrinceOfPuppers/sync-dl-ytapi.git
 
 cd sync-dl-ytapi
 
 pip install -e .
 ```
 This will build and install sync-dl in place, allowing you to work on the code without having to reinstall after changes, it will also install sync-dl as it is a dependancy
-
-
```

