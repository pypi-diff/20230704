# Comparing `tmp/fl-api-requester-1.0.2.tar.gz` & `tmp/fl-api-requester-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl-api-requester-1.0.2.tar", last modified: Mon Jun 26 17:13:01 2023, max compression
+gzip compressed data, was "fl-api-requester-1.0.3.tar", last modified: Mon Jul  3 21:59:07 2023, max compression
```

## Comparing `fl-api-requester-1.0.2.tar` & `fl-api-requester-1.0.3.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.692184 fl-api-requester-1.0.2/
--rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-06-26 17:13:01.691183 fl-api-requester-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-06-26 17:09:29.000000 fl-api-requester-1.0.2/README.md
--rw-rw-rw-   0        0        0      597 2023-06-26 17:12:29.000000 fl-api-requester-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 17:13:01.692184 fl-api-requester-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.578059 fl-api-requester-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.630061 fl-api-requester-1.0.2/src/fl_api_requester/
--rw-rw-rw-   0        0        0     2237 2023-06-26 16:51:37.000000 fl-api-requester-1.0.2/src/fl_api_requester/FLAPIConnectionData.py
--rw-rw-rw-   0        0        0     7921 2023-06-26 17:05:48.000000 fl-api-requester-1.0.2/src/fl_api_requester/FLAPIRequester.py
--rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.2/src/fl_api_requester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.658191 fl-api-requester-1.0.2/src/fl_api_requester/dto/
--rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/DTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.582059 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.661188 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/
--rw-rw-rw-   0        0        0      164 2023-06-26 16:25:59.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
--rw-rw-rw-   0        0        0      170 2023-06-26 16:26:03.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.664186 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/authentication/
--rw-rw-rw-   0        0        0      188 2023-06-26 16:26:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.669192 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/
--rw-rw-rw-   0        0        0      246 2023-06-26 16:26:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
--rw-rw-rw-   0        0        0      214 2023-06-26 16:26:47.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
--rw-rw-rw-   0        0        0      204 2023-06-26 16:26:57.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.672188 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/
--rw-rw-rw-   0        0        0      210 2023-06-26 16:27:19.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
--rw-rw-rw-   0        0        0      196 2023-06-26 16:27:28.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
--rw-rw-rw-   0        0        0      226 2023-06-26 16:27:44.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.676184 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/
--rw-rw-rw-   0        0        0      161 2023-06-26 16:30:05.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
--rw-rw-rw-   0        0        0      173 2023-06-26 16:30:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
--rw-rw-rw-   0        0        0      196 2023-06-26 16:30:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
--rw-rw-rw-   0        0        0      244 2023-06-26 16:30:38.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.680195 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/
--rw-rw-rw-   0        0        0      161 2023-06-26 16:31:11.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/StartWarDTO.py
--rw-rw-rw-   0        0        0      159 2023-06-26 16:30:56.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/StopWarDTO.py
--rw-rw-rw-   0        0        0      252 2023-06-26 16:31:09.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.592064 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.683222 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/
--rw-rw-rw-   0        0        0      341 2023-06-26 16:10:18.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
--rw-rw-rw-   0        0        0      161 2023-06-26 16:11:22.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.684207 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/authentication/
--rw-rw-rw-   0        0        0      255 2023-06-26 16:08:21.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.685222 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/discord/
--rw-rw-rw-   0        0        0      285 2023-06-26 16:31:38.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/discord/DiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.687183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/
--rw-rw-rw-   0        0        0      225 2023-06-26 16:11:39.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/PlanetDTO.py
--rw-rw-rw-   0        0        0      250 2023-06-26 16:31:50.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.688183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/player/
--rw-rw-rw-   0        0        0      398 2023-06-26 16:24:19.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/player/PlayerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.690183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/
--rw-rw-rw-   0        0        0      493 2023-06-26 16:45:51.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
--rw-rw-rw-   0        0        0      332 2023-06-26 16:11:00.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/WarDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.690183 fl-api-requester-1.0.2/src/fl_api_requester/exception/
--rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/exception/APIErrorException.py
-drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.657183 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.883219 fl-api-requester-1.0.3/
+-rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1313 2023-07-03 21:59:07.883219 fl-api-requester-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-03 21:57:13.000000 fl-api-requester-1.0.3/README.md
+-rw-rw-rw-   0        0        0      597 2023-07-03 21:58:38.000000 fl-api-requester-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 21:59:07.883219 fl-api-requester-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.785222 fl-api-requester-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.821219 fl-api-requester-1.0.3/src/fl_api_requester/
+-rw-rw-rw-   0        0        0     2237 2023-06-26 16:51:37.000000 fl-api-requester-1.0.3/src/fl_api_requester/FLAPIConnectionData.py
+-rw-rw-rw-   0        0        0     8488 2023-07-03 21:35:34.000000 fl-api-requester-1.0.3/src/fl_api_requester/FLAPIRequester.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.3/src/fl_api_requester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.844212 fl-api-requester-1.0.3/src/fl_api_requester/dto/
+-rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/DTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.803225 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.847214 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/alliance/
+-rw-rw-rw-   0        0        0      164 2023-06-26 16:25:59.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
+-rw-rw-rw-   0        0        0      170 2023-06-26 16:26:03.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.848219 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/authentication/
+-rw-rw-rw-   0        0        0      188 2023-06-26 16:26:13.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.854212 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/
+-rw-rw-rw-   0        0        0      246 2023-06-26 16:26:26.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
+-rw-rw-rw-   0        0        0      358 2023-07-03 19:59:49.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/AddChannelsToDiscordDTO.py
+-rw-rw-rw-   0        0        0      339 2023-07-03 19:59:59.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
+-rw-rw-rw-   0        0        0      258 2023-07-03 19:58:33.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/RemoveChannelsFromDiscordDTO.py
+-rw-rw-rw-   0        0        0      204 2023-06-26 16:26:57.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.855212 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord_channel/
+-rw-rw-rw-   0        0        0      213 2023-07-03 19:59:46.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/discord_channel/DiscordChannelRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.860216 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/planet/
+-rw-rw-rw-   0        0        0      210 2023-06-26 16:27:19.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:27:28.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
+-rw-rw-rw-   0        0        0      226 2023-06-26 16:27:44.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.865221 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/player/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:30:05.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
+-rw-rw-rw-   0        0        0      173 2023-06-26 16:30:13.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:30:26.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
+-rw-rw-rw-   0        0        0      244 2023-06-26 16:30:38.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.869226 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/war/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:31:11.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/war/StartWarDTO.py
+-rw-rw-rw-   0        0        0      159 2023-06-26 16:30:56.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/war/StopWarDTO.py
+-rw-rw-rw-   0        0        0      252 2023-06-26 16:31:09.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.808213 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.871223 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/alliance/
+-rw-rw-rw-   0        0        0      341 2023-06-26 16:10:18.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:11:22.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.872212 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/authentication/
+-rw-rw-rw-   0        0        0      255 2023-06-26 16:08:21.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.873214 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/discord/
+-rw-rw-rw-   0        0        0      422 2023-07-03 20:01:47.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/discord/DiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.874214 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/discord_channel/
+-rw-rw-rw-   0        0        0      192 2023-07-03 20:01:18.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/discord_channel/DiscordChannelResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.876290 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/planet/
+-rw-rw-rw-   0        0        0      225 2023-06-26 16:11:39.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/planet/PlanetDTO.py
+-rw-rw-rw-   0        0        0      250 2023-06-26 16:31:50.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.878212 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/player/
+-rw-rw-rw-   0        0        0      398 2023-06-26 16:24:19.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/player/PlayerDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.880219 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/war/
+-rw-rw-rw-   0        0        0      494 2023-07-03 19:43:57.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
+-rw-rw-rw-   0        0        0      499 2023-07-03 19:43:20.000000 fl-api-requester-1.0.3/src/fl_api_requester/dto/response/war/WarDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.881212 fl-api-requester-1.0.3/src/fl_api_requester/exception/
+-rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.3/src/fl_api_requester/exception/APIErrorException.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:59:07.843212 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/
+-rw-rw-rw-   0        0        0     1313 2023-07-03 21:59:07.000000 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2253 2023-07-03 21:59:07.000000 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 21:59:07.000000 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 21:59:07.000000 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 21:59:07.000000 fl-api-requester-1.0.3/src/fl_api_requester.egg-info/top_level.txt
```

### Comparing `fl-api-requester-1.0.2/LICENSE` & `fl-api-requester-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.2/PKG-INFO` & `fl-api-requester-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.2
+Version: 1.0.3
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -43,7 +43,8 @@
     # Get a War attack
     attack = api_requester.get_player_attacks("Galactifer")
 
     print(f"Galactifer attacked on {attack[0].timestamp_to_datetime():%d/%m/%Y at %H:%M:%S}")
 except APIErrorException as e:
     print(e.api_error)
 ```
+
```

