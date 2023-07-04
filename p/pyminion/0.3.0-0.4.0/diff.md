# Comparing `tmp/pyminion-0.3.0.tar.gz` & `tmp/pyminion-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyminion-0.3.0.tar", last modified: Sun Feb  5 22:25:20 2023, max compression
+gzip compressed data, was "pyminion-0.4.0.tar", last modified: Tue Jul  4 17:44:21 2023, max compression
```

## Comparing `pyminion-0.3.0.tar` & `pyminion-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.874788 pyminion-0.3.0/
--rw-r--r--   0 eslack     (503) staff       (20)     1066 2023-01-31 02:16:15.000000 pyminion-0.3.0/LICENSE
--rw-r--r--   0 eslack     (503) staff       (20)     4345 2023-02-05 22:25:20.874635 pyminion-0.3.0/PKG-INFO
--rw-r--r--   0 eslack     (503) staff       (20)     3917 2023-01-31 02:16:15.000000 pyminion-0.3.0/README.md
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.871830 pyminion-0.3.0/pyminion/
--rw-r--r--   0 eslack     (503) staff       (20)      243 2023-02-05 06:11:43.000000 pyminion-0.3.0/pyminion/__init__.py
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.872799 pyminion-0.3.0/pyminion/bots/
--rw-r--r--   0 eslack     (503) staff       (20)        0 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/__init__.py
--rw-r--r--   0 eslack     (503) staff       (20)     6067 2023-02-02 03:43:16.000000 pyminion-0.3.0/pyminion/bots/bot.py
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.873804 pyminion-0.3.0/pyminion/bots/examples/
--rw-r--r--   0 eslack     (503) staff       (20)      335 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/examples/__init__.py
--rw-r--r--   0 eslack     (503) staff       (20)     1863 2023-02-02 03:27:27.000000 pyminion-0.3.0/pyminion/bots/examples/bandit_bot.py
--rw-r--r--   0 eslack     (503) staff       (20)      664 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/examples/big_money.py
--rw-r--r--   0 eslack     (503) staff       (20)      710 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/examples/big_money_smithy.py
--rw-r--r--   0 eslack     (503) staff       (20)     1636 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/examples/big_money_ultimate.py
--rw-r--r--   0 eslack     (503) staff       (20)     1498 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/bots/examples/chapel_bot.py
--rw-r--r--   0 eslack     (503) staff       (20)    12520 2023-02-02 03:38:26.000000 pyminion-0.3.0/pyminion/bots/optimized_bot.py
--rw-r--r--   0 eslack     (503) staff       (20)     6001 2023-02-02 03:39:07.000000 pyminion-0.3.0/pyminion/core.py
--rw-r--r--   0 eslack     (503) staff       (20)     3790 2023-02-02 03:38:26.000000 pyminion-0.3.0/pyminion/decisions.py
--rw-r--r--   0 eslack     (503) staff       (20)     1323 2023-02-02 03:38:26.000000 pyminion-0.3.0/pyminion/exceptions.py
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.874406 pyminion-0.3.0/pyminion/expansions/
--rw-r--r--   0 eslack     (503) staff       (20)        0 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/expansions/__init__.py
--rw-r--r--   0 eslack     (503) staff       (20)    43398 2023-02-02 04:43:28.000000 pyminion-0.3.0/pyminion/expansions/base.py
--rw-r--r--   0 eslack     (503) staff       (20)       36 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/expansions/intrigue.py
--rw-r--r--   0 eslack     (503) staff       (20)       26 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyminion/expansions/seaside.py
--rw-r--r--   0 eslack     (503) staff       (20)    10267 2023-02-05 05:33:59.000000 pyminion-0.3.0/pyminion/game.py
--rw-r--r--   0 eslack     (503) staff       (20)    14458 2023-02-04 10:39:54.000000 pyminion-0.3.0/pyminion/players.py
--rw-r--r--   0 eslack     (503) staff       (20)     2559 2023-02-05 05:36:43.000000 pyminion-0.3.0/pyminion/result.py
--rw-r--r--   0 eslack     (503) staff       (20)     2382 2023-02-05 04:10:12.000000 pyminion-0.3.0/pyminion/simulator.py
-drwxr-xr-x   0 eslack     (503) staff       (20)        0 2023-02-05 22:25:20.872379 pyminion-0.3.0/pyminion.egg-info/
--rw-r--r--   0 eslack     (503) staff       (20)     4345 2023-02-05 22:25:20.000000 pyminion-0.3.0/pyminion.egg-info/PKG-INFO
--rw-r--r--   0 eslack     (503) staff       (20)      764 2023-02-05 22:25:20.000000 pyminion-0.3.0/pyminion.egg-info/SOURCES.txt
--rw-r--r--   0 eslack     (503) staff       (20)        1 2023-02-05 22:25:20.000000 pyminion-0.3.0/pyminion.egg-info/dependency_links.txt
--rw-r--r--   0 eslack     (503) staff       (20)        9 2023-02-05 22:25:20.000000 pyminion-0.3.0/pyminion.egg-info/top_level.txt
--rw-r--r--   0 eslack     (503) staff       (20)       92 2023-01-31 02:16:15.000000 pyminion-0.3.0/pyproject.toml
--rw-r--r--   0 eslack     (503) staff       (20)       38 2023-02-05 22:25:20.874838 pyminion-0.3.0/setup.cfg
--rw-r--r--   0 eslack     (503) staff       (20)      789 2023-02-05 06:11:25.000000 pyminion-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.270979 pyminion-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-04 17:44:04.000000 pyminion-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-04 17:44:21.270979 pyminion-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-04 17:44:04.000000 pyminion-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.262979 pyminion-0.4.0/pyminion/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.266979 pyminion-0.4.0/pyminion/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.266979 pyminion-0.4.0/pyminion/bots/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/bandit_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/big_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/big_money_smithy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/big_money_ultimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/examples/chapel_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42388 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/bots/optimized_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/decider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.270979 pyminion-0.4.0/pyminion/expansions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/expansions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34792 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/expansions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39709 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/expansions/intrigue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/expansions/seaside.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/human.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyminion/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:44:21.266979 pyminion-0.4.0/pyminion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-04 17:44:21.000000 pyminion-0.4.0/pyminion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 17:44:21.000000 pyminion-0.4.0/pyminion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:44:21.000000 pyminion-0.4.0/pyminion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 17:44:21.000000 pyminion-0.4.0/pyminion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-04 17:44:04.000000 pyminion-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:44:21.270979 pyminion-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-04 17:44:04.000000 pyminion-0.4.0/setup.py
```

### Comparing `pyminion-0.3.0/LICENSE` & `pyminion-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyminion-0.3.0/PKG-INFO` & `pyminion-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyminion
-Version: 0.3.0
+Version: 0.4.0
 Summary: Dominion but make it python
 Home-page: https://github.com/evanofslack/pyminion
 Author: Evan Slack
 Author-email: evan.slack@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,120 +13,145 @@
 License-File: LICENSE
 
 # Pyminion
 
 [![tests](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml/badge.svg)](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/evanofslack/pyminion/branch/master/graph/badge.svg?token=5GW65KFEL5)](https://codecov.io/gh/evanofslack/pyminion)
 
+<img width="800" alt="pyminion-logo" src="https://github.com/evanofslack/pyminion/assets/51209817/85e6ed9f-8cbf-4781-9c0b-f29c1d0a2162">
+<br></br>
 
-Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/). At its core, pyminion implements the rules and logic of Dominion and provides an API to interact with the game engine. In addition, it enables interactive games through the command line and simulation of games between bots.
+Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/).
+At its core, pyminion implements the rules and logic of Dominion and provides
+an API to interact with the game engine. In addition, it enables interactive
+games through the command line and simulation of games between bots.
 
 ## Table of Contents
 
--   [Installation](#installation)
--   [Usage](#usage)
--   [Support](#support)
--   [Contributing](#contributing)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [Contributing](#contributing)
 
-## Getting Started
+## Installation
 
 Pyminion requires at least Python 3.8 and can easily be installed through pypi
 
-```
+```bash
 python3 -m pip install pyminion
 ```
 
 ## Usage
 
 ### Setting up a game
 
-To play an interactive game through the command line against a bot, initialize a human and a bot and assign them as players. Alternatively, games can be created between multiple humans or multiple bots. 
+To play an interactive game through the command line against a bot, initialize
+a human and a bot and assign them as players. Alternatively, games can be
+created between multiple humans or multiple bots.
 
 ```python
-from pyminion.expansions.base import base_set 
+from pyminion.expansions.base import base_set
+from pyminion.expansions.intrigue import intrigue_set
 from pyminion.game import Game
 from pyminion.bots.examples import BigMoney
-from pyminion.players import Human
+from pyminion.human import Human
 
 # Initialize human and bot
 human = Human()
 bot = BigMoney()
 
 # Setup the game
-game = Game(players=[human, bot], expansions=[base_set])
+game = Game(players=[human, bot], expansions=[base_set, intrigue_set])
 
 # Play game
 game.play()
 
 ```
+
 ### Creating Bots
 
-Defining new bots is relatively straightforward. Inherit from the `Bot` class and implement play and buy strategies in the `action_priority` and `buy_priority` methods respectively.
+Defining new bots is relatively straightforward. Inherit from the
+`BotDecider` class and implement play and buy strategies in the
+`action_priority` and `buy_priority` methods respectively.
 
 For example, here is a simple big money + smithy bot:
 
 ```python
-from pyminion.bots.bot import Bot
+from pyminion.bots.bot import Bot, BotDecider
+from pyminion.expansions.base import gold, province, silver, smithy
+from pyminion.player import Player
 from pyminion.game import Game
-from pyminion.expansions.base import silver, gold, province, smithy
 
-class BigMoneySmithy(Bot):
+class BigMoneySmithyDecider(BotDecider):
+    """
+    Big money + smithy
 
-    def __init__(
-        self,
-        player_id: str = "big_money_smithy",
-    ):
-        super().__init__(player_id=player_id)
+    """
 
-    def action_priority(self, game: Game):
+    def action_priority(self, player: Player, game: Game):
         yield smithy
 
-    def buy_priority(self, game: Game):
-        money = self.state.money
+    def buy_priority(self, player: Player, game: Game):
+        money = player.state.money
         if money >= 8:
             yield province
         if money >= 6:
             yield gold
         if money == 4:
             yield smithy
         if money >= 3:
             yield silver
+
+class BigMoneySmithy(Bot):
+    def __init__(
+        self,
+        player_id: str = "big_money_smithy",
+    ):
+        super().__init__(decider=BigMoneySmithyDecider(), player_id=player_id)
 ```
 
 To see other bot implementations with more advanced decision trees, see [/bots](https://github.com/evanofslack/pyminion/tree/master/pyminion/bots)
 
 ### Running Simulations
 
-Simulating multiple games is good metric for determining bot performance. To create a simulation, pass a pyminion game instance into the `Simulator` class and set the number of iterations to be run. 
+Simulating multiple games is good metric for determining bot performance.
+To create a simulation, pass a pyminion game instance into the `Simulator`
+class and set the number of iterations to be run.
 
 ```python
 from pyminion.bots.examples import BigMoney, BigMoneySmithy
 from pyminion.expansions.base import base_set, smithy
 from pyminion.game import Game
 from pyminion.simulator import Simulator
 
 bm = BigMoney()
 bm_smithy = BigMoneySmithy()
 
-game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy])
+game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy], log_stdout=False)
 sim = Simulator(game, iterations=1000)
-sim.run()
+result = sim.run()
+print(result)
 ```
 
-with the following terminal output: 
+with the following terminal output:
+
 ```console
 ~$ python simulation.py
-Simulation of 1000 games
-big_money wins: 16.8% (168)
-big_money_smithy wins: 57.5% (575)
-Ties: 25.7% (257)
+Simulation Result: ran 1000 games
+big_money won 110, lost 676, tied 214
+big_money_smithy won 676, lost 110, tied 214
 ```
-Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.  
+
+Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.
+
 ## Support
 
 Please [open an issue](https://github.com/evanofslack/pyminion/issues/new) for support.
 
 ## Contributing
 
-Install this library, test it out, and report any bugs. A welcome contribution would be to create new bots, especially an implementation that uses machine learning to determine optimal play. 
+Install this library, test it out, and report any bugs. A welcome contribution
+would be to create new bots, especially an implementation that uses machine
+learning to determine optimal play.
 
-If you would like to contribute, please create a branch, add commits, and [open a pull request](https://github.com/evanofslack/pyminion/pulls).
+If you would like to contribute, please create a branch, add commits, and
+[open a pull request](https://github.com/evanofslack/pyminion/pulls).
```

### Comparing `pyminion-0.3.0/README.md` & `pyminion-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,143 @@
 # Pyminion
 
 [![tests](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml/badge.svg)](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/evanofslack/pyminion/branch/master/graph/badge.svg?token=5GW65KFEL5)](https://codecov.io/gh/evanofslack/pyminion)
 
+<img width="800" alt="pyminion-logo" src="https://github.com/evanofslack/pyminion/assets/51209817/85e6ed9f-8cbf-4781-9c0b-f29c1d0a2162">
+<br></br>
 
-Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/). At its core, pyminion implements the rules and logic of Dominion and provides an API to interact with the game engine. In addition, it enables interactive games through the command line and simulation of games between bots.
+Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/).
+At its core, pyminion implements the rules and logic of Dominion and provides
+an API to interact with the game engine. In addition, it enables interactive
+games through the command line and simulation of games between bots.
 
 ## Table of Contents
 
--   [Installation](#installation)
--   [Usage](#usage)
--   [Support](#support)
--   [Contributing](#contributing)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [Contributing](#contributing)
 
-## Getting Started
+## Installation
 
 Pyminion requires at least Python 3.8 and can easily be installed through pypi
 
-```
+```bash
 python3 -m pip install pyminion
 ```
 
 ## Usage
 
 ### Setting up a game
 
-To play an interactive game through the command line against a bot, initialize a human and a bot and assign them as players. Alternatively, games can be created between multiple humans or multiple bots. 
+To play an interactive game through the command line against a bot, initialize
+a human and a bot and assign them as players. Alternatively, games can be
+created between multiple humans or multiple bots.
 
 ```python
-from pyminion.expansions.base import base_set 
+from pyminion.expansions.base import base_set
+from pyminion.expansions.intrigue import intrigue_set
 from pyminion.game import Game
 from pyminion.bots.examples import BigMoney
-from pyminion.players import Human
+from pyminion.human import Human
 
 # Initialize human and bot
 human = Human()
 bot = BigMoney()
 
 # Setup the game
-game = Game(players=[human, bot], expansions=[base_set])
+game = Game(players=[human, bot], expansions=[base_set, intrigue_set])
 
 # Play game
 game.play()
 
 ```
+
 ### Creating Bots
 
-Defining new bots is relatively straightforward. Inherit from the `Bot` class and implement play and buy strategies in the `action_priority` and `buy_priority` methods respectively.
+Defining new bots is relatively straightforward. Inherit from the
+`BotDecider` class and implement play and buy strategies in the
+`action_priority` and `buy_priority` methods respectively.
 
 For example, here is a simple big money + smithy bot:
 
 ```python
-from pyminion.bots.bot import Bot
+from pyminion.bots.bot import Bot, BotDecider
+from pyminion.expansions.base import gold, province, silver, smithy
+from pyminion.player import Player
 from pyminion.game import Game
-from pyminion.expansions.base import silver, gold, province, smithy
 
-class BigMoneySmithy(Bot):
+class BigMoneySmithyDecider(BotDecider):
+    """
+    Big money + smithy
 
-    def __init__(
-        self,
-        player_id: str = "big_money_smithy",
-    ):
-        super().__init__(player_id=player_id)
+    """
 
-    def action_priority(self, game: Game):
+    def action_priority(self, player: Player, game: Game):
         yield smithy
 
-    def buy_priority(self, game: Game):
-        money = self.state.money
+    def buy_priority(self, player: Player, game: Game):
+        money = player.state.money
         if money >= 8:
             yield province
         if money >= 6:
             yield gold
         if money == 4:
             yield smithy
         if money >= 3:
             yield silver
+
+class BigMoneySmithy(Bot):
+    def __init__(
+        self,
+        player_id: str = "big_money_smithy",
+    ):
+        super().__init__(decider=BigMoneySmithyDecider(), player_id=player_id)
 ```
 
 To see other bot implementations with more advanced decision trees, see [/bots](https://github.com/evanofslack/pyminion/tree/master/pyminion/bots)
 
 ### Running Simulations
 
-Simulating multiple games is good metric for determining bot performance. To create a simulation, pass a pyminion game instance into the `Simulator` class and set the number of iterations to be run. 
+Simulating multiple games is good metric for determining bot performance.
+To create a simulation, pass a pyminion game instance into the `Simulator`
+class and set the number of iterations to be run.
 
 ```python
 from pyminion.bots.examples import BigMoney, BigMoneySmithy
 from pyminion.expansions.base import base_set, smithy
 from pyminion.game import Game
 from pyminion.simulator import Simulator
 
 bm = BigMoney()
 bm_smithy = BigMoneySmithy()
 
-game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy])
+game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy], log_stdout=False)
 sim = Simulator(game, iterations=1000)
