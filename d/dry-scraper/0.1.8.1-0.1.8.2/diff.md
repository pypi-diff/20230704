# Comparing `tmp/dry_scraper-0.1.8.1.tar.gz` & `tmp/dry_scraper-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.1.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.2.tar", max compression
```

## Comparing `dry_scraper-0.1.8.1.tar` & `dry_scraper-0.1.8.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.1/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.1/README.md
--rw-r--r--   0        0        0      548 2023-07-04 01:36:31.905667 dry_scraper-0.1.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.1/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.1/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.1/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    28322 2023-07-04 01:45:24.301174 dry_scraper-0.1.8.1/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    12134 2023-07-04 01:13:48.210528 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.1/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.1/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.2/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.2/README.md
+-rw-r--r--   0        0        0      548 2023-07-04 02:02:53.579888 dry_scraper-0.1.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.2/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.2/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.2/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.2/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      556 2023-07-04 02:01:14.178820 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      912 2023-07-04 02:01:03.298700 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5631 2023-07-04 02:01:03.305367 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    12167 2023-07-04 02:01:03.312034 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1632 2023-07-04 02:01:58.519301 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2011 2023-07-04 02:01:58.515968 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1914 2023-07-04 02:01:58.522635 dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.2/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.2/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.2/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.1/LICENSE` & `dry_scraper-0.1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/README.md` & `dry_scraper-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/pyproject.toml` & `dry_scraper-0.1.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.1"
+version = "0.1.8.2"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from typing import List, Optional, Literal
 
-from pydantic import BaseModel, Field, constr
+from base_model import BaseModelNoException
+from pydantic import Field, constr
 
 from dry_scraper.nhl.pydantic_models.nhl_conferences_api_source import (
     ShortConference,
 )
 
 DivisionLink = constr(regex=r"^/api/v1/divisions/(\d+|null)$")
 
 
-class ShortDivision(BaseModel):
+class ShortDivision(BaseModelNoException):
     id: int
     name: str
     name_short: Optional[str] = Field(alias="nameShort")
     link: DivisionLink
     abbreviation: Optional[str]
 
 
-class Division(BaseModel):
+class Division(BaseModelNoException):
     id: int
     name: str
     name_short: Optional[str] = Field(alias="nameShort")
     link: DivisionLink
     abbreviation: Optional[str]
     conference: ShortConference
     active: bool
 
 
-class NullDivision(BaseModel):
+class NullDivision(BaseModelNoException):
     link: Literal["/api/v1/divisions/null"]
 
     class Config:
         extra = "forbid"
 
 
-class Divisions(BaseModel):
+class Divisions(BaseModelNoException):
     divisions: List[NullDivision | Division]
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 from datetime import datetime
 from typing import List, Dict, Optional, Annotated, Literal
 from uuid import UUID
-from pydantic import BaseModel, constr, Field, HttpUrl
+from base_model import BaseModelNoException
+from pydantic import constr, Field, HttpUrl
 
 GameContentLink = constr(regex=r"^/api/v1/game/\d{10}/content$")
 ResolutionString = constr(regex=r"^\d{2,4}x\d{2,4}$")
 
 
-class Empty(BaseModel):
+class Empty(BaseModelNoException):
     ...
 
     class Config:
         extra = "forbid"
 
 
-class ContributorEntry(BaseModel):
+class ContributorEntry(BaseModelNoException):
     name: str
     twitter: str
 
 
-class Contributor(BaseModel):
+class Contributor(BaseModelNoException):
     contributors: List[ContributorEntry]
     source: str
 
 
-class ImageCut(BaseModel):
+class ImageCut(BaseModelNoException):
     aspect_ratio: str = Field(alias="aspectRatio")
     width: int
     height: int
     src: HttpUrl
     at2x: HttpUrl
     at3x: HttpUrl
 
 
-class Image(BaseModel):
+class Image(BaseModelNoException):
     title: str
     alt_text: str = Field(alias="altText")
     cuts: Dict[ResolutionString, ImageCut]
 
 