### Comparing `fl-api-requester-1.0.2/pyproject.toml` & `fl-api-requester-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fl-api-requester"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name="FL-GL", email="franceleadergl@gmail.com" }
 ]
 description = "The France Leader API requester."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fl-api-requester-1.0.2/src/fl_api_requester/FLAPIConnectionData.py` & `fl-api-requester-1.0.3/src/fl_api_requester/FLAPIConnectionData.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.2/src/fl_api_requester/FLAPIRequester.py` & `fl-api-requester-1.0.3/src/fl_api_requester/FLAPIRequester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Dict, List
 from dacite import from_dict
 import requests
 
 from . import FLAPIConnectionData
 from .dto.DTO import DTO
+from .dto.request.discord.AddChannelsToDiscordDTO import AddChannelsToDiscordDTO
+from .dto.request.discord.RemoveChannelsFromDiscordDTO import RemoveChannelsFromDiscordDTO
 from .dto.request.alliance.CreateAllianceDTO import CreateAllianceDTO
 from .dto.request.alliance.RemoveAllianceDTO import RemoveAllianceDTO
 from .dto.request.authentication.AuthenticationRequestDTO import AuthenticationRequestDTO
 from .dto.request.discord.AddAllianceToDiscordDTO import AddAllianceToDiscordDTO
 from .dto.request.discord.CreateDiscordDTO import CreateDiscordDTO
 from .dto.request.discord.RemoveDiscordDTO import RemoveDiscordDTO
 from .dto.request.planet.AddPlanetDTO import AddPlanetDTO
