# Comparing `tmp/sync_dl-2.3.5-py3-none-any.whl.zip` & `tmp/sync_dl-2.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,24 @@
-Zip file size: 34562 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1495 b- defN 22-Oct-30 03:59 sync_dl/__init__.py
--rw-r--r--  2.0 unx    20284 b- defN 22-Oct-30 04:00 sync_dl/cli.py
--rw-r--r--  2.0 unx    23946 b- defN 22-Oct-30 04:02 sync_dl/commands.py
+Zip file size: 37712 bytes, number of entries: 22
+-rw-r--r--  2.0 unx     1495 b- defN 23-Feb-24 22:32 sync_dl/__init__.py
+-rw-r--r--  2.0 unx    20221 b- defN 22-Nov-03 00:06 sync_dl/cli.py
+-rw-r--r--  2.0 unx    23946 b- defN 23-Feb-06 23:25 sync_dl/commands.py
 -rw-r--r--  2.0 unx     4395 b- defN 22-Oct-30 04:02 sync_dl/config.py
--rw-r--r--  2.0 unx    15243 b- defN 22-Oct-30 04:02 sync_dl/helpers.py
--rw-r--r--  2.0 unx     7797 b- defN 22-Oct-30 04:02 sync_dl/plManagement.py
--rw-r--r--  2.0 unx     9650 b- defN 22-Oct-30 04:02 sync_dl/ytapiInterface.py
--rw-r--r--  2.0 unx     3631 b- defN 22-Oct-30 04:02 sync_dl/ytdlWrappers.py
--rw-r--r--  2.0 unx     4706 b- defN 22-Oct-30 04:00 sync_dl/timestamps/__init__.py
--rw-r--r--  2.0 unx     7441 b- defN 22-Oct-30 04:00 sync_dl/timestamps/scraping.py
+-rw-r--r--  2.0 unx    15013 b- defN 22-Nov-03 00:06 sync_dl/helpers.py
+-rw-r--r--  2.0 unx     7797 b- defN 23-Feb-06 23:25 sync_dl/plManagement.py
+-rw-r--r--  2.0 unx     8573 b- defN 23-Jul-04 17:35 sync_dl/ytapiInterface.py
+-rw-r--r--  2.0 unx     4730 b- defN 23-Feb-24 22:35 sync_dl/ytdlWrappers.py
+-rw-r--r--  2.0 unx     1253 b- defN 23-Jul-04 17:33 sync_dl/config/__init__.py
+-rw-r--r--  2.0 unx     1284 b- defN 22-Nov-03 00:06 sync_dl/config/parsing.py
+-rw-r--r--  2.0 unx     1910 b- defN 22-Nov-03 00:06 sync_dl/config/tmpdir.py
+-rw-r--r--  2.0 unx     2335 b- defN 22-Nov-03 00:06 sync_dl/config/ytdlParams.py
+-rw-r--r--  2.0 unx     5347 b- defN 22-Nov-03 00:06 sync_dl/timestamps/__init__.py
+-rw-r--r--  2.0 unx     7452 b- defN 22-Nov-03 00:06 sync_dl/timestamps/scraping.py
 -rw-r--r--  2.0 unx     3773 b- defN 22-Feb-15 09:51 sync_dl/timestamps/timestamps.py
--rwxr-xr-x  2.0 unx       76 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.data/scripts/sync-dl
--rw-r--r--  2.0 unx     1072 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/LICENCE
--rw-r--r--  2.0 unx     5990 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1449 b- defN 22-Oct-30 04:16 sync_dl-2.3.5.dist-info/RECORD
-18 files, 111089 bytes uncompressed, 32206 bytes compressed:  71.0%
+-rwxr-xr-x  2.0 unx       76 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.data/scripts/sync-dl
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/LICENCE
+-rw-r--r--  2.0 unx     5968 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1780 b- defN 23-Jul-04 18:07 sync_dl-2.3.7.dist-info/RECORD
+22 files, 118561 bytes uncompressed, 34846 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -18,38 +18,50 @@
 
 Filename: sync_dl/ytapiInterface.py
 Comment: 
 
 Filename: sync_dl/ytdlWrappers.py
 Comment: 
 