-sim.run()
+result = sim.run()
+print(result)
 ```
 
-with the following terminal output: 
+with the following terminal output:
+
 ```console
 ~$ python simulation.py
-Simulation of 1000 games
-big_money wins: 16.8% (168)
-big_money_smithy wins: 57.5% (575)
-Ties: 25.7% (257)
+Simulation Result: ran 1000 games
+big_money won 110, lost 676, tied 214
+big_money_smithy won 676, lost 110, tied 214
 ```
-Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.  
+
+Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.
+
 ## Support
 
 Please [open an issue](https://github.com/evanofslack/pyminion/issues/new) for support.
 
 ## Contributing
 
-Install this library, test it out, and report any bugs. A welcome contribution would be to create new bots, especially an implementation that uses machine learning to determine optimal play. 
+Install this library, test it out, and report any bugs. A welcome contribution
+would be to create new bots, especially an implementation that uses machine
+learning to determine optimal play.
 
-If you would like to contribute, please create a branch, add commits, and [open a pull request](https://github.com/evanofslack/pyminion/pulls).
+If you would like to contribute, please create a branch, add commits, and
+[open a pull request](https://github.com/evanofslack/pyminion/pulls).
```

### Comparing `pyminion-0.3.0/pyminion/bots/examples/bandit_bot.py` & `pyminion-0.4.0/pyminion/bots/examples/big_money_ultimate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,60 @@
 import logging
 from typing import Iterator
 
-from pyminion.bots.optimized_bot import OptimizedBot
-from pyminion.core import Card
-from pyminion.expansions.base import (
-    bandit,
-    duchy,
-    estate,
-    gold,
-    province,
-    silver,
-    smithy,
-)
+from pyminion.bots.bot import Bot, BotDecider
+from pyminion.core import CardType, Card
+from pyminion.expansions.base import duchy, estate, gold, province, silver, smithy
+from pyminion.player import Player
 from pyminion.game import Game
 
 logger = logging.getLogger()
 
 
-class BanditBot(OptimizedBot):
+class BigMoneyUltimateDecider(BotDecider):
     """
     Attempt the following buys in order:
 
     Buy Province if total money in deck is > 15
     Buy Duchy if remaining Provinces < 5
     Buy Estate if remaining Provinces < 3
     Buy Gold
     Buy Duchy if remaining Provinces < 7
-    Buy Bandit if #Bandits < 1
     Buy Smithy if #Smithies < (#Treasures / 11)
     Buy Silver
 
     """
 
-    def __init__(
-        self,
-        player_id: str = "bandit_bot",
-    ):
-        super().__init__(player_id=player_id)
-
-    def action_priority(self, game: Game) -> Iterator[Card]:
-        yield bandit
+    def action_priority(self, player: "Player", game: "Game") -> Iterator[Card]:
         yield smithy
 
-    def buy_priority(self, game: Game) -> Iterator[Card]:
-
-        money = self.state.money
-        deck_money = self.get_deck_money()
+    def buy_priority(self, player: "Player", game: "Game") -> Iterator["Card"]:
+        money = player.state.money
+        deck_money = player.get_deck_money()
         num_province = game.supply.pile_length(pile_name="Province")
-        num_smithy = self.get_card_count(card=smithy)
-        num_bandit = self.get_card_count(card=bandit)
+        num_smithy = player.get_card_count(card=smithy)
         num_treasure = len(
-            [card for card in self.get_all_cards() if "Treasure" in card.type]
+            [card for card in player.get_all_cards() if CardType.Treasure in card.type]
         )
 
         if deck_money > 15 and money >= 8:
             yield province
         if num_province < 5 and money >= 5:
             yield duchy
         if num_province < 3 and money >= 2:
             yield estate
         if money >= 6:
             yield gold
         if num_province < 7 and money >= 5:
             yield duchy
-        if num_bandit < 1 and money >= 5:
-            yield bandit
         if num_smithy < num_treasure / 11 and money >= 4:
             yield smithy
         if money >= 3:
             yield silver
+
+
+class BigMoneyUltimate(Bot):
+    def __init__(
+        self,
+        player_id: str = "big_money_ultimate",
+    ):
+        super().__init__(decider=BigMoneyUltimateDecider(), player_id=player_id)
```

### Comparing `pyminion-0.3.0/pyminion/bots/examples/big_money.py` & `pyminion-0.4.0/pyminion/bots/examples/big_money_smithy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import logging
-from typing import Iterator
-
-from pyminion.bots.bot import Bot
-from pyminion.core import Card
-from pyminion.expansions.base import gold, province, silver
+from pyminion.bots.bot import Bot, BotDecider
+from pyminion.expansions.base import gold, province, silver, smithy
+from pyminion.player import Player
 from pyminion.game import Game
 
-logger = logging.getLogger()
-
 
-class BigMoney(Bot):
+class BigMoneySmithyDecider(BotDecider):
     """
-    Only buys money and provinces
+    Big money + smithy
 
     """
 
-    def __init__(
-        self,
-        player_id: str = "big_money",
-    ):
-        super().__init__(player_id=player_id)
+    def action_priority(self, player: Player, game: Game):
+        yield smithy
 
-    def buy_priority(self, game: Game) -> Iterator[Card]:
-        money = self.state.money
+    def buy_priority(self, player: Player, game: Game):
+        money = player.state.money
         if money >= 8:
             yield province
         if money >= 6:
             yield gold
+        if money == 4:
+            yield smithy
         if money >= 3:
             yield silver
+
+
+class BigMoneySmithy(Bot):
+    def __init__(
+        self,
+        player_id: str = "big_money_smithy",
+    ):
+        super().__init__(decider=BigMoneySmithyDecider(), player_id=player_id)
```

### Comparing `pyminion-0.3.0/pyminion/bots/examples/chapel_bot.py` & `pyminion-0.4.0/pyminion/bots/examples/chapel_bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-import logging
 from typing import Iterator
 
-from pyminion.bots.optimized_bot import OptimizedBot
+from pyminion.bots.optimized_bot import OptimizedBot, OptimizedBotDecider
 from pyminion.core import Card
 from pyminion.expansions.base import chapel, duchy, estate, gold, province, silver
+from pyminion.player import Player
 from pyminion.game import Game
 
-logger = logging.getLogger()
-
-
-class ChapelBot(OptimizedBot):
+class ChapelBotDecider(OptimizedBotDecider):
     """
     Attempt the following buys in order:
 
     Buy Chapel if #Chapel < 1
     Buy Province if total money in deck is > 15
     Buy Duchy if remaining Provinces < 5
     Buy Estate if remaining Provinces < 3
     Buy Gold
     Buy Duchy if remaining Provinces < 7
     Buy Silver
 
     """
 
-    def __init__(
-        self,
-        player_id: str = "chapel_bot",
-    ):
-        super().__init__(player_id=player_id)
-
-    def action_priority(self, game: Game) -> Iterator[Card]:
+    def action_priority(self, player: Player, game: Game) -> Iterator[Card]:
         yield chapel
 
-    def buy_priority(self, game: Game) -> Iterator[Card]:
+    def buy_priority(self, player: Player, game: Game) -> Iterator[Card]:
 
-        money = self.state.money
-        deck_money = self.get_deck_money()
+        money = player.state.money
+        deck_money = player.get_deck_money()
         num_province = game.supply.pile_length(pile_name="Province")
-        num_chapel = self.get_card_count(card=chapel)
+        num_chapel = player.get_card_count(card=chapel)
 
         if num_chapel < 1 and money >= 2:
             yield chapel
         if deck_money > 15 and money >= 8:
             yield province
         if num_province < 5 and money >= 5:
             yield duchy
@@ -49,7 +40,15 @@
             yield estate
         if money >= 6:
             yield gold
         if num_province < 7 and money >= 5:
             yield duchy
         if money >= 3:
             yield silver
+
+
+class ChapelBot(OptimizedBot):
+    def __init__(
+        self,
+        player_id: str = "chapel_bot",
+    ):
+        super().__init__(decider=ChapelBotDecider(), player_id=player_id)
```

### Comparing `pyminion-0.3.0/pyminion/core.py` & `pyminion-0.4.0/pyminion/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 import logging
 import random
 from collections import Counter
-from typing import TYPE_CHECKING, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Iterable, Iterator, List, Optional, Tuple
 
 if TYPE_CHECKING:
-    from pyminion.players import Player
+    from pyminion.game import Game
+    from pyminion.player import Player
 
+from enum import Enum
 from pyminion.exceptions import EmptyPile, InsufficientActions, PileNotFound
 
 logger = logging.getLogger()
 
 
+
+class CardType(Enum):
+    """
+    Enum class for all card types that are currently used in the implemented expansions
+
+    """
+    Treasure = 1
+    Victory = 2
+    Curse = 3
+    Action = 4
+    Attack = 5
+    Reaction = 6
+
 class Card:
 
     """
     Base class representing a dominion card
 
     """
 
-    def __init__(self, name: str, cost: int, type: Tuple[str]):
+    def __init__(self, name: str, cost: int, type: Tuple[CardType]):
         self.name = name
-        self.cost = cost
+        self._cost = cost
         self.type = type
 
     def __repr__(self):
         return f"{self.name}"
 
+    def get_cost(self, player: "Player", game: "Game") -> int:
+        cost = max(0, self._cost - game.card_cost_reduction)
+        return cost
+
 
 class Victory(Card):
-    def __init__(self, name: str, cost: int, type: Tuple[str]):
+    def __init__(self, name: str, cost: int, type: Tuple[CardType]):
         super().__init__(name, cost, type)
 
-    def score(self):
+    def score(self, player: "Player") -> int:
         """
         Specific score method unique to each victory card
 
         """
         raise NotImplementedError(f"Score method must be implemented for {self.name}")
 
 
 class Treasure(Card):
-    def __init__(self, name: str, cost: int, type: Tuple[str], money: int):
+    def __init__(self, name: str, cost: int, type: Tuple[CardType], money: int):
         super().__init__(name, cost, type)
         self.money = money
 
     def play(self, player: "Player"):
         """
         Specific play method unique to each treasure card
 
@@ -53,45 +72,55 @@
 
 
 class Action(Card):
     def __init__(
         self,
         name: str,
         cost: int,
-        type: Tuple[str],
+        type: Tuple[CardType],
         actions: int = 0,
         draw: int = 0,
         money: int = 0,
     ):
         super().__init__(name, cost, type)
         self.actions = actions
         self.draw = draw
         self.money = money
 
-    def play(self):
+    def play(self, player: "Player", game: "Game", generic_play: bool = True) -> None:
         """
         Specific play method unique to each action card
 
         """
         raise NotImplementedError(f"play method must be implemented for {self.name}")
 
-    def generic_play(self, player: "Player"):
+    def generic_play(self, player: "Player") -> None:
         """
         Generic play method that gets executes for all action cards
 
         """
         if player.state.actions < 1:
             raise InsufficientActions(
                 f"{player.player_id}: Not enough actions to play {self.name}"
             )
 
         player.playmat.add(self)
         player.hand.remove(self)
         player.state.actions -= 1
 
+    def multi_play(self, player: "Player", game: "Game", state: Any, generic_play: bool = True) -> Any:
+        """
+        Called by "Throne Room variants" to play a card multiple times.
+        By default this just calls self.play() but can be overridden by derived
+        cards to implement different behavior.
+
+        """
+        self.play(player, game, generic_play)
+        return None
+
 
 class DeckCounter(Counter):
     def __str__(self):
         return ", ".join(f"{value} {key}" for key, value in (self).items())
 
 
 class AbstractDeck:
@@ -188,37 +217,52 @@
 
     def __repr__(self):
         return str(self.avaliable_cards())
 
     def __len__(self):
         return len(self.piles)
 
-    def gain_card(self, card: Card) -> Card:
+    def get_pile(self, pile_name: str) -> Pile:
         """
-        Gain a card from the supply.
+        Get a pile by name.
 
         """
         for pile in self.piles:
-            if card.name == pile.name:
-                try:
-                    return pile.remove(card)
+            if pile.name == pile_name:
+                return pile
+        raise PileNotFound(f"{pile_name} pile is not valid")
 
-                except EmptyPile as e:
-                    raise e
+    def gain_card(self, card: Card) -> Card:
+        """
+        Gain a card from the supply.
 
