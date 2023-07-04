# Comparing `tmp/freefang-server-0.2.1.tar.gz` & `tmp/freefang-server-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freefang-server-0.2.1.tar", last modified: Sun Jul  2 12:01:08 2023, max compression
+gzip compressed data, was "freefang-server-0.3.0.tar", last modified: Mon Jul  3 20:32:49 2023, max compression
```

## Comparing `freefang-server-0.2.1.tar` & `freefang-server-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aaron     (1000) aaron     (1000)        0 2023-07-02 12:01:08.256485 freefang-server-0.2.1/
--rw-r--r--   0 aaron     (1000) aaron     (1000)    34523 2023-06-22 19:10:27.000000 freefang-server-0.2.1/LICENSE
--rw-r--r--   0 aaron     (1000) aaron     (1000)     2415 2023-07-02 12:01:08.256485 freefang-server-0.2.1/PKG-INFO
--rw-r--r--   0 aaron     (1000) aaron     (1000)     1749 2023-06-30 15:20:21.000000 freefang-server-0.2.1/README.md
-drwxr-xr-x   0 aaron     (1000) aaron     (1000)        0 2023-07-02 12:01:08.256485 freefang-server-0.2.1/freefang/
--rw-r--r--   0 aaron     (1000) aaron     (1000)        0 2023-06-27 13:29:28.000000 freefang-server-0.2.1/freefang/__init__.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)      406 2023-06-19 20:38:30.000000 freefang-server-0.2.1/freefang/example.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     5233 2023-07-01 13:16:28.000000 freefang-server-0.2.1/freefang/main.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     9735 2023-07-01 13:16:38.000000 freefang-server-0.2.1/freefang/models.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     1101 2023-07-01 13:16:53.000000 freefang-server-0.2.1/freefang/net.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     3015 2023-06-26 22:17:49.000000 freefang-server-0.2.1/freefang/packets.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     4594 2023-07-01 13:16:48.000000 freefang-server-0.2.1/freefang/roles.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)      551 2023-06-22 13:21:38.000000 freefang-server-0.2.1/freefang/utils.py
--rw-r--r--   0 aaron     (1000) aaron     (1000)     1775 2023-06-30 15:21:44.000000 freefang-server-0.2.1/freefang/voting.py
-drwxr-xr-x   0 aaron     (1000) aaron     (1000)        0 2023-07-02 12:01:08.256485 freefang-server-0.2.1/freefang_server.egg-info/
--rw-r--r--   0 aaron     (1000) aaron     (1000)     2415 2023-07-02 12:01:08.000000 freefang-server-0.2.1/freefang_server.egg-info/PKG-INFO
--rw-r--r--   0 aaron     (1000) aaron     (1000)      407 2023-07-02 12:01:08.000000 freefang-server-0.2.1/freefang_server.egg-info/SOURCES.txt
--rw-r--r--   0 aaron     (1000) aaron     (1000)        1 2023-07-02 12:01:08.000000 freefang-server-0.2.1/freefang_server.egg-info/dependency_links.txt
--rw-r--r--   0 aaron     (1000) aaron     (1000)       55 2023-07-02 12:01:08.000000 freefang-server-0.2.1/freefang_server.egg-info/entry_points.txt
--rw-r--r--   0 aaron     (1000) aaron     (1000)        9 2023-07-02 12:01:08.000000 freefang-server-0.2.1/freefang_server.egg-info/top_level.txt
--rw-r--r--   0 aaron     (1000) aaron     (1000)      716 2023-07-02 11:57:44.000000 freefang-server-0.2.1/pyproject.toml
--rw-r--r--   0 aaron     (1000) aaron     (1000)       38 2023-07-02 12:01:08.256485 freefang-server-0.2.1/setup.cfg
--rw-r--r--   0 aaron     (1000) aaron     (1000)      344 2023-07-01 13:09:14.000000 freefang-server-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:49.497880 freefang-server-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 20:32:36.000000 freefang-server-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-03 20:32:49.497880 freefang-server-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-03 20:32:36.000000 freefang-server-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:49.497880 freefang-server-0.3.0/freefang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-03 20:32:36.000000 freefang-server-0.3.0/freefang/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:49.497880 freefang-server-0.3.0/freefang_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-03 20:32:49.000000 freefang-server-0.3.0/freefang_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 20:32:49.000000 freefang-server-0.3.0/freefang_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:32:49.000000 freefang-server-0.3.0/freefang_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 20:32:49.000000 freefang-server-0.3.0/freefang_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 20:32:49.000000 freefang-server-0.3.0/freefang_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-03 20:32:36.000000 freefang-server-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:32:49.497880 freefang-server-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-03 20:32:36.000000 freefang-server-0.3.0/setup.py
```

### Comparing `freefang-server-0.2.1/LICENSE` & `freefang-server-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freefang-server-0.2.1/PKG-INFO` & `freefang-server-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.2.1
+Version: 0.3.0
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,28 +20,35 @@
 This game opposes two sides, the werewolves (minority) and the town (majority).
 The goal of the town is to exterminate the werewolves and the goal of the werewolves is to reach numerical parity with the town.
 The game happens in a cycle of night and day. During the night roles with different powers (such as finding out the role of another player) wake up and the werewolves vote to kill one non-werewolf.
 During the day the town (with the werewolves hidden among them) vote to kill one player which they suspect to be a werewolf. The town does not know who the werewolves are and rely on clues/info given to them by the different roles.
 
 This game is about social deduction, lying, persuasion, finding and using clues, etc.
 