+Filename: sync_dl/config/__init__.py
+Comment: 
+
+Filename: sync_dl/config/parsing.py
+Comment: 
+
+Filename: sync_dl/config/tmpdir.py
+Comment: 
+
+Filename: sync_dl/config/ytdlParams.py
+Comment: 
+
 Filename: sync_dl/timestamps/__init__.py
 Comment: 
 
 Filename: sync_dl/timestamps/scraping.py
 Comment: 
 
 Filename: sync_dl/timestamps/timestamps.py
 Comment: 
 
-Filename: sync_dl-2.3.5.data/scripts/sync-dl
+Filename: sync_dl-2.3.7.data/scripts/sync-dl
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/LICENCE
+Filename: sync_dl-2.3.7.dist-info/LICENCE
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/METADATA
+Filename: sync_dl-2.3.7.dist-info/METADATA
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/WHEEL
+Filename: sync_dl-2.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/entry_points.txt
+Filename: sync_dl-2.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/top_level.txt
+Filename: sync_dl-2.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: sync_dl-2.3.5.dist-info/RECORD
+Filename: sync_dl-2.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sync_dl/__init__.py

```diff
@@ -1,13 +1,13 @@
 
 from threading import current_thread
 from sync_dl import config as cfg
 from signal import signal, SIGINT, Signals#,SIGABRT,SIGTERM
 
-__version__ = "2.3.5"
+__version__ = "2.3.7"
 
 class InterruptTriggered(Exception):
     pass
 
 class _NoInterrupt:
     noInterruptDepth = 0
     signalReceived=False
```

## sync_dl/cli.py

```diff
@@ -251,26 +251,24 @@
             else:
                 cfg.logger.info(cfg.musicDir)
             return
 
         # reset musicDir to relative pathing
         if args.local_dir == '':
             cfg.writeToConfig('musicDir','')
-            cfg.musicDir = ''
 
         #set music dir to args.local_dir
         else:
             if not os.path.exists(args.local_dir):
                 cfg.logger.error("Provided Music Directory Does not Exist")
                 return
             #saves args.local_dir to config
             music = os.path.abspath(args.local_dir)
 
             cfg.writeToConfig('musicDir',music)
-            cfg.musicDir = music
 
     if args.audio_format:
         if args.audio_format == '\n':
             cfg.logger.info(cfg.audioFormat)
             return
         fmt = args.audio_format.lower()
         if fmt not in cfg.knownFormats:
```

## sync_dl/helpers.py

```diff
@@ -444,15 +444,7 @@
 
 
     cfg.logger.info(f"\n------------[Note]-----------")
     cfg.logger.info(f"For Best Remote Playlists Results, Ensure Local and Remote Playlists are Synced")
     cfg.logger.info(f"(failing to do so may lead to ordering changes in remote if there are duplicate songs)")
 
 
-def clearTmpDownloadPath():
-    if not os.path.exists(cfg.tmpDownloadPath):
-        os.mkdir(cfg.tmpDownloadPath)
-        return
-
-    for f in os.listdir(path=cfg.tmpDownloadPath):
-        os.remove(f"{cfg.tmpDownloadPath}/{f}")
-
```

## sync_dl/ytapiInterface.py

