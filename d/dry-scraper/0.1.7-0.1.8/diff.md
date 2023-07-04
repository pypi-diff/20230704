# Comparing `tmp/dry_scraper-0.1.7.tar.gz` & `tmp/dry_scraper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.7.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.tar", max compression
```

## Comparing `dry_scraper-0.1.7.tar` & `dry_scraper-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.7/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.7/README.md
--rw-r--r--   0        0        0      546 2023-07-04 01:14:24.237391 dry_scraper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.7/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2444 2023-06-30 23:14:23.236239 dry_scraper-0.1.7/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.7/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    28334 2023-07-03 23:43:45.569901 dry_scraper-0.1.7/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    12134 2023-07-04 01:13:48.210528 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.7/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.7/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 dry_scraper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8/README.md
+-rw-r--r--   0        0        0      546 2023-07-04 01:35:37.475311 dry_scraper-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2444 2023-07-04 01:35:14.738495 dry_scraper-0.1.8/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28334 2023-07-03 23:43:45.569901 dry_scraper-0.1.8/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    12134 2023-07-04 01:13:48.210528 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 dry_scraper-0.1.8/PKG-INFO
```

### Comparing `dry_scraper-0.1.7/LICENSE` & `dry_scraper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/README.md` & `dry_scraper-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/pyproject.toml` & `dry_scraper-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.7"
+version = "0.1.8"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.7/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8/src/dry_scraper/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return self._extension
 
     def fetch_content(self) -> Self:
         """
         Use requests.get to retrieve file at self.url and store response in self.content
         """
         try:
-            response = requests.get(self.url, timeout=10)
+            response = requests.get(self.url, timeout=60)
             response.raise_for_status()
             self.content = response.text
         except requests.exceptions.HTTPError as errh:
             print(errh)
         except requests.exceptions.ConnectionError as errc:
             print(errc)
         except requests.exceptions.Timeout as errt:
```

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/shared.py` & `dry_scraper-0.1.8/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/src/dry_scraper/teams.py` & `dry_scraper-0.1.8/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.7/PKG-INFO` & `dry_scraper-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

