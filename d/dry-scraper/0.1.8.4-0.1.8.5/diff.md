# Comparing `tmp/dry_scraper-0.1.8.4.tar.gz` & `tmp/dry_scraper-0.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.4.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.5.tar", max compression
```

## Comparing `dry_scraper-0.1.8.4.tar` & `dry_scraper-0.1.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.4/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.4/README.md
--rw-r--r--   0        0        0      548 2023-07-04 02:11:13.768185 dry_scraper-0.1.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.4/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.4/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.4/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.4/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/base_model.py
--rw-r--r--   0        0        0      588 2023-07-04 02:07:35.382750 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      944 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5663 2023-07-04 02:07:35.359417 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    12661 2023-07-04 02:10:39.874531 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1664 2023-07-04 02:07:35.376084 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     2043 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1946 2023-07-04 02:07:35.372750 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.4/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.4/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.5/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.5/README.md
+-rw-r--r--   0        0        0      548 2023-07-04 02:50:20.109973 dry_scraper-0.1.8.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.5/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.5/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.5/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.5/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      688 2023-07-04 02:40:37.712254 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0     1044 2023-07-04 02:41:13.692518 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     6823 2023-07-04 02:46:41.274969 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    14453 2023-07-04 02:38:10.804523 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1874 2023-07-04 02:46:14.581433 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     2186 2023-07-04 02:50:05.229858 dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.5/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.5/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.5/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.4/LICENSE` & `dry_scraper-0.1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/README.md` & `dry_scraper-0.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/pyproject.toml` & `dry_scraper-0.1.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.4"
+version = "0.1.8.5"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8.5/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.5/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/base_model.py` & `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/base_model.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py` & `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from dry_scraper.nhl.pydantic_models.base_model import BaseModelNoException
 from pydantic import constr, Field
 
 ConferenceLink = constr(regex=r"^/api/v1/conferences/(\d+|null)$")
 
 
 class Conference(BaseModelNoException):
-    id: int
-    name: str
-    link: ConferenceLink
-    abbreviation: str
-    short_name: str = Field(alias="shortName")
-    active: bool
+    id: Optional[int]
+    name: Optional[str]
+    link: Optional[ConferenceLink]
+    abbreviation: Optional[str]
+    short_name: Optional[str] = Field(alias="shortName")
+    active: Optional[bool]
 
 
 class ShortConference(BaseModelNoException):
-    id: Optional[int]
-    name: Optional[str]
-    link: ConferenceLink
+    id: Optional[Optional[int]]
+    name: Optional[Optional[str]]
+    link: Optional[ConferenceLink]
 
 
 class Conferences(BaseModelNoException):
-    conferences: List[Conference]
+    conferences: Optional[List[Conference]]
```

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,33 +7,33 @@
     ShortConference,
 )
 
 DivisionLink = constr(regex=r"^/api/v1/divisions/(\d+|null)$")
 
 
 class ShortDivision(BaseModelNoException):
-    id: int
-    name: str
+    id: Optional[int]
+    name: Optional[str]
     name_short: Optional[str] = Field(alias="nameShort")
-    link: DivisionLink
+    link: Optional[DivisionLink]
     abbreviation: Optional[str]
 
 
 class Division(BaseModelNoException):
-    id: int
-    name: str
+    id: Optional[int]
+    name: Optional[str]
     name_short: Optional[str] = Field(alias="nameShort")
-    link: DivisionLink
+    link: Optional[DivisionLink]
     abbreviation: Optional[str]
-    conference: ShortConference
-    active: bool
+    conference: Optional[ShortConference]
+    active: Optional[bool]
 
 
 class NullDivision(BaseModelNoException):
-    link: Literal["/api/v1/divisions/null"]
+    link: Optional[Literal["/api/v1/divisions/null"]]
 
     class Config:
         extra = "forbid"
 
 
 class Divisions(BaseModelNoException):
-    divisions: List[NullDivision | Division]
+    divisions: Optional[List[NullDivision | Division]]
```

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.5/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.5/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.4/PKG-INFO` & `dry_scraper-0.1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.4
+Version: 0.1.8.5
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

