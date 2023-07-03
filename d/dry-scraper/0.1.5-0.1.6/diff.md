# Comparing `tmp/dry_scraper-0.1.5.tar.gz` & `tmp/dry_scraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.5.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.6.tar", max compression
```

## Comparing `dry_scraper-0.1.5.tar` & `dry_scraper-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.5/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.5/README.md
--rw-r--r--   0        0        0      546 2023-07-01 23:34:52.916761 dry_scraper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.5/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2444 2023-06-30 23:14:23.236239 dry_scraper-0.1.5/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.5/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    26088 2023-07-03 00:36:30.136173 dry_scraper-0.1.5/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    11711 2023-07-02 23:21:46.793235 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.5/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.5/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 dry_scraper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.6/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.6/README.md
+-rw-r--r--   0        0        0      546 2023-07-03 20:41:11.601910 dry_scraper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.6/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-30 23:14:23.236239 dry_scraper-0.1.6/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.6/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28334 2023-07-03 23:43:45.569901 dry_scraper-0.1.6/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    12134 2023-07-03 22:38:23.766400 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.6/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.6/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 dry_scraper-0.1.6/PKG-INFO
```

### Comparing `dry_scraper-0.1.5/LICENSE` & `dry_scraper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/README.md` & `dry_scraper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/pyproject.toml` & `dry_scraper-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.5"
+version = "0.1.6"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.5/src/dry_scraper/data_source.py` & `dry_scraper-0.1.6/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -520,14 +520,37 @@
             f"{self.season[:4]}"
             "0"
             f"{self.gamePk}"
             "/linescore"
         )
 
 