-        raise PileNotFound(f"{card} not found in the supply")
+        """
+        pile = self.get_pile(card.name)
+        try:
+            return pile.remove(card)
+
+        except EmptyPile as e:
+            raise e
 
     def return_card(self, card: Card):
         """
         Return a card to the supply.
 
         """
-        for pile in self.piles:
-            if card.name == pile.name:
-                pile.add(card)
+        pile = self.get_pile(card.name)
+        pile.add(card)
+
+    def trash_card(self, card: Card, trash: "Trash") -> None:
+        """
+        Trash a card from the supply.
+
+        """
+        pile = self.get_pile(card.name)
+        pile.remove(card)
+        trash.add(card)
 
     def avaliable_cards(self) -> List[Card]:
         """
         Returns a list containing a single card from each non-empty pile in the supply.
 
         """
         cards = [pile.cards[0] for pile in self.piles if pile]
@@ -236,11 +280,30 @@
         return empty_piles
 
     def pile_length(self, pile_name: str) -> int:
         """
         Get the number of cards in a specified pile in the supply.
 
         """
-        for pile in self.piles:
-            if pile.name == pile_name:
-                return len(pile)
-        raise PileNotFound(f"{pile_name} pile is not valid")
+        pile = self.get_pile(pile_name)
+        return len(pile)
+
+
+def get_action_cards(cards: Iterable[Card]) -> Iterator[Action]:
+    for card in cards:
+        if CardType.Action in card.type:
+            assert isinstance(card, Action)
+            yield card
+
+
+def get_treasure_cards(cards: Iterable[Card]) -> Iterator[Treasure]:
+    for card in cards:
+        if CardType.Treasure in card.type:
+            assert isinstance(card, Treasure)
+            yield card
+
+
+def get_victory_cards(cards: Iterable[Card]) -> Iterator[Victory]:
+    for card in cards:
+        if CardType.Victory in card.type:
+            assert isinstance(card, Victory)
+            yield card
```

### Comparing `pyminion-0.3.0/pyminion/exceptions.py` & `pyminion-0.4.0/pyminion/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,14 +71,28 @@
 class InvalidMultiCardInput(InvalidInput):
     """
     Invalid response, that input cannot be discarded
 
     """
 
 
+class InvalidMultiOptionInput(InvalidInput):
+    """
+    Invalid response, not a valid option
+
+    """
+
+
+class InvalidDeckPositionInput(InvalidInput):
+    """
+    Invalid deck position response
+
+    """
+
+
 class InvalidPlayerCount(Exception):
     """
     Invalid number of players in game
 
     """
```

### Comparing `pyminion-0.3.0/pyminion/expansions/base.py` & `pyminion-0.4.0/pyminion/expansions/intrigue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1570 +1,1448 @@
+from enum import IntEnum, unique
 import logging
-import math
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, List
 
-from pyminion.bots.bot import Bot
-from pyminion.core import AbstractDeck, Action, Card, Treasure, Victory
-from pyminion.decisions import validate_input
-from pyminion.exceptions import (EmptyPile, InvalidBotImplementation,
-                                 InvalidMultiCardInput, InvalidSingleCardInput)
-from pyminion.players import Human, Player
+from pyminion.core import AbstractDeck, Action, Card, CardType, Treasure, Victory
+from pyminion.player import Player
+from pyminion.exceptions import EmptyPile
+from pyminion.expansions.base import curse, duchy, estate, gold, silver
 
 if TYPE_CHECKING:
     from pyminion.game import Game
 
 
 logger = logging.getLogger()
 
 
-class Copper(Treasure):
-    def __init__(
-        self,
-        name: str = "Copper",
-        cost: int = 0,
-        type: Tuple[str] = ("Treasure",),
-        money: int = 1,
-    ):
-        super().__init__(name, cost, type, money)
-
-    def play(self, player: Player, game: "Game"):
-        player.playmat.add(self)
-        player.hand.remove(self)
-        player.state.money += self.money
+class Baron(Action):
+    """
+    +1 Buy
 
+    You may discard an Estate for +4 money. If you don't, gain an Estate.
 
-class Silver(Treasure):
-    def __init__(
-        self,
-        name: str = "Silver",
-        cost: int = 3,
-        type: Tuple[str] = ("Treasure",),
-        money: int = 2,
-    ):
-        super().__init__(name, cost, type, money)
-
-    def play(self, player: Player, game: "Game"):
-
-        # check if this is the first silver played and if there are any merchants in play
-        if self not in player.playmat.cards:
-            if num_merchants := len(
-                [card for card in player.playmat.cards if card.name == "Merchant"]
-            ):
-                player.state.money += num_merchants
+    """
 
-        player.playmat.add(self)
-        player.hand.remove(self)
-        player.state.money += self.money
+    @unique
+    class Choice(IntEnum):
+        DiscardEstate = 0
+        GainEstate = 1
 
+    def __init__(self):
+        super().__init__(name="Baron", cost=4, type=(CardType.Action,))
 
-class Gold(Treasure):
-    def __init__(
-        self,
-        name: str = "Gold",
-        cost: int = 6,
-        type: Tuple[str] = ("Treasure",),
-        money: int = 3,
-    ):
-        super().__init__(name, cost, type, money)
+    def play(
+        self, player: Player, game: "Game", generic_play: bool = True
+    ) -> None:
 
-    def play(self, player: Player, game: "Game"):
-        player.playmat.add(self)
-        player.hand.remove(self)
-        player.state.money += self.money
+        logger.info(f"{player} plays {self}")
+        if generic_play:
+            super().generic_play(player)
 
+        player.state.buys += 1
 
-class Estate(Victory):
-    def __init__(
-        self,
-        name: str = "Estate",
-        cost: int = 2,
-        type: Tuple[str] = ("Victory",),
-    ):
-        super().__init__(name, cost, type)
+        discard_estate = False
+        if estate in player.hand.cards:
+            options = [
+                "Discard estate for +4 money",
+                "Gain an estate",
+            ]
+            responses = player.decider.multiple_option_decision(self, options, player, game)
+            assert len(responses) == 1
+            response = responses[0]
 
-    def score(self, player: Player) -> int:
-        vp = 1
-        return vp
+            discard_estate = (response == Baron.Choice.DiscardEstate)
 
+        if discard_estate:
+            player.discard(estate)
+            player.state.money += 4
+        elif game.supply.pile_length(estate.name) > 0:
+            player.gain(estate, game.supply)
 
-class Duchy(Victory):
-    def __init__(
-        self,
-        name: str = "Duchy",
-        cost: int = 5,
-        type: Tuple[str] = ("Victory",),
-    ):
-        super().__init__(name, cost, type)
 
-    def score(self, player: Player) -> int:
-        vp = 3
-        return vp
+class Bridge(Action):
+    """
+    +1 buy, +$1
 
+    This turn, cards (everywhere) cost $1 less.
 
-class Province(Victory):
-    def __init__(
-        self,
-        name: str = "Province",
-        cost: int = 8,
-        type: Tuple[str] = ("Victory",),
-    ):
-        super().__init__(name, cost, type)
+    """
 
-    def score(self, player: Player) -> int:
-        vp = 6
-        return vp
+    def __init__(self):
+        super().__init__(name="Bridge", cost=4, type=(CardType.Action,), money=1)
 
+    def play(
+        self, player: Player, game: "Game", generic_play: bool = True
+    ) -> None:
 
-class Curse(Victory):
-    def __init__(
-        self,
-        name: str = "Curse",
-        cost: int = 0,
-        type: Tuple[str] = ("Curse",),
-    ):
-        super().__init__(name, cost, type)
+        logger.info(f"{player} plays {self}")
+        if generic_play:
+            super().generic_play(player)
 
-    def score(self, player: Player) -> int:
-        vp = -1
-        return vp
+        player.state.buys += 1
+        player.state.money += 1
 
+        game.card_cost_reduction += 1
 
-class Gardens(Victory):
-    """
-    Worth 1VP for every 10 cards you have (round down)
 
+class Conspirator(Action):
     """
+    +2 Money
 
-    def __init__(
-        self,
-        name: str = "Gardens",
-        cost: int = 4,
-        type: Tuple[str] = ("Victory",),
-    ):
-        super().__init__(name, cost, type)
-
-    def score(self, player: Player) -> int:
-        total_count = len(player.get_all_cards())
-        vp = math.floor(total_count / 10)
-        return vp
-
-
-class Smithy(Action):
-    """
-    + 3 cards
+    If you've played 3 or more Actions this turn (counting this), +1 Card and +1 Action.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Smithy",
-        cost: int = 4,
-        type: Tuple[str] = ("Action",),
-        draw: int = 3,
-    ):
-        super().__init__(name, cost, type, draw=draw)
+    def __init__(self):
+        super().__init__(name="Conspirator", cost=4, type=(CardType.Action,), money=2)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
-
         if generic_play:
             super().generic_play(player)
 
-        player.draw(3)
+        player.state.money += 2
+
+        if player.actions_played_this_turn >= 3:
+            player.draw(1)
+            player.state.actions += 1
 
 
-class Village(Action):
+class Courtier(Action):
     """
-    + 1 card, + 2 actions
+    Reveal a card from your hand. For each type it has (Action, Attack, etc.),
+    choose one: +1 Action; or +1 Buy; or +3 Money; or gain a Gold. The choices
+    must be different.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Village",
-        cost: int = 3,
-        type: Tuple[str] = ("Action",),
-        actions: int = 2,
-        draw: int = 1,
-    ):
-        super().__init__(name, cost, type, actions=actions, draw=draw)
+    @unique
+    class Choice(IntEnum):
+        Action = 0
+        Buy = 1
+        Money = 2
+        GainGold = 3
+
+    def __init__(self):
+        super().__init__(name="Courtier", cost=5, type=(CardType.Action,))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
-
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 2
-        player.draw()
+        hand_len = len(player.hand)
+
+        if hand_len == 0:
+            return
+
+        if hand_len == 1:
+            reveal_card = player.hand.cards[0]
+        else:
+            reveal_cards = player.decider.reveal_decision(
+                prompt="Reveal a card from your hand: ",
+                card=self,
+                valid_cards=player.hand.cards,
+                player=player,
+                game=game,
+                min_num_reveal = 1,
+                max_num_reveal = 1,
+            )
+            assert len(reveal_cards) == 1
+            reveal_card = reveal_cards[0]
+
+        logger.info(f"{player} reveals {reveal_card}")
+
+        num_choices = min(len(reveal_card.type), 4)
+
+        if num_choices == 4:
+            choices = [c.value for c in Courtier.Choice]
+        else:
+            options = [
+                "+1 Action",
+                "+1 Buy",
+                "+3 Money",
+                "Gain a Gold",
+            ]
+            choices = player.decider.multiple_option_decision(
+                card=self,
+                options=options,
+                player=player,
+                game=game,
+                num_choices=num_choices,
+                unique=True,
+            )
+            assert len(set(choices)) == num_choices # ensure number of unique choices is correct
+
+        for choice in choices:
+            if choice == Courtier.Choice.Action:
+                player.state.actions += 1
+            elif choice == Courtier.Choice.Buy:
+                player.state.buys += 1
+            elif choice == Courtier.Choice.Money:
+                player.state.money += 3
+            elif choice == Courtier.Choice.GainGold:
+                player.gain(gold, game.supply)
+            else:
+                raise ValueError(f"Unknown courtier choice '{choice}'")
 
 
-class Laboratory(Action):
+class Courtyard(Action):
     """
-    +2 cards, +1 action
+    +3 Cards
+
+    Put a card from your hand onto your deck.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Laboratory",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 2,
-    ):
-        super().__init__(name, cost, type, actions=actions, draw=draw)
+    def __init__(self):
+        super().__init__(name="Courtyard", cost=2, type=(CardType.Action,), draw=3)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
-
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 1
-        player.draw(2)
+        player.draw(3)
+
+        topdeck_cards = player.decider.topdeck_decision(
+            prompt="Enter the card you would like to topdeck: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_topdeck=1,
+            max_num_topdeck=1,
+        )
+        assert len(topdeck_cards) == 1
+        topdeck_card = topdeck_cards[0]
+
+        player.hand.remove(topdeck_card)
+        player.deck.add(topdeck_card)
 
 
-class Market(Action):
+class Diplomat(Action):
     """
-    +1 card, +1 action, +1 money, +1 buy
+    +2 Cards
+
+    If you have 5 or fewer cards in hand (after drawing), +2 Actions.
+
+    When another player plays an Attack card, you may first reveal this from a
+    hand of 5 or more cards, to draw 2 cards then discard 3.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Market",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 1,
-        money: int = 1,
-    ):
-        super().__init__(name, cost, type, actions, draw, money)
+    def __init__(self):
+        super().__init__("Diplomat", 4, (CardType.Action, CardType.Reaction), draw=2)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
-
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 1
-        player.draw()
-        player.state.money += 1
-        player.state.buys += 1
+        player.draw(2)
+        if len(player.hand) <= 5:
+            player.state.actions += 2
 
+    def on_attack(self, player: "Player", attack_card: Card, game: "Game") -> None:
+        if len(player.hand) < 5:
+            return
 
-class Moneylender(Action):
-    """
-    You may trash a copper from your hand for + 3 money
+        reveal = player.decider.binary_decision(
+            prompt=f"Reveal {self} to draw 2 cards then discard 3? y/n: ",
+            card=self,
+            player=player,
+            game=game,
+            relevant_cards=[attack_card],
+        )
+        if not reveal:
+            return
 
-    """
+        logger.info(f"{player} reveals {self}")
+
+        player.draw(2)
 
-    def __init__(
-        self,
-        name: str = "Moneylender",
-        cost: int = 4,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+        discard_cards = player.decider.discard_decision(
+            prompt="Enter the cards you would like to discard: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_discard=3,
+            max_num_discard=3,
+        )
+        assert len(discard_cards) == 3
 
-    def play(
-        self,
-        player: Union[Human, Bot],
-        game: "Game",
-        generic_play: bool = True,
-    ) -> None:
+        for card in discard_cards:
+            player.discard(card)
 
-        logger.info(f"{player} plays {self}")
 
-        if generic_play:
-            super().generic_play(player)
+class Duke(Victory):
+    """
+    Worth 1VP per Duchy you have.
 
-        if copper not in player.hand.cards:
-            return
+    """
 
-        if isinstance(player, Human):
-            response = player.binary_decision(
-                prompt="Do you want to trash a copper from your hand for +3 money? y/n: ",
-            )
+    def __init__(self):
+        super().__init__("Duke", 5, (CardType.Victory,))
 
-        elif isinstance(player, Bot):
-            response = player.binary_resp(game=game, card=self)
+    def score(self, player: Player) -> int:
+        vp = 0
+        for card in player.get_all_cards():
+            if card.name == duchy.name:
+                vp += 1
+        return vp
 
-        if response:
-            player.trash(target_card=copper, trash=game.trash)
-            player.state.money += 3
 
+class Harem(Treasure, Victory):
+    def __init__(self):
+        Treasure.__init__(
+            self,
+            name="Harem",
+            cost=6,
+            type=(CardType.Treasure, CardType.Victory),
+            money=2,
+        )
 
-class Cellar(Action):
+    def play(self, player: Player, game: "Game") -> None:
+        player.playmat.add(self)
+        player.hand.remove(self)
+        player.state.money += self.money
+
+    def score(self, player: Player) -> int:
+        vp = 2
+        return vp
+
+
+class Ironworks(Action):
     """
-    +1 Action
+    Gain a card costing up to $4.
+    If the gained card is an...
 
-    Discard any number of cards, then draw that many
+    Action card, +1 Action
+    Treasure card, +$1
+    Victory card, +1 Card
 
     """
 
-    def __init__(
-        self,
-        name: str = "Cellar",
-        cost: int = 2,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-    ):
-        super().__init__(name, cost, type, actions=actions)
+    def __init__(self):
+        super().__init__(name="Ironworks", cost=4, type=(CardType.Action,))
 
     def play(
-        self,
-        player: Union[Human, Bot],
-        game: "Game",
-        generic_play: bool = True,
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
-
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 1
+        gain_cards = player.decider.gain_decision(
+            prompt="Gain a card costing up to 4 money: ",
+            card=self,
+            valid_cards=[
+                card for card in game.supply.avaliable_cards() if card.get_cost(player, game) <= 4
+            ],
+            player=player,
+            game=game,
+            min_num_gain=1,
+            max_num_gain=1,
+        )
+        assert len(gain_cards) == 1
+        gain_card = gain_cards[0]
+        assert gain_card.get_cost(player, game) <= 4
 
-        if not player.hand.cards:
-            return
+        player.gain(card=gain_card, supply=game.supply)
 
-        if isinstance(player, Human):
-            discard_cards = player.multiple_card_decision(
-                prompt="Enter the cards you would like to discard seperated by commas: ",
-                valid_cards=player.hand.cards,
-            )
+        if CardType.Action in gain_card.type:
+            player.state.actions += 1
 
-        elif isinstance(player, Bot):
-            discard_cards = player.multiple_discard_resp(
-                card=self,
-                valid_cards=player.hand.cards,
-                game=game,
-                required=False,
-            )
+        if CardType.Treasure in gain_card.type:
+            player.state.money += 1
 
-        if discard_cards:
-            for card in discard_cards:
-                player.discard(card)
-            player.draw(len(discard_cards))
+        if CardType.Victory in gain_card.type:
+            player.draw(1)
 
 
-class Chapel(Action):
+class Lurker(Action):
     """
