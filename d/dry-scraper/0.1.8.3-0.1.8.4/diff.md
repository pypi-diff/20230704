# Comparing `tmp/dry_scraper-0.1.8.3.tar.gz` & `tmp/dry_scraper-0.1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.3.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.4.tar", max compression
```

## Comparing `dry_scraper-0.1.8.3.tar` & `dry_scraper-0.1.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.3/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.3/README.md
--rw-r--r--   0        0        0      548 2023-07-04 02:06:04.355182 dry_scraper-0.1.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.3/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.3/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.3/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.3/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/base_model.py
--rw-r--r--   0        0        0      588 2023-07-04 02:07:35.382750 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      944 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5663 2023-07-04 02:07:35.359417 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    12199 2023-07-04 02:07:35.369417 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1664 2023-07-04 02:07:35.376084 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     2043 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1946 2023-07-04 02:07:35.372750 dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.3/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.3/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.4/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.4/README.md
+-rw-r--r--   0        0        0      548 2023-07-04 02:11:13.768185 dry_scraper-0.1.8.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.4/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.4/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.4/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    28322 2023-07-04 02:02:10.842767 dry_scraper-0.1.8.4/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2103 2023-07-04 02:01:03.308700 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      588 2023-07-04 02:07:35.382750 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      944 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5663 2023-07-04 02:07:35.359417 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    12661 2023-07-04 02:10:39.874531 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1664 2023-07-04 02:07:35.376084 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2043 2023-07-04 02:07:35.366083 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1946 2023-07-04 02:07:35.372750 dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.4/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.4/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.4/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.3/LICENSE` & `dry_scraper-0.1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/README.md` & `dry_scraper-0.1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/pyproject.toml` & `dry_scraper-0.1.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.3"
+version = "0.1.8.4"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/data_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/data_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/base_model.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/base_model.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,216 +16,216 @@
     ShortTeam,
     ShortVenue,
 )
 
 LiveFeedLink = constr(regex=r"^/api/v1/game/\d{10}/feed/live$")
 
 
-class Metadata(BaseModel):
+class Metadata(BaseModelNoException):
     wait: int
     timestamp: str = Field(alias="timeStamp")
 
 
-class Game(BaseModel):
+class Game(BaseModelNoException):
     pk: int
     season: str
     type: str
 
 
-class GameDateTime(BaseModel):
+class GameDateTime(BaseModelNoException):
     date_time: datetime = Field(alias="dateTime")
     end_date_time: Optional[datetime] = Field(alias="endDateTime")
 
 
-class Status(BaseModel):
+class Status(BaseModelNoException):
     abstract_game_state: str = Field(alias="abstractGameState")
     coded_game_state: str = Field(alias="codedGameState")
     detailed_state: str = Field(alias="detailedState")
     status_code: str = Field(alias="statusCode")
     start_time_tbd: bool = Field(alias="startTimeTBD")
 
 
-class Teams(BaseModel):
+class Teams(BaseModelNoException):
     away: Team
     home: Team
 
 
-class GameData(BaseModel):
+class GameData(BaseModelNoException):
     game: Game
     date_time: GameDateTime = Field(alias="datetime")
     status: Status
     teams: Teams
     players: Dict[PersonIdString, Player]
     venue: ShortVenue
 
 
-class PlaysByPeriod(BaseModel):
+class PlaysByPeriod(BaseModelNoException):
     start_index: int = Field(alias="startIndex")
     plays: List[int]
     end_index: int = Field(alias="endIndex")
 
 
-class Strength(BaseModel):
+class Strength(BaseModelNoException):
     code: str
     name: str
 
 
-class Result(BaseModel):
+class Result(BaseModelNoException):
     event: str
     event_code: str = Field(alias="eventCode")
     event_type_id: str = Field(alias="eventTypeId")
     description: str
     secondary_type: Optional[str] = Field(alias="secondaryType")
     strength: Optional[Strength]
     game_winning_goal: Optional[bool] = Field(alias="gameWinningGoal")
     empty_net: Optional[bool] = Field(alias="emptyNet")
 
 
-class Goals(BaseModel):
+class Goals(BaseModelNoException):
     away: int
     home: int
 
 
-class About(BaseModel):
+class About(BaseModelNoException):
     event_idx: int = Field(alias="eventIdx")
     event_id: int = Field(alias="eventId")
     period: int
     period_type: str = Field(alias="periodType")
     ordinal_num: str = Field(alias="ordinalNum")
     period_time: str = Field(alias="periodTime")
     period_time_remaining: str = Field(alias="periodTimeRemaining")
     date_time: datetime = Field(alias="dateTime")
     goals: Goals
 
 
-class Coordinates(BaseModel):
+class Coordinates(BaseModelNoException):
     x: Optional[int]
     y: Optional[int]
 
 