```diff
@@ -4,62 +4,21 @@
 
 from sync_dl import noInterrupt
 from sync_dl.ytdlWrappers import getIDs
 from sync_dl.plManagement import correctStateCorruption
 from sync_dl.helpers import getLocalSongs, relabel, getNumDigets, copy, delete, padZeros, calcuateTransferMoves, logTransferInfo, promptAndSanitize
 import sync_dl.config as cfg
 
-_sync_dl_api_installed = False
-
-def promptInstall():
-    global _sync_dl_api_installed
-
-    if _sync_dl_api_installed:
-        return True
-
-    try:
-        from sync_dl_ytapi.commands import pushLocalOrder, logout, getPlAdder, getPlRemover
-    except:
-
-        answer = input("Missing Optional Dependancies For This Command.\nWould You Like to Install Them? (y)es/(n)o: ").lower().strip()
-        if answer!='y':
-            return False
-
-        try:
-            import subprocess
-            subprocess.run(["pip","install", '-U','sync-dl-ytapi'],check=True)
-        except:
-            cfg.logger.error("Unable to Install Optional Dependancies")
-            return False
-        cfg.logger.info("Optional Dependancies Installed")
-
-        _sync_dl_api_installed = True
-        cfg.logger.info("----------------------------------")
-
-    _sync_dl_api_installed = True
-    return True
-
 
 def pushLocalOrder(plPath):
-
-    installed = promptInstall()
-
-    if not installed:
-        return
-
     from sync_dl_ytapi.commands import pushLocalOrder
     pushLocalOrder(plPath)
 
 
 def logout():
-    installed = promptInstall()
-
-    if not installed:
-        return
-
     from sync_dl_ytapi.commands import logout
     logout()
 
 
 def transferSongs(srcPlPath: str, destPlPath: str, srcStart: int, srcEnd: int, destIndex: int):
     '''
     transfers block of songs in srcPl from srcStart to srcEnd indices, to after destIndex in destPl
@@ -67,19 +26,14 @@
     ie)srcStart = 4, srcEnd = 6, destIndex = 2
     srcPl: s0 s1 s2 s3 s4 s5 s6 s7   destPl: d0 d1 d2 d3 d4 d5 d6
 
     becomes:
     srcPl: s0 s1 s2 s3 s7   destPl: d0 d1 d2 s4 s5 s6 d3 d4 d5 d6
     '''
 
-    installed = promptInstall()
-
-    if not installed:
-        return
-
     from sync_dl_ytapi.commands import getPlAdder, getPlRemover
 
 
     srcMetaDataPath = f"{srcPlPath}/{cfg.metaDataName}"
     destMetaDataPath = f"{destPlPath}/{cfg.metaDataName}"
     with shelve.open(srcMetaDataPath, 'c',writeback=True) as srcMetaData, shelve.open(destMetaDataPath, 'c',writeback=True) as destMetaData:
         correctStateCorruption(srcPlPath, srcMetaData)
@@ -104,15 +58,15 @@
         plAdder = getPlAdder(destPlUrl)
         if plAdder is None:
             return
 
         destRemoteIds = getIDs(destPlUrl)
 
         plRemover, srcRemoteIds = getPlRemover(srcPlUrl)
-        if plRemover is None:
+        if plRemover is None or srcRemoteIds is None:
             return
 
 
         ### Src start/end sanitization
         if srcStart>=srcIdsLen:
             cfg.logger.error(f"No Song has Index {srcStart} in {srcPlName}, Largest Index is {srcIdsLen-1}")
             return
```

## sync_dl/ytdlWrappers.py