-    Trash up to 4 cards from your hand
+    +1 Action
+
+    Choose one: Trash an Action card from the Supply, or gain an Action card from the trash.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Chapel",
-        cost: int = 2,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    @unique
+    class Choice(IntEnum):
+        TrashAction = 0
+        GainAction = 1
+
+    def __init__(self):
+        super().__init__(name="Lurker", cost=2, type=(CardType.Action,), actions=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
         if generic_play:
             super().generic_play(player)
 
-        if not player.hand.cards:
+        player.state.actions += 1
+
+        supply_action_cards = [
+            c for c in game.supply.avaliable_cards() if CardType.Action in c.type
+        ]
+        trash_action_cards = [
+            c for c in game.trash.cards if CardType.Action in c.type
+        ]
+
+        if len(supply_action_cards) == 0 and len(trash_action_cards) == 0:
             return
 
-        @validate_input(exceptions=InvalidMultiCardInput)
-        def get_trash_cards() -> Optional[List[Card]]:
+        options = [
+            "Trash an Action card from the Supply",
+            "Gain an Action card from the trash",
+        ]
+        choices = player.decider.multiple_option_decision(
+            card=self,
+            options=options,
+            player=player,
+            game=game,
+        )
+        assert len(choices) == 1
+        choice = choices[0]
 
-            trash_cards = player.multiple_card_decision(
-                prompt="Enter up to 4 cards you would like to trash from your hand: ",
-                valid_cards=player.hand.cards,
-            )
+        if choice == Lurker.Choice.TrashAction:
+            if len(supply_action_cards) == 0:
+                return
 
-            if trash_cards and len(trash_cards) > 4:
-                raise InvalidMultiCardInput(
-                    "You cannot trash more than 4 cards with chapel"
-                )
+            trash_cards = player.decider.trash_decision(
+                prompt="Choose a card from the Supply to trash",
+                card=self,
+                valid_cards=supply_action_cards,
+                player=player,
+                game=game,
+                min_num_trash=1,
+                max_num_trash=1,
+            )
+            assert len(trash_cards) == 1
+            trash_card = trash_cards[0]
 
-            return trash_cards
+            game.supply.trash_card(trash_card, game.trash)
 
-        if isinstance(player, Human):
-            trash_cards = get_trash_cards()
+        elif choice == Lurker.Choice.GainAction:
+            if len(trash_action_cards) == 0:
+                return
 
-        elif isinstance(player, Bot):
-            trash_cards = player.multiple_trash_resp(
+            gain_cards = player.decider.gain_decision(
+                prompt="Choose a card to gain from the trash",
                 card=self,
-                valid_cards=player.hand.cards,
+                valid_cards=trash_action_cards,
+                player=player,
                 game=game,
-                required=False,
+                min_num_gain=1,
+                max_num_gain=1,
             )
-            if trash_cards and len(trash_cards) > 4:
-                raise InvalidMultiCardInput(
-                    "Attempted to trash more than 4 cards with chapel"
-                )
-        if not trash_cards:
-            return
-        for card in trash_cards:
-            player.trash(card, game.trash)
+            assert len(gain_cards) == 1
+            gain_card = gain_cards[0]
+
+            game.trash.remove(gain_card)
+            player.discard_pile.add(gain_card)
+
+        else:
+            raise ValueError(f"Unknown lurker choice '{choice}'")
 
 
-class Workshop(Action):
+class Masquerade(Action):
     """
-    Gain a card costing up to 4 money
+    +2 Cards
+
+    Each player with any cards in hand passes one to the next such player to
+    their left, at once. Then you may trash a card from your hand.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Workshop",
-        cost: int = 3,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Masquerade", cost=3, type=(CardType.Action,), draw=2)
 
-    def play(self, player: Player, game: "Game", generic_play: bool = True) -> None:
+    def play(
+        self, player: Player, game: "Game", generic_play: bool = True
+    ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        @validate_input(exceptions=InvalidSingleCardInput)
-        def get_gain_card() -> Card:
+        player.draw(2)
+
+        # get players who have at least 1 card in their hand
+        valid_players = [p for p in game.players if len(p.hand) > 0]
 
-            gain_card = player.single_card_decision(
-                prompt="Gain a card costing up to 4 money: ",
-                valid_cards=game.supply.avaliable_cards(),
+        # prompt each player to choose a card to pass
+        passed_cards: List[Card] = []
+        for p in valid_players:
+            pass_cards = player.decider.pass_decision(
+                prompt="Pick a card to pass to the player on your left: ",
+                card=self,
+                valid_cards=p.hand.cards,
+                player=player,
+                game=game,
+                min_num_pass=1,
+                max_num_pass=1,
             )
+            assert len(pass_cards) == 1
+            pass_card = pass_cards[0]
 
-            if not gain_card:
-                raise InvalidSingleCardInput("You must gain a card")
-            if gain_card.cost > 4:
-                raise InvalidSingleCardInput("Card must cost less than 4 money")
+            passed_cards.append(pass_card)
 
-            return gain_card
+        # pass the cards
+        for idx, p in enumerate(valid_players):
+            c = passed_cards[idx]
+            p.hand.remove(c)
+            next_idx = (idx + 1) % len(valid_players)
+            next_player = valid_players[next_idx]
+            next_player.hand.add(c)
+            logger.info(f"{p} passes {c} to {next_player}")
 
-        if isinstance(player, Human):
-            gain_card = get_gain_card()
+        if len(player.hand) == 0:
+            return
 
-        elif isinstance(player, Bot):
-            gain_card = player.gain_resp(
+        trash = player.decider.binary_decision(
+            prompt="Would you like to trash a card from your hand?",
+            card=self,
+            player=player,
+            game=game,
+        )
+
+        if trash:
+            trash_cards = player.decider.trash_decision(
+                prompt="Choose a card from your hand to trash",
                 card=self,
-                valid_cards=[
-                    card for card in game.supply.avaliable_cards() if card.cost <= 4
-                ],
+                valid_cards=player.hand.cards,
+                player=player,
                 game=game,
-                required=True,
+                min_num_trash=1,
+                max_num_trash=1,
             )
-            if not gain_card:
-                raise InvalidSingleCardInput("You must gain a card")
-            if gain_card.cost > 4:
-                raise InvalidSingleCardInput("Card must cost less than 4 money")
+            assert len(trash_cards) == 1
+            trash_card = trash_cards[0]
 
-        player.gain(gain_card, game.supply)
+            player.trash(trash_card, game.trash)
 
 
-class Festival(Action):
+class Mill(Action, Victory):
     """
-    + 2 actions, + 1 buy, + 2 money
+    +1 card, +1 action
+
+    You may discard 2 cards, for +$2.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Festival",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-        actions: int = 2,
-        money: int = 2,
-    ):
-        super().__init__(name, cost, type, actions=actions, money=money)
+    def __init__(self):
+        Action.__init__(self, "Mill", 4, (CardType.Action, CardType.Victory), actions=1, draw=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 2
-        player.state.money += 2
-        player.state.buys += 1
+        player.draw(1)
+        player.state.actions += 1
+
+        discard = player.decider.binary_decision(
+            prompt="Do you want to discard 2 cards for +2 money?",
+            card=self,
+            player=player,
+            game=game,
+        )
+
+        if discard:
+            hand_len = len(player.hand)
+            if hand_len <= 2:
+                discard_cards = player.hand.cards[:]
+            else:
+                discard_cards = player.decider.discard_decision(
+                    prompt="Enter the cards you would like to discard: ",
+                    card=self,
+                    valid_cards=player.hand.cards,
+                    player=player,
+                    game=game,
+                    min_num_discard=2,
+                    max_num_discard=2,
+                )
+                assert len(discard_cards) == 2
+
+            if len(discard_cards) == 2:
+                player.state.money += 2
+
+            for c in discard_cards:
+                player.discard(c)
+
+    def score(self, player: Player) -> int:
+        vp = 1
+        return vp
 
 
-class Harbinger(Action):
+class MiningVillage(Action):
     """
-    +1 card, +1 action
+    +1 card, +2 actions
 
-    Look through your discard pile. You may put a card from it onto your deck
+    You may trash this for +$2.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Harbinger",
-        cost: int = 3,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 1,
-    ):
-        super().__init__(name, cost, type, actions=actions, draw=draw)
+    def __init__(self):
+        super().__init__(name="Mining Village", cost=4, type=(CardType.Action,), actions=2, draw=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.state.actions += 1
-        player.draw()
+        self._play(player, game, None, generic_play)
 
-        if not player.discard_pile:
-            return
+    def multi_play(
+        self, player: Player, game: "Game", state: Any, generic_play: bool = True
+    ) -> Any:
+        return self._play(player, game, state, generic_play)
 
-        if isinstance(player, Human):
-            topdeck_card = player.single_card_decision(
-                prompt="You may select a card from your discard pile to put onto your deck: ",
-                valid_cards=player.discard_pile.cards,
-            )
+    def _play(
+        self, player: Player, game: "Game", state: Any, generic_play: bool = True
+    ) -> Any:
+        player.draw(1)
+        player.state.actions += 2
+
+        trashed = False if state is None else bool(state)
 
-        elif isinstance(player, Bot):
-            topdeck_card = player.topdeck_resp(
+        # if the card has not previously been trashed, give the player the
+        # option to trash it now
+        if not trashed:
+            trashed = player.decider.binary_decision(
+                prompt="Trash Mining Village for +2 money? ",
                 card=self,
-                valid_cards=player.discard_pile.cards,
+                player=player,
                 game=game,
-                required=False,
             )
 
-        if not topdeck_card or isinstance(topdeck_card, str):
-            return
+            if trashed:
+                player.state.money += 2
+                player.trash(self, game.trash, source=player.playmat)
 
-        player.deck.add(player.discard_pile.remove(topdeck_card))
+        return trashed
 
 
-class Vassal(Action):
+class Minion(Action):
     """
-    +2 money
+    +1 action
 
-    Discard the top card of your deck. If it's an action card you may play it.
+    Choose one: +$2; or discard your hand, +4 Cards, and each other player
+    with at least 5 cards in hand discards their hand and draws 4 cards.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Vassal",
-        cost: int = 3,
-        type: Tuple[str] = ("Action",),
-        money: int = 2,
-    ):
-        super().__init__(name, cost, type, money=money)
+    @unique
+    class Choice(IntEnum):
+        Money = 0
+        DiscardDrawAttack = 1
+
+    def __init__(self):
+        super().__init__(name="Minion", cost=5, type=(CardType.Action, CardType.Attack), actions=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.state.money += 2
-        player.draw(destination=player.discard_pile, silent=True)
-
-        if not player.discard_pile:
-            return
-
-        discard_card = player.discard_pile.cards[-1]
-
-        logger.info(f"{player} discards {discard_card}")
+        player.state.actions += 1
 
-        if "Action" not in discard_card.type:
-            return
+        # opponents react to the card before the choice is made
+        is_attacked: List[bool] = []
+        for opponent in game.players:
+            if opponent is not player:
+                ret = opponent.is_attacked(player, self, game)
+                is_attacked.append(ret)
 
-        if isinstance(player, Human):
-            decision = player.binary_decision(
-                prompt=f"You discarded {discard_card.name}, would you like to play it? (y/n):  "
-            )
-        elif isinstance(player, Bot):
-            decision = player.binary_resp(game=game, card=self)
+        options = [
+            "+2 Money",
+            "Discard your hand, draw 4 cards, and each other player with at least 5 cards discards their hand and draws 4 cards",
+        ]
+        choices = player.decider.multiple_option_decision(
+            card=self,
+            options=options,
+            player=player,
+            game=game,
+        )
+        assert len(choices) == 1
+        choice = choices[0]
 
-        if not decision:
-            return
+        if choice == Minion.Choice.Money:
+            player.state.money += 2
+        elif choice == Minion.Choice.DiscardDrawAttack:
+            for _ in range(len(player.hand.cards)):
+                player.discard(player.hand.cards[0])
+            player.draw(4)
 
-        played_card = player.discard_pile.cards.pop()
-        player.playmat.add(played_card)
-        player.exact_play(card=player.playmat.cards[-1], game=game, generic_play=False)
-        return
+            i = 0
+            for opponent in game.players:
+                if opponent is not player and is_attacked[i]:
+                    if len(opponent.hand) >= 5:
+                        for _ in range(len(opponent.hand.cards)):
+                            opponent.discard(opponent.hand.cards[0])
+                        opponent.draw(4)
+                    i += 1
+        else:
+            raise ValueError(f"Unknown minion choice '{choice}'")
 
 
-class Artisan(Action):
+class Nobles(Action, Victory):
     """
-    Gain a card to your hand costing up to 5 money.
-
-    Put a card from your hand onto your deck
+    Choose one: +3 Cards; or +2 Actions.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Artisan",
-        cost: int = 6,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    @unique
+    class Choice(IntEnum):
+        Cards = 0
+        Actions = 1
+
+    def __init__(self):
+        Action.__init__(self, "Nobles", 6, (CardType.Action, CardType.Victory))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        @validate_input(exceptions=InvalidSingleCardInput)
-        def get_gain_card() -> Card:
-            gain_card = player.single_card_decision(
-                prompt="Gain a card costing up to 5 money: ",
-                valid_cards=game.supply.avaliable_cards(),
-            )
-            if not gain_card or isinstance(gain_card, str):
-                raise InvalidSingleCardInput("You must gain a card")
-            if gain_card.cost > 4:
-                raise InvalidSingleCardInput("Card must cost at most 5 money")
-            return gain_card
-
-        @validate_input(exceptions=InvalidSingleCardInput)
-        def get_topdeck_card() -> Card:
-            topdeck_card = player.single_card_decision(
-                prompt="Put a card from your hand onto your deck: ",
-                valid_cards=player.hand.cards,
-            )
-            if not topdeck_card or isinstance(topdeck_card, str):
-                raise InvalidSingleCardInput("You must topdeck a card")
-            return topdeck_card
-
-        if isinstance(player, Human):
-            gain_card = get_gain_card()
-            player.gain(card=gain_card, supply=game.supply, destination=player.hand)
-            topdeck_card = get_topdeck_card()
-
-        elif isinstance(player, Bot):
-            gain_card = player.gain_resp(
-                card=self,
-                valid_cards=[
-                    card for card in game.supply.avaliable_cards() if card.cost <= 5
-                ],
-                game=game,
-                required=True,
-            )
-
-            if not gain_card:
-                raise InvalidSingleCardInput("Must gain a card with Artisan")
-            if gain_card.cost > 5:
-                raise InvalidSingleCardInput("Card must cost at most 5 money")
-
-            player.gain(card=gain_card, supply=game.supply, destination=player.hand)
+        options = [
+            "+3 Cards",
+            "+2 Actions",
+        ]
+        choices = player.decider.multiple_option_decision(
+            card=self,
+            options=options,
+            player=player,
+            game=game,
+        )
+        assert len(choices) == 1
+        choice = choices[0]
 
-            topdeck_card = player.topdeck_resp(
-                card=self,
-                valid_cards=player.hand.cards,
-                game=game,
-                required=True,
-            )
+        if choice == Nobles.Choice.Cards:
+            player.draw(3)
+        elif choice == Nobles.Choice.Actions:
+            player.state.actions += 2
+        else:
+            raise ValueError(f"Unknown nobles choice '{choice}'")
 
-        for card in player.hand.cards:
-            if card == topdeck_card:
-                player.deck.add(player.hand.remove(card))
-                return
+    def score(self, player: Player) -> int:
+        vp = 2
+        return vp
 
 
-class Poacher(Action):
+class Patrol(Action):
     """
-    +1 card, +1 action, + 1 money
+    +3 cards
 
-    Discard a card per empty Supply pile
+    Reveal the top 4 cards of your deck. Put the Victory cards and Curses into
+    your hand. Put the rest back in any order.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Poacher",
-        cost: int = 4,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 1,
-        money: int = 1,
-    ):
-        super().__init__(name, cost, type, actions, draw, money)
+    def __init__(self):
+        super().__init__(name="Patrol", cost=5, type=(CardType.Action,), draw=3)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.draw()
-        player.state.actions += 1
-        player.state.money += 1
-
-        empty_piles = game.supply.num_empty_piles()
-
-        if empty_piles == 0:
-            return
-
-        discard_num = min(empty_piles, len(player.hand))
-
-        if isinstance(player, Human):
-
-            @validate_input(exceptions=InvalidMultiCardInput)
-            def get_discard_cards() -> List[Card]:
-                discard_cards = player.multiple_card_decision(
-                    prompt=f"Discard {discard_num} card(s) from your hand: ",
-                    valid_cards=player.hand.cards,
-                )
-                if not discard_cards or len(discard_cards) != discard_num:
-                    raise InvalidMultiCardInput(
-                        f"You must discard {discard_num} card(s)"
-                    )
-
-                return discard_cards
+        player.draw(3)
 
-            discard_cards = get_discard_cards()
+        revealed = AbstractDeck()
+        player.draw(num_cards=4, destination=revealed, silent=True)
+        logger.info(f"{player} reveals {revealed}")
 
-        elif isinstance(player, Bot):
-            discard_cards = player.multiple_discard_resp(
+        victory_curse_cards = [
+            card
+            for card in revealed.cards
+            if CardType.Curse in card.type or CardType.Victory in card.type
+        ]
+
+        for card in victory_curse_cards:
+            player.hand.add(revealed.remove(card))
+
+        num_topdeck = len(revealed.cards)
+        if num_topdeck <= 1:
+            topdeck_cards = revealed.cards
+        else:
+            topdeck_cards = player.decider.topdeck_decision(
+                prompt="Enter the cards in the order you would like to topdeck: ",
                 card=self,
-                valid_cards=player.hand.cards,
+                valid_cards=revealed.cards,
+                player=player,
                 game=game,
-                num_discard=discard_num,
-                required=True,
+                min_num_topdeck=num_topdeck,
+                max_num_topdeck=num_topdeck,
             )
-            if not discard_cards or len(discard_cards) != discard_num:
-                raise InvalidMultiCardInput(f"You must discard {discard_num} card(s)")
 
-        for discard_card in discard_cards:
-            player.discard(discard_card)
+        for card in topdeck_cards:
+            player.deck.add(card)
 
 
-class CouncilRoom(Action):
+class Pawn(Action):
     """
-    +4 cards, +1 buy
-
-    Each other player draws a card
+    Choose two: +1 Card; +1 Action; +1 Buy; +1 Money.
+    The choices must be different.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Council Room",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-        draw: int = 4,
-    ):
-        super().__init__(name, cost, type, draw=draw)
+    @unique
+    class Choice(IntEnum):
+        Card = 0
+        Action = 1
+        Buy = 2
+        Money = 3
+
+    def __init__(self):
+        super().__init__(name="Pawn", cost=2, type=(CardType.Action,))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.draw(4)
-        player.state.buys += 1
+        options = [
+            "+1 Card",
+            "+1 Action",
+            "+1 Buy",
+            "+1 Money",
+        ]
+        choices = player.decider.multiple_option_decision(
+            card=self,
+            options=options,
+            player=player,
+            game=game,
+            num_choices=2,
+            unique=True,
+        )
+        assert len(set(choices)) == 2 # ensure number of unique choices is correct
 
-        for p in game.players:
-            if p is not player:
-                p.draw()
+        for choice in choices:
+            if choice == Pawn.Choice.Card:
+                player.draw(1)
+            elif choice == Pawn.Choice.Action:
+                player.state.actions += 1
+            elif choice == Pawn.Choice.Buy:
+                player.state.buys += 1
+            elif choice == Pawn.Choice.Money:
+                player.state.money += 1
+            else:
+                raise ValueError(f"Unknown pawn choice '{choice}'")
 
 
-class Witch(Action):
+class Replace(Action):
     """
-    +2 cards
-
-    Each other player gains a curse
+    Trash a card from your hand. Gain a card costing up to $2 more than it. If
+    the gained card is an Action or Treasure, put it onto your deck; if it's a
+    Victory card, each other player gains a Curse.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Witch",
-        cost: int = 5,
-        type: Tuple[str] = ("Action", "Attack"),
-        draw: int = 2,
-    ):
-        super().__init__(name, cost, type, draw=draw)
+    def __init__(self):
+        super().__init__(name="Replace", cost=5, type=(CardType.Action, CardType.Attack))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.draw(2)
+        trash_cards = player.decider.trash_decision(
+            prompt="Trash a card form your hand: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_trash=1,
+            max_num_trash=1,
+        )
+        assert len(trash_cards) == 1
+        trash_card = trash_cards[0]
 
-        for opponent in game.players:
-            if opponent is not player:
-                if opponent.is_attacked(player=player, attack_card=self):
+        max_cost = trash_card.get_cost(player, game) + 2
+        gain_cards = player.decider.gain_decision(
+            prompt=f"Gain a card costing up to {max_cost} money: ",
+            card=self,
+            valid_cards=[
+                card
+                for card in game.supply.avaliable_cards()
+                if card.get_cost(player, game) <= max_cost
+            ],
+            player=player,
+            game=game,
+            min_num_gain=1,
+            max_num_gain=1,
+        )
+        assert len(gain_cards) == 1
+        gain_card = gain_cards[0]
+        assert gain_card.get_cost(player, game) <= max_cost
+
+        player.trash(trash_card, trash=game.trash)
 
+        if CardType.Action in gain_card.type or CardType.Treasure in gain_card.type:
+            player.gain(gain_card, game.supply, destination=player.deck)
+        else:
+            player.gain(gain_card, game.supply)
+
+        if CardType.Victory in gain_card.type:
+            for opponent in game.players:
+                if opponent is not player and opponent.is_attacked(player, self, game):
                     # attempt to gain a curse. if curse pile is empty, proceed
                     try:
-                        opponent.gain(
-                            card=curse,
-                            supply=game.supply,
-                        )
+                        opponent.gain(curse, game.supply)
                     except EmptyPile:
                         pass
 
 
-class Moat(Action):
+class SecretPassage(Action):
     """
     +2 cards
+    +1 action
 
-    When another player plays an attack card, you may first
-    reveal this from your hand, to be unaffected by it
+    Take a card from your hand and put it anywhere in your deck.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Moat",
-        cost: int = 2,
-        type: Tuple[str] = ("Action", "Reaction"),
-        draw: int = 2,
-    ):
-        super().__init__(name, cost, type, draw=draw)
+    def __init__(self):
+        super().__init__(name="Secret Passage", cost=4, type=(CardType.Action,), actions=1, draw=2)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
         player.draw(2)
+        player.state.actions += 1
 
+        insert_cards = player.decider.topdeck_decision(
+            prompt="Enter the card you would like to insert in your deck: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_topdeck=1,
+            max_num_topdeck=1,
+        )
+        assert len(insert_cards) == 1
+        insert_card = insert_cards[0]
+
+        len_deck = len(player.deck)
+        if len_deck == 0:
+            index = 0
+        else:
+            index = player.decider.deck_position_decision(
+                prompt=f"Enter the deck position (bottom = 1, top = {len_deck+1}): ",
+                card=self,
+                player=player,
+                game=game,
+                num_deck_cards=len_deck,
+            )
+            assert 0 <= index <= len_deck
 
-class Merchant(Action):
-    """
-    +1 card, +1 action
+        player.hand.remove(insert_card)
+        player.deck.cards.insert(index, insert_card)
 
-    The first time you play a Silver this turn, +1 money
 
+class ShantyTown(Action):
     """
+    +2 Actions
 
-    def __init__(
-        self,
-        name: str = "Merchant",
-        cost: int = 3,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 1,
-    ):
-        super().__init__(name, cost, type, actions=actions, draw=draw)
-
-    def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
-    ) -> None:
-
-        logger.info(f"{player} plays {self}")
-
-        if generic_play:
-            super().generic_play(player)
-
-        player.draw(1)
-        player.state.actions += 1
-
+    Reveal your hand.
+    If you have no Action cards in hand, +2 Cards.
 
-class Bandit(Action):
     """
-    Gain a Gold. Each other player reveals the top 2 cards of their deck,
-    trashes a revealed treasure other than Copper, and discards the rest
 
-    """
-
-    def __init__(
-        self,
-        name: str = "Bandit",
-        cost: int = 5,
-        type: Tuple[str] = ("Action", "Attack"),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Shanty Town", cost=3, type=(CardType.Action,), actions=2)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        # attempt to gain a gold. if gold pile is empty, proceed
-        try:
-            player.gain(card=gold, supply=game.supply)
-        except EmptyPile:
-            pass
-
-        for opponent in game.players:
-            if opponent is not player:
-                if opponent.is_attacked(player=player, attack_card=self):
-
-                    revealed_cards = AbstractDeck()
-                    opponent.draw(num_cards=2, destination=revealed_cards, silent=True)
-
-                    logger.info(f"{opponent} reveals {revealed_cards}")
-
-                    trash_card = None
-                    for card in revealed_cards.cards:
-                        if card.name == "Silver":
-                            trash_card = card
-                        elif card.name == "Gold" and not trash_card:
-                            trash_card = card
-                        elif (
-                            "Treasure" in card.type
-                            and card.name != "Copper"
-                            and not trash_card
-                        ):
-                            trash_card = card
-
-                    if trash_card:
-                        game.trash.add(revealed_cards.remove(trash_card))
+        player.state.actions += 2
 
-                    revealed_cards.move_to(opponent.discard_pile)
-                    del revealed_cards
+        if not any(CardType.Action in c.type for c in player.hand.cards):
+            player.draw(2)
 
 
-class Bureaucrat(Action):
+class Steward(Action):
     """
-    Gain a Silver onto your deck. Each other player reveals a victory card from
-    their hand and puts it onto their deck (or reveals a hand with no victory cards)
+    Choose one: +2 Cards; or +2 money; or trash 2 cards from your hand.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Bureaucrat",
-        cost: int = 4,
-        type: Tuple[str] = ("Action", "Attack"),
-    ):
-        super().__init__(name, cost, type)
+    @unique
+    class Choice(IntEnum):
+        Cards = 0
+        Money = 1
+        Trash = 2
+
+    def __init__(self):
+        super().__init__(name="Steward", cost=3, type=(CardType.Action,))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        # attempt to gain a silver. if silver pile is empty, proceed
-        try:
-            player.gain(card=silver, supply=game.supply, destination=player.deck)
-        except EmptyPile:
-            pass
-
-        for opponent in game.players:
-            if opponent is not player and opponent.is_attacked(
-                player=player, attack_card=self
-            ):
-
-                victory_cards = []
-                for card in opponent.hand.cards:
-                    if "Victory" in card.type:
-                        victory_cards.append(card)
-
-                if not victory_cards:
-                    # Log opponent revealed hand
-                    return
-
-                @validate_input(exceptions=InvalidSingleCardInput)
-                def get_topdeck_card(opponent: Human) -> Card:
-                    topdeck_card = opponent.single_card_decision(
-                        prompt="You must topdeck a Victory card from your hand: ",
-                        valid_cards=victory_cards,
-                    )
-                    if not topdeck_card or isinstance(topdeck_card, str):
-                        raise InvalidSingleCardInput("You must topdeck a Victory card")
-
-                    return topdeck_card
-
-                if isinstance(opponent, Human):
-                    topdeck_card = get_topdeck_card(opponent)
+        options = [
+            "+2 Cards",
+            "+2 Money",
+            "Trash 2 cards from your hand",
+        ]
+        choices = player.decider.multiple_option_decision(
+            card=self,
+            options=options,
+            player=player,
+            game=game,
+        )
+        assert len(choices) == 1
+        choice = choices[0]
 