@@ -129,21 +131,27 @@
     def get_discord_alliances(self, discord_id: int) -> List[AllianceDTO]:
         return [
             from_dict(AllianceDTO, alliance) 
             for alliance in self._send_get_request(f"/discord/{discord_id}/alliances")
         ]
     
     def create_discord(self, discord_data: CreateDiscordDTO) -> DiscordDTO:
-        return from_dict(DiscordDTO, self._send_post_request("/discord/create", "POST", discord_data))
+        return from_dict(DiscordDTO, self.__send_request("/discord/create", "POST", discord_data))
 
     def add_alliance_to_discord(self, discord_data: AddAllianceToDiscordDTO) -> DiscordDTO:
-        return from_dict(DiscordDTO, self._send_post_request("/discord/add-alliance", "POST", discord_data))
+        return from_dict(DiscordDTO, self.__send_request("/discord/add-alliance", "POST", discord_data))
+
+    def add_discord_channels(self, channels_data: AddChannelsToDiscordDTO) -> DiscordDTO:
+        return from_dict(DiscordDTO, self.__send_request("/discord/add-channel", "POST", channels_data))
+    
+    def remove_discord_channels(self, channels_data: RemoveChannelsFromDiscordDTO) -> DiscordDTO:
+        return from_dict(DiscordDTO, self.__send_request("/discord/remove-channel", "DELETE", channels_data))
 
     def remove_discord(self, discord_data: RemoveDiscordDTO) -> DiscordDTO:
-        return from_dict(DiscordDTO, self._send_delete_request("/discord/remove", "DELETE", discord_data))
+        return from_dict(DiscordDTO, self.__send_request("/discord/remove", "DELETE", discord_data))
 
     #######################
     # Getters and setters #
     #######################
 
     def get_connection_data(self) -> FLAPIConnectionData:
         return self.connection_data
```

### Comparing `fl-api-requester-1.0.2/src/fl_api_requester/exception/APIErrorException.py` & `fl-api-requester-1.0.3/src/fl_api_requester/exception/APIErrorException.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.2/src/fl_api_requester.egg-info/PKG-INFO` & `fl-api-requester-1.0.3/src/fl_api_requester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.2
+Version: 1.0.3
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -43,7 +43,8 @@
     # Get a War attack
     attack = api_requester.get_player_attacks("Galactifer")
 
     print(f"Galactifer attacked on {attack[0].timestamp_to_datetime():%d/%m/%Y at %H:%M:%S}")
 except APIErrorException as e:
     print(e.api_error)
 ```
+
```

### Comparing `fl-api-requester-1.0.2/src/fl_api_requester.egg-info/SOURCES.txt` & `fl-api-requester-1.0.3/src/fl_api_requester.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,33 @@
 src/fl_api_requester.egg-info/requires.txt
 src/fl_api_requester.egg-info/top_level.txt
 src/fl_api_requester/dto/DTO.py
 src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
 src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
 src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
 src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
+src/fl_api_requester/dto/request/discord/AddChannelsToDiscordDTO.py
 src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
+src/fl_api_requester/dto/request/discord/RemoveChannelsFromDiscordDTO.py
 src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
+src/fl_api_requester/dto/request/discord_channel/DiscordChannelRequestDTO.py
 src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
 src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
 src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
 src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
 src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
 src/fl_api_requester/dto/request/player/SetAllianceDTO.py
 src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
 src/fl_api_requester/dto/request/war/StartWarDTO.py
 src/fl_api_requester/dto/request/war/StopWarDTO.py
 src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
 src/fl_api_requester/dto/response/alliance/AllianceDTO.py
 src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
 src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
 src/fl_api_requester/dto/response/discord/DiscordDTO.py
+src/fl_api_requester/dto/response/discord_channel/DiscordChannelResponseDTO.py
 src/fl_api_requester/dto/response/planet/PlanetDTO.py
 src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
 src/fl_api_requester/dto/response/player/PlayerDTO.py
 src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
 src/fl_api_requester/dto/response/war/WarDTO.py
 src/fl_api_requester/exception/APIErrorException.py
```

