# Comparing `tmp/lemmy_nhl-1.5.3.tar.gz` & `tmp/lemmy_nhl-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemmy_nhl-1.5.3.tar", last modified: Mon Jul  3 04:10:51 2023, max compression
+gzip compressed data, was "lemmy_nhl-1.5.4.tar", last modified: Tue Jul  4 07:52:22 2023, max compression
```

## Comparing `lemmy_nhl-1.5.3.tar` & `lemmy_nhl-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/lemmy_nhl/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/draft_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-07-03 04:10:40.000000 lemmy_nhl-1.5.3/src/lemmy_nhl/post_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:10:51.380851 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 04:10:51.000000 lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/src/lemmy_nhl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/src/lemmy_nhl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/src/lemmy_nhl/draft_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-07-04 07:52:11.000000 lemmy_nhl-1.5.4/src/lemmy_nhl/post_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:52:22.676021 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 07:52:22.000000 lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/top_level.txt
```

### Comparing `lemmy_nhl-1.5.3/LICENSE` & `lemmy_nhl-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.3/PKG-INFO` & `lemmy_nhl-1.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemmy_nhl
-Version: 1.5.3
+Version: 1.5.4
 Summary: bot to add live scores to lemmy community for hockey games
 Home-page: https://github.com/socphoenix/lemmy_nhl_bot
 Author: socphoenix
 License: Apache 2.0
 Keywords: lemmy,hockey,bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -72,18 +72,19 @@
 ### Run config.py:
 > Linux: lemmy_nhl_config
 
 >FreeBSD: lemmy_nhl_config.py ##This requires path set. for sh (default shell): "PATH=${PATH}:/home/'put user here'/.local/bin" "export PATH" (as an interesting note, python seems to only add the path to the root user during install)
 
 ### run daemon
 
-Unix:
- > lemmy_nhl_daemon
+Linux:
+ > lemmy_nhl_daemon &
  >
- > add " &" to run in the background. Working on creating service files but they are not done yet.
+ > FreeBSD:
+ > daemon lemmy_nhl_daemon
 
 
 ### run draft bot
 
 Unix: lemmy_nhl_draft
```

### Comparing `lemmy_nhl-1.5.3/README.md` & `lemmy_nhl-1.5.4/src/lemmy_nhl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: lemmy-nhl
+Version: 1.5.4
+Summary: bot to add live scores to lemmy community for hockey games
+Home-page: https://github.com/socphoenix/lemmy_nhl_bot
+Author: socphoenix
+License: Apache 2.0
+Keywords: lemmy,hockey,bot
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # A few things to note currently:
 
 > Without modifying files, there is currently no way to test this. I've tested that it works with old data, and will be testing/
 > fixing whatever needs it during the first preseason game of the Flyers (or earlier if someone reports an issue before this).
 
 
 # lemmy_nhl_bot
@@ -61,18 +72,19 @@
 ### Run config.py:
 > Linux: lemmy_nhl_config
 
 >FreeBSD: lemmy_nhl_config.py ##This requires path set. for sh (default shell): "PATH=${PATH}:/home/'put user here'/.local/bin" "export PATH" (as an interesting note, python seems to only add the path to the root user during install)
 
 ### run daemon
 
-Unix:
- > lemmy_nhl_daemon
+Linux:
+ > lemmy_nhl_daemon &
  >
- > add " &" to run in the background. Working on creating service files but they are not done yet.
+ > FreeBSD:
+ > daemon lemmy_nhl_daemon
 
 
 ### run draft bot
 
 Unix: lemmy_nhl_draft
```

### Comparing `lemmy_nhl-1.5.3/setup.cfg` & `lemmy_nhl-1.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lemmy_nhl
-version = 1.5.3
+version = 1.5.4
 author = socphoenix
 url = https://github.com/socphoenix/lemmy_nhl_bot
 description = bot to add live scores to lemmy community for hockey games
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = lemmy, hockey, bot
 license = Apache 2.0
