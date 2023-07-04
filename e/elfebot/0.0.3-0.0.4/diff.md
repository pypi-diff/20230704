# Comparing `tmp/elfebot-0.0.3-py3-none-any.whl.zip` & `tmp/elfebot-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32741 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx    54721 b- defN 23-May-08 19:05 elfebot/__init__.py
+Zip file size: 32785 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx    54956 b- defN 23-Jul-04 12:50 elfebot/__init__.py
 -rwxrwxrwx  2.0 unx    54650 b- defN 23-Apr-12 07:29 oimbot/__init__.py
 -rwxrwxrwx  2.0 unx    54773 b- defN 23-Apr-01 08:51 oimbot/hahaha.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      620 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        8 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      532 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx      819 b- defN 23-May-08 19:06 elfebot-0.0.3.dist-info/RECORD
-10 files, 166272 bytes uncompressed, 31357 bytes compressed:  81.1%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      620 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      532 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      819 b- defN 23-Jul-04 13:28 elfebot-0.0.4.dist-info/RECORD
+10 files, 166507 bytes uncompressed, 31401 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: oimbot/__init__.py
 Comment: 
 
 Filename: oimbot/hahaha.py
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/DESCRIPTION.rst
+Filename: elfebot-0.0.4.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/dependency_links.txt
+Filename: elfebot-0.0.4.dist-info/dependency_links.txt
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/metadata.json
+Filename: elfebot-0.0.4.dist-info/metadata.json
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/top_level.txt
+Filename: elfebot-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/WHEEL
+Filename: elfebot-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/METADATA
+Filename: elfebot-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: elfebot-0.0.3.dist-info/RECORD
+Filename: elfebot-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elfebot/__init__.py

```diff
@@ -222,16 +222,14 @@
         {
             "display_name": name
         }
     )
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = '💎 {party_size}/16 Use Code ELFE #Ad 💎'
-
         self.loop = asyncio.get_event_loop()
         self.fortnite_api = FortniteAPIAsync.APIClient()
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
             auth=fortnitepy.DeviceAuth(
@@ -499,14 +497,40 @@
 
                 if not self.vr == self.bl:
                     python = sys.executable
                     os.execl(python, python, *sys.argv)
 
             await asyncio.sleep(3600)
 
+    async def verify(self):
+      try:
+        global code          
+        if len(self.friends) >= 0 and len(self.friends) <= 300:
+          await self.set_presence('💔 {party_size}/16 | USE CODE ELFE #AD')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        elif len(self.friends) >= 301 and len(self.friends) <= 600:
+          await self.set_presence('🧡 {party_size}/16 |  + USE CODE ELFE #AD ')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        elif len(self.friends) >= 601 and len(self.friends) <= 1100:
+          await self.set_presence('💚 {party_size}/16 | USE CODE ELFE #AD')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        else:
+          await self.set_presence('💚 {party_size}/16 | USE CODE ELFE #AD')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+          
+      except:
+        pass
+
     async def auto_add_s(self):
         x = requests.get(f"https://ninja.aerozoff.com/add_auto",headers={
                 'host': 'ninja.aerozoff.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.12',
                 'enable-super-fast': "TRUE",
                 'x-gorgon': "B37SHJWI28",
                 "x-signature": "HD82KS02KD2"
@@ -533,31 +557,14 @@
                     print(f'Send i friend request to {user.display_name}.')
 
             except fortnitepy.HTTPException:
                 print("There was a problem trying to add this friend.")
             except AttributeError:
                 print("I can't find a player with that name.")
 
-    async def checker_status(self):
-        q = requests.get(f"https://ninja.aerozoff.com/status",headers={
-                'host': 'ninja.aerozoff.com',
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.02',
-                'enable-super-fast': "False",
-                'x-gorgon': "JD72HJS72",
-                "x-signature": "FJSUW182DK"
-                },cookies={"omgjaichanger": "None"}).json()
-
-        self.status_verif = q['status']
-
-        if not self.status_verif == self.status:
-            self.status = self.status_verif
-
-            await self.set_presence(self.status)
-            await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
-
     async def checker_skin_bl(self):
         w = requests.get("https://ninja.aerozoff.com/skinbl",headers={
                 'host': 'ninja.aerozoff.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.09',
                 'enable-super-fast': "True",
                 'x-gorgon': "HSUWJ27DK29S",
                 "x-signature": "NSL37SHQUD"
```

## Comparing `elfebot-0.0.3.dist-info/metadata.json` & `elfebot-0.0.4.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.0.4'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

## Comparing `elfebot-0.0.3.dist-info/METADATA` & `elfebot-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: elfebot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `elfebot-0.0.3.dist-info/RECORD` & `elfebot-0.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-elfebot/__init__.py,sha256=apdEekbsnzt7Ls3_bw0q1XtceSGFO8EPRmWfKAbFCGE,54721
-elfebot-0.0.3.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-elfebot-0.0.3.dist-info/METADATA,sha256=eoVMO0ogqJaX_WT1Bdx11vMqFJNW7OokaX4oZaUzq6Q,532
-elfebot-0.0.3.dist-info/RECORD,,
-elfebot-0.0.3.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-elfebot-0.0.3.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
-elfebot-0.0.3.dist-info/metadata.json,sha256=NBB5x9ouhsr9xYVI8SqbKu2tl58LSS9XukK84wcuHwM,620
-elfebot-0.0.3.dist-info/top_level.txt,sha256=235hKT0BqtGq-kN9JAZ-eJnLwNO2mVVWyiLs5_e2k1E,8
+elfebot/__init__.py,sha256=VDkJEui4ZP9USjm1OPNpyk4Bi1roAlpkNUAc5MFkevg,54956
+elfebot-0.0.4.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+elfebot-0.0.4.dist-info/METADATA,sha256=Ri-cddAxcFmOujwY12fuUu6jACbBVABSWK0K1oPD_Xs,532
+elfebot-0.0.4.dist-info/RECORD,,
+elfebot-0.0.4.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+elfebot-0.0.4.dist-info/dependency_links.txt,sha256=qghdsulj9f7KujhhUbgS6dtbeW8ot_ySInuAyvtQmzg,47
+elfebot-0.0.4.dist-info/metadata.json,sha256=BBJrKx5iIGQbspEgVvACRfgWYXk5rJi41l0hhHLziUo,620
+elfebot-0.0.4.dist-info/top_level.txt,sha256=235hKT0BqtGq-kN9JAZ-eJnLwNO2mVVWyiLs5_e2k1E,8
 oimbot/__init__.py,sha256=dsmxuN1hgo6LQ0aMO-DMp9uRA3FrZyT6LKxnFYPkpDA,54650
 oimbot/hahaha.py,sha256=ngLYUAJKbJUu6iOyTvj7-mnEliL0Fy8CdRfoRDz5jCQ,54773
```

