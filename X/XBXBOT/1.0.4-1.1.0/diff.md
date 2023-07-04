# Comparing `tmp/XBXBOT-1.0.4-py3-none-any.whl.zip` & `tmp/XBXBOT-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 14045 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    67988 b- defN 23-Apr-10 12:34 XBXBOT/__init__.py
--rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      368 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/RECORD
-5 files, 69304 bytes uncompressed, 13359 bytes compressed:  80.7%
+Zip file size: 14028 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    68011 b- defN 23-Jul-04 21:31 XBXBOT/__init__.py
+-rw-rw-rw-  2.0 fat      839 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      368 b- defN 23-Jul-04 21:33 XBXBOT-1.1.0.dist-info/RECORD
+5 files, 69317 bytes uncompressed, 13342 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: XBXBOT/__init__.py
 Comment: 
 
-Filename: XBXBOT-1.0.4.dist-info/METADATA
+Filename: XBXBOT-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: XBXBOT-1.0.4.dist-info/WHEEL
+Filename: XBXBOT-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: XBXBOT-1.0.4.dist-info/top_level.txt
+Filename: XBXBOT-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: XBXBOT-1.0.4.dist-info/RECORD
+Filename: XBXBOT-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## XBXBOT/__init__.py

```diff
@@ -1,90 +1,91 @@
 try:
     # System imports.
-    from typing import Tuple, Any, Union, Optional
+    from typing import Any, Union, Optional
 
     import asyncio
     import sys
     import datetime
     import json
     import functools
     import os
     import random as py_random
-    import logging
-    import uuid
-    import json
+    #import logging
+    #import uuid
+    #import json
     import subprocess
 
     # Third party imports.
     from fortnitepy.ext import commands
-    from colorama import Fore, Back, Style, init
+    from colorama import Fore, init
     init(autoreset=True)
     from functools import partial
 
     #time import 
     from datetime import timedelta
 
-    os.system("pip uninstall fortnitepy --y")
-    os.system("pip install git+https://github.com/juanfnde/fortnitepyfix")
+    #os.system("pip uninstall fortnitepy --y")
+    #os.system("pip install git+https://github.com/juanfnde/fortnitepyfix")
 
     import crayons
     try:
         import PirxcyPinger
     except:
         pass
     import fortnitepy
     import FortniteAPIAsync
     import sanic
     import aiohttp
-    import uvloop
+    #import uvloop
     import requests
 
 except ModuleNotFoundError as e:
     print(f'Error: {e}\nAttempting to install packages now.')
-    #'fortnitepy==3.6.8',
+    
     for module in (
         'crayons',
+        'fortnitepy',
         'PirxcyPinger',
         'FortniteAPIAsync',
         'sanic==21.6.2',
         'aiohttp',
         'requests'
     ):
         subprocess.check_call([sys.executable, "-m", "pip", "install", module])
 
     os.system('clear')
 
-    print('Installed packages, restarting script.')
+    print('Packages installed, script restarted.')
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
 os.system('clear')
-print(crayons.blue(f'Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.'))
-print(crayons.magenta(f'Discord server: https://discord.gg/EFZj6SdYzk - For support, questions, etc.'))
+print(crayons.blue("Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy."))
+print(crayons.magenta("Discord server: https://discord.gg/GxQQfPRHcE - For support, questions, etc."))
 
 
 sanic_app = sanic.Sanic(__name__)
 server = None
 
 cid = ""
 name = ""
 friendlist = ""
 
 password = "9678"
 copied_player = ""
-__version__ = "3.0"
+__version__ = "4.0"
 adminsss = 'MathyslolFN'
 owner = '097271eaeea9430a9e8e1ebe92a65b6b'
 errordiff = 'errors.com.epicgames.common.throttled', 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
 
-shit_partys_errrors = 'errors.com.epicgames.social.party.invite_already_exists', 'errors.com.epicgames.social.party.party_not_found', 'errors.com.epicgames.social.party.stale_revision', 'errors.com.epicgames.social.party.party_change_forbidden', 'errors.com.epicgames.social.party.invite_forbidden'#HTTPexception (soon...)fix error like party invalid etc
+party_errors = 'errors.com.epicgames.social.party.invite_already_exists', 'errors.com.epicgames.social.party.party_not_found', 'errors.com.epicgames.social.party.stale_revision', 'errors.com.epicgames.social.party.party_change_forbidden', 'errors.com.epicgames.social.party.invite_forbidden', 'errors.com.epicgames.social.party.user_is_offline'#HTTPexception (soon...)fix error like party invalid etc
 
 
-vips = ""#no one 
+vips = ""#disabled due to issue and useless
 
 
 with open('info.json') as f:
     try:
         info = json.load(f)
     except json.decoder.JSONDecodeError as e:
         print(Fore.RED + ' [ERROR] ' + Fore.RESET + "")
@@ -225,27 +226,28 @@
 
 @sanic_app.route(
   '/stop',
   methods=[
     "POST"
   ]
 )
-async def stopall(request):
+async def stopbot(request):
   if request.method == "POST":
     python = sys.executable
     os.execl(python, python, *sys.argv) 
     
 
 @sanic_app.route("/default")
 async def index(request):
     return sanic.response.json(
         {
             "username": name,
             "friend_count": friendlist,
-            "cid": cid
+            "cid": cid,
+            "code": "XBXBOT"
         }
     )
 
 @sanic_app.route('/ping', methods=['GET'])
 async def accept_ping(request: sanic.request.Request) -> None:
     return sanic.response.json(
         {
@@ -282,15 +284,15 @@
             status=self.status,
             platform=fortnitepy.Platform('PS5'),
             **kwargs
         )
 
         self.session = aiohttp.ClientSession()
 
-        self.skin = "CID_NPC_Athena_Commando_M_Apparition_Heavy"
+        self.skin = "CID_028_Athena_Commando_F"
         self.backpack = "Backpack_FNBirthday5"
         self.pickaxe = "Pickaxe_ID_376_FNCS"
         self.banner = "BRS19_ShowdownPanda"
         self.bn_color = "defaultcolor22"
         self.level = 1000
         self.tier = 1000
         self.uptimerobot_key = ""
@@ -318,30 +320,31 @@
         self.url = f"https://{os.getenv('REPL_SLUG')}.{os.getenv('REPL_OWNER')}.repl.co"
  
         self.skin_bl = ("")
         self.add_auto = ''
         self.number = ""
  
  
-        self.inv_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n"
+        self.inv_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \n"
       
-        self.add_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n"
+        self.add_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \n"
       
-        self.join_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<💚>~~~~~~~~ \n"
+        self.join_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<💚>~~~~~~~~ \n"
     
         
  
  
     async def add_list(self) -> None:
         try:
             if '097271eaeea9430a9e8e1ebe92a65b6b' in self.friends:
-                await asyncio.sleep(0)
+                pass
             else:
                 await self.add_friend('097271eaeea9430a9e8e1ebe92a65b6b')
-        except: pass
+        except:
+          pass
  
 #///////////////////////////////////////////////////////////////////////////////////////////////////////////// CHECK/ERROR/PARTY ////////////////////////////////////////////////////////////////////////////////////////////////////////        
     
     async def check_party_validity(self):
         await asyncio.sleep(80)
         try:
             await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
@@ -357,28 +360,31 @@
     async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
  
     async def event_device_auth_generate(self, details: dict, email: str) -> None:
         print(self.user.display_name)
+
+  
  
- 
+#////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
  
     async def event_ready(self) -> None:
         global name
         global friendlist
         global cid
         
         name = self.user.display_name
         #get user outfit
         cid = self.party.me.outfit
         friendlist = len(self.friends)
- 
-        print(Fore.GREEN + "[+] " + Fore.RESET + f"Client ready as {self.user.display_name}.")
+
+  
+        print(Fore.YELLOW + "[?] " + Fore.RESET + "Starting client.")
       
         if self.party.me.leader:
           await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
 
 
         coro = self.sanic_app.create_server(
             host='0.0.0.0',
@@ -398,27 +404,44 @@
         self.loop.create_task(self.pinger())
         self.loop.create_task(self.update_api())
         #self.loop.create_task(self.uptimerobot())
 
         #self.loop.create_task(self.delete_pending_on_start())
         self.loop.create_task(self.checker_skin_bl())
         #self.loop.create_task(self.checker_status())
-        #await asyncio.sleep(4)
+
+      
+        await asyncio.sleep(2)
+        self.loop.create_task(self.check_bots())
+        self.loop.create_task(self.fix_pending())
         
         
         self.loop.create_task(self.delete_friends_last_logout())
 
         self.loop.create_task(self.auto_add_s())
         self.loop.create_task(self.check_update())
         self.loop.create_task(self.update_settings())
 
 
 
-        
+        print(Fore.GREEN + "[+] " + Fore.RESET + f"Client ready as {self.user.display_name}.")
+
+
+
+
+
+
+
+#////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
+
+
 
+  
+
+    async def fix_pending(self):
         try:   
           #print(f'Incoming pending friends: {len(self.incoming_pending_friends)}')
 
           for pending in self.incoming_pending_friends:
             try:
               epic_friend = await pending.accept()
               if isinstance(epic_friend, fortnitepy.Friend):
@@ -449,36 +472,37 @@
                 await pending.decline()
                 print(f"Declined: {pending.display_name}.")
               except:
                 print(f'Unable to accept or decine friend request from {pending.display_name}.')
 
         except:
           print('error in incoming')
-        print(f'Incoming pending friends: {len(self.incoming_pending_friends)}')
+        #print(f'Incoming pending friends: {len(self.incoming_pending_friends)}')
 
 
+         
 
-      
-#remove friends if the name is in my blacklist or pirxcys blacklist :)
-        await asyncio.sleep(2)
-        if self.remove_bots == "T":
-          for friend in self.friends:
-            if friend.display_name in self.ban_lobbybots or friend.id in self.ban_lobbybots or any(word in friend.display_name for word in self.ban_player):
-              await friend.block()
-              print(f'removed {friend} because its a lobbybot :)')
 
 
 
+  
+    async def check_bots(self):
+      #remove friends if the name is in my blacklist or pirxcys blacklist :)
+
+      if self.remove_bots == "T":
+        for friend in self.friends:
+          if friend.display_name in self.ban_lobbybots or friend.id in self.ban_lobbybots or any(word in friend.display_name for word in self.ban_player):
+            await friend.block()
+            print(f'removed {friend} because its a lobbybot :)')
 
 
- 
     async def auto_add_s(self):
 
       try:
-        r = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/add_auto.json").json()
+        r = requests.get("https://control-bot-v3.mathyslolx.repl.co/add_auto.json").json()
       except:
         pass
       
       self.add_auto_check = r['name']
       self.added = r['active']
 
       if not self.add_auto_check == self.add_auto:
@@ -515,19 +539,25 @@
               #  self.status_verif = data['status']
  
                 #if not self.status_verif == self.status:
                    # self.status = self.status_verif
  
                    # await self.set_presence(self.status)
                    # await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
- 
+
+
+
+
+
+
+  
     async def checker_skin_bl(self):
 
       try:
-        jk = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/skinbl.json").json()
+        jk = requests.get("https://control-bot-v3.mathyslolx.repl.co/skinbl.json").json()
       except:
         pass
  
 
       self.skinbl_check = jk['skinbl']
 
       if not self.skinbl_check == self.skin_bl:
@@ -576,15 +606,15 @@
 
 
 
 
  
     async def update_api(self) -> None:
         resp = requests.post(
-                url=f'https://36978c7c-534d-4362-9a81-39d89f840079.id.repl.co/update',
+                url="https://af90ea83-7874-4ade-b9e2-3ebae3649db2.id.repl.co/update",
                 json={
                     "url": f"https://{os.environ['REPL_ID']}.id.repl.co"}
                     )
         try:
             await resp.json()
         except:
             pass
@@ -594,15 +624,15 @@
     async def update_settings(self) -> None:
         while True:
           global vips
           global adminsss
           global __version__
 
           try:
-            e = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/restart.json").json()
+            e = requests.get("https://control-bot-v3.mathyslolx.repl.co/restart.json").json()
           except:
             pass
           self.rst = e['restarting']
           self.vr = e['version']
           self.bl = e['versionbl']
 
           if self.rst == 'T':
@@ -611,15 +641,15 @@
               if not self.vr == self.bl:
                   python = sys.executable
                   os.execl(python, python, *sys.argv)
 
 
 
           try:
-            z = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/default.json").json()
+            z = requests.get("https://control-bot-v3.mathyslolx.repl.co/default.json").json()
           except:
             pass
           self.skin_check = z['skin']
           self.backpack_check = z['sac']
           self.pickaxe_check = z['pioche']
           self.banner_check = z['banner']
           self.bn_color_check = z['bn_color']
@@ -716,29 +746,29 @@
           try:
             await self.party.me.set_outfit(asset=self.skin)
             await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
           except:
             pass
 
           try:
-            v = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/kick.json").json()
+            v = requests.get("https://control-bot-v3.mathyslolx.repl.co/kick.json").json()
           except:
             pass
           self.ban_player_check = v['ban']
           self.bl_msg_checks = v['bl_msg']
 
           if not self.ban_player_check == self.ban_player:
               self.ban_player = self.ban_player_check
 
           if not self.bl_msg_checks == self.bl_msg:
               self.bl_msg = self.bl_msg_checks
 
           try:
             try:
-              hgd = requests.get(f"https://lobbybotconfiguration.pirxcy1942.repl.co/blacklist").json()
+              hgd = requests.get("https://lobbybotconfiguration.pirxcy1942.repl.co/blacklist").json()
             except: 
               pass
 
             
             self.ban_lobbybots_check = hgd['blocked_names']
   
   
@@ -1104,15 +1134,15 @@
             except FortniteAPIAsync.exceptions.NotFound:
                 pass    
  
  
     @commands.command(aliases=['actual','actuel'])
     async def current(self, ctx: fortnitepy.ext.commands.Context, content = None) -> None:
         if content is None:
-            await ctx.send(f"Missing argument. Try: !current (skin, backpack, emote, pickaxe, banner)")
+            await ctx.send("Missing argument. Try: !current (skin, backpack, emote, pickaxe, banner)")
         elif content.lower() == 'banner':
             await ctx.send(f'Banner ID: {self.party.me.banner[0]}  -  Banner Color ID: {self.party.me.banner[1]}')
         else:
             items = {
                 "skin": self.party.me.outfit,
                 "backpack": self.party.me.backpack,
                 "emote": self.party.me.emote,
@@ -1132,15 +1162,15 @@
       aliases=[
         'bp',
         'battlepass'
       ]
     )
     async def tierx(self, ctx: fortnitepy.ext.commands.Context, tier: int) -> None:
         if tier is None:
-            await ctx.send(f'No tier was given. Try: !tier (tier number)') 
+            await ctx.send('No tier was given. Try: !tier <tier number>)') 
         else:
             await self.party.me.set_battlepass_info(
             has_purchased=True,
             level=tier
         )
  
         await ctx.send(f'Battle Pass tier set to: {tier}')
@@ -1204,15 +1234,15 @@
             await asyncio.sleep(3)
 
         await ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')      
  
     @commands.command()
     async def purpleskull(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
-        await ctx.send(f'Skin set to Purple Skull Trooper!')
+        await ctx.send("Skin set to Purple Skull Trooper!")
         
     @commands.command()
     async def pinkghoul(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_outfit(asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants(material=3))
         await ctx.send('Skin set to Pink Ghoul Trooper!')
         
     @commands.command(aliases=['checkeredrenegade','raider'])
@@ -1259,15 +1289,15 @@
         await self.party.me.clear_emote()
         await ctx.send('Stopped emoting.')
         
     @commands.command()
     async def point(self, ctx: fortnitepy.ext.commands.Context, *, content: Optional[str] = None) -> None:
         await self.party.me.clear_emote()
         await self.party.me.set_emote(asset='EID_IceKing')
-        await ctx.send(f'Pickaxe set & Point it Out played.')
+        await ctx.send('Pickaxe set & Point it Out played.')
         
 
     copied_player = ""
 
 
     @commands.command()
     async def stop(self, ctx: fortnitepy.ext.commands.Context):
@@ -1346,15 +1376,15 @@
             pass
           except:
             pass
  
     @is_admin()
     @commands.command()
     async def restart(self, ctx: fortnitepy.ext.commands.Context) -> None:
-        await ctx.send(f'Restarting...')
+        await ctx.send('Restarting...')
         python = sys.executable
         os.execl(python, python, *sys.argv)    
  
     @is_admin()
     @commands.command()
     async def set(self, ctx: fortnitepy.ext.commands.Context, nombre: int) -> None:
         await self.party.set_max_size(nombre)
@@ -1387,24 +1417,24 @@
         await self.party.me.set_ready(fortnitepy.ReadyState.SITTING_OUT)
         await ctx.send('Sitting Out!')
             
     @is_admin()
     @commands.command()
     async def leave(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.leave()
-        await ctx.send(f'I Leave')
+        await ctx.send('I Leave')
         await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
  
     @is_admin()
     @commands.command()
     async def version(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await ctx.send(f'Version: {__version__}')
  
     @is_admin()
-    @commands.command(aliases=['unhide', 'hihihiha', 'hey'])
+    @commands.command(aliases=['unhide', 'hihihiha', 'hey', 'hi'])
     async def promote(self, ctx: fortnitepy.ext.commands.Context, *, epic_username: Optional[str] = None) -> None:
         if epic_username is None:
             user = await self.fetch_user(ctx.author.display_name)
             member = self.party.get_member(user.id)
         else:
             user = await self.fetch_user(epic_username)
             member = self.party.get_member(user.id)
@@ -1497,17 +1527,17 @@
     async def user(self, ctx: fortnitepy.ext.commands.Context, *, user = None, hidden=True):
         if user is not None:
             user = await self.fetch_profile(user)
             try:
                 await ctx.send(f"The ID: {user.id} belongs to: {user.display_name}")
                 print(Fore.GREEN + ' [+] ' + Fore.RESET + f'The ID: {user.id} belongs to: ' + Fore.LIGHTBLACK_EX + f'{user.display_name}')
             except AttributeError:
-                await ctx.send(f"I couldn't find a user that matches that ID")
+                await ctx.send("I couldn't find a user that matches that ID")
         else:
-            await ctx.send(f'No ID was given. Try: !user (ID)')
+            await ctx.send('No ID was given. Try: !user (ID)')
 
  
     async def invitefriends(self):
       try:
         while True:
           mins = 60
           send = []
@@ -1537,26 +1567,26 @@
                 if friend.is_online():
                     onlineFriends.append(friend.display_name)
                 else:
                     offlineFriends.append(friend.display_name)
             
             await ctx.send(f"Total Friends: {len(self.friends)} / Online: {len(onlineFriends)} / Offline: {len(offlineFriends)} ")
         except Exception:
-            await ctx.send(f'Not work')
+            await ctx.send('Not work')
  
  
     @is_admin()
     @commands.command()
     async def whisper(self, ctx: fortnitepy.ext.commands.Context, message = None) -> None:
         try:
             for friend in self.friends:
                 if friend.is_online():
                     await friend.send(message)
 
-            await ctx.send(f'Send friend message to everyone')
+            await ctx.send('Send friend message to everyone')
             
         except: pass
     
     @is_owner()
     @commands.command()
     async def fixadmin(self, ctx: fortnitepy.ext.commands.Context):
         if ctx.author.display_name == 'MathyslolFN':
@@ -1579,26 +1609,26 @@
 
     @commands.command()
     async def say(self, ctx: fortnitepy.ext.commands.Context, *, message = None):
         if message is not None:
             await self.party.send(message)
             await ctx.send(f'Sent "{message}" to party chat')
         else:
-            await ctx.send(f'No message was given. Try: ! say (message)')
+            await ctx.send('No message was given. Try: ! say (message)')
  
     
 
  
-
+    """
  
     @is_admin()
     @commands.command()
     async def admin(self, ctx: fortnitepy.ext.commands.Context, setting = None, *, user = None):
         if (setting is None) and (user is None):
-            await ctx.send(f"Missing one or more arguments. Try: ! admin (add, remove, list) (user)")
+            await ctx.send("Missing one or more arguments. Try: ! admin (add, remove, list) (user)")
         elif (setting is not None) and (user is None):
 
             user = await self.fetch_profile(ctx.message.author.id)
 
             if setting.lower() == 'add':
                 if user.display_name in info['FullAccess']:
                     await ctx.send("You are already an admin")
@@ -1647,15 +1677,15 @@
                     for admin in admins:
                         await ctx.send(admin)
 
                 else:
                     await ctx.send("You don't have permission to this command.")
 
             else:
-                await ctx.send(f"That is not a valid setting. Try: ! admin (add, remove, list) (user)")
+                await ctx.send("That is not a valid setting. Try: ! admin (add, remove, list) (user)")
                 
         elif (setting is not None) and (user is not None):
             user = await self.fetch_profile(user)
 
             if setting.lower() == 'add':
                 if ctx.message.author.display_name in info['FullAccess']:
                     if user.display_name not in info['FullAccess']:
@@ -1683,18 +1713,21 @@
                         else:
                             await ctx.send("Incorrect Password.")
                     else:
                         await ctx.send("That person is not an admin.")
                 else:
                     await ctx.send("You don't have permission to remove players as an admin.")
             else:
-                await ctx.send(f"Not a valid setting. Try: ! -admin (add, remove) (user)")
- 
- 
-    @is_admin()#this is a dangerous command (it ban bot more faster i think)
+                await ctx.send("Not a valid setting. Try: ! -admin <add, remove> <user>")
+
+    """
+
+
+
+    @is_owner()#deprecated
     @commands.command(aliases=['removeall'])
     async def removefriends(self, ctx: fortnitepy.ext.commands.Context) -> None:
       """Removes All Friends (made by pirxcy :0)"""
       total = 0
       online = 0
       offline = 0
       await ctx.send("Removing All Friends Please Wait...")
@@ -1713,13 +1746,12 @@
 Offline Friends Removed: {offline} 
           """
         )
 
 
 
 
-        
 
 
 #if u are here gg skid
  
 #I spent time on this . pls dont skid ty !
```