+# Getting started
+The FreeFang server is available on pypi as `freefang-server`.  
+To get started with hosting simply run  
+
+`python -m pip install freefang-server`  
+`freefang-server`  
+
+For all the options available run `freefang-server -h`
 # Features
 
 - Full werewolf experience with quite a few roles to pick from.  
 - No moderator needed, the server takes care of everything from role attribution to voting to role actions.  
 - Create a custom ruleset on game creation with only the roles you want and more custom options!.  
 - No signup, enter a server, game id, pick a name and you're good.  
-- Selfhostable, git clone, run freefang/main.py, done. No dependencies. Very simple to get started with.
+- Selfhostable, very simple to get started with.
 
 
 # Clients
 
 [freefang-qt](https://github.com/FreeFangGame/freefang-qt) is the reference client written by the devs.
 You are free to write your own and PR to have it added here, full protocol documentation is coming.
 
 
-
 # Protocol documentation
 
 Full protocol documentation in PROTOCOL.md with examples and complete descriptions.
```

### Comparing `freefang-server-0.2.1/README.md` & `freefang-server-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,35 @@
 This game opposes two sides, the werewolves (minority) and the town (majority).
 The goal of the town is to exterminate the werewolves and the goal of the werewolves is to reach numerical parity with the town.
 The game happens in a cycle of night and day. During the night roles with different powers (such as finding out the role of another player) wake up and the werewolves vote to kill one non-werewolf.
 During the day the town (with the werewolves hidden among them) vote to kill one player which they suspect to be a werewolf. The town does not know who the werewolves are and rely on clues/info given to them by the different roles.
 
 This game is about social deduction, lying, persuasion, finding and using clues, etc.
 
+# Getting started
+The FreeFang server is available on pypi as `freefang-server`.  
+To get started with hosting simply run  
+
+`python -m pip install freefang-server`  
+`freefang-server`  
+
+For all the options available run `freefang-server -h`
 # Features
 
 - Full werewolf experience with quite a few roles to pick from.  
 - No moderator needed, the server takes care of everything from role attribution to voting to role actions.  
 - Create a custom ruleset on game creation with only the roles you want and more custom options!.  
 - No signup, enter a server, game id, pick a name and you're good.  
-- Selfhostable, git clone, run freefang/main.py, done. No dependencies. Very simple to get started with.
+- Selfhostable, very simple to get started with.
 
 
 # Clients
 
 [freefang-qt](https://github.com/FreeFangGame/freefang-qt) is the reference client written by the devs.
 You are free to write your own and PR to have it added here, full protocol documentation is coming.
 
 
-
 # Protocol documentation
 
 Full protocol documentation in PROTOCOL.md with examples and complete descriptions.
```

### Comparing `freefang-server-0.2.1/freefang/main.py` & `freefang-server-0.3.0/freefang/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import time
 import struct 
 import argparse
 import ssl
 import os
 
 VERSIONSTR = """
-FreeFang Server 0.2.1
+FreeFang Server 0.3.0
 Written by @Solirs and @lukakralik
 Licensed under AGPLv3.0
 Source code at https://github.com/FreeFangGame/freefang-server
 """
 
 def parse_ruleset(ruleset, game):
 	if ruleset.town_voting_scheme:
@@ -65,14 +65,16 @@
 	print(f"Listening on {args.addr}:{args.port}")
 	
 	inputs = [s]
 	outputs = []
 	
 	connections = {} # Associating connections to players
 	
+	write = 0
+	read = 0
 	
 	while True:
 		time.sleep(0.05)
 		read, write, excp = select.select(inputs, outputs, inputs)
 		
 		for i in read:
 			if i is s:
@@ -116,14 +118,18 @@
 					
 					# Game joining
 					elif packet.action == "game_join":
 						if not games.get(packet.headers.gameid): # If the game for the proposed gameid doesn't exist
 							net.send_packet(utils.obj_to_json(packets.Action_failure(error="game_not_found")), i)
 						else:
 							game = games[packet.headers.gameid]
+
+							if packet.headers.name in [s.name for s in game.players]:
+								net.send_failure(i, "name_already_taken")
+								continue
 								
 							p = models.Player()
 							p.name = packet.headers.name
 							p.connection = i
 							connections[i] = p
 							p.game = game
 							for spl in game.players:
@@ -144,19 +150,24 @@
 						for spl in sender.game.players:
 							net.send_message(sender.name, packet.headers.message, spl.connection)
 								
 				except Exception as e:
 					print(e)
 					inputs.remove(i)
 					outputs.remove(i)
+					read.remove(i)
+					write.remove(i)
 					player = connections[i]
 					if player:
 						player.game.players.remove(player)
 						for spl in player.game.players:
-							net.send_packet(utils.obj_to_json(packets.Player_leave(username=player.name)), spl.connection)
+							try:
+								net.send_packet(utils.obj_to_json(packets.Player_leave(username=player.name)), spl.connection)
+							except:
+								continue
 					del connections[i]
 						
 				
 def main():
 	parser = argparse.ArgumentParser()
 	parser.add_argument("-v", "--version", help="Show version", action="store_true")
```

### Comparing `freefang-server-0.2.1/freefang/models.py` & `freefang-server-0.3.0/freefang/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,32 @@
 
 
 except ImportError:
 	from roles import *
 	import net as fn
 	import packets
 	import utils
+	
 
 
 class Player:
 	def __init__(self):
 		self.role = None
 		self.alive = True
 		self.name = ""
 		self.connection = 0
 		self.voted_by = 0 # Number of people who voted for this player
 		self.voted = False
 		self.time = 0 # 0 = Night, 1 = Day
 		self.protected = None # name of the protected player
 		self.game = None
+
+		#Witch stuff
+		self.haskilled = 0
+		self.hasrevived = 0
 	def iswerewolf(self):
 		return issubclass(self.role, Werewolf) and self.alive
 			
 
 
 class WWgame:
 	def __init__(self):
@@ -37,18 +42,20 @@
 		self.dead = []
 		self.playercap = 0
 		self.werewolves = []
 		self.villagers = []
 		self.socket = 0
 		self.inputs = []
 		self.outputs = []
+		self.read = []
+		self.write = []
 		self.msgqueues = {}
 		self.nightroles = [] # Roles that should be woken up at night, in order
 		self.up = 0 # The current role which is woken up, 0 if day.
-		self.action_to_function = {"werewolf_vote": Werewolf.vote, "town_vote": Villager.vote, "town_message": self.townmessage, "werewolf_message": self.werewolfmessage, "hunter_kill": Hunter.kill, "seer_reveal":Seer.reveal, "protector_protect": Protector.protect}
+		self.action_to_function = {"werewolf_vote": Werewolf.vote, "town_vote": Villager.vote, "town_message": self.townmessage, "werewolf_message": self.werewolfmessage, "hunter_kill": Hunter.kill, "seer_reveal":Seer.reveal, "protector_protect": Protector.protect, "witch_kill": Witch.kill, "witch_revive": Witch.revive}
 		self.votes = []
 		self.connections = {} # Dictionnary associating connections to players
 
 		self.roles = {} # The number of players for each role should be decided by the client upon game creation and should be implemented alongside the protocol
 		
 		self.town_voting_scheme = "absmaj"
 		self.werewolf_voting_scheme = "relmaj"
@@ -96,22 +103,24 @@
 	def update_player_count(self):
 		num_players = len(self.players)
 		print(f"Number of present players: {num_players}")
 	
 	def remove_player(self, i):
 		self.inputs.remove(i)
 		self.outputs.remove(i)
+		self.read.remove(i)
+		self.write.remove(i)
 		player = self.connections[i]
 		self.players.remove(player)
 		if player in self.villagers:
 			self.villagers.remove(player)
 		elif player in self.werewolves:
 			self.werewolves.remove(player)
 		for spl in self.players:
-			fn.send_packet(utils.obj_to_json(packets.Player_leave(username=player.name)), spl.connection)
+			self.send_packet(utils.obj_to_json(packets.Player_leave(username=player.name)), spl.connection)
 
 						
 		print(f"{player.name} disconnected")
 		
 	
 	# This function checks if the conditions for game end are met
 	def game_continues(self):
@@ -120,23 +129,23 @@
 		
 	def kill_player(self, player, reason=None):
 		
 		# If the player is protected we do nothing. 
 		if player.protected:
 			return 1
 		print(player.name + " died")
-		player.alive = False
 
 		
 		# If the player died during the night we keep it in a list to notify the other players when the day rises
 		# Otherwise we just send the packet right away
 		if self.up != 0 and self.up != Hunter:
 			self.nightdeaths.append(player)
 			return 0
-			
+		player.alive = False
+
 		
 		# Notify everyone that player died
 		event = packets.Player_death(name=player.name, role=player.role.__name__, reason=reason)
 		
 		self.sendall(utils.obj_to_json(event))
 		
 		# Remove player from various lists reserved to living players
@@ -174,35 +183,40 @@
 			self.msgqueues.setdefault(i, [])
 			self.msgqueues[i].append(string)
 
 	def queuewerewolves(self, string): # Send a message to all wolves
 		for i in self.werewolves:				
 			self.msgqueues.setdefault(i.connection, [])
 			self.msgqueues[i.connection].append(string)
+
 				
 	# Those two functions instantly send a packet to their destined targets, either all players or all werewolves
 	def sendall(self, string):
 		for i in self.players:
 			self.send_packet(string, i.connection)
 			
 	def sendwerewolves(self, string):
 		for i in self.werewolves:
 			self.send_packet(string,i.connection)
-			
+	def sendrole(self, string, role):
+		for i in self.alive:
+			if i.role == role:
+				self.send_packet(string, i.connection)
+				
 
 	def getplayerbyname(self, name):
 		return [i for i in self.players if i.name == name][0]
 		
 	def eventloop(self): 
 		end = None
-		while not end: # This loop will eventually be broken, can be while true.
+		while not end and len(self.players) > 1: # This loop will eventually be broken, can be while true.
 			time.sleep(0.05)
 
-			read, write, exceptional = select.select(self.inputs, self.outputs, self.inputs)
-			for i in read: # Check every connection that has sent a message
+			self.read, self.write, exceptional = select.select(self.inputs, self.outputs, self.inputs)
+			for i in self.read: # Check every connection that has sent a message
 				try:
 						
 					packet = fn.read_packet(i)
 					if not packet:
 						fn.send_packet("", i)
 
 						continue
@@ -227,15 +241,15 @@
 						traceback.print_exc()
 						fn.send_failure(i, error=None)
 				except:
 					self.remove_player(i)
 					
 
 
-			for i in write:
+			for i in self.write:
 				if self.msgqueues.get(i): # If a message is pending for a player send it to them
 					for x in self.msgqueues[i]:
 						self.send_packet(x, i)
 					del self.msgqueues[i] # No more message needed to send
 					
 				else:
 					continue
@@ -271,14 +285,19 @@
 
 		while self.game_continues(): 
 			# Game should go on as long as there are villagers and werewolves, keeping the day night cycle
 			self.sendall(utils.obj_to_json(packets.Time_change(time="night"))) # Notify everyone night has fallen
 			for i in self.nightroles:
 				self.queueall(utils.obj_to_json(packets.Role_wakeup(role=i.__name__))) # Notify everyone role has woken up
 				self.up = i
+				# Run the role's wake up event function
+				try:
+					i.onwakeup(self)
+				except:
+					pass
 				self.eventloop()
 			
 			# Remove all protections 
 			for player in self.players:
 				player.protected = None
 			self.sendall(utils.obj_to_json(packets.Time_change(time="day"))) # Notify everyone day has risen
 			self.up = 0
```

### Comparing `freefang-server-0.2.1/freefang/net.py` & `freefang-server-0.3.0/freefang/net.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.2.1/freefang/packets.py` & `freefang-server-0.3.0/freefang/packets.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,8 +123,14 @@
 	def __init__(self):
 		self.action = "town_vote_begin"
 
 class Check_alive:
 	def __init__(self):
 		self.action = "check_alive"
 	
-
+# This packet is supposed to be sent to the witch upon wakeup to
+# Notify them of the players which have died during the night
+class Witch_send_dead:
+	def __init__(self, players):
+		self.action = "witch_send_dead"
+		self.dead = players
+
```

### Comparing `freefang-server-0.2.1/freefang/roles.py` & `freefang-server-0.3.0/freefang/roles.py`

 * *Files 16% similar despite different names*

```diff
@@ -146,14 +146,45 @@
     
 		# if both protector and target are alive, modify the headers
 		if headers.sender.alive and target.alive and game.up == Protector:
 			target.protected = True
 			return 2
 		return 1
 
+# The witch can kill and revive one player per game who died during the night.
+# She is supposed to wake up last as she can only revive people who died during each night she wakes up in
+class Witch(Role):
+	nightrole = 1
+	order = 4
+	@staticmethod
+	def kill(headers, game, connection):
+		target = game.getplayerbyname(headers.target)
+		if game.up == Witch and headers.sender.role == Witch and not headers.sender.haskilled and target.alive:
+			game.kill_player(target)
+			headers.sender.haskilled = 1
+			return 2
+		else:
+			return 1
+	@staticmethod
+	def revive(headers, game, connection):
+		target = game.getplayerbyname(headers.target)
+		if game.up == Witch and headers.sender.role == Witch and not headers.sender.hasrevived and target in game.nightdeaths:
+			# The witch can only save people who died during the night she wakes up, therefore removing them
+			# from the nightdeaths list is what we want
+			game.nightdeaths.remove(target)
+			headers.sender.hasrevived = 1
+			return 2
+		else:
+			return 1
+	@staticmethod
+	def onwakeup(game):
+		dead = [i.name for i in game.nightdeaths]
+		event = utils.obj_to_json(packets.Witch_send_dead(dead))
+		game.sendrole(event, Witch)
+
 class Vote:
     def __init__(self, target, sender):
         self.sender = sender
         self.target = target
 
 class TownVote(Vote):
     def __init__(self, target, sender):
```

### Comparing `freefang-server-0.2.1/freefang/utils.py` & `freefang-server-0.3.0/freefang/utils.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.2.1/freefang/voting.py` & `freefang-server-0.3.0/freefang/voting.py`

 * *Files identical despite different names*

### Comparing `freefang-server-0.2.1/freefang_server.egg-info/PKG-INFO` & `freefang-server-0.3.0/freefang_server.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-server
-Version: 0.2.1
+Version: 0.3.0
 Summary: The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)
 Author: FreeFang Development Team
 Author-email: Solaris <iusegentoobtw@protonmail.com>, lukakralik <luka.kralik@gmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-server
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,28 +20,35 @@
 This game opposes two sides, the werewolves (minority) and the town (majority).
 The goal of the town is to exterminate the werewolves and the goal of the werewolves is to reach numerical parity with the town.
 The game happens in a cycle of night and day. During the night roles with different powers (such as finding out the role of another player) wake up and the werewolves vote to kill one non-werewolf.
 During the day the town (with the werewolves hidden among them) vote to kill one player which they suspect to be a werewolf. The town does not know who the werewolves are and rely on clues/info given to them by the different roles.
 
 This game is about social deduction, lying, persuasion, finding and using clues, etc.
 
+# Getting started
+The FreeFang server is available on pypi as `freefang-server`.  
+To get started with hosting simply run  
+
+`python -m pip install freefang-server`  
+`freefang-server`  
+
+For all the options available run `freefang-server -h`
 # Features
 
 - Full werewolf experience with quite a few roles to pick from.  
 - No moderator needed, the server takes care of everything from role attribution to voting to role actions.  
 - Create a custom ruleset on game creation with only the roles you want and more custom options!.  
 - No signup, enter a server, game id, pick a name and you're good.  
-- Selfhostable, git clone, run freefang/main.py, done. No dependencies. Very simple to get started with.
+- Selfhostable, very simple to get started with.
 
 
 # Clients
 
 [freefang-qt](https://github.com/FreeFangGame/freefang-qt) is the reference client written by the devs.
 You are free to write your own and PR to have it added here, full protocol documentation is coming.
 
 
-
 # Protocol documentation
 
 Full protocol documentation in PROTOCOL.md with examples and complete descriptions.
```

### Comparing `freefang-server-0.2.1/pyproject.toml` & `freefang-server-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name  = "freefang-server"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Solaris", email="iusegentoobtw@protonmail.com" },
   { name="lukakralik", email="luka.kralik@gmail.com"}
 ]
 description = "The server for FreeFang, a libre python implementation of Werewolf (also known as Mafia)"
 readme = "README.md"
 classifiers = [
```