```

### Comparing `lemmy_nhl-1.5.3/src/lemmy_nhl/config.py` & `lemmy_nhl-1.5.4/src/lemmy_nhl/config.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.3/src/lemmy_nhl/draft_bot.py` & `lemmy_nhl-1.5.4/src/lemmy_nhl/draft_bot.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.3/src/lemmy_nhl/post_body.py` & `lemmy_nhl-1.5.4/src/lemmy_nhl/post_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,18 @@
     body = body + "| " + str(currentPeriod) + " | " + timeLeft + " | \n"
     body = body + "## Scores: \n"
     if(numPeriods <= 2):
         body = body + "| Team | Period 1: | Period 2:  | Period 3: | Totals | \n"
         body = body + "| ----- | -------- | ---------- | ----------- | ------| \n"
         body = body + "| " + away_name + " | " +  str(period[0].get("away").get("goals")) + " | "
         body = body +  str(period[1].get("away").get("goals")) + " | " +  str(period[2].get("away").get("goals")) + " | "
-        body = body + away_goals + " | \n"
+        body = body + str(away_goals) + " | \n"
         body = body + "| " + home_name + " | " +  str(period[0].get("home").get("goals")) + " | "
         body = body + str(period[1].get("home").get("goals")) + " | " + str(period[2].get("home").get("goals")) + " | "
-        body = body + home_goals + " | \n"
+        body = body + str(home_goals) + " | \n"
     else:
         body = body + "| Team | Period 1: | Period 2:  | Period 3: | OT | Totals | \n"
         body = body + "| ----- | -------- | ---------- | --------- | ------| ----- | \n"
         body = body + "| " + away_name + " | " +  str(period[0].get("away").get("goals")) + " | "
         body = body +  str(period[1].get("away").get("goals")) + " | " +  str(period[2].get("away").get("goals")) + " | "
         body = body + str(period[numPeriods].get("away").get("goals")) + " | " + str(away_goals) + " | \n"
         body = body + "| " + home_name + " | " +  str(period[0].get("home").get("goals")) + " | "
@@ -199,8 +199,14 @@
         body = body + str(homeOtShots) + " | " + str(home_shots) + " | \n"
     #Power Play status
     body = body + "## Power Play \n"
     body = body + "| Team | On PowerPlay | \n"
     body = body + "| ----- | ------------ | \n"
     body = body + "| " + away_name + " | " + str(away_power) + " | \n"
     body = body + "| " + home_name + " | " + str(home_power) + " | \n"
+    # game highlights
+    r = requests.get("https://statsapi.web.nhl.com/api/v1/game/" + str(gamePK) + "/content")
+    body = body + "# Game Highlights \n"
+    for x in range(len(r.json().get("highlights").get("scoreboard").get("items"))):
+        body = body + "\n" + "[" + r.json().get("highlights").get("scoreboard").get("items")[x].get("description") + "]("
+        body = body + r.json().get("highlights").get("scoreboard").get("items")[x].get("playbacks")[3].get("url") + ") \n"
     return body, gameOver
```

### Comparing `lemmy_nhl-1.5.3/src/lemmy_nhl.egg-info/PKG-INFO` & `lemmy_nhl-1.5.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: lemmy-nhl
-Version: 1.5.3
-Summary: bot to add live scores to lemmy community for hockey games
-Home-page: https://github.com/socphoenix/lemmy_nhl_bot
-Author: socphoenix
-License: Apache 2.0
-Keywords: lemmy,hockey,bot
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # A few things to note currently:
 
 > Without modifying files, there is currently no way to test this. I've tested that it works with old data, and will be testing/
 > fixing whatever needs it during the first preseason game of the Flyers (or earlier if someone reports an issue before this).
 
 
 # lemmy_nhl_bot
@@ -72,18 +61,19 @@
 ### Run config.py:
 > Linux: lemmy_nhl_config
 
 >FreeBSD: lemmy_nhl_config.py ##This requires path set. for sh (default shell): "PATH=${PATH}:/home/'put user here'/.local/bin" "export PATH" (as an interesting note, python seems to only add the path to the root user during install)
 
 ### run daemon
 
-Unix:
- > lemmy_nhl_daemon
+Linux:
+ > lemmy_nhl_daemon &
  >
- > add " &" to run in the background. Working on creating service files but they are not done yet.
+ > FreeBSD:
+ > daemon lemmy_nhl_daemon
 
 
 ### run draft bot
 
 Unix: lemmy_nhl_draft
```