+def determine_team_decision(team_win: bool, ordinal: str) -> str:
+    """
+    Determine the decision of the game from the perspective of one team
+    e.g., RW, OTL, SOW, etc.
+
+    Parameters
+    ----------
+    team_win : bool
+        bool describing if the team in question won or not
+    ordinal : str
+        ordinal str describing the most recent period played
+        e.g., 3rd, OT, SO
+
+    Returns
+    -------
+    decision : str
+        string describing decision of game from the perspective of one team
+        e.g., RW, OTL, SOW, etc.
+    """
+    decision = "R" if ordinal == "3rd" else ordinal
+    return decision + "W" if team_win else decision + "L"
+
+
 class NhlGameLiveFeedApiSource(NhlGameApiSource):
     """
     Subclass of NhlApiSource that represents a request from the NHL live feed API
 
     ...
 
     Attributes
@@ -742,29 +765,59 @@
         away_stats_pyd = self.content_pyd.live_data.box_score.teams.away
         team_stats_df = pd.DataFrame(
             {
                 col: pd.Series(dtype=typ)
                 for col, typ in nhl_game_live_feed_api_source.team_stats_df_model.items()
             }
         )
-        for home, team in [(True, home_stats_pyd), (False, away_stats_pyd)]:
-            stats = team.team_stats.team_skater_stats
+        home_win = (
+            self.content_pyd.live_data.line_score.teams.home.goals
+            > self.content_pyd.live_data.line_score.teams.away.goals
+        )
+        for home, team, opp in [
+            (True, home_stats_pyd, away_stats_pyd),
+            (False, away_stats_pyd, home_stats_pyd),
+        ]:
+            team_stats = team.team_stats.team_skater_stats
+            opp_stats = opp.team_stats.team_skater_stats
             team_dict = {
                 "season": int(self.season),
                 "gamePk": int(self.gamePk),
+                "start_date_time": self.content_pyd.game_data.date_time.date_time,
+                "end_date_time": self.content_pyd.game_data.date_time.end_date_time,
                 "team_id": int(team.team.id),
                 "team_name": str(team.team.name),
-                "home": home,
-                "goals": int(stats.goals),
-                "pim": int(stats.pim),
-                "shots": int(stats.shots),
-                "power_play_percentage": float(stats.power_play_percentage),
-                "power_play_goals": int(stats.power_play_goals),
-                "power_play_opportunities": int(stats.power_play_opportunities),
-                "face_off_win_percentage": float(stats.face_off_win_percentage),
-                "blocked": int(stats.blocked),
-                "takeaways": int(stats.takeaways),
-                "giveaways": int(stats.giveaways),
-                "hits": int(stats.hits),
+                "opp_id": int(opp.team.id),
+                "opp_name": str(opp.team.name),
+                "team_home": home,
+                "team_goals": int(team_stats.goals),
+                "team_pim": int(team_stats.pim),
+                "team_sog": int(team_stats.shots),
+                "team_ppp": float(team_stats.power_play_percentage),
+                "team_ppg": int(team_stats.power_play_goals),
+                "team_ppo": int(team_stats.power_play_opportunities),
+                "team_fop": float(team_stats.face_off_win_percentage),
+                "team_blocked": int(team_stats.blocked),
+                "team_takeaways": int(team_stats.takeaways),
+                "team_giveaways": int(team_stats.giveaways),
+                "team_hits": int(team_stats.hits),
+                "opp_goals": int(opp_stats.goals),
+                "opp_pim": int(opp_stats.pim),
+                "opp_sog": int(opp_stats.shots),
+                "opp_ppp": float(opp_stats.power_play_percentage),
+                "opp_ppg": int(opp_stats.power_play_goals),
+                "opp_ppo": int(opp_stats.power_play_opportunities),
+                "opp_fop": float(opp_stats.face_off_win_percentage),
+                "opp_blocked": int(opp_stats.blocked),
+                "opp_takeaways": int(opp_stats.takeaways),
+                "opp_giveaways": int(opp_stats.giveaways),
+                "opp_hits": int(opp_stats.hits),
+                "team_gd": int(team_stats.goals) - int(opp_stats.goals),
+                "team_decision": determine_team_decision(
+                    home_win if home else not home_win,
+                    self.content_pyd.live_data.line_score.current_period_ordinal,
+                ),
             }
-            team_stats_df.loc["Home" if home else "Away"] = team_dict
+            team_stats_df.loc[
+                f"{self.gamePk} Home" if home else f"{self.gamePk} Away"
+            ] = team_dict
         return team_stats_df
```

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -391,22 +391,39 @@
     "team_name": "str",
     "team_tricode": "str",
 }
 
 team_stats_df_model = {
     "season": "int",
     "gamePk": "int",
+    "start_date_time": "datetime64[s]",
+    "end_date_time": "datetime64[s]",
     "team_id": "int",
     "team_name": "str",
-    "home": "bool",
-    "goals": "int",
-    "pim": "int",
-    "shots": "int",
-    "power_play_percentage": "float",
-    "power_play_goals": "int",
-    "power_play_opportunities": "int",
-    "face_off_win_percentage": "float",
-    "blocked": "int",
-    "takeaways": "int",
-    "giveaways": "int",
-    "hits": "int",
+    "opp_id": "int",
+    "opp_name": "str",
+    "team_home": "bool",
+    "team_goals": "int",
+    "team_pim": "int",
+    "team_shg": "int",
+    "team_ppp": "float",
+    "team_ppg": "int",
+    "team_ppo": "int",
+    "team_fop": "float",
+    "team_blocked": "int",
+    "team_takeaways": "int",
+    "team_giveaways": "int",
+    "team_hits": "int",
+    "opp_goals": "int",
+    "opp_pim": "int",
+    "opp_shg": "int",
+    "opp_ppp": "float",
+    "opp_ppg": "int",
+    "opp_ppo": "int",
+    "opp_fop": "float",
+    "opp_blocked": "int",
+    "opp_takeaways": "int",
+    "opp_giveaways": "int",
+    "opp_hits": "int",
+    "team_gd": "int",
+    "team_decision": "str",
 }
```

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.6/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/shared.py` & `dry_scraper-0.1.6/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/src/dry_scraper/teams.py` & `dry_scraper-0.1.6/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.5/PKG-INFO` & `dry_scraper-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