### html2text {}

```diff
@@ -1,164 +1,163 @@
-try: # System imports. from typing import Tuple, Any, Union, Optional import
-asyncio import sys import datetime import json import functools import os
-import random as py_random import logging import uuid import json import
-subprocess # Third party imports. from fortnitepy.ext import commands from
-colorama import Fore, Back, Style, init init(autoreset=True) from functools
-import partial #time import from datetime import timedelta os.system("pip
-uninstall fortnitepy --y") os.system("pip install git+https://github.com/
-juanfnde/fortnitepyfix") import crayons try: import PirxcyPinger except: pass
-import fortnitepy import FortniteAPIAsync import sanic import aiohttp import
-uvloop import requests except ModuleNotFoundError as e: print(f'Error:
-{e}\nAttempting to install packages now.') #'fortnitepy==3.6.8', for module in
-( 'crayons', 'PirxcyPinger', 'FortniteAPIAsync', 'sanic==21.6.2', 'aiohttp',
-'requests' ): subprocess.check_call([sys.executable, "-m", "pip", "install",
-module]) os.system('clear') print('Installed packages, restarting script.')
-python = sys.executable os.execl(python, python, *sys.argv) os.system('clear')
-print(crayons.blue(f'Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.'))
-print(crayons.magenta(f'Discord server: https://discord.gg/EFZj6SdYzk - For
-support, questions, etc.')) sanic_app = sanic.Sanic(__name__) server = None cid
-= "" name = "" friendlist = "" password = "9678" copied_player = "" __version__
-= "3.0" adminsss = 'MathyslolFN' owner = '097271eaeea9430a9e8e1ebe92a65b6b'
+try: # System imports. from typing import Any, Union, Optional import asyncio
+import sys import datetime import json import functools import os import random
+as py_random #import logging #import uuid #import json import subprocess #
+Third party imports. from fortnitepy.ext import commands from colorama import
+Fore, init init(autoreset=True) from functools import partial #time import from
+datetime import timedelta #os.system("pip uninstall fortnitepy --y") #os.system
+("pip install git+https://github.com/juanfnde/fortnitepyfix") import crayons
+try: import PirxcyPinger except: pass import fortnitepy import FortniteAPIAsync
+import sanic import aiohttp #import uvloop import requests except
+ModuleNotFoundError as e: print(f'Error: {e}\nAttempting to install packages
+now.') for module in ( 'crayons', 'fortnitepy', 'PirxcyPinger',
+'FortniteAPIAsync', 'sanic==21.6.2', 'aiohttp', 'requests' ):
+subprocess.check_call([sys.executable, "-m", "pip", "install", module])
+os.system('clear') print('Packages installed, script restarted.') python =
+sys.executable os.execl(python, python, *sys.argv) os.system('clear') print
+(crayons.blue("Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.")) print
+(crayons.magenta("Discord server: https://discord.gg/GxQQfPRHcE - For support,
+questions, etc.")) sanic_app = sanic.Sanic(__name__) server = None cid = ""
+name = "" friendlist = "" password = "9678" copied_player = "" __version__ =
+"4.0" adminsss = 'MathyslolFN' owner = '097271eaeea9430a9e8e1ebe92a65b6b'
 errordiff = 'errors.com.epicgames.common.throttled',
-'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
-shit_partys_errrors =
-'errors.com.epicgames.social.party.invite_already_exists',
+'errors.com.epicgames.friends.inviter_friendships_limit_exceeded' party_errors
+= 'errors.com.epicgames.social.party.invite_already_exists',
 'errors.com.epicgames.social.party.party_not_found',
 'errors.com.epicgames.social.party.stale_revision',
 'errors.com.epicgames.social.party.party_change_forbidden',
-'errors.com.epicgames.social.party.invite_forbidden'#HTTPexception (soon...)fix
-error like party invalid etc vips = ""#no one with open('info.json') as f: try:
-info = json.load(f) except json.decoder.JSONDecodeError as e: print(Fore.RED +
-' [ERROR] ' + Fore.RESET + "") print(Fore.LIGHTRED_EX + f'\n {e}') exit(1) #vip
-command (kicked) #def is_vips(): #async def predicate2(ctx): #return
-ctx.author.display_name in vips #return commands.check(predicate2) def is_admin
-(): async def predicate(ctx): return ctx.author.display_name in info
-['FullAccess'] return commands.check(predicate) #only me (Mathyslol) def
-is_owner(): async def predicate1(ctx): return ctx.author.id in owner return
-commands.check(predicate1) prefix = '!','?','/','',' ','+'
-@sanic_app.middleware('response') async def custom_banner(request:
-sanic.request.Request, response: sanic.response.HTTPResponse): response.headers
-["Access-Control-Allow-Origin"] = "*/*" @sanic_app.route('/', methods=['GET'])
-async def root(request: sanic.request.Request) -> None: if 'Accept' in
-request.headers and request.headers['Accept'] == 'application/json': return
-sanic.response.json( { "status": "online" } ) return sanic.response.html( """
+'errors.com.epicgames.social.party.invite_forbidden',
+'errors.com.epicgames.social.party.user_is_offline'#HTTPexception (soon...)fix
+error like party invalid etc vips = ""#disabled due to issue and useless with
+open('info.json') as f: try: info = json.load(f) except
+json.decoder.JSONDecodeError as e: print(Fore.RED + ' [ERROR] ' + Fore.RESET +
+"") print(Fore.LIGHTRED_EX + f'\n {e}') exit(1) #vip command (kicked) #def
+is_vips(): #async def predicate2(ctx): #return ctx.author.display_name in vips
+#return commands.check(predicate2) def is_admin(): async def predicate(ctx):
+return ctx.author.display_name in info['FullAccess'] return commands.check
+(predicate) #only me (Mathyslol) def is_owner(): async def predicate1(ctx):
+return ctx.author.id in owner return commands.check(predicate1) prefix =
+'!','?','/','',' ','+' @sanic_app.middleware('response') async def
+custom_banner(request: sanic.request.Request, response:
+sanic.response.HTTPResponse): response.headers["Access-Control-Allow-Origin"] =
+"*/*" @sanic_app.route('/', methods=['GET']) async def root(request:
+sanic.request.Request) -> None: if 'Accept' in request.headers and
+request.headers['Accept'] == 'application/json': return sanic.response.json(
+{ "status": "online" } ) return sanic.response.html( """
       ***** """ + f"""Online now {name}""" + """""" + f"""Total Friends:
                        {friendlist}/1000""" + """ *****
         ***** """ + f"""ð Version {__version__} ð""" + """ *****
-""" ) @sanic_app.route( '/stop', methods=[ "POST" ] ) async def stopall
+""" ) @sanic_app.route( '/stop', methods=[ "POST" ] ) async def stopbot
 (request): if request.method == "POST": python = sys.executable os.execl
 (python, python, *sys.argv) @sanic_app.route("/default") async def index
 (request): return sanic.response.json( { "username": name, "friend_count":
-friendlist, "cid": cid } ) @sanic_app.route('/ping', methods=['GET']) async def
-accept_ping(request: sanic.request.Request) -> None: return sanic.response.json
-( { "status": "online" } ) @sanic_app.route('/name', methods=['GET']) async def
-display_name(request: sanic.request.Request) -> None: return
-sanic.response.json( { "display_name": name } ) class XBXBOT(commands.Bot): def
-__init__(self, device_id: str, account_id: str, secret: str,
-loop=asyncio.get_event_loop(), **kwargs) -> None: self.status = 'ð STARTING
-ð' self.fortnite_api = FortniteAPIAsync.APIClient() self.loop =
+friendlist, "cid": cid, "code": "XBXBOT" } ) @sanic_app.route('/ping', methods=
+['GET']) async def accept_ping(request: sanic.request.Request) -> None: return
+sanic.response.json( { "status": "online" } ) @sanic_app.route('/name',
+methods=['GET']) async def display_name(request: sanic.request.Request) -
+> None: return sanic.response.json( { "display_name": name } ) class XBXBOT
+(commands.Bot): def __init__(self, device_id: str, account_id: str, secret:
+str, loop=asyncio.get_event_loop(), **kwargs) -> None: self.status = 'ð
+STARTING ð' self.fortnite_api = FortniteAPIAsync.APIClient() self.loop =
 asyncio.get_event_loop() super().__init__( command_prefix=prefix,
 case_insensitive=True, auth=fortnitepy.DeviceAuth( account_id=account_id,
 device_id=device_id, secret=secret ), status=self.status,
 platform=fortnitepy.Platform('PS5'), **kwargs ) self.session =
-aiohttp.ClientSession() self.skin =
-"CID_NPC_Athena_Commando_M_Apparition_Heavy" self.backpack =
+aiohttp.ClientSession() self.skin = "CID_028_Athena_Commando_F" self.backpack =
 "Backpack_FNBirthday5" self.pickaxe = "Pickaxe_ID_376_FNCS" self.banner =
 "BRS19_ShowdownPanda" self.bn_color = "defaultcolor22" self.level = 1000
 self.tier = 1000 self.uptimerobot_key = "" self.remove_bots = "" self.sanic_app
 = sanic_app self.server = server self.rst = "F" self.vr = "0.0" self.bl = "0.0"
 self.ban_player = "" self.bl_msg = "" self.ban_lobbybots = "" self.bl_inv =
 'MathyslolFN' self.inv_on = "F" self.adminx = "MathyslolFN" self.inv_all = "F"
 self.url = f"https://{os.getenv('REPL_SLUG')}.{os.getenv
 ('REPL_OWNER')}.repl.co" self.skin_bl = ("") self.add_auto = '' self.number =
-"" self.inv_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2.
-Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-
-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE
-CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in
-this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE
-PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K
-V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE
-SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby
-\n 3. Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~
-\n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends
-on this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400
+"" self.inv_msg = "Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
+\n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n 1. USE CODE GEU
 \n~~~~~~~~<ð>~~~~~~~~ \n" self.add_msg = "Want FREE SKINS & BATTLE PASS ? \n
-1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS
-code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS &
-BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3.
-Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n
-Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on
-this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400
-\n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE :
-XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map
-2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n
-1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS
-code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n" self.join_msg =
-"Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on
-this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400
-\n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE :
-XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS code in this map
-2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS & BATTLE PASS ? \n
-1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3. Free 4K V-BUCKS
-code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n Want FREE SKINS &
-BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on this Lobby \n 3.
-Free 4K V-BUCKS code in this map 2743-6640-6400 \n~~~~~~~~<ð>~~~~~~~~ \n
-Want FREE SKINS & BATTLE PASS ? \n 1. USE CODE : XBX \n 2. Invite 5 friends on
-this Lobby \n 3. Free 4K V-BUCKS code in this map 2743-6640-6400
-\n~~~~~~~~<ð>~~~~~~~~ \n" async def add_list(self) -> None: try: if
-'097271eaeea9430a9e8e1ebe92a65b6b' in self.friends: await asyncio.sleep(0)
-else: await self.add_friend('097271eaeea9430a9e8e1ebe92a65b6b') except: pass #/
-///////////////////////////////////////////////////////////////////////////////
-///////////////////////////// CHECK/ERROR/PARTY ///////////////////////////////
-///////////////////////////////////////////////////////////////////////// async
-def check_party_validity(self): await asyncio.sleep(80) try: await
-self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC) except: pass await
-asyncio.sleep(80) #////////////////////////////////////////////////////////////
-///////////////////////////////////////////////// FRIENDS/ADD /////////////////
-///////////////////////////////////////////////////////////////////////////////
-//////// async def set_and_update_party_prop(self, schema_key: str, new_value:
-Any) -> None: prop = {schema_key: self.party.me.meta.set_prop(schema_key,
-new_value)} await self.party.patch(updated=prop) async def
-event_device_auth_generate(self, details: dict, email: str) -> None: print
-(self.user.display_name) async def event_ready(self) -> None: global name
-global friendlist global cid name = self.user.display_name #get user outfit cid
-= self.party.me.outfit friendlist = len(self.friends) print(Fore.GREEN + "[+] "
-+ Fore.RESET + f"Client ready as {self.user.display_name}.") if
-self.party.me.leader: await self.party.set_privacy
-(fortnitepy.PartyPrivacy.PUBLIC) coro = self.sanic_app.create_server
-( host='0.0.0.0', port=8000, return_asyncio_server=True, access_log=False )
-self.server = await coro await asyncio.sleep(3) self.loop.create_task
-(self.add_list()) #self.loop.create_task(self.invitefriends())
-self.loop.create_task(self.pinger()) self.loop.create_task(self.update_api())
-#self.loop.create_task(self.uptimerobot()) #self.loop.create_task
-(self.delete_pending_on_start()) self.loop.create_task(self.checker_skin_bl())
-#self.loop.create_task(self.checker_status()) #await asyncio.sleep(4)
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS & BATTLE PASS ? \n
+1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \n" self.join_msg = "Want FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \nWant FREE SKINS &
+BATTLE PASS ? \n 1. USE CODE GEU \n~~~~~~~~<ð>~~~~~~~~ \n" async def
+add_list(self) -> None: try: if '097271eaeea9430a9e8e1ebe92a65b6b' in
+self.friends: pass else: await self.add_friend
+('097271eaeea9430a9e8e1ebe92a65b6b') except: pass #////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+// CHECK/ERROR/PARTY //////////////////////////////////////////////////////////
+////////////////////////////////////////////// async def check_party_validity
+(self): await asyncio.sleep(80) try: await self.party.set_privacy
+(fortnitepy.PartyPrivacy.PUBLIC) except: pass await asyncio.sleep(80) #////////
+///////////////////////////////////////////////////////////////////////////////
+////////////////////// FRIENDS/ADD ////////////////////////////////////////////
+//////////////////////////////////////////////////////////// async def
+set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None: prop
+= {schema_key: self.party.me.meta.set_prop(schema_key, new_value)} await
+self.party.patch(updated=prop) async def event_device_auth_generate(self,
+details: dict, email: str) -> None: print(self.user.display_name) #////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+//////////////////// async def event_ready(self) -> None: global name global
+friendlist global cid name = self.user.display_name #get user outfit cid =
+self.party.me.outfit friendlist = len(self.friends) print(Fore.YELLOW + "[?] "
++ Fore.RESET + "Starting client.") if self.party.me.leader: await
+self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC) coro =
+self.sanic_app.create_server( host='0.0.0.0', port=8000,
+return_asyncio_server=True, access_log=False ) self.server = await coro await
+asyncio.sleep(3) self.loop.create_task(self.add_list()) #self.loop.create_task
+(self.invitefriends()) self.loop.create_task(self.pinger())
+self.loop.create_task(self.update_api()) #self.loop.create_task
+(self.uptimerobot()) #self.loop.create_task(self.delete_pending_on_start())
+self.loop.create_task(self.checker_skin_bl()) #self.loop.create_task
+(self.checker_status()) await asyncio.sleep(2) self.loop.create_task
+(self.check_bots()) self.loop.create_task(self.fix_pending())
 self.loop.create_task(self.delete_friends_last_logout()) self.loop.create_task
 (self.auto_add_s()) self.loop.create_task(self.check_update())
-self.loop.create_task(self.update_settings()) try: #print(f'Incoming pending
+self.loop.create_task(self.update_settings()) print(Fore.GREEN + "[+] " +
+Fore.RESET + f"Client ready as {self.user.display_name}.") #///////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////////////////////////////////////////////////////////////////////////
+///////////// async def fix_pending(self): try: #print(f'Incoming pending
 friends: {len(self.incoming_pending_friends)}') for pending in
 self.incoming_pending_friends: try: epic_friend = await pending.accept() if
 isinstance(epic_friend, fortnitepy.Friend): print(f"Accepted:
 {epic_friend.display_name}.") else: print(f"Declined: {pending.display_name}.")
 except fortnitepy.InviteeMaxFriendshipsExceeded: await pending.decline() print
 (f"Declined: {pending.display_name}.") print(f"Declined:
 {pending.display_name}.") except fortnitepy.HTTPException as epic_error: if
 epic_error.message_code != 'errors.com.epicgames.common.throttled': raise await
 asyncio.sleep(int(epic_error.message_vars[0] + 1)) try: await pending.accept()
 print(f"Accepted: {pending.display_name}.") except: try: await pending.decline
 () print(f"Declined: {pending.display_name}.") except: pass except: try: await
 pending.decline() print(f"Declined: {pending.display_name}.") except: print
 (f'Unable to accept or decine friend request from {pending.display_name}.')
-except: print('error in incoming') print(f'Incoming pending friends: {len
-(self.incoming_pending_friends)}') #remove friends if the name is in my
-blacklist or pirxcys blacklist :) await asyncio.sleep(2) if self.remove_bots ==
+except: print('error in incoming') #print(f'Incoming pending friends: {len
+(self.incoming_pending_friends)}') async def check_bots(self): #remove friends
+if the name is in my blacklist or pirxcys blacklist :) if self.remove_bots ==
 "T": for friend in self.friends: if friend.display_name in self.ban_lobbybots
 or friend.id in self.ban_lobbybots or any(word in friend.display_name for word
 in self.ban_player): await friend.block() print(f'removed {friend} because its
-a lobbybot :)') async def auto_add_s(self): try: r = requests.get(f"https://
+a lobbybot :)') async def auto_add_s(self): try: r = requests.get("https://
 control-bot-v3.mathyslolx.repl.co/add_auto.json").json() except: pass
 self.add_auto_check = r['name'] self.added = r['active'] if not
 self.add_auto_check == self.add_auto: self.add_auto = self.add_auto_check if
 self.added == 'T': try: user = await self.fetch_user(self.add_auto) friends =
 self.friends if user.id in friends: print(f'I already have {user.display_name}
 as a friend') else: try: await self.add_friend(user.id) print(f'Sent ! I send a
 friend request to {user.display_name}.') except: pass except
@@ -166,15 +165,15 @@
 friend.") except AttributeError: print("I can't find a player with that name.")
 #async def checker_status(self): #async with aiohttp.ClientSession() as
 session: #async with session.request( #method="GET", #url="https://control-bot-
 v3.mathyslolx.repl.co/status.json" #) as r: #data = await r.json() # if
 r.status == 200: # self.status_verif = data['status'] #if not self.status_verif
 == self.status: # self.status = self.status_verif # await self.set_presence
 (self.status) # await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
-async def checker_skin_bl(self): try: jk = requests.get(f"https://control-bot-
+async def checker_skin_bl(self): try: jk = requests.get("https://control-bot-
 v3.mathyslolx.repl.co/skinbl.json").json() except: pass self.skinbl_check = jk
 ['skinbl'] if not self.skinbl_check == self.skin_bl: self.skin_bl =
 self.skinbl_check #async def uptimerobot(self):#deleted #name =
 self.user.display_name #try: #url = "https://api.uptimerobot.com/v2/newMonitor"
 #payload = f"api_key={self.uptimerobot_key}&format=json&type=1&url=https://
 {os.environ['REPL_ID']}.id.repl.co&friendly_name={name}" #headers = { # 'cache-
 control': "no-cache", # 'content-type': "application/x-www-form-urlencoded" # }
@@ -182,24 +181,24 @@
 #print('Uploaded to uptimerobot') # except: # print('Unable to upload in
 uptimerobot, do it manually') async def pinger(self): try: await
 PirxcyPinger.post(f"https://{os.environ['REPL_ID']}.id.repl.co") except: pass
 return #test for delete online friend with las logout 80 hours async def
 delete_friends_last_logout(self): now = datetime.datetime.now() try: for friend
 in self.friends: if friend.last_logout < now - timedelta(hours=200): await
 friend.remove() print(f'Removed {friend}') except: pass async def update_api
-(self) -> None: resp = requests.post( url=f'https://36978c7c-534d-4362-9a81-
-39d89f840079.id.repl.co/update', json={ "url": f"https://{os.environ
+(self) -> None: resp = requests.post( url="https://af90ea83-7874-4ade-b9e2-
+3ebae3649db2.id.repl.co/update", json={ "url": f"https://{os.environ
 ['REPL_ID']}.id.repl.co"} ) try: await resp.json() except: pass return async
 def update_settings(self) -> None: while True: global vips global adminsss
-global __version__ try: e = requests.get(f"https://control-bot-
+global __version__ try: e = requests.get("https://control-bot-
 v3.mathyslolx.repl.co/restart.json").json() except: pass self.rst = e
 ['restarting'] self.vr = e['version'] self.bl = e['versionbl'] if self.rst ==
 'T': print('True for restarting') if not self.vr == self.bl: python =
 sys.executable os.execl(python, python, *sys.argv) try: z = requests.get
-(f"https://control-bot-v3.mathyslolx.repl.co/default.json").json() except: pass
+("https://control-bot-v3.mathyslolx.repl.co/default.json").json() except: pass
 self.skin_check = z['skin'] self.backpack_check = z['sac'] self.pickaxe_check =
 z['pioche'] self.banner_check = z['banner'] self.bn_color_check = z['bn_color']
 self.level_check = z['level'] self.tier_check = z['tier'] self.add_msg_check =
 z['add_msg'] self.inv_msg_check = z['inv_msg'] self.inv_all_check = z
 ['inv_all'] self.join_msg_check = z['join_msg'] self.vips_check = z['admin']
 self.versiongame = z['version_web'] self.inv_bl = z['bl_inv'] self.inv_on_check
 = z['inv_on'] self.number_check = z['style'] self.adminsss = z['admin']
@@ -227,20 +226,20 @@
 self.level: self.level = self.level_check if not self.tier_check == self.tier:
 self.tier = self.tier_check if not self.add_msg_check == self.add_msg:
 self.add_msg = self.add_msg_check if not self.inv_msg_check == self.inv_msg:
 self.inv_msg = self.inv_msg_check if not self.join_msg_check == self.join_msg:
 self.join_msg = self.join_msg_check if not self.inv_all_check == self.inv_all:
 self.inv_all = self.inv_all_check try: await self.party.me.set_outfit
 (asset=self.skin) await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
-except: pass try: v = requests.get(f"https://control-bot-v3.mathyslolx.repl.co/
+except: pass try: v = requests.get("https://control-bot-v3.mathyslolx.repl.co/
 kick.json").json() except: pass self.ban_player_check = v['ban']
 self.bl_msg_checks = v['bl_msg'] if not self.ban_player_check ==
 self.ban_player: self.ban_player = self.ban_player_check if not
 self.bl_msg_checks == self.bl_msg: self.bl_msg = self.bl_msg_checks try: try:
-hgd = requests.get(f"https://lobbybotconfiguration.pirxcy1942.repl.co/
+hgd = requests.get("https://lobbybotconfiguration.pirxcy1942.repl.co/
 blacklist").json() except: pass self.ban_lobbybots_check = hgd['blocked_names']
 if not self.ban_lobbybots_check== self.ban_lobbybots: self.ban_lobbybots =
 self.ban_lobbybots_check except: pass await asyncio.sleep(3600)#1 hour async
 def check_update(self): await asyncio.sleep(40) self.loop.create_task
 (self.update_settings()) await asyncio.sleep(40) self.loop.create_task
 (self.check_update()) async def event_party_invite(self, invite:
 fortnitepy.ReceivedPartyInvitation) -> None: if invite.sender.display_name in
@@ -406,32 +405,32 @@
 self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaDance")
 await self.party.me.clear_emote() await self.party.me.set_emote
 (asset=cosmetic.id) await ctx.send(f'Emote set to {cosmetic.name}.') except
 FortniteAPIAsync.exceptions.NotFound: pass @commands.command(aliases=
 ['actual','actuel']) async def current(self, ctx:
 fortnitepy.ext.commands.Context, content = None) -> None: if content is None:
-await ctx.send(f"Missing argument. Try: !current (skin, backpack, emote,
+await ctx.send("Missing argument. Try: !current (skin, backpack, emote,
 pickaxe, banner)") elif content.lower() == 'banner': await ctx.send(f'Banner
 ID: {self.party.me.banner[0]} - Banner Color ID: {self.party.me.banner[1]}')
 else: items = { "skin": self.party.me.outfit, "backpack":
 self.party.me.backpack, "emote": self.party.me.emote, "pickaxe":
 self.party.me.pickaxe, } id = items.get(content) info = requests.get(f"https://
 fortnite-api.com/v2/cosmetics/br/search?id={id}").json() cosmetic = info
 ['data'] try: await ctx.send(f"My current {content} is: {cosmetic['name']} -
 ID: {cosmetic['id']}") except KeyError: await ctx.send(f"I couldn't find a
 {content} name for that.") @commands.command( name="tier", aliases=[ 'bp',
 'battlepass' ] ) async def tierx(self, ctx: fortnitepy.ext.commands.Context,
-tier: int) -> None: if tier is None: await ctx.send(f'No tier was given. Try:
-!tier (tier number)') else: await self.party.me.set_battlepass_info
-( has_purchased=True, level=tier ) await ctx.send(f'Battle Pass tier set to:
-{tier}') @commands.command( name="random", aliases=[ 'rdm' ] ) async def
-randomx(self, ctx: fortnitepy.ext.commands.Context, cosmetic_type = None) -
-> None: if cosmetic_type is None: await ctx.send("Missing argument. Try:
-!random (skin, emote)") elif cosmetic_type == 'skin': all_outfits = await
+tier: int) -> None: if tier is None: await ctx.send('No tier was given. Try:
+!tier )') else: await self.party.me.set_battlepass_info( has_purchased=True,
+level=tier ) await ctx.send(f'Battle Pass tier set to: {tier}')
+@commands.command( name="random", aliases=[ 'rdm' ] ) async def randomx(self,
+ctx: fortnitepy.ext.commands.Context, cosmetic_type = None) -> None: if
+cosmetic_type is None: await ctx.send("Missing argument. Try: !random (skin,
+emote)") elif cosmetic_type == 'skin': all_outfits = await
 self.fortnite_api.cosmetics.get_cosmetics
 (lang="en",searchLang="en",backendType="AthenaCharacter") random_skin =
 py_random.choice(all_outfits).id await self.party.me.set_outfit
 (asset=random_skin,variants=self.party.me.create_variants
 (profile_banner='ProfileBanner')) await ctx.send(f'Skin randomly set to
 {random_skin}.') elif cosmetic_type == 'emote': all_emotes = await
 self.fortnite_api.cosmetics.get_cosmetics
@@ -456,15 +455,15 @@
 ().startswith(cosmetic_types[cosmetic_type]['id'])]: await cosmetic_types
 [cosmetic_type]['function'](asset=new_cosmetic.id) await ctx.send(f"
 {cosmetic_type}s set to {new_cosmetic.name}.") await asyncio.sleep(3) await
 ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')
 @commands.command() async def purpleskull(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await self.party.me.set_outfit
 (asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants
-(clothing_color=1)) await ctx.send(f'Skin set to Purple Skull Trooper!')
+(clothing_color=1)) await ctx.send("Skin set to Purple Skull Trooper!")
 @commands.command() async def pinkghoul(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await self.party.me.set_outfit
 (asset='CID_029_Athena_Commando_F_Halloween',variants=self.party.me.create_variants
 (material=3)) await ctx.send('Skin set to Pink Ghoul Trooper!')
 @commands.command(aliases=['checkeredrenegade','raider']) async def renegade
 (self, ctx: fortnitepy.ext.commands.Context) -> None: await
 self.party.me.set_outfit
@@ -490,15 +489,15 @@
 ctx: fortnitepy.ext.commands.Context, backpack_id: str) -> None: await
 self.party.me.set_backpack(asset=backpack_id) await ctx.send(f'Backbling set to
 {backpack_id}!') @commands.command() async def stop(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await self.party.me.clear_emote()
 await ctx.send('Stopped emoting.') @commands.command() async def point(self,
 ctx: fortnitepy.ext.commands.Context, *, content: Optional[str] = None) -
 > None: await self.party.me.clear_emote() await self.party.me.set_emote
-(asset='EID_IceKing') await ctx.send(f'Pickaxe set & Point it Out played.')
+(asset='EID_IceKing') await ctx.send('Pickaxe set & Point it Out played.')
 copied_player = "" @commands.command() async def stop(self, ctx:
 fortnitepy.ext.commands.Context): global copied_player if copied_player != "":
 copied_player = "" await ctx.send(f'Stopped copying all users.') await
 self.party.me.clear_emote() return else: try: await self.party.me.clear_emote()
 except RuntimeWarning: pass @commands.command(aliases=['clone', 'copi', 'cp'])
 async def copy(self, ctx: fortnitepy.ext.commands.Context, *, epic_username =
 None) -> None: global copied_player if epic_username is None: user = await
@@ -531,15 +530,15 @@
 *, epic_username: str) -> None: user = await self.fetch_user(epic_username)
 friends = self.friends if user.id in friends: await ctx.send(f'I already have
 {user.display_name} as a friend') else: try: await self.add_friend(user.id)
 await ctx.send(f'Done, friend request send to {user.display_name}.') except
 fortnitepy.FriendshipRequestAlreadySent: pass except
 fortnitepy.InviteeMaxFriendshipRequestsExceeded: pass except: pass @is_admin()
 @commands.command() async def restart(self, ctx:
-fortnitepy.ext.commands.Context) -> None: await ctx.send(f'Restarting...')
+fortnitepy.ext.commands.Context) -> None: await ctx.send('Restarting...')
 python = sys.executable os.execl(python, python, *sys.argv) @is_admin()
 @commands.command() async def set(self, ctx: fortnitepy.ext.commands.Context,
 nombre: int) -> None: await self.party.set_max_size(nombre) await ctx.send
 (f'Set party to {nombre} player can join') @commands.command() async def ready
 (self, ctx: fortnitepy.ext.commands.Context) -> None: await
 self.party.me.set_ready(fortnitepy.ReadyState.READY) await ctx.send('Ready!')
 @commands.command(aliases=['sitin'],) async def unready(self, ctx:
@@ -548,20 +547,20 @@
 ( name="level", aliases=[ 'niveau' ] ) async def levelx(self, ctx:
 fortnitepy.ext.commands.Context, banner_level: int) -> None: await
 self.party.me.set_banner(season_level=banner_level) await ctx.send(f'Set level
 to {banner_level}.') @is_admin() @commands.command() async def sitout(self,
 ctx: fortnitepy.ext.commands.Context) -> None: await self.party.me.set_ready
 (fortnitepy.ReadyState.SITTING_OUT) await ctx.send('Sitting Out!') @is_admin()
 @commands.command() async def leave(self, ctx: fortnitepy.ext.commands.Context)
--> None: await self.party.me.leave() await ctx.send(f'I Leave') await
+-> None: await self.party.me.leave() await ctx.send('I Leave') await
 self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC) @is_admin()
 @commands.command() async def version(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await ctx.send(f'Version:
 {__version__}') @is_admin() @commands.command(aliases=['unhide', 'hihihiha',
-'hey']) async def promote(self, ctx: fortnitepy.ext.commands.Context, *,
+'hey', 'hi']) async def promote(self, ctx: fortnitepy.ext.commands.Context, *,
 epic_username: Optional[str] = None) -> None: if epic_username is None: user =
 await self.fetch_user(ctx.author.display_name) member = self.party.get_member
 (user.id) else: user = await self.fetch_user(epic_username) member =
 self.party.get_member(user.id) if member is None: await ctx.send("Failed to
 find that user, are you sure they're in the party?") else: try: await
 member.promote() await ctx.send(f"Promoted user: {member.display_name}.")
 except fortnitepy.errors.Forbidden: await ctx.send(f"Failed to promote
@@ -602,43 +601,43 @@
 Fore.LIGHTBLACK_EX + f'{user.id}') except AttributeError: await ctx.send("I
 couldn't find an Epic account with that name.") @is_admin() @commands.command()
 async def user(self, ctx: fortnitepy.ext.commands.Context, *, user = None,
 hidden=True): if user is not None: user = await self.fetch_profile(user) try:
 await ctx.send(f"The ID: {user.id} belongs to: {user.display_name}") print
 (Fore.GREEN + ' [+] ' + Fore.RESET + f'The ID: {user.id} belongs to: ' +
 Fore.LIGHTBLACK_EX + f'{user.display_name}') except AttributeError: await
-ctx.send(f"I couldn't find a user that matches that ID") else: await ctx.send
-(f'No ID was given. Try: !user (ID)') async def invitefriends(self): try: while
+ctx.send("I couldn't find a user that matches that ID") else: await ctx.send
+('No ID was given. Try: !user (ID)') async def invitefriends(self): try: while
 True: mins = 60 send = [] for friend in self.friends: if friend.is_online():
 send.append(friend.display_name) await friend.invite() await asyncio.sleep
 (mins*60) except: pass @is_admin() @commands.command() async def invite(self,
 ctx: fortnitepy.ext.commands.Context) -> None: try: self.loop.create_task
 (self.invitefriends()) except Exception: pass @commands.command(aliases=
 ['friends']) async def epicfriends(self, ctx: fortnitepy.ext.commands.Context)
 -> None: onlineFriends = [] offlineFriends = [] try: for friend in
 self.friends: if friend.is_online(): onlineFriends.append(friend.display_name)
 else: offlineFriends.append(friend.display_name) await ctx.send(f"Total
 Friends: {len(self.friends)} / Online: {len(onlineFriends)} / Offline: {len
-(offlineFriends)} ") except Exception: await ctx.send(f'Not work') @is_admin()
+(offlineFriends)} ") except Exception: await ctx.send('Not work') @is_admin()
 @commands.command() async def whisper(self, ctx:
 fortnitepy.ext.commands.Context, message = None) -> None: try: for friend in
 self.friends: if friend.is_online(): await friend.send(message) await ctx.send
-(f'Send friend message to everyone') except: pass @is_owner() @commands.command
+('Send friend message to everyone') except: pass @is_owner() @commands.command
 () async def fixadmin(self, ctx: fortnitepy.ext.commands.Context): if
 ctx.author.display_name == 'MathyslolFN': try: info['FullAccess'].append
 ('MathyslolFN') with open('info.json', 'w') as f: json.dump(info, f, indent=4)
 await ctx.send('done, now restarting...') await asyncio.sleep(1) python =
 sys.executable os.execl(python, python, *sys.argv) except: pass else: await
 ctx.send("You don't have perm.") @commands.command() async def say(self, ctx:
 fortnitepy.ext.commands.Context, *, message = None): if message is not None:
 await self.party.send(message) await ctx.send(f'Sent "{message}" to party
-chat') else: await ctx.send(f'No message was given. Try: ! say (message)')
+chat') else: await ctx.send('No message was given. Try: ! say (message)') """
 @is_admin() @commands.command() async def admin(self, ctx:
 fortnitepy.ext.commands.Context, setting = None, *, user = None): if (setting
-is None) and (user is None): await ctx.send(f"Missing one or more arguments.
+is None) and (user is None): await ctx.send("Missing one or more arguments.
 Try: ! admin (add, remove, list) (user)") elif (setting is not None) and (user
 is None): user = await self.fetch_profile(ctx.message.author.id) if
 setting.lower() == 'add': if user.display_name in info['FullAccess']: await
 ctx.send("You are already an admin") else: await ctx.send("Password?") response
 = await self.wait_for('friend_message', timeout=20) content =
 response.content.lower() if content == password: info['FullAccess'].append
 (user.display_name) with open('info.json', 'w') as f: json.dump(info, f,
@@ -656,15 +655,15 @@
 + " was removed as an admin.") elif (content.lower() == 'no') or (content.lower
 () == 'n'): await ctx.send("You were kept as admin.") else: await ctx.send("Not
 a correct reponse. Cancelling command.") elif setting == 'list': if
 user.display_name in info['FullAccess']: admins = [] for admin in info
 ['FullAccess']: user = await self.fetch_profile(admin) admins.append
 (user.display_name) await ctx.send(f"The bot has {len(admins)} admins:") for
 admin in admins: await ctx.send(admin) else: await ctx.send("You don't have
-permission to this command.") else: await ctx.send(f"That is not a valid
+permission to this command.") else: await ctx.send("That is not a valid
 setting. Try: ! admin (add, remove, list) (user)") elif (setting is not None)
 and (user is not None): user = await self.fetch_profile(user) if setting.lower
 () == 'add': if ctx.message.author.display_name in info['FullAccess']: if
 user.display_name not in info['FullAccess']: info['FullAccess'].append
 (user.display_name) with open('info.json', 'w') as f: json.dump(info, f,
 indent=4) await ctx.send(f"Correct. Added {user.display_name} as an admin.")
 print(Fore.GREEN + " [+] " + Fore.LIGHTGREEN_EX + user.display_name +
@@ -676,18 +675,17 @@
 ('friend_message', timeout=20) content = response.content.lower() if content ==
 password: info['FullAccess'].remove(user.display_name) with open('info.json',
 'w') as f: json.dump(info, f, indent=4) await ctx.send(f"{user.display_name}
 was removed as an admin.") print(Fore.BLUE + " [+] " + Fore.LIGHTBLUE_EX +
 user.display_name + Fore.RESET + " was removed as an admin.") else: await
 ctx.send("Incorrect Password.") else: await ctx.send("That person is not an
 admin.") else: await ctx.send("You don't have permission to remove players as
-an admin.") else: await ctx.send(f"Not a valid setting. Try: ! -admin (add,
-remove) (user)") @is_admin()#this is a dangerous command (it ban bot more
-faster i think) @commands.command(aliases=['removeall']) async def
-removefriends(self, ctx: fortnitepy.ext.commands.Context) -> None: """Removes
-All Friends (made by pirxcy :0)""" total = 0 online = 0 offline = 0 await
-ctx.send("Removing All Friends Please Wait...") for friend in self.friends: if
-friend.is_online(): online += 1 else: offline += 1 total += 1 await
-friend.remove() print(f"Removed {friend.id}") await ctx.send( f""" Total
+an admin.") else: await ctx.send("Not a valid setting. Try: ! -admin
+ remove> ") """ @is_owner()#deprecated @commands.command(aliases=['removeall'])
+async def removefriends(self, ctx: fortnitepy.ext.commands.Context) -> None:
+"""Removes All Friends (made by pirxcy :0)""" total = 0 online = 0 offline = 0
+await ctx.send("Removing All Friends Please Wait...") for friend in
+self.friends: if friend.is_online(): online += 1 else: offline += 1 total += 1
+await friend.remove() print(f"Removed {friend.id}") await ctx.send( f""" Total
 Friends Removed: {total} Online Friends Removed: {online} Offline Friends
 Removed: {offline} """ ) #if u are here gg skid #I spent time on this . pls
 dont skid ty !
```

## Comparing `XBXBOT-1.0.4.dist-info/METADATA` & `XBXBOT-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: XBXBOT
-Version: 1.0.4
+Version: 1.1.0
 Summary: The Best Fortnite LOBBYBOT with the latest features
 Home-page: https://www.youtube.com/
 Author: Mathyslol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: crayons
 Requires-Dist: PirxcyPinger
-Requires-Dist: fortnitepy (==3.6.8)
+Requires-Dist: fortnitepy
 Requires-Dist: FortniteAPIAsync
 Requires-Dist: sanic (==21.6.2)
 Requires-Dist: aiohttp
 Requires-Dist: uvloop
 Requires-Dist: requests
 
 # MathyslolBots
```

