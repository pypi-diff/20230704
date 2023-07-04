# Comparing `tmp/dry_scraper-0.1.8.5.tar.gz` & `tmp/dry_scraper-0.1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.5.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.6.tar", max compression
```

## Comparing `dry_scraper-0.1.8.5.tar` & `dry_scraper-0.1.8.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.5/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.5/README.md
--rw-r--r--   0        0        0      548 2023-07-04 02:50:20.109973 dry_scraper-0.1.8.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.5/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.5/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.5/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.5/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/base_model.py
--rw-r--r--   0        0        0      688 2023-07-04 02:40:37.712254 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0     1044 2023-07-04 02:41:13.692518 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     6823 2023-07-04 02:46:41.274969 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    14453 2023-07-04 02:38:10.804523 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1874 2023-07-04 02:46:14.581433 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     2186 2023-07-04 02:50:05.229858 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.5/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.5/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.6/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.6/README.md
+-rw-r--r--   0        0        0      548 2023-07-04 03:22:15.617160 dry_scraper-0.1.8.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.6/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.6/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.6/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28441 2023-07-04 03:22:06.620418 dry_scraper-0.1.8.6/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      688 2023-07-04 02:40:37.712254 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0     1044 2023-07-04 02:41:13.692518 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     6823 2023-07-04 02:46:41.274969 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    14453 2023-07-04 02:38:10.804523 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1874 2023-07-04 02:46:14.581433 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     2186 2023-07-04 02:50:05.229858 dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.6/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.6/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.6/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.5/LICENSE` & `dry_scraper-0.1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/README.md` & `dry_scraper-0.1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/pyproject.toml` & `dry_scraper-0.1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.5"
+version = "0.1.8.6"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,19 +775,21 @@
         )
         for home, team, opp in [
             (True, home_stats_pyd, away_stats_pyd),
             (False, away_stats_pyd, home_stats_pyd),
         ]:
             team_stats = team.team_stats.team_skater_stats
             opp_stats = opp.team_stats.team_skater_stats
+            start = self.content_pyd.game_data.date_time.date_time
+            end = (self.content_pyd.game_data.date_time.end_date_time,)
             team_dict = {
                 "season": int(self.season),
                 "gamePk": int(self.gamePk),
-                "start_date_time": self.content_pyd.game_data.date_time.date_time,
-                "end_date_time": self.content_pyd.game_data.date_time.end_date_time,
+                "start_date_time": datetime.min if start is None else start,
+                "end_date_time": datetime.min if end is None else end,
                 "team_id": int(team.team.id),
                 "team_name": str(team.team.name),
                 "opp_id": int(opp.team.id),
                 "opp_name": str(opp.team.name),
                 "team_home": home,
                 "team_goals": int(team_stats.goals),
                 "team_pim": int(team_stats.pim),
```

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/base_model.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/base_model.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8.6/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.6/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.6/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.5/PKG-INFO` & `dry_scraper-0.1.8.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.5
+Version: 0.1.8.6
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