-class Playback(BaseModel):
+class Playback(BaseModelNoException):
     name: str
     width: Optional[int | str]
     height: Optional[int | str]
     url: HttpUrl | str
 
 
-class Keyword(BaseModel):
+class Keyword(BaseModelNoException):
     type: str
     value: str
     display_name: str = Field(alias="displayName")
 
 
-class PhotoMediaItem(BaseModel):
+class PhotoMediaItem(BaseModelNoException):
     type: str
     image: Image
 
 
-class MediaItem(BaseModel):
+class MediaItem(BaseModelNoException):
     type: str
     id: int
     date: datetime
     title: str
     blurb: str
     description: str
     duration: str
@@ -69,15 +70,15 @@
     media_playback_id: int = Field(alias="mediaPlaybackId")
     media_state: str = Field(alias="mediaState")
     keywords: List[Keyword]
     image: Image
     playbacks: List[Playback]
 
 
-class EditorialItem(BaseModel):
+class EditorialItem(BaseModelNoException):
     type: str
     state: str
     date: datetime
     id: str
     headline: str
     subhead: str
     seo_title: str = Field(alias="seoTitle")
@@ -92,70 +93,70 @@
     approval: str
     url: str
     data_URI: str = Field(alias="dataURI")
     media: MediaItem | PhotoMediaItem | Empty
     preview: str
 
 
-class NhlTvItem(BaseModel):
+class NhlTvItem(BaseModelNoException):
     guid: UUID
     media_state: str = Field(alias="mediaState")
     media_playback_id: int = Field(alias="mediaPlaybackId")
     media_feed_type: str = Field(alias="mediaFeedType")
     call_letters: str = Field(alias="callLetters")
     event_id: str = Field(alias="eventId")
     language: str
     free_game: bool = Field(alias="freeGame")
     feed_name: str = Field(alias="feedName")
     game_plus: bool = Field(alias="gamePlus")
 
 
-class AudioItem(BaseModel):
+class AudioItem(BaseModelNoException):
     media_state: str = Field(alias="mediaState")
     media_playback_id: int = Field(alias="mediaPlaybackId")
     media_feed_type: str = Field(alias="mediaFeedType")
     call_letters: str = Field(alias="callLetters")
     event_id: str = Field(alias="eventId")
     language: str
     free_game: bool = Field(alias="freeGame")
     feed_name: str = Field(alias="feedName")
     game_plus: bool = Field(alias="gamePlus")
 
 
-class EditorialCategory(BaseModel):
+class EditorialCategory(BaseModelNoException):
     title: str
     topic_list: str = Field(alias="topicList")
     items: List[EditorialItem]
 
 
-class NhlTvEntry(BaseModel):
+class NhlTvEntry(BaseModelNoException):
     title: Literal["NHLTV"]
     platform: str
     items: List[NhlTvItem]
 
 
-class AudioEpgEntry(BaseModel):
+class AudioEpgEntry(BaseModelNoException):
     title: Literal["Audio"]
     topic_list: Optional[int | str] = Field(alias="topicList")
     items: List[AudioItem]
 
 
-class ExtendedHighlightsEpgEntry(BaseModel):
+class ExtendedHighlightsEpgEntry(BaseModelNoException):
     title: Literal["Extended Highlights"]
     topic_list: Optional[int | str] = Field(alias="topicList")
     items: List[MediaItem]
 
 
-class RecapEpgEntry(BaseModel):
+class RecapEpgEntry(BaseModelNoException):
     title: Literal["Recap"]
     topic_list: Optional[int | str] = Field(alias="topicList")
     items: List[MediaItem]
 
 
-class PowerPlayEpgEntry(BaseModel):
+class PowerPlayEpgEntry(BaseModelNoException):
     title: Literal["Power Play"]
     topic_list: Optional[int | str] = Field(alias="topicList")
     items: List[MediaItem]
 
 
 EpgEntry = Annotated[
     NhlTvEntry
@@ -163,21 +164,21 @@
     | ExtendedHighlightsEpgEntry
     | RecapEpgEntry
     | PowerPlayEpgEntry,
     Field(discriminator="title"),
 ]
 
 