-class PlayPlayer(BaseModel):
+class PlayPlayer(BaseModelNoException):
     player: Person
     player_type: str = Field(alias="playerType")
     season_total: Optional[str] = Field(alias="seasonTotal")
 
 
-class Play(BaseModel):
+class Play(BaseModelNoException):
     result: Result
     about: About
     coordinates: Coordinates
     players: Optional[List[PlayPlayer]]
     team: Optional[ShortTeam]
 
 
-class Plays(BaseModel):
+class Plays(BaseModelNoException):
     all_plays: List[Play] = Field(alias="allPlays")
     scoring_plays: List[int] = Field(alias="scoringPlays")
     penalty_plays: List[int] = Field(alias="penaltyPlays")
     plays_by_period: List[PlaysByPeriod] = Field(alias="playsByPeriod")
     current_play: Play = Field(alias="currentPlay")
 
 
-class TeamPeriodLineScore(BaseModel):
+class TeamPeriodLineScore(BaseModelNoException):
     goals: int
     shots_on_goal: int = Field(alias="shotsOnGoal")
     rink_side: Optional[str] = Field(alias="rinkSide")
 
 
-class Period(BaseModel):
+class Period(BaseModelNoException):
     period_type: str = Field(alias="periodType")
     start_time: datetime = Field(alias="startTime")
     end_time: Optional[datetime] = Field(alias="endTime")
     num: int
     ordinal_num: str = Field(alias="ordinalNum")
     home: TeamPeriodLineScore
     away: TeamPeriodLineScore
 
 
-class TeamShootoutInfo(BaseModel):
+class TeamShootoutInfo(BaseModelNoException):
     scores: int
     attempts: int
 
 
-class ShootoutInfo(BaseModel):
+class ShootoutInfo(BaseModelNoException):
     away: TeamShootoutInfo
     home: TeamShootoutInfo
     start_time: Optional[datetime] = Field(alias="startTime")
 
 
-class TeamLineScore(BaseModel):
+class TeamLineScore(BaseModelNoException):
     team: ShortTeam
     goals: int
     shots_on_goal: int = Field(alias="shotsOnGoal")
     goalie_pulled: bool = Field(alias="goaliePulled")
     num_skaters: int = Field(alias="numSkaters")
     power_play: bool = Field(alias="powerPlay")
 
 
-class TeamsLineScore(BaseModel):
+class TeamsLineScore(BaseModelNoException):
     away: TeamLineScore
     home: TeamLineScore
 
 
-class IntermissionInfo(BaseModel):
+class IntermissionInfo(BaseModelNoException):
     intermission_time_remaining: int = Field(alias="intermissionTimeRemaining")
     intermission_time_elapsed: int = Field(alias="intermissionTimeElapsed")
     in_intermission: bool = Field(alias="inIntermission")
 
 
-class PowerPlayInfo(BaseModel):
+class PowerPlayInfo(BaseModelNoException):
     situation_time_remaining: int = Field(alias="situationTimeRemaining")
     situation_time_elapsed: int = Field(alias="situationTimeElapsed")
     in_situation: bool = Field(alias="inSituation")
 
 
-class LineScore(BaseModel):
+class LineScore(BaseModelNoException):
     current_period: str = Field(alias="currentPeriod")
     current_period_ordinal: str = Field(alias="currentPeriodOrdinal")
     current_period_time_remaining: str = Field(alias="currentPeriodTimeRemaining")
     periods: List[Period]
     shootout_info: ShootoutInfo = Field(alias="shootoutInfo")
     teams: TeamsLineScore
     power_play_strength: str = Field(alias="powerPlayStrength")
     has_shootout: bool = Field(alias="hasShootout")
     intermission_info: IntermissionInfo = Field(alias="intermissionInfo")
     power_play_info: PowerPlayInfo = Field(alias="powerPlayInfo")
 
 
-class Official(BaseModel):
+class Official(BaseModelNoException):
     official: Person
     official_type: str = Field(alias="officialType")
 
 
-class TeamSkaterStats(BaseModel):
+class TeamSkaterStats(BaseModelNoException):
     goals: int
     pim: int
     shots: int
     power_play_percentage: float = Field(alias="powerPlayPercentage")
     power_play_goals: int = Field(alias="powerPlayGoals")
     power_play_opportunities: int = Field(alias="powerPlayOpportunities")
     face_off_win_percentage: float = Field(alias="faceOffWinPercentage")
     blocked: int
     takeaways: int
     giveaways: int
     hits: int
 
 
-class TeamStats(BaseModel):
+class TeamStats(BaseModelNoException):
     team_skater_stats: TeamSkaterStats = Field(alias="teamSkaterStats")
 
 
-class PlayerStatsPerson(BaseModel):
+class PlayerStatsPerson(BaseModelNoException):
     id: PersonIdString
     full_name: str = Field(alias="fullName")
     link: constr(regex=r"^/api/v1/people/\d+$")
     shoots_catches: Optional[str] = Field(alias="shootsCatches")
     roster_status: str = Field(alias="rosterStatus")
 
 