```diff
@@ -76,47 +76,42 @@
         title = ydl.prepare_filename(song)
     return title
 
 
 def downloadToTmp(videoId,numberStr):
     url = f"https://www.youtube.com/watch?v={videoId}"
 
-    if not os.path.exists(cfg.tmpDownloadPath):
-        os.mkdir(cfg.tmpDownloadPath)
+    cfg.dlParams["outtmpl"] = f'{cfg.songDownloadPath}/{numberStr}_%(title)s.%(ext)s'
+    cfg.dlParams['logger'] = MyLogger()
 
-    cfg.params["outtmpl"] = f'{cfg.tmpDownloadPath}/{numberStr}_%(title)s.%(ext)s'
-    cfg.params['logger'] = MyLogger()
+    with youtube_dl.YoutubeDL(cfg.dlParams) as ydl:
 
-    with youtube_dl.YoutubeDL(cfg.params) as ydl:
-
-        #ensures tmp is empty
-        tmp = os.listdir(path=cfg.tmpDownloadPath)
-        for f in tmp:
-            os.remove(f"{cfg.tmpDownloadPath}/{f}")
+        cfg.clearTmpSubPath(cfg.songDownloadPath)
 
         attemptNumber = 1
         numAttempts = 2
 
         while True:
             try:
                 ydl.download([url])
                 return True
             except Exception as e:
                 cfg.logger.debug(e)
                 cfg.logger.info(f"Unable to Download Song at {url}")
                 if attemptNumber == numAttempts:
+                    cfg.logger.info(f"Max Download Retries Reached! If Song URL is Accessable Try Updating yt-dlp")
                     return False
                 cfg.logger.info("Retrying...")
                 time.sleep(0.5)
                 attemptNumber += 1
 
 
 def moveFromTmp(path):
-    tmp = os.listdir(path=cfg.tmpDownloadPath)
-    shutil.move(f"{cfg.tmpDownloadPath}/{tmp[0]}", path)
+    tmp = os.listdir(path=cfg.songDownloadPath)
+    shutil.move(f"{cfg.songDownloadPath}/{tmp[0]}", path)
     return tmp[0]
 
 def getJsonPlData(url):
     '''returns list of dicts of data for each video in playlist at url (order is playlist order)'''
     params = {}
     params['extract_flat'] = True
 
@@ -125,7 +120,56 @@
     with youtube_dl.YoutubeDL(params) as ydl:
         try:
             entries = ydl.extract_info(url,download=False)['entries']
         except:
             cfg.logger.error(f"No Playlist At URL: {url}")
             entries = []
     return entries
+
+
+def _getBestThumbnail(thumbnails):
+    maxWidth = 0
+    best = None
+    for thumbnail in thumbnails:
+        width = thumbnail['width']
+        if width > maxWidth:
+            maxWidth = width
+            best = thumbnail['url']
+
+    if best is None:
+        return None
+
+    return best.split('?')[0]
+
+def getThumbnailUrls(url:str) -> dict:
+    '''
+    used to check for corrupted metadata in integration tests
+    Title will differ from what is on youtube because it is sanitized for use in filenames
+    '''
+
+    params = {
+        "extract_flat": True, 
+        "quiet": True, 
+        "simulate": True,
+        #"list_thumbnails": True,
+        "logger": MyLogger(),
+    }
+
+    with youtube_dl.YoutubeDL(params) as ydl:
+        result = ydl.extract_info(url,download=False)
+
+    try:
+        entries = result['entries']
+    except KeyError:
+        return {}
+
+    thumbnails = {}
+    for entry in entries:
+        try:
+            thumbnail = _getBestThumbnail(entry['thumbnails'])
+            if thumbnail is None:
+                continue
+            thumbnails[entry['id']] = thumbnail
+        except KeyError:
+            continue
+
+    return thumbnails
```

## sync_dl/timestamps/__init__.py