-class Editorial(BaseModel):
+class Editorial(BaseModelNoException):
     preview: EditorialCategory
     articles: EditorialCategory
     recap: EditorialCategory
 
 
-class Milestone(BaseModel):
+class Milestone(BaseModelNoException):
     title: str
     description: str
     type: str
     type: str
     time_absolute: datetime = Field(alias="timeAbsolute")
     time_offset: datetime = Field(alias="timeOffset")
     period: int | str
@@ -185,34 +186,34 @@
     team_id: int | str = Field(alias="teamId")
     player_id: int | str = Field(alias="playerId")
     period_time: str = Field(alias="periodTime")
     ordinal_num: str = Field(alias="ordinalNum")
     highlight: MediaItem | Empty
 
 
-class Milestones(BaseModel):
+class Milestones(BaseModelNoException):
     title: Literal["Milestones"]
     steam_start: datetime = Field(alias="streamStart")
     items: List[Milestone]
 
 
-class Media(BaseModel):
+class Media(BaseModelNoException):
     epg: List[EpgEntry]
     milestones: Milestones | Empty
 
 
-class HighlightEntries(BaseModel):
+class HighlightEntries(BaseModelNoException):
     title: str
     topic_list: str = Field(alias="topicList")
     items: List[MediaItem]
 
 
-class Highlights(BaseModel):
+class Highlights(BaseModelNoException):
     scoreboard: HighlightEntries
     gamecenter: HighlightEntries = Field(alias="gameCenter")
 
 