-                elif isinstance(opponent, Bot):
-                    topdeck_card = opponent.topdeck_resp(
-                        card=self,
-                        valid_cards=victory_cards,
-                        game=game,
-                        required=True,
-                    )
-                    if not topdeck_card:
-                        raise InvalidSingleCardInput("You must topdeck a Victory card")
+        if choice == Steward.Choice.Cards:
+            player.draw(2)
+        elif choice == Steward.Choice.Money:
+            player.state.money += 2
+        elif choice == Steward.Choice.Trash:
+            trash_cards = self._get_trash_cards(player, game)
+            for card in trash_cards:
+                player.trash(card, game.trash)
+        else:
+            raise ValueError(f"Unknown steward choice '{choice}'")
+
+    def _get_trash_cards(self, player: Player, game: "Game") -> List[Card]:
+
+        if len(player.hand) <= 2:
+            return player.hand.cards[:]
+
+        trash_cards = player.decider.trash_decision(
+            prompt="Enter 2 cards you would like to trash from your hand: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_trash=2,
+            max_num_trash=2,
+        )
+        assert len(trash_cards) == 2
 
-                opponent.deck.add(opponent.hand.remove(topdeck_card))
+        return trash_cards
 
 
-class ThroneRoom(Action):
+class Swindler(Action):
     """
-    You may play an Action card from your hand twice
+    +2 Money
+
+    Each other player trashes the top card of their deck and gains a card with
+    the same cost that you choose.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Throne Room",
-        cost: int = 4,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Swindler", cost=3, type=(CardType.Action, CardType.Attack), money=2)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        action_cards = [card for card in player.hand.cards if "Action" in card.type]
-
-        if not action_cards:
-            return
+        player.state.money += 2
 
-        if isinstance(player, Human):
-            dp_card = player.single_card_decision(
-                prompt="You may play an action card from your hand twice: ",
-                valid_cards=action_cards,
-            )
+        for opponent in game.players:
+            if opponent is not player and opponent.is_attacked(player, self, game):
+                revealed_cards = AbstractDeck()
+                opponent.draw(num_cards=1, destination=revealed_cards, silent=True)
+                trashed_card = revealed_cards.cards[0]
+                game.trash.add(trashed_card)
+                trashed_cost = trashed_card.get_cost(player, game)
+
+                logger.info(f"{opponent} trashes {trashed_card}")
+
+                valid_cards = [
+                    c
+                    for c in game.supply.avaliable_cards()
+                    if c.get_cost(player, game) == trashed_cost
+                ]
+                if len(valid_cards) == 0:
+                    continue
+
+                gain_cards = player.decider.gain_decision(
+                    prompt=f"Pick a cost {trashed_cost} card for {opponent} to gain: ",
+                    card=self,
+                    valid_cards=valid_cards,
+                    player=player,
+                    game=game,
+                    min_num_gain=1,
+                    max_num_gain=1,
+                )
+                assert len(gain_cards) == 1
+                gain_card = gain_cards[0]
+                opponent.discard_pile.add(gain_card)
 
-        elif isinstance(player, Bot):
-            dp_card = player.double_play_resp(
-                card=self,
-                valid_cards=action_cards,
-                game=game,
-                required=True,
-            )
+                logger.info(f"{opponent} gains {gain_card}")
 
-        if not dp_card or isinstance(dp_card, str):
-            return
 
-        for card in player.hand.cards:
-            if card.name == dp_card.name:
-                player.playmat.add(player.hand.remove(card))
-                for i in range(2):
-                    player.exact_play(card=card, game=game, generic_play=False)
-                return
+class Torturer(Action):
+    """
+    +3 cards
 