```diff
@@ -3,15 +3,14 @@
 import subprocess
 import shutil
 
 import sync_dl.config as cfg
 from sync_dl.timestamps.scraping import Timestamp
 from typing import List
 from sync_dl import noInterrupt
-from sync_dl.helpers import clearTmpDownloadPath
 
 from sync_dl.timestamps.scraping import scrapeCommentsForTimestamps
 
 
 chapterRe = re.compile(r"\[CHAPTER\]\nTIMEBASE=(.+)\nSTART=(.+)\nEND=(.+)\ntitle=(.+)\n",flags = re.M)
 
 def _getSongLengthSeconds(songPath:str) -> float:
@@ -28,31 +27,44 @@
         contents = f.read()
         timestamps = []
         for (timebase, start, _, title) in chapterRe.findall(contents):
             timestamps.append(Timestamp.fromFfmpegChapter(timebase, start, title))
 
         return timestamps
 
+def extractChapters(songPath:str) -> List[Timestamp]:
+    cfg.clearTmpSubPath(cfg.ffmpegMetadataPath)
+    createChapterFileCmd = ['ffmpeg', '-hide_banner', '-loglevel', 'error', '-i', songPath, '-an', '-vn', '-sn','-f', 'ffmetadata', cfg.ffmpegMetadataPath]
+
+    try:
+        cfg.logger.debug(f"Extracting Chapters from Song Using FFMPEG Metadata File")
+        subprocess.run(createChapterFileCmd, check=True)
+    except subprocess.CalledProcessError as e:
+        cfg.logger.debug(e)
+        cfg.logger.error(f"Failed to Extract Chapters for Song: {songName}")
+        return []
+
+    return getTimestamps(cfg.ffmpegMetadataPath)
 
 
 def createChapterFile(songPath:str, songName:str) -> bool:
     if not os.path.exists(songPath):
         cfg.logger.error(f"No Song at Path {songPath}")
         return False
 
-    clearTmpDownloadPath()
+    cfg.clearTmpSubPath(cfg.ffmpegMetadataPath)
 
     createChapterFileCmd = ['ffmpeg', '-hide_banner', '-loglevel', 'error', '-i', songPath,'-f', 'ffmetadata', cfg.ffmpegMetadataPath]
 
     try:
         cfg.logger.debug(f"Creating FFMPEG Metadata File")
         subprocess.run(createChapterFileCmd, check=True)
     except subprocess.CalledProcessError as e:
         cfg.logger.debug(e)
-        cfg.logger.error(f"Failed to Create ffmpeg Chapter File For Song {songName}")
+        cfg.logger.error(f"Failed to Create ffmpeg Chapter File for Song: {songName}")
         return False
 
     return True
 
 def wipeChapterFile() -> List[Timestamp]:
     '''detects chapters in file and wipes them. returns list of existing timestamps'''
 
@@ -90,24 +102,26 @@
             end = _getSongLengthSeconds(songPath)
             ch = t1.toFfmpegChapter(end)
             cfg.logger.debug(f"Adding Chapter to FFMPEG Metadata File: \n{ch}")
             f.write(ch)
 
 
 def applyChapterFileToSong(songPath:str, songName:str) -> bool:
-    applyChapterFile = ['ffmpeg', '-hide_banner', '-loglevel', 'error', '-i', songPath, '-i', cfg.ffmpegMetadataPath, '-map_metadata', '1', '-map_chapters', '1', '-codec', 'copy', f"{cfg.tmpDownloadPath}/{songName}"]
+    cfg.clearTmpSubPath(cfg.songEditPath)
+
+    applyChapterFile = ['ffmpeg', '-hide_banner', '-loglevel', 'error', '-i', songPath, '-i', cfg.ffmpegMetadataPath, '-map_metadata', '1', '-map_chapters', '1', '-codec', 'copy', f"{cfg.songEditPath}/{songName}"]
 
     try:
         subprocess.run(applyChapterFile,check=True)
     except subprocess.CalledProcessError as e:
         cfg.logger.debug(e)
         return False
 
     with noInterrupt:
-        shutil.move(f"{cfg.tmpDownloadPath}/{songName}", songPath)
+        shutil.move(f"{cfg.songEditPath}/{songName}", songPath)
     return True
 
 
 def addTimestampsIfNoneExist(plPath, songName, videoId):
     songPath = f"{plPath}/{songName}"
     if not createChapterFile(songPath, songName):
         return
```

## sync_dl/timestamps/scraping.py

```diff
@@ -44,19 +44,19 @@
         hours = minutes//60
 
         return self.reprFmt.format(hh=hours, mm=minutesRemainder, ss=secondsRemainder, ll=self.label)
 
     @classmethod
     def fromFfmpegChapter(cls, timeBase:str, start, title) -> 'Timestamp':
         timeBaseNum = eval(timeBase)
-        return cls(label = title, time = int(timeBaseNum*int(start)))
+        return cls(label = title, time = round(timeBaseNum*int(start)))
 
 
     def toFfmpegChapter(self, nextTime):
-        return self.chapterFmt.format(start = 1000*self.time, end = int(1000*nextTime) - 1, title = self.label)
+        return self.chapterFmt.format(start = round(1000*self.time), end = round(1000*nextTime) - 1, title = self.label)
 
 
 
 
 def scrapeJson(j, desiredKey: str, results:List):
     if isinstance(j,List):
         for value in j:
```