-class GoalieStats(BaseModel):
+class GoalieStats(BaseModelNoException):
     time_on_ice: str = Field(alias="timeOnIce")
     assists: int
     goals: int
     pim: int
     shots: int
     saves: int
     power_play_saves: int = Field(alias="powerPlaySaves")
@@ -236,15 +236,15 @@
     power_play_shots_against: int = Field(alias="powerPlayShotsAgainst")
     decision: str
     save_percentage: float = Field(alias="savePercentage")
     power_play_save_percentage: float = Field(alias="powerPlaySavePercentage")
     even_strength_save_percentage: float = Field(alias="evenStrengthSavePercentage")
 
 
-class SkaterStats(BaseModel):
+class SkaterStats(BaseModelNoException):
     time_on_ice: str = Field(alias="timeOnIce")
     assists: int
     goals: int
     shots: int
     hits: int
     power_play_goals: int = Field(alias="powerPlayGoals")
     power_play_assists: int = Field(alias="powerPlayAssists")
@@ -258,87 +258,87 @@
     blocked_shots: int = Field(alias="blocked")
     plus_minus: int = Field(alias="plusMinus")
     even_time_on_ice: str = Field(alias="evenTimeOnIce")
     power_play_time_on_ice: str = Field(alias="powerPlayTimeOnIce")
     shorthanded_time_on_ice: str = Field(alias="shortHandedTimeOnIce")
 
 
-class PlayerStats(BaseModel):
+class PlayerStats(BaseModelNoException):
     skater_stats: Optional[SkaterStats] = Field(alias="skaterStats")
     goalie_stats: Optional[GoalieStats] = Field(alias="goalieStats")
 
 
-class PlayerStatsEntry(BaseModel):
+class PlayerStatsEntry(BaseModelNoException):
     person: PlayerStatsPerson
     jersey_number: Optional[int] = Field(alias="jerseyNumber")
     position: Position
     stats: Union[PlayerStats, None, Dict]
 
 
-class ShortPerson(BaseModel):
+class ShortPerson(BaseModelNoException):
     full_name: str = Field(alias="fullName")
     link: PersonLink
 
 
-class Coach(BaseModel):
+class Coach(BaseModelNoException):
     person: Person
     position: Position
 
 
-class OnIcePlusPlayer(BaseModel):
+class OnIcePlusPlayer(BaseModelNoException):
     player_id: PersonIdString = Field(alias="playerId")
     shift_duration: int = Field(alias="shiftDuration")
     stamina: int
 
 
-class PenaltyBox(BaseModel):
+class PenaltyBox(BaseModelNoException):
     id: PersonIdString
     time_remaining: str = Field(alias="timeRemaining")
     active: bool
 
 
-class TeamBoxScore(BaseModel):
+class TeamBoxScore(BaseModelNoException):
     team: ShortTeam
     team_stats: TeamStats = Field(alias="teamStats")
     players: Dict[PersonIdString, PlayerStatsEntry]
     goalies: List[PersonIdString]
     skaters: List[PersonIdString]
     on_ice: List[PersonIdString] = Field(alias="onIce")
     on_ice_plus: List[OnIcePlusPlayer] = Field(alias="onIcePlus")
     scratches: List[PersonIdString]
     penalty_box: List[PenaltyBox] = Field(alias="penaltyBox")
     coaches: List[Coach]
 
 
-class TeamsBoxScore(BaseModel):
+class TeamsBoxScore(BaseModelNoException):
     away: TeamBoxScore
     home: TeamBoxScore
 
 
-class BoxScore(BaseModel):
+class BoxScore(BaseModelNoException):
     teams: TeamsBoxScore
     officials: List[Official]
 
 
-class Decisions(BaseModel):
+class Decisions(BaseModelNoException):
     winner: Optional[Person]
     loser: Optional[Person]
     first_star: Optional[Person] = Field(alias="firstStar")
     second_star: Optional[Person] = Field(alias="secondStar")
     third_star: Optional[Person] = Field(alias="thirdStar")
 
 
-class LiveData(BaseModel):
+class LiveData(BaseModelNoException):
     plays: Plays
     line_score: LineScore = Field(alias="linescore")
     box_score: BoxScore = Field(alias="boxscore")
     decisions: Decisions
 
 
-class LiveFeed(BaseModel):
+class LiveFeed(BaseModelNoException):
     game_pk: int = Field(alias="gamePk")
     link: LiveFeedLink
     metadata: Metadata = Field(alias="metaData")
     game_data: GameData = Field(alias="gameData")
     live_data: LiveData = Field(alias="liveData")
```

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8.4/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.4/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.4/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.3/PKG-INFO` & `dry_scraper-0.1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.3
+Version: 0.1.8.4
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