-class GameContent(BaseModel):
+class GameContent(BaseModelNoException):
     link: GameContentLink
     editorial: Editorial
     media: Media
     highlights: Highlights
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
-from pydantic import BaseModel, Field, constr
+from base_model import BaseModelNoException
+from pydantic import Field, constr
 from typing import List, Dict, Optional, Union
 
 
 from dry_scraper.nhl.pydantic_models.nhl_people_api_source import (
     PersonIdString,
     PersonLink,
     Position,
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from datetime import date
 from typing import List, Optional
 
-from pydantic import BaseModel, constr, Field
+from base_model import BaseModelNoException
+from pydantic import constr, Field
 
 from dry_scraper.nhl.pydantic_models.nhl_teams_api_source import ShortTeam
 
 PersonIdString = constr(regex=r"^(ID)?\d{4,7}$")
 
 
 PersonLink = constr(regex=r"^/api/v1/people/(\d+|null)$")
 
 
-class Position(BaseModel):
+class Position(BaseModelNoException):
     code: str
     name: str
     type: str
     abbreviation: str
 
 
-class Player(BaseModel):
+class Player(BaseModelNoException):
     id: int
     full_name: str = Field(alias="fullName")
     link: PersonLink
     first_name: str = Field(alias="firstName")
     last_name: str = Field(alias="lastName")
     primary_number: Optional[int] = Field(alias="primaryNumber")
     birth_date: date = Field(alias="birthDate")
@@ -39,15 +40,15 @@
     rookie: bool
     shoots_catches: Optional[str] = Field(alias="shootsCatches")
     roster_status: str = Field(alias="rosterStatus")
     current_team: Optional[ShortTeam] = Field(alias="currentTeam")
     primary_position: Position = Field(alias="primaryPosition")
 
 
-class Person(BaseModel):
+class Person(BaseModelNoException):
     id: Optional[PersonIdString]
     full_name: str = Field(alias="fullName")
     link: PersonLink
 
 
-class People(BaseModel):
+class People(BaseModelNoException):
     people: List[Player]
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import datetime
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+from base_model import BaseModelNoException
+from pydantic import Field
 
 from dry_scraper.nhl.pydantic_models.nhl_game_live_feed_api_source import (
     LiveFeedLink,
     Status,
 )
 from dry_scraper.nhl.pydantic_models.nhl_teams_api_source import (
     ShortTeam,
     ShortVenue,
 )
 
 
-class LeagueRecord(BaseModel):
+class LeagueRecord(BaseModelNoException):
     wins: int
     losses: int
     ot: Optional[int]
     type: str
 
 
-class Team(BaseModel):
+class Team(BaseModelNoException):
     league_record: LeagueRecord = Field(alias="leagueRecord")
     score: int
     team: ShortTeam
 
 
-class Teams(BaseModel):
+class Teams(BaseModelNoException):
     away: Team
     home: Team
 
 
-class Game(BaseModel):
+class Game(BaseModelNoException):
     gamePk: int
     link: LiveFeedLink
     game_type: str = Field(alias="gameType")
     season: str = Field(alias="season")
     game_date: datetime.datetime = Field(alias="gameDate")
     status: Status
     teams: Teams
     venue: ShortVenue
 
 
-class Date(BaseModel):
+class Date(BaseModelNoException):
     date: datetime.date
     total_items: int = Field(alias="totalItems")
     total_games: int = Field(alias="totalGames")
     games: List[Game]
 
 
-class Schedule(BaseModel):
+class Schedule(BaseModelNoException):
     total_items: int = Field(alias="totalItems")
     total_games: int = Field(alias="totalGames")
     dates: List[Date]
 
 
 schedule_df_model = {
     "date": "str",
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8.2/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, List
 
-from pydantic import BaseModel, constr, Field, HttpUrl
+from base_model import BaseModelNoException
+from pydantic import constr, Field, HttpUrl
 
 from dry_scraper.nhl.pydantic_models.nhl_conferences_api_source import (
     ShortConference,
 )
 from dry_scraper.nhl.pydantic_models.nhl_divisions_api_source import (
     NullDivision,
     ShortDivision,
@@ -12,49 +13,49 @@
 
 VenueLink = constr(regex=r"^/api/v1/venues/(\d+|null)$")
 
 FranchiseLink = constr(regex=r"^/api/v1/franchises/(\d+|null)$")
 TeamLink = constr(regex=r"^/api/v1/teams/(\d+|null)$")
 
 
-class ShortTeam(BaseModel):
+class ShortTeam(BaseModelNoException):
     id: int
     name: str
     link: TeamLink
     abbreviation: Optional[str]
     tricode: Optional[str] = Field(alias="triCode")
 
 
-class TimeZone(BaseModel):
+class TimeZone(BaseModelNoException):
     id: str
     offset: int
     tz: str
 
 
-class Venue(BaseModel):
+class Venue(BaseModelNoException):
     id: Optional[int]
     name: Optional[str]
     link: VenueLink
     city: Optional[str]
     time_zone: TimeZone = Field(alias="timeZone")
 
 
-class ShortVenue(BaseModel):
+class ShortVenue(BaseModelNoException):
     id: Optional[int]
     name: str
     link: VenueLink
 
 
-class Franchise(BaseModel):
+class Franchise(BaseModelNoException):
     franchise_id: int = Field(alias="franchiseId")
     team_name: str = Field(alias="teamName")
     link: FranchiseLink
 
 
-class Team(BaseModel):
+class Team(BaseModelNoException):
     id: int
     name: str
     link: Optional[TeamLink]
     venue: Optional[Venue]
     abbreviation: Optional[str]
     tricode: Optional[str] = Field(alias="triCode")
     team_name: str = Field(alias="teamName")
@@ -65,9 +66,9 @@
     franchise: Franchise
     short_name: str = Field(alias="shortName")
     official_site_url: Optional[HttpUrl] = Field(alias="officialSiteUrl")
     franchise_id: int = Field(alias="franchiseId")
     active: bool
 
 
-class Teams(BaseModel):
+class Teams(BaseModelNoException):
     teams: List[Team]
```

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.2/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.2/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.1/PKG-INFO` & `dry_scraper-0.1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