## Comparing `sync_dl-2.3.5.dist-info/LICENCE` & `sync_dl-2.3.7.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `sync_dl-2.3.5.dist-info/METADATA` & `sync_dl-2.3.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sync-dl
-Version: 2.3.5
+Version: 2.3.7
 Summary: A tool for downloading and syncing remote playlists to your computer
 Home-page: https://github.com/PrinceOfPuppers/sync-dl
 Author: Joshua McPherson
 Author-email: joshuamcpherson5@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: yt-dlp
+Requires-Dist: sync-dl-ytapi (>=1.1.1)
 
 <img align="left" width="80" height="80" src="https://raw.githubusercontent.com/PrinceOfPuppers/sync-dl/main/icon.png">
 
 # sync-dl
 <p>
 <img src="https://img.shields.io/pypi/dm/sync-dl">
 <img src="https://img.shields.io/pypi/l/sync-dl">
@@ -89,15 +90,14 @@
 ```
 sync-dl ytapi --push order [PLAYLIST]
 ```
 sync-dl has a submodule which uses the youtube api the preform the reverse of Smart Sync called Push Order. sync-dl will prompt you to install the submodule if you use any of its options ie) --push-order. you must also sign in with google (so sync-dl can edit the order of your playlist).
 
 For more information see https://github.com/PrinceOfPuppers/sync-dl-ytapi
 
-the order of songs which work well for large playlists, ie) 
 ## Many More!
 Includes tools managing large playlists, For example `sync-dl edit --move-range [I1] [I2] [NI] [PLAYLIST]` which allows a user to move a block of songs From [I1] to [I2] to after song [N1].
 
 Moving large blocks of songs on youtube requires dragging each song individually up/down a the page as it trys to dynamically load the hunders of songs you're scrolling past, which you would have to do every time you would want to add new music to somewhere other than the end of the playlist... (ask me how I know :^P)
 
 
 # EXAMPLE
```

## Comparing `sync_dl-2.3.5.dist-info/RECORD` & `sync_dl-2.3.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-sync_dl/__init__.py,sha256=gV386DtlUdg4xEHaAmV36rUVaXmXSLwJLhGT5vOzkhA,1495
-sync_dl/cli.py,sha256=6iJN8c6PRhY5O2iKEcwLgIkNhuqRMoaAIYGs_Iwf9Ik,20284
+sync_dl/__init__.py,sha256=YTvKX4kYJoUbYh1a6804-DGLbLnOiwU1O4kkHOPbUp4,1495
+sync_dl/cli.py,sha256=TdM7chldnzkTuUMFSeA572VFEW6phlhAFnrBEC6w-zs,20221
 sync_dl/commands.py,sha256=ko7r1mBVi5sjEbqJC9ZRxULbicxqyLA9nB0HvGZp9-8,23946
 sync_dl/config.py,sha256=JF6qeaKYSP9LMLoO0R7SrCc9FcdDAUHNhTd4bmtdM1s,4395
-sync_dl/helpers.py,sha256=cPJuiv6qacCXDRjNisbu-n1d4XaJco51Yl9jXqx5TSU,15243
+sync_dl/helpers.py,sha256=4CTE6iUv6PjLjqCPWQ0af4FLUsfA5aXguOU4enVHUHk,15013
 sync_dl/plManagement.py,sha256=EjNxl39U9mjXczOBpvr34NLUFR9rZlibHBUQwwNQvMk,7797