+    Each other player either discards 2 cards or gains a Curse to their
+    hand, their choice. (They may pick an option they can't do.)
 
-class Remodel(Action):
     """
-    Trash a card from your hand. Gain a card costing up to $2 more than it
 
-    """
+    @unique
+    class Choice(IntEnum):
+        Discard = 0
+        GainCurse = 1
 
-    def __init__(
-        self,
-        name: str = "Remodel",
-        cost: int = 4,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Torturer", cost=5, type=(CardType.Action, CardType.Attack), draw=3)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        if isinstance(player, Human):
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def get_trash_card() -> Card:
+        player.draw(3)
 
-                trash_card = player.single_card_decision(
-                    prompt="Trash a card form your hand: ",
-                    valid_cards=player.hand.cards,
+        for opponent in game.players:
+            if opponent is not player and opponent.is_attacked(player, self, game):
+                options = [
+                    "Discard 2 cards",
+                    "Gain a Curse to your hand",
+                ]
+                choices = opponent.decider.multiple_option_decision(
+                    card=self,
+                    options=options,
+                    player=opponent,
+                    game=game,
                 )
+                assert len(choices) == 1
+                choice = choices[0]
 
-                if not trash_card or isinstance(trash_card, str):
-                    raise InvalidSingleCardInput("You must trash a card")
-                return trash_card
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def get_gain_card(trash_card: Card) -> Card:
-
-                gain_card = player.single_card_decision(
-                    prompt=f"Gain a card costing up to {trash_card.cost + 2} money: ",
-                    valid_cards=game.supply.avaliable_cards(),
-                )
+                if choice == Torturer.Choice.Discard:
+                    self._discard(opponent, game)
+                elif choice == Torturer.Choice.GainCurse:
+                    self._gain_curse(opponent, game)
+                else:
+                    raise ValueError(f"Unknown torturer choice '{choice}'")
+
+    def _discard(self, opponent: Player, game: "Game") -> None:
+        num_discard = min(2, len(opponent.hand))
+        if num_discard == 0:
+            return
 
-                if not gain_card or isinstance(gain_card, str):
-                    raise InvalidSingleCardInput("You must gain a card")
-                if gain_card.cost > trash_card.cost + 2:
-                    raise InvalidSingleCardInput(
-                        f"Card must cost less than {trash_card.cost + 2} money"
-                    )
-                return gain_card
+        discard_cards = opponent.decider.discard_decision(
+            prompt=f"You must discard {num_discard} card(s) from your hand: ",
+            card=self,
+            valid_cards=opponent.hand.cards,
+            player=opponent,
+            game=game,
+            min_num_discard=num_discard,
+            max_num_discard=num_discard,
+        )
+        assert len(discard_cards) == num_discard
 
-            trash_card = get_trash_card()
-            gain_card = get_gain_card(trash_card)
+        for card in discard_cards:
+            opponent.discard(target_card=card)
 
-        elif isinstance(player, Bot):
-            trash_card = player.trash_resp(
-                card=self,
-                valid_cards=player.hand.cards,
-                game=game,
-                required=True,
-            )
-            if not trash_card:
-                raise InvalidBotImplementation(
-                    "Card must be trashed when playing remodel"
-                )
-            gain_card = player.gain_resp(
-                card=self,
-                valid_cards=[
-                    card
-                    for card in game.supply.avaliable_cards()
-                    if card.cost <= trash_card.cost + 2
-                ],
-                game=game,
-                required=True,
+    def _gain_curse(self, opponent: Player, game: "Game") -> None:
+        try:
+            opponent.gain(
+                card=curse,
+                supply=game.supply,
+                destination=opponent.hand,
             )
-            if not gain_card:
-                raise InvalidBotImplementation(
-                    "Card must be gained when playing remodel"
-                )
-
-        player.trash(trash_card, trash=game.trash)
-        player.gain(gain_card, game.supply)
+        except EmptyPile:
+            pass
 
 
-class Mine(Action):
+class TradingPost(Action):
     """
-    You may trash a Treasure from your hand. Gain a Treasure to your hand costing up to $3 more than it
+    Trash 2 cards from your hand. If you did, gain a Silver to your hand.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Mine",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Trading Post", cost=5, type=(CardType.Action,))
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        treasures = [card for card in player.hand.cards if "Treasure" in card.type]
-
-        if not treasures:
+        len_hand = len(player.hand)
+        if len_hand == 0:
             return
-
-        if isinstance(player, Human):
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def get_trash_card() -> Optional[Card]:
-
-                trash_card = player.single_card_decision(
-                    prompt="You may trash a Treasure from your hand: ",
-                    valid_cards=treasures,
-                )
-                if isinstance(trash_card, str):
-                    raise InvalidSingleCardInput(f"You can not trash {trash_card}")
-
-                return trash_card
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def get_gain_card(trash_card: Card) -> Card:
-
-                gain_card = player.single_card_decision(
-                    prompt=f"Gain a Treasure card costing up to {trash_card.cost + 3} money to your hand: ",
-                    valid_cards=game.supply.avaliable_cards(),
-                )
-
-                if not gain_card or isinstance(gain_card, str):
-                    raise InvalidSingleCardInput("You must gain a card")
-                if "Treasure" not in trash_card.type:
-                    raise InvalidSingleCardInput("Card must be a Treasure")
-                if gain_card.cost > trash_card.cost + 3:
-                    raise InvalidSingleCardInput(
-                        f"Card must cost less than {trash_card.cost + 3} money"
-                    )
-                return gain_card
-
-            trash_card = get_trash_card()
-            if not trash_card:
-                return
-            gain_card = get_gain_card(trash_card)
-
-        elif isinstance(player, Bot):
-            trash_card = player.trash_resp(
-                card=self,
-                valid_cards=treasures,
-                game=game,
-                required=False,
-            )
-            if not trash_card:
-                return
-
-            gain_card = player.gain_resp(
+        elif len_hand <= 2:
+            trash_cards = player.hand.cards[:]
+        else:
+            trash_cards = player.decider.trash_decision(
+                prompt="Trash 2 cards from your hand: ",
                 card=self,
-                valid_cards=[
-                    card
-                    for card in game.supply.avaliable_cards()
-                    if "Treasure" in card.type and card.cost <= trash_card.cost + 3
-                ],
+                valid_cards=player.hand.cards,
+                player=player,
                 game=game,
-                required=True,
+                min_num_trash=2,
+                max_num_trash=2,
             )
-            if not gain_card:
-                raise InvalidBotImplementation("Card must be gained when playing mine")
-
-        player.trash(trash_card, trash=game.trash)
-        player.gain(gain_card, game.supply, destination=player.hand)
-
-
-class Militia(Action):
-    """
-    +2 Money
-
-    Each other player discards down to 3 cards in hand
-
-    """
-
-    def __init__(
-        self,
-        name: str = "Militia",
-        cost: int = 4,
-        type: Tuple[str] = ("Action", "Attack"),
-        money: int = 2,
-    ):
-        super().__init__(name, cost, type, money=money)
+            assert len(trash_cards) == 2
 
-    def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
-    ) -> None:
-
-        logger.info(f"{player} plays {self}")
-
-        if generic_play:
-            super().generic_play(player)
-
-        player.state.money += 2
-
-        for opponent in game.players:
-            if opponent is not player and opponent.is_attacked(
-                player=player, attack_card=self
-            ):
-
-                num_discard = len(opponent.hand) - 3
-                if num_discard <= 0:
-                    return
-
-                @validate_input(exceptions=InvalidMultiCardInput)
-                def get_discard_cards() -> List[Card]:
-                    cards = opponent.multiple_card_decision(
-                        prompt=f"You must discard {num_discard} cards from your hand: ",
-                        valid_cards=opponent.hand.cards,
-                    )
-                    if len(cards) != num_discard:
-                        raise InvalidMultiCardInput(
-                            f"You must discard {num_discard} cards, you selected {len(cards)}"
-                        )
-                    return cards
-
-                if isinstance(opponent, Human):
-                    discard_cards = get_discard_cards()
-
-                elif isinstance(opponent, Bot):
-                    discard_cards = opponent.multiple_discard_resp(
-                        card=self,
-                        valid_cards=opponent.hand.cards,
-                        game=game,
-                        num_discard=num_discard,
-                        required=True,
-                    )
-                    if not discard_cards:
-                        return
+        for card in trash_cards:
+            player.trash(card, game.trash)
 
-                for card in discard_cards:
-                    opponent.discard(target_card=card)
+        if len(trash_cards) == 2:
+            # attempt to gain a silver to player's hand.
+            # if silver pile is empty, proceed
+            try:
+                player.gain(silver, game.supply, player.hand)
+            except EmptyPile:
+                pass
 
 
-class Sentry(Action):
+class Upgrade(Action):
     """
     +1 card, +1 action
-
-    Look at the top 2 cards of your deck. Trash and/or discard any number of them. Put the rest back on top in any order
+    Trash a card from your hand. Gain a card costing exactly $1 more than it.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Sentry",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-        actions: int = 1,
-        draw: int = 1,
-    ):
-        super().__init__(name, cost, type, actions=actions, draw=draw)
+    def __init__(self):
+        super().__init__(name="Upgrade", cost=5, type=(CardType.Action,), actions=1, draw=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        player.draw()
+        player.draw(1)
         player.state.actions += 1
 
-        revealed = AbstractDeck()
-        player.draw(num_cards=2, destination=revealed, silent=True)
-        logger.info(f"{player} looks at {revealed}")
-
-        if isinstance(player, Human):
+        trash_cards = player.decider.trash_decision(
+            prompt="Trash a card form your hand: ",
+            card=self,
+            valid_cards=player.hand.cards,
+            player=player,
+            game=game,
+            min_num_trash=1,
+            max_num_trash=1,
+        )
+        assert len(trash_cards) == 1
+        trash_card = trash_cards[0]
 
-            def get_trash_cards() -> Optional[List[Card]]:
-                trash_cards = player.multiple_card_decision(
-                    prompt="Enter the cards you would like to trash: ",
-                    valid_cards=revealed.cards,
-                )
-                return trash_cards
+        player.trash(trash_card, trash=game.trash)
 
-            def get_discard_cards(
-                revealed: AbstractDeck,
-            ) -> Optional[List[Card]]:
-                if not revealed.cards:
-                    return None
+        new_cost = trash_card.get_cost(player, game) + 1
+        valid_cards = [
+            card
+            for card in game.supply.avaliable_cards()
+            if card.get_cost(player, game) == new_cost
+        ]
 
-                discard_cards = player.multiple_card_decision(
-                    prompt="Enter the cards you would like to discard: ",
-                    valid_cards=revealed.cards,
-                )
-                return discard_cards
+        if len(valid_cards) == 0:
+            return
 
-            trash_cards = get_trash_cards()
-            if trash_cards:
-                for card in trash_cards:
-                    revealed.remove(card)
-            discard_cards = get_discard_cards(revealed=revealed)
-            if discard_cards:
-                for card in discard_cards:
-                    revealed.remove(card)
-            reorder = False
-            if len(revealed.cards) == 2:
-                logger.info(
-                    f"Current order: {revealed.cards[0]} (Top), {revealed.cards[1]} (Bottom)"
-                )
-                reorder = player.binary_decision(
-                    prompt="Would you like to switch the order of the cards?"
-                )
+        gain_cards = player.decider.gain_decision(
+            prompt=f"Gain a card costing {new_cost} money: ",
+            card=self,
+            valid_cards=valid_cards,
+            player=player,
+            game=game,
+            min_num_gain=1,
+            max_num_gain=1,
+        )
+        assert len(gain_cards) == 1
+        gain_card = gain_cards[0]
+        assert gain_card.get_cost(player, game) == new_cost
 
-        elif isinstance(player, Bot):
-            trash_cards = player.multiple_trash_resp(
-                card=self,
-                valid_cards=revealed.cards,
-                game=game,
-                required=False,
-            )
-            if trash_cards:
-                for card in trash_cards:
-                    revealed.remove(card)
-            discard_cards = player.multiple_discard_resp(
-                card=self,
-                valid_cards=revealed.cards,
-                game=game,
-                required=False,
-            )
-            if discard_cards:
-                for card in discard_cards:
-                    revealed.remove(card)
-            reorder = False
-            if len(revealed.cards) == 2:
-                reorder = player.binary_resp(game=game, card=self)
-
-        if trash_cards:
-            for card in trash_cards:
-                game.trash.add(card)
-                logger.info(f"{player} trashes {card}")
-        if discard_cards:
-            for card in discard_cards:
-                player.discard_pile.add(card)
-                logger.info(f"{player} discards {card}")
-        if revealed.cards:
-            if reorder:
-                for card in revealed.cards:
-                    player.deck.add(card)
-            else:
-                for card in reversed(revealed.cards):
-                    player.deck.add(card)
-            logger.info(f"{player} topdecks {len(revealed.cards)} cards")
+        player.gain(gain_card, game.supply)
 
 
-class Library(Action):
+class WishingWell(Action):
     """
-    Draw until you have 7 cards in hand, skipping any Action cards you choose to; set those aside, discarding them afterwards
+    +1 card, +1 action
+
+    Name a card, then reveal the top card of your deck. If you named it,
+    put it into your hand.
 
     """
 
-    def __init__(
-        self,
-        name: str = "Library",
-        cost: int = 5,
-        type: Tuple[str] = ("Action",),
-    ):
-        super().__init__(name, cost, type)
+    def __init__(self):
+        super().__init__(name="Wishing Well", cost=3, type=(CardType.Action,), actions=1, draw=1)
 
     def play(
-        self, player: Union[Human, Bot], game: "Game", generic_play: bool = True
+        self, player: Player, game: "Game", generic_play: bool = True
     ) -> None:
 
         logger.info(f"{player} plays {self}")
 
         if generic_play:
             super().generic_play(player)
 
-        set_aside = AbstractDeck()
-        while len(player.hand) < 7:
-
-            if len(player.deck) == 0 and len(player.discard_pile) == 0:
-                return
-
-            player.draw(num_cards=1, destination=set_aside)
-            drawn_card = set_aside.cards[-1]
-
-            if "Action" in drawn_card.type:
-                if isinstance(player, Human):
-                    if player.binary_decision(
-                        prompt=f"You drew {drawn_card}, would you like to skip it? y/n: "
-                    ):
-                        pass
-                    else:
-                        player.hand.add(set_aside.remove(drawn_card))
+        player.draw(1)
+        player.state.actions += 1
 
-                    pass
-                if isinstance(player, Bot):
-                    if player.binary_resp(
-                        game=game, card=self, relevant_cards=[drawn_card]
-                    ):
-                        pass
-                    else:
-                        player.hand.add(set_aside.remove(drawn_card))
+        named_cards = player.decider.name_card_decision(
+            prompt="Name a card: ",
+            card=self,
+            valid_cards=game.all_game_cards,
+            player=player,
+            game=game,
+            min_num_name=1,
+            max_num_name=1,
+        )
+        assert len(named_cards) == 1
+        name = named_cards[0].name
 
-            else:
-                player.hand.add(set_aside.remove(drawn_card))
+        logger.info(f"{player} names {name}")
 
-        if set_aside.cards:
-            logger.info(f"{player} discards {set_aside}")
-            set_aside.move_to(destination=player.discard_pile)
-
-
-copper = Copper()
-silver = Silver()
-gold = Gold()
-estate = Estate()
-duchy = Duchy()
-province = Province()
-curse = Curse()
-
-artisan = Artisan()
-bandit = Bandit()
-bureaucrat = Bureaucrat()
-cellar = Cellar()
-chapel = Chapel()
-council_room = CouncilRoom()
-festival = Festival()
-gardens = Gardens()
-harbinger = Harbinger()
-laboratory = Laboratory()
-library = Library()
-market = Market()
-merchant = Merchant()
-militia = Militia()
-mine = Mine()
-moat = Moat()
-moneylender = Moneylender()
-poacher = Poacher()
-remodel = Remodel()
-sentry = Sentry()
-smithy = Smithy()
-throne_room = ThroneRoom()
-vassal = Vassal()
-village = Village()
-witch = Witch()
-workshop = Workshop()
-
-
-base_set = [
-    artisan,
-    bandit,
-    bureaucrat,
-    cellar,
-    chapel,
-    council_room,
-    festival,
-    gardens,
-    harbinger,
-    laboratory,
-    library,
-    market,
-    merchant,
-    militia,
-    mine,
-    moat,
-    moneylender,
-    poacher,
-    remodel,
-    sentry,
-    smithy,
-    throne_room,
-    vassal,
-    village,
-    witch,
-    workshop,
+        revealed = AbstractDeck()
+        player.draw(1, revealed, silent=True)
+        revealed_card = revealed.cards[0]
+        revealed_name = revealed_card.name
+
+        msg = f"{player} reveals {revealed_name} and "
+        if revealed_name == name:
+            player.hand.add(revealed_card)
+            msg += "puts it into their hand"
+        else:
+            player.deck.add(revealed_card)
+            msg += "topdecks it"
+
+        logger.info(msg)
+
+
+baron = Baron()
+bridge = Bridge()
+conspirator = Conspirator()
+courtier = Courtier()
+courtyard = Courtyard()
+diplomat = Diplomat()
+duke = Duke()
+harem = Harem()
+ironworks = Ironworks()
+lurker = Lurker()
+masquerade = Masquerade()
+mill = Mill()
+mining_village = MiningVillage()
+minion = Minion()
+nobles = Nobles()
+patrol = Patrol()
+pawn = Pawn()
+replace = Replace()
+secret_passage = SecretPassage()
+shanty_town = ShantyTown()
+steward = Steward()
+swindler = Swindler()
+torturer = Torturer()
+trading_post = TradingPost()
+upgrade = Upgrade()
+wishing_well = WishingWell()
+
+
+intrigue_set: List[Card] = [
+    baron,
+    bridge,
+    conspirator,
+    courtier,
+    courtyard,
+    diplomat,
+    duke,
+    harem,
+    ironworks,
+    lurker,
+    masquerade,
+    mill,
+    mining_village,
+    minion,
+    nobles,
+    patrol,
+    pawn,
+    replace,
+    secret_passage,
+    shanty_town,
+    steward,
+    swindler,
+    torturer,
+    trading_post,
+    upgrade,
+    wishing_well,
 ]
```

### Comparing `pyminion-0.3.0/pyminion/game.py` & `pyminion-0.4.0/pyminion/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import copy
 import logging
 import random
 from typing import List, Optional
 
-from pyminion.core import Card, Deck, DeckCounter, Pile, Supply, Trash
+from pyminion.core import CardType, Card, Deck, DeckCounter, Pile, Supply, Trash
 from pyminion.exceptions import InvalidGameSetup, InvalidPlayerCount
 from pyminion.expansions.base import (copper, curse, duchy, estate, gold,
                                       province, silver)
-from pyminion.players import Player
+from pyminion.player import Player
 from pyminion.result import GameOutcome, GameResult, PlayerSummary
 
 logger = logging.getLogger()
 
 
 class Game:
     """
@@ -44,14 +43,16 @@
         if len(players) < 1:
             raise InvalidPlayerCount("Game must have at least one player")
         if len(players) > 4:
             raise InvalidPlayerCount("Game can have at most four players")
         self.players = players
         self.expansions = expansions
         self.kingdom_cards = kingdom_cards
+        self.all_game_cards: List[Card] = []
+        self.card_cost_reduction = 0
         self.start_deck = start_deck
         self.random_order = random_order
         self.trash = Trash()
 
         if log_stdout:
             # Set up a handler that logs to stdout
             c_handler = logging.StreamHandler()
@@ -111,17 +112,17 @@
         for card in basic_cards:
             if card.name == "Copper":
                 basic_piles.append(Pile([card] * COPPER_LENGTH))
             elif card.name == "Silver":
                 basic_piles.append(Pile([card] * SILVER_LENGTH))
             elif card.name == "Gold":
                 basic_piles.append(Pile([card] * GOLD_LENGTH))
-            elif "Victory" in card.type:
+            elif CardType.Victory in card.type:
                 basic_piles.append(Pile([card] * VICTORY_LENGTH))
-            elif card.name == "Curse":
+            elif CardType.Curse in card.type:
                 basic_piles.append(Pile([card] * CURSE_LENGTH))
 
         return basic_piles
 
     def _create_kingdom_piles(self) -> List[Pile]:
         """
         Create the kingdom piles that vary from kingdom to kingdom.
@@ -167,30 +168,32 @@
         avaliable in every kingdom as well
         as the kingdom specific cards.
 
         """
 
         basic_piles = self._create_basic_piles()
         kingdom_piles = self._create_kingdom_piles()
-        return Supply(basic_piles + kingdom_piles)
+        all_piles = basic_piles + kingdom_piles
+        self.all_game_cards = [pile.cards[0] for pile in all_piles]
+        return Supply(all_piles)
 
     def start(self) -> None:
         logger.info("\nStarting Game...\n")
 
         self.supply = self._create_supply()
         logger.info(f"Supply: \n{self.supply}")
 
         if self.random_order:
             random.shuffle(self.players)
         if not self.start_deck:
             self.start_deck = [copper] * 7 + [estate] * 3
 
         for player in self.players:
             player.reset()
-            player.discard_pile = Deck(copy.deepcopy(self.start_deck))
+            player.discard_pile = Deck(self.start_deck[:])
             logger.info(f"\n{player} starts with {player.discard_pile}")
             player.draw(5)
 
     def is_over(self) -> bool:
         """
         The game is over if any 3 supply piles are empty or
         if the province pile is empty.
@@ -214,14 +217,18 @@
         return False
 
     def play(self) -> GameResult:
         self.start()
         while True:
             for player in self.players:
                 player.take_turn(self)
+
+                # reset card cost reduction
+                self.card_cost_reduction = 0
+
                 if self.is_over():
                     result = self.summerize_game()
                     logging.info(f"\n{result}")
                     return result
 
     def get_winners(self) -> List[Player]:
         """
```

### Comparing `pyminion-0.3.0/pyminion/players.py` & `pyminion-0.4.0/pyminion/player.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional
 
-from pyminion.core import (AbstractDeck, Card, Deck, DiscardPile, Hand,
+from pyminion.core import (AbstractDeck, Action, CardType, Card, Deck, DiscardPile, Hand,
                            Playmat, Supply, Trash)
-from pyminion.decisions import (binary_decision, multiple_card_decision,
-                                single_card_decision, validate_input)
+from pyminion.decider import Decider
 from pyminion.exceptions import (CardNotFound, EmptyPile, InsufficientBuys,
-                                 InsufficientMoney, InvalidBinaryInput,
-                                 InvalidCardPlay, InvalidMultiCardInput,
-                                 InvalidSingleCardInput)
+                                 InsufficientMoney, InvalidCardPlay)
 
 if TYPE_CHECKING:
     from pyminion.game import Game
 
 
 logger = logging.getLogger()
 
@@ -35,41 +32,45 @@
     Basic representation of a player including the piles of cards they own
     and the basic actions they can take to manipulate the state of the game.
 
     """
 
     def __init__(
         self,
+        decider: Decider,
         deck: Optional[Deck] = None,
         discard_pile: Optional[DiscardPile] = None,
         hand: Optional[Hand] = None,
         playmat: Optional[Playmat] = None,
         state: Optional[State] = None,
         player_id: str = "",
     ):
+        self.decider = decider
         self.deck = deck if deck else Deck()
         self.discard_pile = discard_pile if discard_pile else DiscardPile()
         self.hand = hand if hand else Hand()
         self.playmat = playmat if playmat else Playmat()
         self.state = state if state else State()
         self.player_id = player_id
         self.turns: int = 0
         self.shuffles: int = 0
+        self.actions_played_this_turn: int = 0
 
     def __repr__(self):
         return f"{self.player_id}"
 
     def reset(self):
         """
         Reset the state of the player to a pre-game state.
         Required for resetting player deck and state between games when running simulations.
 
         """
         self.turns = 0
         self.shuffles = 0
+        self.actions_played_this_turn = 0
         self.deck.cards = []
         self.discard_pile.cards = []
         self.hand.cards = []
 
     def draw(
         self,
         num_cards: int = 1,
@@ -127,55 +128,71 @@
         but is overridden for cards like vassal and throne room.
 
         """
         if target_card not in self.hand.cards:
             raise CardNotFound(f"Invalid play, {target_card} not in hand")
         for card in self.hand.cards:
             if card.name == target_card.name:
-                if "Action" in card.type:
+                if CardType.Action in card.type:
+                    self.actions_played_this_turn += 1
                     card.play(player=self, game=game, generic_play=generic_play)
                     return
-                if "Treasure" in card.type:
+                if CardType.Treasure in card.type:
                     card.play(player=self, game=game)
                     return
         raise InvalidCardPlay(f"Invalid play, {target_card} could not be played")
 
     def exact_play(self, card: Card, game: "Game", generic_play: bool = True) -> None:
         """
         Similar to previous play method, except exact card to play must be specified.
         This is method is necessary when playing cards not in the player's hand, such as vassal.
 
         """
-        if "Action" in card.type:
+        if CardType.Action in card.type:
+            self.actions_played_this_turn += 1
             card.play(player=self, game=game, generic_play=generic_play)
-        elif "Treasure" in card.type:
+        elif CardType.Treasure in card.type:
             card.play(player=self, game=game)
         else:
             raise InvalidCardPlay(f"Unable to play {card} with type {card.type}")
 
-    def buy(self, card: Card, supply: "Supply") -> None:
+    def multi_play(self, card: Card, game: "Game", state: Any, generic_play: bool = True) -> Any:
+        """
+        Similar to previous exact_play method, except card's multi_play method is called.
+        This is method is necessary when playing "Throne Room variants".
+
+        """
+        if CardType.Action in card.type:
+            assert isinstance(card, Action)
+            self.actions_played_this_turn += 1
+            state = card.multi_play(player=self, game=game, state=state, generic_play=generic_play)
+        else:
+            raise InvalidCardPlay(f"Unable to play {card} with type {card.type}")
+        return state
+
+    def buy(self, card: Card, game: "Game") -> None:
         """
         Buy a card from the supply and add to player's discard pile.
         Check that player has sufficient money and buys to gain the card.
 
         """
         assert isinstance(card, Card)
-        if card.cost > self.state.money:
+        if card.get_cost(self, game) > self.state.money:
             raise InsufficientMoney(
                 f"{self.player_id}: Not enough money to buy {card.name}"
             )
         if self.state.buys < 1:
             raise InsufficientBuys(
                 f"{self.player_id}: Not enough buys to buy {card.name}"
             )
         try:
-            supply.gain_card(card)
+            game.supply.gain_card(card)
         except EmptyPile as e:
             raise e
-        self.state.money -= card.cost
+        self.state.money -= card.get_cost(self, game)
         self.state.buys -= 1
         self.discard_pile.add(card)
         logger.info(f"{self} buys {card}")
 
     def gain(
         self, card: Card, supply: "Supply", destination: Optional[AbstractDeck] = None
     ) -> None:
@@ -187,68 +204,121 @@
         if destination is None:
             destination = self.discard_pile
 
         gain_card = supply.gain_card(card)
         destination.add(gain_card)
         logger.info(f"{self} gains {gain_card}")
 
-    def trash(self, target_card: Card, trash: "Trash") -> None:
+    def trash(
+        self, target_card: Card, trash: "Trash", source: Optional[AbstractDeck] = None
+    ) -> None:
         """
-        Move card from player's hand to the trash.
+        Move a card from source to the trash.
+        Defaults to moving the card from the player's hand.
 
         """
-        for card in self.hand.cards:
+        if source is None:
+            source = self.hand
+
+        for card in source.cards:
             if card == target_card:
-                trash.add(self.hand.remove(card))
+                trash.add(source.remove(card))
                 logger.info(f"{self} trashes {card}")
 
                 break
 
-    def autoplay_treasures(
-        self, viable_treasures: Optional[List[Card]], game: "Game"
-    ) -> None:
-        """
-        Play all treasures in hand
-
-        """
-        if not viable_treasures:
-            return
-
-        i = 0
-        while i < len(viable_treasures):
-            self.exact_play(viable_treasures[i], game)
-            viable_treasures.remove(viable_treasures[i])
-
     def start_turn(self) -> None:
         """
         Increase turn counter and reset state
 
         """
         self.turns += 1
+        self.actions_played_this_turn = 0
         self.state.actions = 1
         self.state.money = 0
         self.state.buys = 1
 
-    def start_cleanup_phase(self):
+    def start_action_phase(self, game: "Game") -> None:
+        while self.state.actions > 0:
+            logger.info(f"{self.player_id}'s hand: {self.hand}")
+
+            viable_actions = [card for card in self.hand.cards if CardType.Action in card.type]
+            if not viable_actions:
+                return
+
+            card = self.decider.action_phase_decision(viable_actions, self, game)
+            if card is None:
+                return
+
+            self.play(card, game)
+
+    def start_treasure_phase(self, game: "Game") -> None:
+        viable_treasures = [card for card in self.hand.cards if CardType.Treasure in card.type]
+        while len(viable_treasures) > 0:
+            logger.info(f"Hand: {self.hand}")
+
+            cards = self.decider.treasure_phase_decision(viable_treasures, self, game)
+            if len(cards) == 0:
+                break
+
+            for card in cards:
+                self.exact_play(card, game)
+            cards_str = ", ".join([str(c) for c in cards])
+            logger.info(f"{self.player_id} played {cards_str}")
+
+            viable_treasures = [card for card in self.hand.cards if CardType.Treasure in card.type]
+
+    def start_buy_phase(self, game: "Game") -> None:
+        while self.state.buys > 0:
+            logger.info(f"\nSupply:{game.supply}")
+            logger.info(f"Money: {self.state.money}")
+            logger.info(f"Buys: {self.state.buys}")
+
+            valid_cards = [
+                c
+                for c in game.supply.avaliable_cards()
+                if c.get_cost(self, game) <= self.state.money
+            ]
+            card = self.decider.buy_phase_decision(
+                valid_cards=valid_cards,
+                player=self,
+                game=game,
+            )
+
+            if card is None:
+                logger.info(f"{self} buys nothing")
+                break
+
+            self.buy(card, game)
+
+    def start_cleanup_phase(self) -> None:
         """
         Move hand and playmat cards into discard pile and draw 5 new cards.
 
         """
         self.discard_pile.cards += self.hand.cards
         self.discard_pile.cards += self.playmat.cards
         self.hand.cards = []
         self.playmat.cards = []
         self.draw(5)
         self.state.actions = 1
         self.state.money = 0
         self.state.buys = 1
 
+    def take_turn(self, game: "Game") -> None:
+        self.start_turn()
+        logger.info(f"\nTurn {self.turns} - {self.player_id}")
+        self.start_action_phase(game)
+        self.start_treasure_phase(game)
+        self.start_buy_phase(game)
+        self.start_cleanup_phase()
+
     def get_all_cards(self) -> List[Card]:
         """
-        Get a list of all the cards the player has in their possesion.
+        Get a list of all the cards the player has in their possession.
 
         """
         all_cards = (
             self.deck.cards
             + self.discard_pile.cards
             + self.playmat.cards
             + self.hand.cards
@@ -265,174 +335,58 @@
     def get_victory_points(self) -> int:
         """
         Return the number of victory points a player has.
 
         """
         total_vp: int = 0
         for card in self.get_all_cards():
-            if "Victory" in card.type or "Curse" in card.type:
+            if CardType.Victory in card.type or CardType.Curse in card.type:
                 total_vp += card.score(self)
         return total_vp
 
     def get_treasure_money(self) -> int:
         """
         Return the amount of money a player has in their deck from treasure cards.
 
         """
         total_money: int = 0
         for card in self.get_all_cards():
-            if "Treasure" in card.type:
+            if CardType.Treasure in card.type:
                 total_money += card.money
         return total_money
 
     def get_action_money(self) -> int:
         """
         Return the amount of money a player has in their deck from action cards.
 
         """
         total_money: int = 0
         for card in self.get_all_cards():
-            if "Action" in card.type:
+            if CardType.Action in card.type:
                 total_money += card.money
         return total_money
 
     def get_deck_money(self) -> int:
         """
         Return total count of all money a player has in their deck.
 
         """
         treasure_money = self.get_treasure_money()
         action_money = self.get_action_money()
         return treasure_money + action_money
 
-
-class Human(Player):
-    """
-    Human player can make choices as to which cards
-    to play and buy in real time through the terminal
-
-    """
-
-    def __init__(
-        self,
-        deck: Optional[Deck] = None,
-        player_id: str = "human",
-    ):
-        super().__init__(deck=deck, player_id=player_id)
-
-    @staticmethod
-    @validate_input(exceptions=InvalidBinaryInput)
-    def binary_decision(prompt: str) -> bool:
-        """
-        Wrap binary_decision with @validate_input decorator to
-        repeat prompt if input is invalid.
-
-        """
-        return binary_decision(prompt=prompt)
-
-    @staticmethod
-    @validate_input(exceptions=InvalidSingleCardInput)
-    def single_card_decision(
-        prompt: str,
-        valid_cards: List[Card],
-    ) -> Optional[Union[Card, str]]:
-        """
-        Wrap single_card_decision with @validate_input decorator to
-        repeat prompt if input is invalid.
-
-        """
-
-        return single_card_decision(prompt=prompt, valid_cards=valid_cards)
-
-    @staticmethod
-    @validate_input(exceptions=InvalidMultiCardInput)
-    def multiple_card_decision(
-        prompt: str,
-        valid_cards: List[Card],
-    ) -> Optional[List[Card]]:
-        """
-        Wrap multiple_card_decision with @validate_input decorator to
-        repeat prompt if input is invalid.
-
-        """
-        return multiple_card_decision(prompt=prompt, valid_cards=valid_cards)
-
-    def is_attacked(self, player: Player, attack_card: Card) -> bool:
+    def is_attacked(self, player: "Player", attack_card: Card, game: "Game") -> bool:
+        attacked = True
         for card in self.hand.cards:
             if card.name == "Moat":
-                block = self.binary_decision(
-                    prompt=f"Would you like to block {player.player_id}'s {attack_card} with your Moat? y/n: "
+                block = self.decider.binary_decision(
+                    prompt=f"Would you like to block {player.player_id}'s {attack_card} with your Moat? y/n: ",
+                    card=card,
+                    player=self,
+                    game=game,
+                    relevant_cards=[attack_card],
                 )
-                return not block
-        return True
-
-    def start_action_phase(self, game: "Game") -> None:
-        while self.state.actions:
+                attacked &= not block
+            elif card.name == "Diplomat":
+                card.on_attack(self, attack_card, game)
 
-            viable_actions = [card for card in self.hand.cards if "Action" in card.type]
-            if not viable_actions:
-                return
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def choose_action(game: "Game") -> None:
-                logger.info(f"Hand: {self.hand}")
-                card = single_card_decision(
-                    prompt="Choose an action card to play: ",
-                    valid_cards=viable_actions,
-                )
-                if not card or isinstance(card, str):
-                    return
-                self.play(card, game)
-                return
-
-            choose_action(game)
-
-    def start_treasure_phase(self, game: "Game") -> None:
-        viable_treasures = [card for card in self.hand.cards if "Treasure" in card.type]
-        while viable_treasures:
-
-            @validate_input(exceptions=InvalidSingleCardInput)
-            def choose_treasure(game: "Game") -> None:
-                logger.info(f"Hand: {self.hand}")
-                response = single_card_decision(
-                    prompt="Choose an treasure card to play or 'all' to autoplay treasures: ",
-                    valid_cards=viable_treasures,
-                    valid_mixin="all",
-                )
-                if response == "all":
-                    self.autoplay_treasures(
-                        viable_treasures=viable_treasures, game=game
-                    )
-                    return
-                if not response or isinstance(response, str):
-                    return
-                self.exact_play(response, game)
-                logger.info(f"{self.player_id} played {response}")
-                viable_treasures.remove(response)
-
-            choose_treasure(game)
-
-    def start_buy_phase(self, game: "Game") -> None:
-        while self.state.buys:
-            logger.info(f"\nSupply:{game.supply}")
-            logger.info(f"Money: {self.state.money}")
-            logger.info(f"Buys: {self.state.buys}")
-
-            @validate_input(exceptions=(InvalidSingleCardInput, InsufficientMoney))
-            def choose_buy(game: "Game") -> None:
-                card = single_card_decision(
-                    prompt="Choose a card to buy: ",
-                    valid_cards=game.supply.avaliable_cards(),
-                )
-                if not card or isinstance(card, str):
-                    return
-                self.buy(card, game.supply)
-
-            choose_buy(game)
-
-    def take_turn(self, game: "Game") -> None:
-        self.start_turn()
-        logger.info(f"\nTurn {self.turns} - {self.player_id}")
-        self.start_action_phase(game)
-        self.start_treasure_phase(game)
-        self.start_buy_phase(game)
-        self.start_cleanup_phase()
+        return attacked
```

### Comparing `pyminion-0.3.0/pyminion/result.py` & `pyminion-0.4.0/pyminion/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from pyminion.core import DeckCounter
     from pyminion.game import Game
-    from pyminion.players import Player
+    from pyminion.player import Player
 
 
 class GameOutcome(Enum):
     """
     player can either lose, tie, or win the game
 
     """
```

### Comparing `pyminion-0.3.0/pyminion/simulator.py` & `pyminion-0.4.0/pyminion/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import logging
 from typing import Dict, List
 
 from pyminion.game import Game
-from pyminion.players import Player
+from pyminion.player import Player
 from pyminion.result import GameResult, PlayerSimulatorResult, SimulatorResult
 
 logger = logging.getLogger()
 
 
 def get_percent(occurrence: int, total: int) -> float:
     """
```

### Comparing `pyminion-0.3.0/pyminion.egg-info/PKG-INFO` & `pyminion-0.4.0/pyminion.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyminion
-Version: 0.3.0
+Version: 0.4.0
 Summary: Dominion but make it python
 Home-page: https://github.com/evanofslack/pyminion
 Author: Evan Slack
 Author-email: evan.slack@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,120 +13,145 @@
 License-File: LICENSE
 
 # Pyminion
 
 [![tests](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml/badge.svg)](https://github.com/evanofslack/pyminion/actions/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/evanofslack/pyminion/branch/master/graph/badge.svg?token=5GW65KFEL5)](https://codecov.io/gh/evanofslack/pyminion)
 
+<img width="800" alt="pyminion-logo" src="https://github.com/evanofslack/pyminion/assets/51209817/85e6ed9f-8cbf-4781-9c0b-f29c1d0a2162">
+<br></br>
 
-Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/). At its core, pyminion implements the rules and logic of Dominion and provides an API to interact with the game engine. In addition, it enables interactive games through the command line and simulation of games between bots.
+Pyminion is a library for executing and analyzing games of [Dominion](https://www.riograndegames.com/games/dominion/).
+At its core, pyminion implements the rules and logic of Dominion and provides
+an API to interact with the game engine. In addition, it enables interactive
+games through the command line and simulation of games between bots.
 
 ## Table of Contents
 
--   [Installation](#installation)
--   [Usage](#usage)
--   [Support](#support)
--   [Contributing](#contributing)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [Contributing](#contributing)
 
-## Getting Started
+## Installation
 
 Pyminion requires at least Python 3.8 and can easily be installed through pypi
 
-```
+```bash
 python3 -m pip install pyminion
 ```
 
 ## Usage
 
 ### Setting up a game
 
-To play an interactive game through the command line against a bot, initialize a human and a bot and assign them as players. Alternatively, games can be created between multiple humans or multiple bots. 
+To play an interactive game through the command line against a bot, initialize
+a human and a bot and assign them as players. Alternatively, games can be
+created between multiple humans or multiple bots.
 
 ```python
-from pyminion.expansions.base import base_set 
+from pyminion.expansions.base import base_set
+from pyminion.expansions.intrigue import intrigue_set
 from pyminion.game import Game
 from pyminion.bots.examples import BigMoney
-from pyminion.players import Human
+from pyminion.human import Human
 
 # Initialize human and bot
 human = Human()
 bot = BigMoney()
 
 # Setup the game
-game = Game(players=[human, bot], expansions=[base_set])
+game = Game(players=[human, bot], expansions=[base_set, intrigue_set])
 
 # Play game
 game.play()
 
 ```
+
 ### Creating Bots
 
-Defining new bots is relatively straightforward. Inherit from the `Bot` class and implement play and buy strategies in the `action_priority` and `buy_priority` methods respectively.
+Defining new bots is relatively straightforward. Inherit from the
+`BotDecider` class and implement play and buy strategies in the
+`action_priority` and `buy_priority` methods respectively.
 
 For example, here is a simple big money + smithy bot:
 
 ```python
-from pyminion.bots.bot import Bot
+from pyminion.bots.bot import Bot, BotDecider
+from pyminion.expansions.base import gold, province, silver, smithy
+from pyminion.player import Player
 from pyminion.game import Game
-from pyminion.expansions.base import silver, gold, province, smithy
 
-class BigMoneySmithy(Bot):
+class BigMoneySmithyDecider(BotDecider):
+    """
+    Big money + smithy
 
-    def __init__(
-        self,
-        player_id: str = "big_money_smithy",
-    ):
-        super().__init__(player_id=player_id)
+    """
 
-    def action_priority(self, game: Game):
+    def action_priority(self, player: Player, game: Game):
         yield smithy
 
-    def buy_priority(self, game: Game):
-        money = self.state.money
+    def buy_priority(self, player: Player, game: Game):
+        money = player.state.money
         if money >= 8:
             yield province
         if money >= 6:
             yield gold
         if money == 4:
             yield smithy
         if money >= 3:
             yield silver
+
+class BigMoneySmithy(Bot):
+    def __init__(
+        self,
+        player_id: str = "big_money_smithy",
+    ):
+        super().__init__(decider=BigMoneySmithyDecider(), player_id=player_id)
 ```
 
 To see other bot implementations with more advanced decision trees, see [/bots](https://github.com/evanofslack/pyminion/tree/master/pyminion/bots)
 
 ### Running Simulations
 
-Simulating multiple games is good metric for determining bot performance. To create a simulation, pass a pyminion game instance into the `Simulator` class and set the number of iterations to be run. 
+Simulating multiple games is good metric for determining bot performance.
+To create a simulation, pass a pyminion game instance into the `Simulator`
+class and set the number of iterations to be run.
 
 ```python
 from pyminion.bots.examples import BigMoney, BigMoneySmithy
 from pyminion.expansions.base import base_set, smithy
 from pyminion.game import Game
 from pyminion.simulator import Simulator
 
 bm = BigMoney()
 bm_smithy = BigMoneySmithy()
 
-game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy])
+game = Game(players=[bm, bm_smithy], expansions=[base_set], kingdom_cards=[smithy], log_stdout=False)
 sim = Simulator(game, iterations=1000)
-sim.run()
+result = sim.run()
+print(result)
 ```
 
-with the following terminal output: 
+with the following terminal output:
+
 ```console
 ~$ python simulation.py
-Simulation of 1000 games
-big_money wins: 16.8% (168)
-big_money_smithy wins: 57.5% (575)
-Ties: 25.7% (257)
+Simulation Result: ran 1000 games
+big_money won 110, lost 676, tied 214
+big_money_smithy won 676, lost 110, tied 214
 ```
-Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.  
+
+Please see [/examples](https://github.com/evanofslack/pyminion/tree/master/examples) to see demo scripts.
+
 ## Support
 
 Please [open an issue](https://github.com/evanofslack/pyminion/issues/new) for support.
 
 ## Contributing
 
-Install this library, test it out, and report any bugs. A welcome contribution would be to create new bots, especially an implementation that uses machine learning to determine optimal play. 
+Install this library, test it out, and report any bugs. A welcome contribution
+would be to create new bots, especially an implementation that uses machine
+learning to determine optimal play.
 
-If you would like to contribute, please create a branch, add commits, and [open a pull request](https://github.com/evanofslack/pyminion/pulls).
+If you would like to contribute, please create a branch, add commits, and
+[open a pull request](https://github.com/evanofslack/pyminion/pulls).
```

### Comparing `pyminion-0.3.0/pyminion.egg-info/SOURCES.txt` & `pyminion-0.4.0/pyminion.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pyminion/__init__.py
 pyminion/core.py
-pyminion/decisions.py
+pyminion/decider.py
 pyminion/exceptions.py
 pyminion/game.py
-pyminion/players.py
+pyminion/human.py
+pyminion/player.py
 pyminion/result.py
 pyminion/simulator.py
 pyminion.egg-info/PKG-INFO
 pyminion.egg-info/SOURCES.txt
 pyminion.egg-info/dependency_links.txt
 pyminion.egg-info/top_level.txt
 pyminion/bots/__init__.py
```

### Comparing `pyminion-0.3.0/setup.py` & `pyminion-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyminion",
-    version="0.3.0",
+    version="0.4.0",
     author="Evan Slack",
     author_email="evan.slack@outlook.com",
     description="Dominion but make it python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/evanofslack/pyminion",
     classifiers=[
```