-sync_dl/ytapiInterface.py,sha256=-YUAJjAz2iV5Hn9TqINomUxkK9NP7R4O7A1UqyovWMg,9650
-sync_dl/ytdlWrappers.py,sha256=uk-BzqpLbgiffwsbP6JkM4JmIiW_5oeOhk0gzam3OA4,3631
-sync_dl/timestamps/__init__.py,sha256=G2Nefro_QPBtBhmHtXCPeiiR-z480dUVA9d7N-VoU6o,4706
-sync_dl/timestamps/scraping.py,sha256=NukFsYtxjeC7T41AQNyjelmzFiKQf9MA0MS2ACm0ZS8,7441
+sync_dl/ytapiInterface.py,sha256=lcSQzdGOG3HhoFVyp-rFZXACXL3dHumHAnxZ5hMWgd0,8573
+sync_dl/ytdlWrappers.py,sha256=J6b86YbQwueWP8fqNCM8vqKGnVD2cfCgZlDYg2eBXws,4730
+sync_dl/config/__init__.py,sha256=TcmYLElieYlRvhn5zYlePVMkePi4l2iJE1PB9kM7b98,1253
+sync_dl/config/parsing.py,sha256=ITvoju71jtCifjTu5mWZkIdJcBj0XgMjND8FCY-mG2o,1284
+sync_dl/config/tmpdir.py,sha256=3YRuG-_vitWHLflcBMPDAdr0jDT32y9UKr6hfhCRUd8,1910
+sync_dl/config/ytdlParams.py,sha256=nnpDGNC0_VXMzmEpY5uCEC-cZEI85MjQvT1V-HRixYk,2335
+sync_dl/timestamps/__init__.py,sha256=taEZtNru3I-RZmvcWwMyxF0zLby-_01hGyT4CniViyY,5347
+sync_dl/timestamps/scraping.py,sha256=myKCWvp2eFsSfXyaygSQbjMRz5RIsi4v1143oasHhCo,7452
 sync_dl/timestamps/timestamps.py,sha256=0tBetx_smmiLiDrMEgrvEZ2DLmfq7lEU1kSbmVeBRUI,3773
-sync_dl-2.3.5.data/scripts/sync-dl,sha256=yNRWou5dVV9sWPDy5qBs5PrM5UcFWR7Wm4AMfiHTUVY,76
-sync_dl-2.3.5.dist-info/LICENCE,sha256=PQ26oIz5SuWOaAz9Wqns4Jw_dsMn_-rxqCbelzCE6mA,1072
-sync_dl-2.3.5.dist-info/METADATA,sha256=O28GQI9ZjTA8dK7j-owPiJjZsqQhBUO2GyYDL5Xl9xo,5990
-sync_dl-2.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sync_dl-2.3.5.dist-info/entry_points.txt,sha256=zqjlp5yM4gv80mJseusbgkvnO3ZW4tjM6kfU8MI31cM,41
-sync_dl-2.3.5.dist-info/top_level.txt,sha256=EY1cyIHBLNz4lnpANbUtCC_A8sygjJe3Ih9E-2mBMZU,8
-sync_dl-2.3.5.dist-info/RECORD,,
+sync_dl-2.3.7.data/scripts/sync-dl,sha256=yNRWou5dVV9sWPDy5qBs5PrM5UcFWR7Wm4AMfiHTUVY,76
+sync_dl-2.3.7.dist-info/LICENCE,sha256=PQ26oIz5SuWOaAz9Wqns4Jw_dsMn_-rxqCbelzCE6mA,1072
+sync_dl-2.3.7.dist-info/METADATA,sha256=-IA3uin2SWddVibG_NnspLilRzoIRwFWNhGhucJ-zIU,5968
+sync_dl-2.3.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sync_dl-2.3.7.dist-info/entry_points.txt,sha256=zqjlp5yM4gv80mJseusbgkvnO3ZW4tjM6kfU8MI31cM,41
+sync_dl-2.3.7.dist-info/top_level.txt,sha256=EY1cyIHBLNz4lnpANbUtCC_A8sygjJe3Ih9E-2mBMZU,8
+sync_dl-2.3.7.dist-info/RECORD,,
```

