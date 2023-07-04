# Comparing `tmp/GailBot-0.1a7.tar.gz` & `tmp/GailBot-0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GailBot-0.1a7.tar", last modified: Tue Aug 23 19:14:23 2022, max compression
+gzip compressed data, was "GailBot-0.1a9.tar", last modified: Tue Jul  4 19:31:28 2023, max compression
```

## Comparing `GailBot-0.1a7.tar` & `GailBot-0.1a9.tar`

### file list

```diff
@@ -1,96 +1,184 @@
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.765103 GailBot-0.1a7/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.736847 GailBot-0.1a7/GailBot.egg-info/
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13416 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2721 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)        1 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)      135 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/requires.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)       13 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/top_level.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1078 2022-08-23 19:13:38.000000 GailBot-0.1a7/LICENSE
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13416 2022-08-23 19:14:23.764765 GailBot-0.1a7/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11324 2022-08-23 19:13:38.000000 GailBot-0.1a7/README.md
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.738372 GailBot-0.1a7/gailbot/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      455 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10680 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/controller.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.738846 GailBot-0.1a7/gailbot/core/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.740171 GailBot-0.1a7/gailbot/core/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      330 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2256 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/engine.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1369 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/engines.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.741466 GailBot-0.1a7/gailbot/core/engines/google/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      228 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8825 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3526 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/google.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.744864 GailBot-0.1a7/gailbot/core/engines/watson/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      214 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    12029 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/acoustic_model.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    17536 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    17514 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/language_model.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13114 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/recognition_results.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6370 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/recognize_callback.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    26034 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/watson.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.747771 GailBot-0.1a7/gailbot/core/io/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      204 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    23318 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/audio.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    18783 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/general.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    25569 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/io.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6128 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/shell.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11533 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/video.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.751164 GailBot-0.1a7/gailbot/core/network/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     7626 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_factory.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6587 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_interface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1810 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_models.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11779 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_protocol.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      184 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4737 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/network.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11452 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/request.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.753091 GailBot-0.1a7/gailbot/core/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      131 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2948 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/component.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3829 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    16013 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/pipeline.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1142 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/stream.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.753587 GailBot-0.1a7/gailbot/plugin/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      164 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.757888 GailBot-0.1a7/gailbot/plugin/plugin_manager/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      365 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      427 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/apply_config.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1207 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/config.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3914 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/loader.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3932 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      585 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/manager_summary.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1503 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      396 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_details.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      344 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_execution_summary.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     9994 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      524 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_source.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      279 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugins.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.758229 GailBot-0.1a7/gailbot/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.760200 GailBot-0.1a7/gailbot/services/objects/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      354 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2365 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/gailbot_settings.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2854 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/settings.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3233 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/source.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      406 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/utt.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.761158 GailBot-0.1a7/gailbot/services/organizer_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      210 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10333 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/organizer_service.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5485 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/source_loader.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.763127 GailBot-0.1a7/gailbot/services/pipeline_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      263 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4718 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5930 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/output_stage.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      901 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/payload.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4108 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/pipeline_service.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5014 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/plugins_stage.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3903 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/transcription_stage.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.764375 GailBot-0.1a7/gailbot/utils/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       17 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2785 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/download.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2025 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1714 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/models.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5674 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/threads.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1447 2022-08-23 19:13:38.000000 GailBot-0.1a7/pyproject.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2022-08-23 19:14:23.765216 GailBot-0.1a7/setup.cfg
--rw-r--r--   0 muhammadumair   (501) staff       (20)      230 2022-08-23 19:13:38.000000 GailBot-0.1a7/setup.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326785 GailBot-0.1a9/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1066 2023-07-04 18:14:11.000000 GailBot-0.1a9/LICENSE
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2023-07-04 19:18:37.000000 GailBot-0.1a9/MANIFEST.in
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13332 2023-07-04 19:31:28.326631 GailBot-0.1a9/PKG-INFO
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11312 2023-07-04 19:27:24.000000 GailBot-0.1a9/README.md
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1349 2023-07-04 19:02:49.000000 GailBot-0.1a9/pyproject.toml
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4339 2023-07-04 18:17:43.000000 GailBot-0.1a9/requirements.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2023-07-04 19:31:28.326821 GailBot-0.1a9/setup.cfg
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      355 2023-07-04 18:14:11.000000 GailBot-0.1a9/setup.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.306103 GailBot-0.1a9/src/
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.310777 GailBot-0.1a9/src/GailBot.egg-info/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13332 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     6142 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        1 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4401 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/requires.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       23 2023-07-04 19:31:28.000000 GailBot-0.1a9/src/GailBot.egg-info/top_level.txt
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.310928 GailBot-0.1a9/src/config_backend/
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.305546 GailBot-0.1a9/src/config_backend/engines/
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311079 GailBot-0.1a9/src/config_backend/engines/google/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      549 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/google/google_config.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311224 GailBot-0.1a9/src/config_backend/engines/watson/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2196 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/watson/watson_config.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311421 GailBot-0.1a9/src/config_backend/engines/whisper/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      929 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/engines/whisper/whisper_config.toml
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      546 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/paths.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311540 GailBot-0.1a9/src/config_backend/plugin/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      142 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/plugin/valid_plugin.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.311905 GailBot-0.1a9/src/config_backend/services/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      407 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/default_setting.toml
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1119 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/format.md
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      448 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/services/service.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312017 GailBot-0.1a9/src/config_backend/settings/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      272 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/settings/default.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312275 GailBot-0.1a9/src/config_backend/toplevel/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1040 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/toplevel/ws_config.toml
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       40 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/toplevel/ws_root.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312414 GailBot-0.1a9/src/config_backend/util/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      163 2023-07-04 19:02:33.000000 GailBot-0.1a9/src/config_backend/util/log.toml
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312683 GailBot-0.1a9/src/gailbot/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      383 2023-07-04 19:31:15.000000 GailBot-0.1a9/src/gailbot/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    19613 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/api.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.312835 GailBot-0.1a9/src/gailbot/configs/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      459 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313086 GailBot-0.1a9/src/gailbot/configs/confs/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/confs/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1163 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/confs/paths.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313196 GailBot-0.1a9/src/gailbot/configs/interfaces/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1767 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313335 GailBot-0.1a9/src/gailbot/configs/interfaces/config/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4599 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/config/ws_config.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.306691 GailBot-0.1a9/src/gailbot/configs/interfaces/core/
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313766 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      683 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/google.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      741 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/watson.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2111 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/engines/whisper.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.313881 GailBot-0.1a9/src/gailbot/configs/interfaces/core/setting/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      900 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/setting/defaults.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314014 GailBot-0.1a9/src/gailbot/configs/interfaces/core/util/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      384 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/core/util/logger.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314398 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       87 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      905 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/pluginsuite.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       72 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/plugin/validstructure.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314682 GailBot-0.1a9/src/gailbot/configs/interfaces/services/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       62 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/services/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2096 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/configs/interfaces/services/service.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.314799 GailBot-0.1a9/src/gailbot/core/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.315218 GailBot-0.1a9/src/gailbot/core/engines/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      323 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1560 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/engine.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1014 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/engineManager.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2361 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/exception.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.315585 GailBot-0.1a9/src/gailbot/core/engines/google/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       26 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    12222 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/core.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2453 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/google/google.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.316538 GailBot-0.1a9/src/gailbot/core/engines/watson/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      260 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11778 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/am.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      367 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/codes.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    12608 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/core.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    17153 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/lm.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13326 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/recognition_results.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5190 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/recognize_callback.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4913 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/watson/watson.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.317057 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      203 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5567 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/core.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.317443 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      199 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3363 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/diarize.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3460 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/diarization/utils.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2824 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/parsers.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2290 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperEngine.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.318402 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      641 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10466 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/alignment.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8927 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    24565 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe_efficient.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8623 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/transcribe_naive.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8383 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/utils.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      412 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/engines/whisperEngine/whisperTimestamped/vars.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.318775 GailBot-0.1a9/src/gailbot/core/pipeline/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      259 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1046 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/component.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11217 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/pipeline/pipeline.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.319515 GailBot-0.1a9/src/gailbot/core/utils/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      163 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2630 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/download.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    14146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/general.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1400 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/logger.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    27794 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/media.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    14967 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/core/utils/threads.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320018 GailBot-0.1a9/src/gailbot/plugins/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      264 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320503 GailBot-0.1a9/src/gailbot/plugins/loader/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8722 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/directoryloader.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      668 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/pluginLoader.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10540 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/loader/urlloader.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10349 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/manager.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1404 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/plugin.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     7991 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/plugins/suite.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.320754 GailBot-0.1a9/src/gailbot/services/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      110 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    21854 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/controller.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.321026 GailBot-0.1a9/src/gailbot/services/converter/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      179 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2651 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/converter.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.321864 GailBot-0.1a9/src/gailbot/services/converter/payload/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      290 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2946 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/audioPayload.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3588 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/conversationDirectoryPayload.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13278 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/payloadObject.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3740 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/transcribedDirPayload.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2105 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/payload/videoPayload.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.322091 GailBot-0.1a9/src/gailbot/services/converter/plugin/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/plugin/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5659 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/plugin/pluginMethod.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.322856 GailBot-0.1a9/src/gailbot/services/converter/result/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      241 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1266 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/analysis.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1534 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/format.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      323 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/processingStatus.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1827 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/resultInterface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5585 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/converter/result/transcribe.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.323090 GailBot-0.1a9/src/gailbot/services/organizer/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      211 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    18069 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/organizer.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.323355 GailBot-0.1a9/src/gailbot/services/organizer/settings/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      104 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324108 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      268 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      534 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2685 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/googleInterface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      326 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/pluginSettingsInterface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2527 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/watsonInterface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2067 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/interface/whisperInterface.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324622 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      136 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3919 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/engineObject.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      185 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/pluginObject.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3441 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/objects/settingObject.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    20186 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/settings/settingManager.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.324998 GailBot-0.1a9/src/gailbot/services/organizer/source/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       81 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8305 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/source_manager.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3203 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/organizer/source/source_object.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.325258 GailBot-0.1a9/src/gailbot/services/pipeline/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       37 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.325912 GailBot-0.1a9/src/gailbot/services/pipeline/components/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      146 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     6085 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/analysisComponent.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2102 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/formatComponent.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      359 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/progress.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10197 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/components/transcribeComponent.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2079 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/services/pipeline/pipeline.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326150 GailBot-0.1a9/src/gailbot/workspace/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       37 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/workspace/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5610 2023-07-04 18:14:11.000000 GailBot-0.1a9/src/gailbot/workspace/manager.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2023-07-04 19:31:28.326393 GailBot-0.1a9/tests/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    16540 2023-07-04 18:14:11.000000 GailBot-0.1a9/tests/test_api.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3335 2023-07-04 18:14:11.000000 GailBot-0.1a9/tests/test_small.py
```

### Comparing `GailBot-0.1a7/GailBot.egg-info/PKG-INFO` & `GailBot-0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.1a7
-Summary: An Automated Transcription System for Conversation Analysis
+Version: 0.1a9
+Summary: GailBot API
+Author-email: Muhammad Umair <muhammad.umair@tufts.edu>
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
-        Copyright (c) 2022 Human Interaction Lab
+        Copyright (c) 2023 jasonycwu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -23,25 +24,24 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/mumair01/GailBot
 Project-URL: source, https://github.com/mumair01/GailBot
-Project-URL: download, https://github.com/mumair01/GailBot/releases
 Project-URL: tracker, https://github.com/mumair01/GailBot/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # GailBot
 
 **NOTE**: This documentation is a work in progress and will be updated.
 
 
@@ -264,16 +264,16 @@
 
 
 class CombineTurns(GBPlugin):
 
     def __init__(self) -> None:
         super().__init__()
 
-    def apply_plugin(self, dependency_outputs: Dict[str, Any],
-                     plugin_input: PluginMethodSuite) -> List[Utt]:
+    def apply(self, dependency_outputs: Dict[str, Any],
+                     methods: PluginMethodSuite) -> List[Utt]:
         # Combine all the utterances in the utterance map into a single
         # conversation.
         combined = list()
         turns_map: Dict[str, List[Utt]
                         ] = dependency_outputs["turn_construct"]
         for turns in turns_map.values():
             combined.extend(turns)
```

### Comparing `GailBot-0.1a7/LICENSE` & `GailBot-0.1a9/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Human Interaction Lab
+Copyright (c) 2023 jasonycwu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `GailBot-0.1a7/PKG-INFO` & `GailBot-0.1a9/src/GailBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.1a7
-Summary: An Automated Transcription System for Conversation Analysis
+Version: 0.1a9
+Summary: GailBot API
+Author-email: Muhammad Umair <muhammad.umair@tufts.edu>
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
-        Copyright (c) 2022 Human Interaction Lab
+        Copyright (c) 2023 jasonycwu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -23,25 +24,24 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/mumair01/GailBot
 Project-URL: source, https://github.com/mumair01/GailBot
-Project-URL: download, https://github.com/mumair01/GailBot/releases
 Project-URL: tracker, https://github.com/mumair01/GailBot/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # GailBot
 
 **NOTE**: This documentation is a work in progress and will be updated.
 
 
@@ -264,16 +264,16 @@
 
 
 class CombineTurns(GBPlugin):
 
     def __init__(self) -> None:
         super().__init__()
 
-    def apply_plugin(self, dependency_outputs: Dict[str, Any],
-                     plugin_input: PluginMethodSuite) -> List[Utt]:
+    def apply(self, dependency_outputs: Dict[str, Any],
+                     methods: PluginMethodSuite) -> List[Utt]:
         # Combine all the utterances in the utterance map into a single
         # conversation.
         combined = list()
         turns_map: Dict[str, List[Utt]
                         ] = dependency_outputs["turn_construct"]
         for turns in turns_map.values():
             combined.extend(turns)
```

### Comparing `GailBot-0.1a7/README.md` & `GailBot-0.1a9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,16 @@
 
 
 class CombineTurns(GBPlugin):
 
     def __init__(self) -> None:
         super().__init__()
 
-    def apply_plugin(self, dependency_outputs: Dict[str, Any],
-                     plugin_input: PluginMethodSuite) -> List[Utt]:
+    def apply(self, dependency_outputs: Dict[str, Any],
+                     methods: PluginMethodSuite) -> List[Utt]:
         # Combine all the utterances in the utterance map into a single
         # conversation.
         combined = list()
         turns_map: Dict[str, List[Utt]
                         ] = dependency_outputs["turn_construct"]
         for turns in turns_map.values():
             combined.extend(turns)
```

### Comparing `GailBot-0.1a7/gailbot/core/engines/engine.py` & `GailBot-0.1a9/src/gailbot/core/engines/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2021-12-02 13:13:08
+# @Date:   2023-01-06 15:49:53
 # @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2022-08-23 10:32:21
+# @Last Modified time: 2023-01-09 11:21:54
 
-# Standard library imports
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List
-# Third party imports
-# Local imports
-from gailbot.core.io import GailBotIO
+from typing import List
+from typing import Any, Dict
 
-
-class STTEngine(ABC):
-    """
-    Template for all speech to text engines.
-
-    Inherits:
-        (ABC)
-    """
+class Engine(ABC):
     @abstractmethod
-    def __init__(self, io: GailBotIO) -> None:
+    def __init__(self, *args, **kwargs):
         pass
 
     @abstractmethod
-    def configure(self, *args, **kwargs) -> bool:
-        """
-        Configure core attributes of the engine.
-
-        Returns:
-            (bool): True if successfully configured. False otherwise.
-        """
-        pass
-
+    def __repr__(self):
+        """Returns all the configurations and additional metadata"""
+        raise NotImplementedError()
+    
     @abstractmethod
-    def get_configurations(self) -> Dict[str, Any]:
-        """
-        Obtain all core configurations of the engine/
-
-        Returns:
-            (Dict[str,Any]): Mapping from core configuration to the values.
-        """
+    def transcribe(self, *args, **kwargs) -> Any:
+        """Use the engine to transcribe an item"""
         pass
+    
+    @abstractmethod
+    def was_transcription_successful(self) -> bool:
+        """ return true if the transcription is successful """
+        pass 
 
     @abstractmethod
     def get_engine_name(self) -> str:
         """
         Obtain the name of the current engine.
 
         Returns:
@@ -71,25 +56,17 @@
         Args:
             file_path (str)
 
         Returns:
             (bool): True if file is supported. False otherwise.
         """
         pass
+    
+    
+    
+
+
+
+
 
-    @abstractmethod
-    # TODO: Needs to define what it returns.
-    def transcribe(self):
-        """
-        Transcribe the audio file that can be added through the configure method
-        """
-        pass
 
-    @abstractmethod
-    def was_transcription_successful(self) -> bool:
-        """
-        Determine whether the transcription was successful.
 
-        Returns:
-            (bool): True if transcription was successful. False otherwise.
-        """
-        pass
```

### Comparing `GailBot-0.1a7/gailbot/core/engines/watson/acoustic_model.py` & `GailBot-0.1a9/src/gailbot/core/engines/watson/am.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,176 +1,195 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2022-04-22 12:33:51
+# @Date:   2023-01-09 11:41:12
 # @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2022-04-22 12:46:39
+# @Last Modified time: 2023-01-16 12:01:31
+
 # Standard library imports
-from typing import BinaryIO, List, Any, Callable, Tuple, Dict, Union
+from typing import Any, BinaryIO, List, TextIO, Tuple, Dict, Callable, Union
 from enum import IntEnum
 # Local imports
+
+# Third party imports
 from ibm_watson import SpeechToTextV1, ApiException
 from ibm_cloud_sdk_core.authenticators import IAMAuthenticator
-# Third party imports
+from gailbot.core.engines import exception as ERR
+from ibm_watson.speech_to_text_v1 import CustomWord
 
+from gailbot.configs import watson_config_loader
+from gailbot.core.utils.media import MediaHandler
 
-class WatsonReturnCodes(IntEnum):
-    """
-    Return codes from Watson.
-    """
-    ok = 200
-    created = 201
-    notFound = 404
-    notAcceptable = 406
-    unsupported = 415
+import logging
+logger = logging.getLogger(__name__)
+
+from .codes import WatsonReturnCodes
 
+WATSON_CONFIG = watson_config_loader()
 
-class WatsonAcousticModel:
+class WatsonAMInterface:
     """
     Responsible for interacting with the IBM Watson STT service and providing
     methods for interacting with acoustic models.
     """
-    # Mappings from region to the region url.
-    regions = {
-        "dallas": "https://api.us-south.speech-to-text.watson.cloud.ibm.com",
-        "washington": "https://api.us-east.speech-to-text.watson.cloud.ibm.com",
-        "frankfurt": "https://api.eu-de.speech-to-text.watson.cloud.ibm.com",
-        "sydney": "https://api.au-syd.speech-to-text.watson.cloud.ibm.com",
-        "tokyo": "https://api.jp-tok.speech-to-text.watson.cloud.ibm.com",
-        "london": "https://api.eu-gb.speech-to-text.watson.cloud.ibm.com",
-        "seoul": "https://api.kr-seo.speech-to-text.watson.cloud.ibm.com"}
+    def __init__(self, apikey : str, region : str):
 
-    def __init__(self) -> None:
-        self.stt = None
+        self.apikey = apikey
+        self.region = region
+        self.media_h = MediaHandler()
         self.connected_to_service = False
-
-    # Custom acoustic models
-
-    def get_custom_models(self) -> Dict[str, str]:
-        """
-        Obtain all custom acoustic models
-
-        Returns:
-            (Dict[str,str]):
-                Mapping from custom acoustic model to the customization id.
-        """
-        custom_models = dict()
-        success, resp = self._execute_watson_method(
-            self.stt.list_acoustic_models, [WatsonReturnCodes.ok])
-        if success:
-            for model in resp["customizations"]:
-                custom_models[model["name"]] = model["customization_id"]
-        return custom_models
-
-    def get_custom_model(self, customization_id: str) \
-            -> Union[Dict[str, Any], None]:
+        # Parse confs
+        self._regions = WATSON_CONFIG.regions_uris
+        self._format_to_content_types = WATSON_CONFIG.format_to_content
+        self._defaults = WATSON_CONFIG.defaults
+        self.max_size_bytes = WATSON_CONFIG.max_file_size_bytes
+
+        if not self._is_api_key_valid(apikey, self._regions[region]):
+            raise Exception(f"Apikey {apikey} invalid")
+        if not region in self._regions:
+            raise Exception(
+                f"Region {region} not in {list(self._regions.keys())}"
+            )
+        try:
+            # Create the stt service and run
+            authenticator = IAMAuthenticator(self.apikey)
+            self.stt = SpeechToTextV1(authenticator=authenticator)
+            self.stt.set_service_url(self._regions[self.region])
+        except: 
+            raise ERR.ConnectionError("ERROR: Failed to connect to the Watson STT")
+        else:
+            self.connected_to_service  = True
+    
+    def get_custom_model(
+        self,
+        customization_id: str
+    ) -> Union[Dict[str, Any], None]:
         """
         Obtain information regarding a specific custom acoustic model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (Union[Dict[str,Any],None]):
                 Mapping from the following keys to their values:
-                customization_id, created, updated,language, dialect,
+                customization_id, CREATED, updated,language, dialect,
                 versions, owner, name, description, base_model_name, status,
                 progress
                 None if unsuccessful.
         """
         _, resp = self._execute_watson_method(
-            self.stt.get_acoustic_model, [WatsonReturnCodes.ok],
+            self.stt.get_acoustic_model, [WatsonReturnCodes.OK],
             [customization_id])
         return resp
 
-    def create_custom_model(self, name: str, base_model_name: str,
-                            description: str) -> bool:
+    def get_custom_models(self) -> Dict[str, str]:
+        """
+        Obtain all custom acoustic models
+
+        Returns:
+            (Dict[str,str]):
+                Mapping from custom acoustic model to the customization id.
+        """
+        custom_models = dict()
+        response = self._execute_watson_method(
+            self.stt.list_acoustic_models, [WatsonReturnCodes.OK])
+        if response:
+            for model in response["customizations"]:
+                custom_models[model["name"]] = model["customization_id"]
+        return custom_models
+
+    def create_custom_model(
+        self,
+        name : str,
+        base_model_name : str,
+        description : str
+    ) -> bool:
         """
         Create a new custom acoustic model.
 
         Args:
             name (str): Name of the model.
             base_model_name (str):
                 Name of the base model. Must be a supported base model.
             description (str): Description of the model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.create_acoustic_model, [WatsonReturnCodes.created],
-            [name, base_model_name, None, description])
-        return success
+        response = self._execute_watson_method(
+            self.stt.create_acoustic_model, [WatsonReturnCodes.CREATED],
+            [name, base_model_name], {"description": description})
+        return response
 
     def delete_custom_model(self, customization_id: str) -> bool:
         """
         Delete an existing custom acoustic model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_acoustic_model, [WatsonReturnCodes.ok],
+        response= self._execute_watson_method(
+            self.stt.delete_acoustic_model, [WatsonReturnCodes.OK],
             [customization_id])
-        return success
+        return response
 
     def train_custom_model(self, customization_id: str) -> bool:
         """
         Train a custom acoustic model with a previously added resource.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.train_acoustic_model, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.train_acoustic_model, [WatsonReturnCodes.OK],
             [customization_id])
-        return success
+        return response
 
     def reset_custom_model(self, customization_id: str) -> bool:
         """
         Reset a custom acoustic model to remove all loaded resources.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.reset_acoustic_model, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.reset_acoustic_model, [WatsonReturnCodes.OK],
             [customization_id])
-        return success
+        return response
 
-    def upgrade_custom_model(self, customization_id: str,
-                             custom_language_model_id: str = None) -> bool:
+    def upgrade_custom_model(self, customization_id: str, 
+                    custom_language_model_id: str = None) -> bool:
         """
         Upgrade the base model of the custom acoustic model to its latest
         version.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
             custom_language_model_id (str):
                 ID of the custom language model (if any) that this acoustic
                 model was trained with a custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
+        response = self._execute_watson_method(
             self.stt.upgrade_acoustic_model,
             [customization_id, custom_language_model_id])
-        return success
-
-    # Custom Audio resources
+        return response
 
+    
     def get_custom_audio_resources(self, customization_id: str) \
             -> Union[List[Dict], None]:
         """
         List information about all audio resources of the specified custom
         acoustic model.
 
         Args:
@@ -178,158 +197,126 @@
 
         Returns:
             (Union[List[Dict],None]):
                 Each internal list contains the following keys:
                 "duration","name","details","status"
                 None if unsuccessful.
         """
-        success, resp = self._execute_watson_method(
+        response = self._execute_watson_method(
             self.stt.list_audio, [customization_id])
-        if success:
-            return resp["audio"]
+        if response:
+            return response["audio"]
 
-    def get_custom_audio_resource(self, customization_id: str,
+        def get_custom_audio_resource(self, customization_id: str,
                                   audio_name: str) -> Union[Dict, None]:
-        """
-        Obtain information about a specific custom acoustic model.
+            """
+            Obtain information about a specific custom acoustic model.
 
-        Args:
-            customization_id (str): Unique ID of the custom acoustic model.
-            audio_name (str): Name of the specific audio resource.
-
-        Returns:
-            (Dict): Contains the following keys:
-                    "duration","name","details","status"
-                    None if unsuccessful
-        """
-        success, resp = self._execute_watson_method(
-            self.stt.get_audio, [WatsonReturnCodes.ok],
-            [customization_id, audio_name])
-        if success:
-            return resp
+            Args:
+                customization_id (str): Unique ID of the custom acoustic model.
+                audio_name (str): Name of the specific audio resource.
+
+            Returns:
+                (Dict): Contains the following keys:
+                        "duration","name","details","status"
+                        None if unsuccessful
+            """
+            response = self._execute_watson_method(
+                self.stt.get_audio, [WatsonReturnCodes.OK],
+                [customization_id, audio_name])
+            if response:
+                return response
 
-    def add_custom_audio_resource(self, customization_id: str,
+        def add_custom_audio_resource(self, customization_id: str,
                                   audio_name: str, audio_resource: BinaryIO, content_type: str)\
             -> bool:
-        """
-        Add an audio resource to the specific custom acoustic model.
+            """
+            Add an audio resource to the specific custom acoustic model.
 
-        Args:
-            customization_id (str): Unique ID of the custom acoustic model.
-            audio_name (str): Name of the specific audio resource.
-            audio_resource (BinaryIO):
-                Audio resources to be added to the custom model.
-            content_type (str):
-                Type of the audio resource. One of:
-                [application/zip,application/gzip,audio/alaw,audio/basic,
-                audio/flac,audio/g729,audio/l16,audio/mp3,audio/mpeg,
-                audio/mulaw,audio/ogg,audio/ogg;codecs=opus,
-                audio/ogg;codecs=vorbis,audio/wav,audio/webm,
-                audio/webm;codecs=opus,audio/webm;codecs=vorbis]
-
-        Returns:
-            (bool): True if successful. False otherwise.
-        """
-        success, _ = self._execute_watson_method(
-            self.stt.add_audio, [WatsonReturnCodes.created],
-            [customization_id, audio_name, audio_resource, content_type])
-        return success
+            Args:
+                customization_id (str): Unique ID of the custom acoustic model.
+                audio_name (str): Name of the specific audio resource.
+                audio_resource (BinaryIO):
+                    Audio resources to be added to the custom model.
+                content_type (str):
+                    Type of the audio resource. One of:
+                    [application/zip,application/gzip,audio/alaw,audio/basic,
+                    audio/flac,audio/g729,audio/l16,audio/mp3,audio/mpeg,
+                    audio/mulaw,audio/ogg,audio/ogg;codecs=opus,
+                    audio/ogg;codecs=vorbis,audio/wav,audio/webm,
+                    audio/webm;codecs=opus,audio/webm;codecs=vorbis]
+
+            Returns:
+                (bool): True if successful. False otherwise.
+            """
+            response = self._execute_watson_method(
+                self.stt.add_audio, [WatsonReturnCodes.CREATED],
+                [customization_id, audio_name, audio_resource, content_type])
+            return response
 
     def delete_custom_audio_resource(self, customization_id: str,
                                      audio_name: str) -> bool:
         """
         Delete the specified resource from the custom audio model.
 
         Args:
             customization_id (str): Unique ID of the custom acoustic model.
             audio_name (str): Name of the specific audio resource.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_audio, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.delete_audio, [WatsonReturnCodes.OK],
             [customization_id, audio_name])
-        return success
-     # Others
-
-    def connect_to_service(self, api_key: str, region: str) -> bool:
-        """
-        Connect to the stt service using the given api key.
-        Must be called before other methods can be used.
-
-        Args:
-            apikey (str): Valid API key for the watson STT service.
-
-        Returns:
-            (bool): True if connected successfully. False otherwise.
-        """
-        if not region in self.regions.keys() or \
-                not self._is_api_key_valid(api_key, self.regions[region]):
-            self.connected_to_service = False
-            return False
-        self.stt = self._initialize_stt_service(api_key)
-        self.stt.set_service_url(self.regions[region])
-        self.connected_to_service = True
-        return True
-
-    ############################# PRIVATE METHODS ############################
-
+        return response
+    
+    ## PRIVATE ##
+    
     def _is_api_key_valid(self, apikey: str, url: str) -> bool:
-        """
-        Determine if the given apikey is valid.
-
-        Args:
-            apikey (str): API key for the watson STT service.
-
-        Returns:
-            (bool): True if the key is valid. False otherwise.
-        """
         try:
             stt = self._initialize_stt_service(apikey)
             stt.set_service_url(url)
             stt.list_models()
             return True
         except:
             return False
 
     def _initialize_stt_service(self, apikey: str) -> SpeechToTextV1:
-        """
-        Initialize a SpeechToTextV1 object given an apikey.
-
-        Args:
-            apikey (str): Valid API key for the watson STT service.
-
-        Returns:
-            (SpeechToTextV1)
-        """
         authenticator = IAMAuthenticator(apikey)
         stt = SpeechToTextV1(authenticator=authenticator)
         return stt
-
-    def _execute_watson_method(self, method: Callable,
-                               expected_response_codes: List[WatsonReturnCodes], args: List = [],
-                               kwargs: Dict = {}) -> Tuple[bool, Any]:
+    
+    def _execute_watson_method(self, 
+                               method: Callable,
+                               expected_response_codes: List[WatsonReturnCodes], 
+                               args: List = [],
+                               kwargs: Dict = {}) -> Union[bool, Any]:
         """
         Execute a watson method only if connected to watson.
 
         Args:
             method (Callable): Method to execute.
             expected_response_codes (List[WatsonReturnCodes]):
                 Watson codes that are expected for a successful response.
             args (List): Arguments to pass to the method.
             kwargs (Dict): Keyword arguments to method
 
         Returns:
-            (Tuple[bool,Any]):
-                True + result if successful. False + None otherwise.
+           (Union[bool,Any]):
+                result from watson if successful. 
+                False otherwise.
         """
         if not self.connected_to_service:
-            return (False, None)
+            raise ERR.ConnectionError
         try:
             resp = method(*args, **kwargs)
             if any([resp.get_status_code() == expected
                     for expected in expected_response_codes]):
-                return (True, resp.get_result())
-            return (False, None)
-        except ApiException:
-            return (False, None)
+                return resp.get_result()
+            raise ERR.WatsonMethodExecutionError
+        except ApiException as e:
+            logger.info(f"Exception raised: {e}", exc_info=e)
+            return False
+        except ERR.WatsonMethodExecutionError as e:
+            logger.info(f"Exception raised: {e}", exc_info=e)
+            return False
```

### Comparing `GailBot-0.1a7/gailbot/core/engines/watson/language_model.py` & `GailBot-0.1a9/src/gailbot/core/engines/watson/lm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,452 +1,499 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2021-12-02 13:13:08
+# @Date:   2023-01-09 11:30:48
 # @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2021-12-02 15:20:18
+# @Last Modified time: 2023-01-16 12:00:25
+
+""" TODO:
+1. only function to create and delete model are tested 
+   function to train the model are not tested 
+"""
 # Standard library imports
 from typing import Any, BinaryIO, List, TextIO, Tuple, Dict, Callable, Union
 from enum import IntEnum
 # Local imports
 
 # Third party imports
+from gailbot.configs import watson_config_loader
+from gailbot.core.engines import exception as ERR
 from ibm_watson import SpeechToTextV1, ApiException
 from ibm_cloud_sdk_core.authenticators import IAMAuthenticator
 from ibm_watson.speech_to_text_v1 import CustomWord
 
+from gailbot.core.utils.media import MediaHandler
 
-class WatsonReturnCodes(IntEnum):
-    """
-    Return codes from Watson.
-    """
-    ok = 200
-    created = 201
-    notFound = 404
-    notAcceptable = 406
-    unsupported = 415
-
-
-class WatsonLanguageModel:
-    """
-    Responsible for interacting with the IBM Watson STT service and providing
-    methods for interacting with language models.
-    """
-    # Mappings from region to the region url.
-    regions = {
-        "dallas": "https://api.us-south.speech-to-text.watson.cloud.ibm.com",
-        "washington": "https://api.us-east.speech-to-text.watson.cloud.ibm.com",
-        "frankfurt": "https://api.eu-de.speech-to-text.watson.cloud.ibm.com",
-        "sydney": "https://api.au-syd.speech-to-text.watson.cloud.ibm.com",
-        "tokyo": "https://api.jp-tok.speech-to-text.watson.cloud.ibm.com",
-        "london": "https://api.eu-gb.speech-to-text.watson.cloud.ibm.com",
-        "seoul": "https://api.kr-seo.speech-to-text.watson.cloud.ibm.com"}
+import logging
+logger = logging.getLogger(__name__)
 
-    def __init__(self) -> None:
-        self.stt = None
-        self.connected_to_service = False
+from .codes import WatsonReturnCodes
 
-    # base model methods
+WATSON_CONFIG = watson_config_loader()
+class WatsonLMInterface:
+    def __init__(self, apikey : str, region : str):
+        self.connected_to_service = False
+        self.apikey = apikey
+        self.region = region
+        self.media_h = MediaHandler()
+
+        # Parse confs
+        self._regions = WATSON_CONFIG.regions_uris
+        self._format_to_content_types = WATSON_CONFIG.format_to_content
+        self._defaults = WATSON_CONFIG.defaults
+        self.max_size_bytes = WATSON_CONFIG.max_file_size_bytes
+
+        if not self._is_api_key_valid(apikey, self._regions[region]):
+            raise Exception(f"Apikey {apikey} invalid")
+        if not region in self._regions:
+            raise Exception(
+                f"Region {region} not in {list(self._regions.keys())}"
+            )
 
-    def get_base_model(self, model_name: str) -> Union[Dict[str, Any], None]:
+        try:
+            # Create the stt service and run
+            authenticator = IAMAuthenticator(self.apikey)
+            self.stt = SpeechToTextV1(authenticator=authenticator)
+            self.stt.set_service_url(self._regions[self.region])
+        except:
+            raise Exception("Connect to STT failed")
+        else:
+            self.connected_to_service = True 
+        
+    def get_base_model(self, model_name : str) -> Dict:
         """
         Obtain information regarding the given base language model.
 
         Args:
             model_name (str): Name of the language model.
 
         Returns:
             (Union[Dict[str,Any],None]):
                 Dictionary with keys: name, language, rate, url,
                 supported_features, description if successful.
                 None if unsuccessful.
         """
-        if not self.connected_to_service:
-            return
-        _, resp = self._execute_watson_method(
-            self.stt.get_model, [WatsonReturnCodes.ok], [model_name], {})
+        if not self.connected_to_service: return {}
+        resp = self._execute_watson_method(
+            self.stt.get_model, [WatsonReturnCodes.OK], model_name
+        )
         return resp
 
     def get_base_models(self) -> List[str]:
         """
         Obtain a list of the names of base language models that are supported.
 
         Returns:
             (List[str]): Names of the base language models.
         """
-        if not self.connected_to_service:
-            return []
-        names = list()
-        success, resp = self._execute_watson_method(
-            self.stt.list_models, [WatsonReturnCodes.ok])
-        if success:
-            for model in resp["models"]:
-                names.append(model["name"])
-        return names
-
-    # Custom model methods
-
-    def get_custom_model(self, customization_id: str) \
-            -> Union[Dict[str, Any], None]:
+        if not self.connected_to_service: return []
+        resp = self._execute_watson_method(
+            self.stt.list_models, [WatsonReturnCodes.OK]
+        )
+        return [model["name"] for model in resp["models"]] if resp != None else []
+
+    def get_custom_model(
+        self,
+        customization_id: str
+    ) -> Dict:
         """
         Obtain information regarding a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[Dict[str,Any],None]):
                 Mapping from the following keys to their values:
-                customization_id, created, updated,language, dialect,
+                customization_id, CREATED, updated,language, dialect,
                 versions, owner, name, description, base_model_name, status,
                 progress
                 None if unsuccessful.
         """
-        if not self.connected_to_service:
-            return
-        success, resp = self._execute_watson_method(
-            self.stt.get_language_model, [WatsonReturnCodes.ok],
-            [customization_id])
-        return resp if success else None
+        if not self.connected_to_service: return []
+        resp = self._execute_watson_method(
+            self.stt.get_language_model, [WatsonReturnCodes.OK], customization_id
+        )
+        return resp
 
     def get_custom_models(self) -> Dict[str, str]:
         """
-        Obtain all custom language models.
+        Get custom language models
 
         Returns:
             (Dict[str,str]):
                  Mapping from custom model name to the customization id.
         """
-        if not self.connected_to_service:
-            return {}
+        if not self.connected_to_service: return {}
         custom_models = dict()
-        success, resp = self._execute_watson_method(
-            self.stt.list_language_models, [WatsonReturnCodes.ok])
-        if success:
+        resp = self._execute_watson_method(
+            self.stt.list_language_models, [WatsonReturnCodes.OK]
+        )
+        if resp != None:
             for model in resp["customizations"]:
                 custom_models[model["name"]] = model["customization_id"]
         return custom_models
 
-    def create_custom_model(self, name: str, base_model_name: str,
-                            description: str) -> bool:
+    def create_custom_model(
+        self,
+        name: str, 
+        base_model_name : str,
+        description : str
+    ):
         """
         Create a new custom language model.
         Does NOT create a new model if one with the same name already exists.
 
         Args:
             name (str): Name of the model.
             base_model_name (str):
                 Name of the base model. Must be a supported base model.
             description (str): Description of the model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        if not self.connected_to_service or \
-                name in self.get_custom_models().keys():
+        if not self.connected_to_service or name in self.get_custom_models().keys():
             return False
-        success, _ = self._execute_watson_method(
-            self.stt.create_language_model, [WatsonReturnCodes.created],
+        response = self._execute_watson_method(
+            self.stt.create_language_model, [WatsonReturnCodes.CREATED],
             [name, base_model_name], {"description": description})
-        return success
+        return response
 
     def delete_custom_model(self, customization_id: str) -> bool:
         """
         Delete an existing custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_language_model, [WatsonReturnCodes.ok],
+        success = self._execute_watson_method(
+            self.stt.delete_language_model, [WatsonReturnCodes.OK],
             [customization_id])
         return success
 
     def train_custom_model(self, customization_id: str) -> bool:
         """
         Train a custom language model with a previously added resource.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, resp = self._execute_watson_method(
-            self.stt.train_language_model, [WatsonReturnCodes.ok],
+        success = self._execute_watson_method(
+            self.stt.train_language_model, [WatsonReturnCodes.OK],
             [customization_id])
         return success
-
+   
     def reset_custom_model(self, customization_id: str) -> bool:
         """
         Reset a custom language model to remove all loaded resources.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.reset_language_model, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.reset_language_model, [WatsonReturnCodes.OK],
             [customization_id])
-        return success
-
+        return response
+    
     def upgrade_custom_model(self, customization_id: str) -> bool:
         """
         Upgrade the base model of the custom language model to its latest
         version.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.upgrade_language_model, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.upgrade_language_model, [WatsonReturnCodes.OK],
             [customization_id])
-        return success
-
-    # Custom corpora methods
-
-    def get_corpora(self, customization_id: str) -> Union[List[Dict], None]:
+        return response
+    
+    def get_corpora(self, customization_id: str) -> Dict:
         """
         Obtain the corpora used to train this custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict],None]):
                 Each internal dict contains the keys: name,
                 out_of_vocabulary_words,total_words, status.
                 None if unsuccessful.
         """
-        success, resp = self._execute_watson_method(
-            self.stt.list_corpora, [WatsonReturnCodes.ok], [customization_id])
-        if success:
-            return resp["corpora"]
-
-    def add_corpus(self, customization_id: str, corpus_name: str,
-                   corpus_file: BinaryIO) -> bool:
+        response = self._execute_watson_method(
+            self.stt.list_corpora, [WatsonReturnCodes.OK], [customization_id])
+        if response:
+            return response["corpora"]
+
+    def add_corpus(
+        self,
+        customization_id: str,
+        corpus_name: str,
+        corpus_file: BinaryIO
+    ) -> bool:
         """
         Add a corpus to the specified custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus
             corpus_file (BinaryIO): utf-8 encoded plain text file.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.add_corpus, [WatsonReturnCodes.created],
+        response = self._execute_watson_method(
+            self.stt.add_corpus, [WatsonReturnCodes.CREATED],
             [customization_id, corpus_name, corpus_file, True])
-        return success
+        return response
 
     def delete_corpus(
-            self, customization_id: str, corpus_name: str) -> bool:
+        self,
+        customization_id: str,
+        corpus_name: str
+    ) -> bool:
         """
         Delete a corpus from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus to delete.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_corpus, [WatsonReturnCodes.ok]
+        response = self._execute_watson_method(
+            self.stt.delete_corpus, 
+            [WatsonReturnCodes.OK], 
             [customization_id, corpus_name])
-        return success
+        return response
 
     def get_corpus(
-        self, customization_id: str, corpus_name: str) \
-            -> Union[Dict[str, Any], None]:
+        self,
+        customization_id: str,
+        corpus_name: str
+    ) -> Dict:
         """
         Obtain information about a specific custom corpus used to train the
         custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             corpus_name (str): Name of the corpus.
 
         Returns:
             (Union[Dict[str,Any],None]): Contains the keys: "name",
             "out_of_vocabulary_words", "total_words","status"
             None if unsuccessful.
         """
-        _, resp = self._execute_watson_method(
-            self.stt.get_corpus, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.get_corpus, [WatsonReturnCodes.OK],
             [customization_id, corpus_name])
-        return resp
-
-    # Custom words methods
-
-    def get_custom_words(
-            self, customization_id: str) -> Union[List[Dict], None]:
+        return response
+    
+    def get_custom_works(
+        self,
+        customization_id : str
+    ) -> List[Dict]:
         """
         Obtain all the custom words used to train a custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict], None]):
                 Each dictionary contains the keys: "word","sounds_like",
                 "display_as","count","source"
                 None if unsuccessful.
         """
-        success, resp = self._execute_watson_method(
-            self.stt.list_words, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.list_words, [WatsonReturnCodes.OK],
             [customization_id])
-        if success:
-            return resp["words"]
+        if response:
+            return response["words"]
 
-    def add_custom_words(
-            self, customization_id: str, words: List[str]) -> bool:
+    def add_custom_works(
+        self,
+        customization_id : str,
+        words : List[str]
+    ) -> bool:
         """
         Add one or more custom words to the specified custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             words (List[str]): List of words to add to the model.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
         custom_words = list()
         for word in words:
             custom_words.append(CustomWord(word=word))
-        success, _ = self._execute_watson_method(
-            self.stt.add_words, [WatsonReturnCodes.created],
+        response = self._execute_watson_method(
+            self.stt.add_words, [WatsonReturnCodes.CREATED],
             [customization_id, custom_words])
-        return success
-
-    def delete_custom_word(
-            self, customization_id: str, word: str) -> bool:
+        return response
+    
+    def delete_custom_words(
+        self,
+        customization_id : str,
+        word : str
+    ) -> bool:
         """
         Delete a word from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             word (str): Word to delete.
 
         Returns:
             (bool): True if successful. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_word, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.delete_word, [WatsonReturnCodes.OK],
             [customization_id, word])
-        return success
-
-    # Custom grammars methods
+        return response
 
-    def get_custom_grammars(self, customization_id: str) \
-            -> Union[List[Dict], None]:
+    def get_custom_grammars(
+        self,
+        customization_id : str
+    ) -> List[Dict]:
         """
         Obtain a list of the grammars of a custom model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
 
         Returns:
             (Union[List[Dict], None]):
                 Internal dictionaries contain the keys:
                 out_of_vocabulary_words","name","status"
                 None of unsuccessful.
         """
-        success, resp = self._execute_watson_method(
+        response = self._execute_watson_method(
             self.stt.list_grammars, [customization_id])
-        if success:
-            return resp["grammars"]
-
+        if response:
+            return response["grammars"]
+        
     def get_custom_grammar(
-            self, customization_id: str, grammar_name: str) \
-            -> Union[Dict, None]:
+        self,
+        customization_id: str,
+        grammar_name: str
+    ) -> Dict:
         """
         Obtain information about a specific grammar in a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
 
         Returns:
             (Union[Dict, None]):
                 Contains the keys: "out_of_vocabulary_words","name","status"
                 None of unsuccessful.
         """
-        _, resp = self._execute_watson_method(
-            self.stt.get_grammar, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.get_grammar, [WatsonReturnCodes.OK],
             [customization_id, grammar_name])
-        return resp
+        return response
 
-    def add_custom_grammar(self, customization_id: str,
-                           grammar_name: str, grammar_file: TextIO,
-                           content_type: str) -> bool:
+    def add_custom_grammar(
+        self,
+        customization_id: str,
+        grammar_name: str,
+        grammar_file: TextIO,
+        content_type: str
+    ) -> bool:
         """
         Add a grammar to the custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
             grammar_file (TextIO): Plain text file containing grammar.
             content_type (str):
                 Format of the grammar. one of:
                     application/srgs, application/srgs+xml
 
         Returns:
             (bool): True if successfully added. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.add_grammar, [WatsonReturnCodes.created],
+        response  = self._execute_watson_method(
+            self.stt.add_grammar, [WatsonReturnCodes.CREATED],
             [customization_id, grammar_name, grammar_file, content_type, True])
-        return success
+        return response
 
     def delete_custom_grammar(
-            self, customization_id: str, grammar_name: str) -> bool:
+        self,
+        customization_id: str,
+        grammar_name: str
+    ) -> bool:
         """
         Delete the specific grammar from a custom language model.
 
         Args:
             customization_id (str): Unique ID of the custom language model.
             grammar_name (str): Name of the custom grammar.
 
         Returns:
             (bool): True if successfully added. False otherwise.
         """
-        success, _ = self._execute_watson_method(
-            self.stt.delete_grammar, [WatsonReturnCodes.ok],
+        response = self._execute_watson_method(
+            self.stt.delete_grammar, [WatsonReturnCodes.OK],
             [customization_id, grammar_name])
-        return success
+        return response
 
     # Others
-
-    def connect_to_service(self, api_key: str, region: str) -> bool:
+    def _execute_watson_method(
+        self,
+        method : Callable,
+        expected_response_codes: List[WatsonReturnCodes],
+        args: List = [],
+        kwargs: Dict = {}
+    ) -> Union[bool, Any]:
         """
-        Connect to the stt service using the given api key.
-        Must be called before other methods can be used.
+        Execute a watson method only if connected to watson.
 
         Args:
-            apikey (str): Valid API key for the watson STT service.
+            method (Callable): Method to execute.
+            expected_response_codes (List[WatsonReturnCodes]):
+                Watson codes that are expected for a successful response.
+            args (List): Arguments to pass to the method.
+            kwargs (Dict): Keyword arguments to method
 
         Returns:
-            (bool): True if connected successfully. False otherwise.
+            (Union[bool,Any]):
+                result from watson if successful. 
+                False otherwise.
         """
-        if not region in self.regions.keys() or \
-                not self._is_api_key_valid(api_key, self.regions[region]):
-            self.connected_to_service = False
+        if not self.connected_to_service:
+            raise ERR.ConnectionError("Error raised: connection error")
+        try:
+            resp = method(*args, **kwargs)
+            if any([resp.get_status_code() == expected
+                        for expected in expected_response_codes]):
+                return resp.get_result()
+            raise ERR.WatsonMethodExecutionError
+        except ApiException as e:
+            logger.info(f"Exception raised: {e}", exc_info=e)
             return False
-        self.stt = self._initialize_stt_service(api_key)
-        self.stt.set_service_url(self.regions[region])
-        self.connected_to_service = True
-        return True
-
-    ############################# PRIVATE METHODS ############################
-
-    def _is_api_key_valid(self, apikey: str, url : str) -> bool:
+        except ERR.WatsonMethodExecutionError as e:
+            logger.info(f"Exception raised: {e}", exc_info=e)
+            return False
+        
+    def _is_api_key_valid(self, apikey: str, url: str) -> bool:
         """
         Determine if the given apikey is valid.
 
         Args:
             apikey (str): API key for the watson STT service.
 
         Returns:
@@ -468,36 +515,8 @@
             apikey (str): Valid API key for the watson STT service.
 
         Returns:
             (SpeechToTextV1)
         """
         authenticator = IAMAuthenticator(apikey)
         stt = SpeechToTextV1(authenticator=authenticator)
-        return stt
-
-    def _execute_watson_method(self, method: Callable,
-                               expected_response_codes: List[WatsonReturnCodes], args: List = [],
-                               kwargs: Dict = {}) -> Tuple[bool, Any]:
-        """
-        Execute a watson method only if connected to watson.
-
-        Args:
-            method (Callable): Method to execute.
-            expected_response_codes (List[WatsonReturnCodes]):
-                Watson codes that are expected for a successful response.
-            args (List): Arguments to pass to the method.
-            kwargs (Dict): Keyword arguments to method
-
-        Returns:
-            (Tuple[bool,Any]):
-                True + result if successful. False + None otherwise.
-        """
-        if not self.connected_to_service:
-            return (False, None)
-        try:
-            resp = method(*args, **kwargs)
-            if any([resp.get_status_code() == expected
-                    for expected in expected_response_codes]):
-                return (True, resp.get_result())
-            return (False, None)
-        except ApiException as e:
-            return (False, e)
+        return stt
```

### Comparing `GailBot-0.1a7/gailbot/core/engines/watson/recognition_results.py` & `GailBot-0.1a9/src/gailbot/core/engines/watson/recognition_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 '''
     The classes in this script model the RecognitionResult object as per
     the documentation for IBM Watson STT service:
     https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-basic-response
 '''
 # Standard library imports
 from typing import Dict, Any, List
+from gailbot.core.utils.logger import makelogger
 import itertools
 # Local imports
 # Third party imports
 
-
+logger = makelogger("recognition_result")
 class Alternative:
     """
     Models the smallest unit of a transcription result.
     """
 
     def __init__(self, data: Dict) -> None:
         self.items = {
@@ -208,14 +209,17 @@
         Returns:
             (List[Dict[str,str]]):
                 List of dictionaries modeling SpeakerLabel objects.
                 Each dictionary has the keys: 'from', 'to', 'speaker',
                 'confidence'.
         """
         labels = list()
+        if not self.items or not self.items["speaker_labels"]:
+            return labels
+        
         for label in self.items["speaker_labels"]:
             labels.append({
                 "start_time": label.get("from"),
                 "end_time": label.get("to"),
                 "speaker": label.get("speaker"),
                 "label_confidence": label.get("confidence")})
         return labels
@@ -369,16 +373,17 @@
             if "results" in watson_data.keys():
                 results_array = list()
                 for results in watson_data["results"]:
                     results_array.append(Result({"results": results}))
                 self.items["results"] = results_array
             return True
         except Exception as e:
-            print("parsing excepion", e)
-
+            logger.error(e, exc_info=e)
+            
+            
     def _aggregate(self, results: List[Result], aggregation_key: str,
                    only_final: bool) -> List[Any]:
         """
         Aggregate the results from a list of Result objects, based on the
         aggregation key. If only_final = True, only use the results of
         Result objects considered final.
         """
```

### Comparing `GailBot-0.1a7/gailbot/core/io/audio.py` & `GailBot-0.1a9/src/gailbot/core/utils/media.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,578 +1,868 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2021-10-19 15:34:24
+# @Date:   2023-01-08 16:28:17
 # @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2021-12-05 17:04:18
-# Standard library imports
+# @Last Modified time: 2023-01-16 14:33:08
+
+from typing import List, Union, Dict
 import os
-from typing import Dict, List, Any, Tuple
 from dataclasses import dataclass
-# Local imports
-# Third party imports
+from abc import ABC 
+from .general import (
+    get_extension,
+    get_name,
+    make_dir, 
+    run_cmd,
+    get_cmd_status,
+    is_directory, 
+    paths_in_dir,
+    CMD_STATUS
+)
+from gailbot.core.utils.logger import makelogger 
 from pydub import AudioSegment
-from copy import deepcopy
-import sounddevice as sd
-
+from pydub.silence import detect_leading_silence
+MERGED_FILE_NAME = "merged"
+logger = makelogger("media")
+@dataclass
+class Stream(ABC):
+    """ Abstract class that defines the representation of a media stream 
+    
+    Attributes
+    name : str
+        the name of the stream file 
+    source : Union [List[str], List[Stream]]
+        the source of the stream, which can either be a list of paths to a media 
+        file or a list of media Stream  
+    extension : str
+        the file extension, which tells the file type 
+    """
+    source : Union[List[str], List["Stream"]]
+    name : str
+    extension : str
 
 @dataclass
-class AudioStream:
-    input_file_path: str
-    input_format: str
-    audio_segment: AudioSegment
-    output_dir_path: str
-    output_format: str
+class AudioStream(Stream):
+    """ A subclass of Steam class which defines the representation of 
+        audio stream 
+    
+    Attributes
+    segment : AudioSegment
+        stores source of an audio segment 
+        
+    """
+    segment : AudioSegment
 
+    def __repr__(self):
+        print(f"audio stream {self.name}\n")
 
-class AudioIO:
+@dataclass
+class VideoStream(Stream):
+    """ A subclass of Steam class which defines the representation of 
+        Video stream 
+    
     """
-    Provides methods that directly interact with and can modify audio streams
-    and files. Intended to be used for audio manipulation.
+    pass
+
+    def __repr__(self):
+        return f"video stream {self.name}\n"
+
+class AudioHandler:
+    """ Implement a class that contains functions to handle audio file 
+
+    Attributes
+        _SUPPORTED_FORMATS: List[str]
+            a list of supported audio format
+        _DEFAULT_FORMAT: 
+            the default audio format         
     """
 
-    # Audio formats that are currently supported.
-    INPUT_AUDIO_FORMATS = ("mp3", "mpeg", "opus", "wav")
-    OUTPUT_AUDIO_FORMATS = ("wav", "opus")
-
-    def __init__(self) -> None:
-        self.streams: Dict[str, AudioStream] = dict()
-        self.default_input_audio_format = "wav"
-        # Recording parameters
-        self.recording_sample_rate = 44100
-        self.recording_channels = 2
-        self.recording_max_duration_seconds = 60 * 5
-        self.recording_sample_width_bytes = 2
-
-    def read_streams(self, file_paths: Dict[str, str]) -> bool:
-        """
-        Read the audio files at the given paths for future operations.
-        If there is an error encountered while reading any single file,
-        none of the files are read.
-        Clears all previously read streams from memory.
-
-        Args:
-            file_paths (Dict[str,str]):
-                Mapping from unique file name to its path.
-        """
-        # Clears all the previous streams when reading new ones.
-        self.streams.clear()
-        # Determine whether all files are valid
-        if not all([self._is_audio_file(path) for path in file_paths.values()]):
-            return False
-         # If all files exist, they are read as AudioSegment objects.
-        for name, file_path in file_paths.items():
-            success, stream = self._initialize_audio_stream_from_file(
-                file_path, self.default_input_audio_format, None, None)
-            # Verify that the stream is successfully created.
-            if not success:
-                self.streams.clear()
-                return False
-            self.streams[name] = stream
-        return True
-
-    # TODO: This does not work properly. Needs to be fixed.
-    def record_stream(self, identifier: str, duration_seconds: float) -> bool:
-        """
-        Record an audio stream with the given identifier and of
-        duration_seconds.
+    _SUPPORTED_FORMATS = ["mp3", "mpeg", "opus", "wav"]
+    _DEFAULT_FORMAT = "wav"
+
+
+    def __repr__(self) -> str:
+        return "Audio Stream handler"
+    
+    @property
+    def supported_formats(self) -> List[str]:
+        """ return a list of string with supported audio format"""
+        return self._SUPPORTED_FORMATS
+
+    @staticmethod    
+    def is_supported(path : str) -> bool:
+        """ tell if a audio file is supported by the AudioHandler
 
         Args:
-            identifier (str): identifier for the audio recording.
-            duration_seconds (float): Recording duration.
+            path (str): a path to a file
+
+        Returns:
+            bool: return true of the file is supported 
         """
-        if not 0 < duration_seconds <= self.recording_max_duration_seconds:
-            return False
-        try:
-            recording = sd.rec(
-                int(duration_seconds * self.recording_sample_rate),
-                samplerate=self.recording_sample_rate,
-                channels=self.recording_channels,
-                blocking=True)
-            # Load the array as an audio segment
-            audio_segment = AudioSegment(
-                data=recording.tobytes(),
-                sample_width=2,
-                frame_rate=self.recording_sample_rate,
-                channels=self.recording_channels)
-            self.streams.clear()
-            success, stream = AudioSegment(
-                "", self.default_input_audio_format, audio_segment, None, None)
-            if success:
-                self.streams[identifier] = stream
-                return True
-            return False
-        except:
-            return False
+        return get_extension(path) in ["mp3", "mpeg", "opus", "wav"]
+        
+    def read_file(self,path : str) -> AudioStream:
+        """ read the audio file data
 
-    def set_output_paths(self, output_dir_paths: Dict[str, str]) -> bool:
+        Args:
+            path (str): a path to a file 
+
+        Returns:
+            AudioStream: return the audio file data as an AudioStream object 
+                         if the file type is supported, return nothing 
+                         if the file type is unsupported  
+        """
+        if not AudioHandler.is_supported(path):
+            return
+        format = get_extension(path)
+        segment = AudioSegment.from_file(
+            path, format=format
+        )
+        return AudioStream(
+            source=[path],
+            name=get_name(path),
+            extension=format,
+            segment=segment
+        )
+
+    def record(
+        self,
+        name : str,
+        out_dir : str,
+        duration_sec : float = -1,
+    ) -> AudioStream:
+        """ record the audio file 
+        """
+        raise NotImplementedError()
+
+    def write_stream(
+        self,
+        stream : AudioStream,
+        outdir : str,
+        name : str = None,
+        format : str = None
+    ) -> str:
+        """ write a stream with the given format. If not format or name is 
+            specified, uses the stream's default name and format.
+        
+        Args: 
+            stream: AudioStream 
+                stores the audio file data as an instance of AudioStream 
+            outdir: str 
+                a path that stores the output directory 
+            name: str (Optional)
+                file name, default to the name of stream 
+            format: str (Optional)
+                file format, default to the extension of  stream 
+        
+        Return:
+            the file path 
+        """
+        if format not in self.supported_formats:
+            raise Exception(f"Format {format} not supported")
+        # Construct output file path
+        name = stream.name if name == None else name
+        ext = stream.extension if format == None else format
+        make_dir(outdir,overwrite=False)
+        path = f"{outdir}/{name}.{ext}"
+        stream.segment.export(path,format=ext)
+        return path
+
+    def info(self, stream : AudioStream) -> Dict:
+        """Get information about the given audio stream
+        
+        Args: 
+            stream: AudioStream 
+                stores the audio file data as an instance of AudioStream 
+        
+        Return:
+            a dictionary with the stream information 
+        """
+        segment = stream.segment
+        return {
+                "name" : stream.name,
+                "format" : stream.extension,
+                "source" : stream.source,
+                "decibels_relative_to_full_scale": segment.dBFS,
+                "channels": segment.channels,
+                "sample_width": segment.sample_width,
+                "frame_rate": segment.frame_rate,
+                "frame_width": segment.frame_width,
+                "root_mean_square": segment.rms,
+                "highest_amplitude": segment.max,
+                "duration_seconds": segment.duration_seconds,
+                "num_frames": segment.frame_count(),
+        }
+
+    def change_volume(
+        self,
+        stream : AudioStream,
+        change_db : float
+    ) -> AudioStream:
+        """
+        Apply the specified gain to the audio stream.
+        Args:
+            stream: AudioStream 
+                stores the audio file data as an instance of AudioStream 
+            change_db: float 
+                the targeting value of the volume
+        
+        Return: 
+            the resulting audio stream as an instance of AudioStream
+        """
+        segment = stream.segment.apply_gain(change_db)
+        stream.segment = segment
+        return stream
+
+    def mono_to_stereo(
+        self,
+        left_stream : AudioStream,
+        right_stream : AudioStream
+    ) -> AudioStream:
+        """
+        Get a new stereo stream from the two mono streams
+        Args: 
+            left_stream: AudioStream
+                stores the data of a mono audio file
+            right_stream: AudioStream
+                stores the data of a mono audio file 
+        
+        Return:
+            the resulting audio stream as an instance of AudioStream
+        """
+        stereo_name = f"{left_stream.name}_{right_stream.name}_stereo"
+        sources = [left_stream,right_stream]
+        segment = AudioSegment.from_mono_audiosegments(
+            left_stream.segment,right_stream.segment
+        )
+        return AudioStream(
+            sources, stereo_name,self._DEFAULT_FORMAT,segment
+        )
+    
+    def stereo_to_mono(
+        self,
+        stream : AudioStream
+    ) -> List[AudioStream]:
+        """
+        Convert the given stereo stream to mono.
+        
+        Args: 
+            stream: AudioStream 
+                stores the data of a stereo audio file 
+        
+        Returns:
+            a list of two mono audio file 
+            
         """
-        Set the output direcotry path for the audio streams associated with
-        the identifiers.
 
+        left_segment, right_segment = stream.segment.split_to_mono()
+        left_stream = AudioStream(
+            [stream],f"{stream.name}_left",self._DEFAULT_FORMAT,left_segment
+        )
+        right_stream = AudioStream(
+            [stream],f"{stream.name}_right", self._DEFAULT_FORMAT,right_segment
+        )
+        return left_stream, right_stream
+
+    def concat(self, streams : List[AudioStream]) -> AudioStream:
+        """
+        Concat the given stream end to end, start to finish, into a single stream.
+        
+        Args: 
+            streams: List[AudioStream]
+                A list of audio streams 
+        
+        Returns: 
+            the resulting audio stream that is composed by concatenating the 
+            input streams 
+        """
+        concatenated = AudioSegment.empty()
+        for stream in streams:
+            concatenated += stream.segment
+        name = "_".join([stream.name for stream in streams])
+        name += "_concatenated"
+        return AudioStream(
+            source=[streams],
+            name=name,
+            extension=self._DEFAULT_FORMAT,
+            segment=concatenated
+        )
+
+    def overlay(
+        self,
+        left_stream : AudioStream,
+        right_stream : AudioStream,
+        loop_shorter_stream : bool = False
+    ) -> AudioStream:
+        """
+        Overlay two audio streams on top of each other
+        
+        Args: 
+            left_stream:AudioStream
+                stores one audio file data that will be overlayed 
+            right_stream:AudioStream
+                stores one audio file data that will be overlayed 
+            loop_shorter_stream: bool
+                if true, the shorter audio file will be looped until it reaches
+                the length of the longer audio file 
+        """
+        # Determine which segment is longer
+        if left_stream.segment.duration_seconds > right_stream.segment.duration_seconds:
+            segments = [left_stream.segment, right_stream.segment]
+        else:
+            segments = [right_stream.segment,left_stream.segment]
+        if loop_shorter_stream:
+            overlaid_segment = segments[0].overlay(segments[1], loop=True)
+        else:
+            # Create a silent stream to cover duration difference
+            duration_diff = segments[0].duration_seconds - segments[1].duration_seconds
+            silence = AudioSegment.silent(duration=duration_diff)
+            segments[1] += silence
+            overlaid_segment = segments[0].overlay(segments[1])
+        name = f"{left_stream.name}_{right_stream.name}_overlaid"
+        return AudioStream(
+            [left_stream,right_stream], name, self._DEFAULT_FORMAT,
+            overlaid_segment
+        )
+
+    
+    
+    def reverse(self, stream : AudioStream) -> AudioStream:
+        """
+        Reverse the given audio stream 
+        
         Args:
-            output_dir_paths (Dict[str,str]):
-                Mapping from identifier to output directory path.
-                The path must be a valid directory path.
+            stream: AudioStream
+                stores the data of an audio stream
+        Returns:
+            the resulting audio stream after reversed
         """
-        # Setting the output paths for each AudioStream
-        for name, output_dir_path in output_dir_paths.items():
-            # Verify identifiers and path
-            if not name in self.streams or \
-                    not self._is_directory(output_dir_path):
-                return False
-            self.streams[name].output_dir_path = output_dir_path
-        return True
+        reversed_segment = stream.segment.reverse()
+        stream.segment = reversed_segment
+        return stream
+
+    def chunk(
+        self,
+        stream : AudioStream,
+        chunk_duration_s : float
+    ) -> List[AudioStream]:
+        """
+        Generate chunks of the given audio with the provided duration.
+        
+        Args: 
+        stream: AudioStream
+                stores the data of an audio stream
+        
+        Returns:
+            a list of audio stream, which are the chunks of the given audio 
+            stream
 
-    def set_output_formats(self, output_formats: Dict[str, str]) -> bool:
         """
-        Set the output formats for the audio streams associated with the
-        identifiers.
+        assert chunk_duration_s > 0, f"Duration must be positive"
+        # Simply return original stream if no chunking possible.
+        if chunk_duration_s > stream.segment.duration_seconds:
+            return [stream]
+
+        duration_ms = chunk_duration_s * 1000
+        chunks = list()
+        for i, chunk_segment in enumerate(stream.segment[::int(duration_ms)]):
+            name = f"{stream.name}_{chunk_duration_s}_chunk_{i}"
+            chunk = AudioStream(
+                [stream],name, self._DEFAULT_FORMAT,chunk_segment
+            )
+            chunks.append(chunk)
+        return chunks
+
+    @staticmethod
+    def convert_to_16bit_wav(input_path, output_path):
+        pid = run_cmd(["ffmpeg", "-i", input_path, "-acodec", "pcm_s16le", "-ar", "16000", output_path])
+        while True:
+            match get_cmd_status(pid):
+                case CMD_STATUS.STOPPED:
+                    logger.error("process was stopped when converting the audio file to 16bit_wav format")
+                    break
+                case CMD_STATUS.FINISHED:
+                    return output_path
+                case CMD_STATUS.ERROR:
+                    logger.error("error in converting the audio file to 16bit_wav format")
+                    break
+                case CMD_STATUS.NOTFOUND:
+                    break
+        logger.warn("cannot convert the file to 16bit_wav file format, use original file instead")
+        return input_path
+    
+    @staticmethod 
+    def compress_to_opus(audio_path:str, output_dir:str):
+        """ compress the audio file stored in audio_path to output_dir, 
+            with the same audio file name with opus format
 
         Args:
-            output_formats (Dict[str,str]):
-                Mapping from identifier to output format
-                The format must be a supported output audio format.
+            audio_path (str): the path to original file 
+            output_dir (str): the path to the directory where the compressed file 
+                              will be stored
+
+        Raises:
+            ChildProcessError: 
+            ChildProcessError: 
+            ProcessLookupError: 
 
         Returns:
-            (bool): True if format successfully set. False otherwise.
-       """
-        # Setting the output paths for each AudioStream
-        for name, output_format in output_formats.items():
-            if not name in self.streams or \
-                    not output_format in self.OUTPUT_AUDIO_FORMATS:
-                return False
-            self.streams[name].output_format = output_format
-        return True
+            str: the path to the compressed file
+        """
+        logger.info("Converting file")
+        out_path = "{}/{}.opus".format(output_dir, get_name(audio_path))
+        logger.info(f"Converting path{out_path}")
+        pid = run_cmd(["ffmpeg", "-y", "-i", audio_path, "-strict", "-2", out_path])
+        
+        while True:
+            match get_cmd_status(pid):
+                case CMD_STATUS.STOPPED:
+                    raise ChildProcessError("ERROR: child process error")
+                case CMD_STATUS.FINISHED:
+                    break 
+                case CMD_STATUS.ERROR:
+                    raise ChildProcessError("ERROR: child process error")
+                case CMD_STATUS.NOTFOUND:
+                    raise ProcessLookupError("ERROR: process lookup error")
+        
+        if get_cmd_status(pid) == CMD_STATUS.FINISHED:
+            return out_path
+        else: 
+            return False
+    
+    @staticmethod 
+    def chunk_audio_to_outpath(audio_path:str, output_path:str, chunk_duration:int) -> List[str]:
+        """ given the audio path, chunking the audio into a series of audio
+            segment
+        
+        Args:
+            audio_path[str]: the file path to the audio file 
+            output_path[str]: the output of the chunked file 
+            duration[int]: the length of each chunk
+            
+        Return:
+            Union[List[str], bool]: return a list of the audio path to the 
+                                    chunked audios in order 
+        """
+        if not is_directory(output_path):
+            make_dir(audio_path)
+        basename = get_name(audio_path)
+        dir = os.path.join(output_path, f"{basename}_audio_chunks")
+        make_dir(dir)
+        idx = 0
+        try:
+            mediaHandler = MediaHandler()
+            stream = mediaHandler.read_file(audio_path)
+            chunks = mediaHandler.chunk(stream, chunk_duration)
+            for chunk in chunks:
+                mediaHandler.write_stream(
+                    chunk, dir, name=f"{basename}-{idx}", 
+                    format=get_extension(audio_path))
+                idx += 1
+                
+            audio_chunks = paths_in_dir(dir)
+            audio_chunks = sorted(audio_chunks, key=lambda file: (len(file), file))
+            
+        except Exception as e:
+            logger.error(e, exc_info=e)
+        else:
+            
+            return audio_chunks
 
-    ################################# GETTERS #############################
 
-    def is_readable(self, file_path: str) -> bool:
-        """
-        Determine if the file at the given path is readable by AudioIO.
-        """
-        return self._is_audio_file(file_path)
+    def overlay_audios(self, audios: List[str], output_path: str, name = MERGED_FILE_NAME):
+        res = self.read_file(audios[0])
+        name = MERGED_FILE_NAME
+        if len(audios) == 1:
+            res = self.read_file(audios[0])
+        else:
+            for i in range(1, len(audios)):
+                if AudioHandler.is_supported(audios[i]):
+                    nxt = self.read_file(audios[i])
+                    res = self.overlay(res, nxt)
+        return self.write_stream(res, output_path, name=name, format=get_extension(audios[0]))
+
+
+class VideoHandler:
+
+    _SUPPORTED_FORMATS = ["mxf"]
+    _BASE_FORMAT = "mp4"
+
+    @property
+    def supported_formats(self) -> List[str]:
+        return self._SUPPORTED_FORMATS
+
+
+    @staticmethod
+    def is_supported(path : str) -> bool:
+        return get_extension(path) in ["mxf"]
+
+
+    def read_file(self, path : str) -> VideoStream:
+        raise NotImplementedError()
+
+    def record(
+        self,
+        name : str,
+        out_dir : str,
+        duration_sec : float = -1,
+    ) -> VideoStream:
+        raise NotImplementedError()
+
+    def write_stream(
+        self,
+        stream : VideoStream,
+        out_dir : str,
+        name : str = None,
+        extension : str = None
+    ) -> str:
+        raise NotImplementedError()
+
+    def info(self, stream : VideoStream) -> Dict:
+        raise NotImplementedError()
+
+    def change_volume(
+        self,
+        stream : VideoStream,
+        change_db : float
+    ) -> VideoStream:
+        raise NotImplementedError()
+
+    def extract_audio(self, stream : VideoStream) -> AudioStream:
+        raise NotImplementedError()
+
+    def remove_audio(self, stream : VideoStream) -> VideoStream:
+        raise NotImplementedError()
+
+class MediaHandler:
+    def __init__(self):
+        """
+        Initializes an object of the MediaHandler class, an abstraction of the AudioHandler and 
+        VideoHandler classes.
+        """
+        self.audio_h = AudioHandler()
+        self.video_h = VideoHandler()
+        self._SUPPORTED_FORMATS = self.audio_h.supported_formats + self.video_h.supported_formats
+    
+    def __repr__(self) -> str:
+        return "Media Stream Handler"
+    
+    
+    @property
+    def supported_formats(self) -> List[str]:
+        """ 
+        Accesses list of supported formats.
 
-    def get_stream_configurations(self) -> Dict[str, Dict[str, Any]]:
+        Args:
+            Self
+        Returns:
+            A list of strings representing supported formats of the given MediaHandler object
         """
-        Obtain important configuration information for all files that have
-        been read.
+        return self._SUPPORTED_FORMATS
+
+    #### Audio and Video
+    @staticmethod
+    def is_supported(path: str) -> bool:
+        return AudioHandler.is_supported(path) or \
+               VideoHandler.is_supported(path)
+
 
+    @staticmethod
+    def is_audio(path : str) -> bool:
+        """
+        Determines if the given file is an audio file.
+        
+        Args:
+            path: Path to given file in string form
+        
         Returns:
-            (Dict[str,Dict[str,Any]]):
-                Dictionary containing mappings from the unique  identifier /
-                name of the file to a dictionary containing configuration
-                information.
+            True if the given file is an audio file, false if the given file 
+            is not an audio file.
         """
-        configs = dict()
-        for name in self.streams.keys():
-            audio_segment = self.streams[name].audio_segment
-            configs[name] = {
-                "decibels_relative_to_full_scale": audio_segment.dBFS,
-                "channels": audio_segment.channels,
-                "sample_width": audio_segment.sample_width,
-                "frame_rate": audio_segment.frame_rate,
-                "frame_width": audio_segment.frame_width,
-                "root_mean_square": audio_segment.rms,
-                "highest_amplitude": audio_segment.max,
-                "duration_seconds": audio_segment.duration_seconds,
-                "num_frames": audio_segment.frame_count()}
-        return configs
+        return AudioHandler.is_supported(path)
 
-    def get_stream_names(self) -> List[str]:
+    @staticmethod
+    def is_video(path : str) -> bool:
         """
-        Get the unique identifiers / names of all the files that are currently
-        ready to have operations performed on.
+        Determines if the given file is a video file.
 
+        Args:
+            path: Path to given file in string form
+        
         Returns:
-            (List[str]): Name of all files in stream.
+            True if the given file is a video file, false if the given file 
+            is not a video file.
         """
-        return list(self.streams.keys())
+        return VideoHandler.is_supported(path)
 
-    def get_streams(self) -> Dict[str, Any]:
+
+    def read_file(self, path : str) -> Stream:
         """
-        Obtain all streams that have been read as byte arrays.
+        Reads inputted file.
+
+        Args:
+            path: Path to given file in string form
 
         Returns:
-            (Dict[str,Any]): Mapping from file identifier / name to byte array.
-        """
-        streams = dict()
-        for name in self.streams.keys():
-            streams[name] = self.streams[name].audio_segment.raw_data
-        return streams
+            An AudioStream or VideoStream containing the read stream.
+            Raises exception if path is not supported.
 
-    def get_supported_input_formats(self) -> List[str]:
         """
-        Get the input audio file formats that are supported.
+        if get_extension(path) in self.audio_h.supported_formats:
+            return self.audio_h.read_file(path)
+        elif get_extension(path) in self.video_h.supported_formats:
+            return self.video_h.read_file(path)
+        else:
+            raise Exception(
+                f"ERROR: Format not supported for file: {path}"
+            )
+
+    def record(
+        self,
+        name : str,
+        out_dir : str,
+        out_stream_type : Union[AudioStream, VideoStream],
+        duration_sec : float = -1,
+    ) -> Stream:
         """
-        return list(self.INPUT_AUDIO_FORMATS)
+        Records audio or video file from inputted stream.
 
-    def get_supported_output_formats(self) -> List[str]:
-        """
-        Get the output audio file formats that are supported.
+        Args:
+            name: File name as a string.
+            out_dir: Path of the desired output directory as a string.
+            out_stream_type: AudioStream or VideoStream, depending on the inputted file.
+            duration_sec: Float containing the duration to record.
+
+        Returns:
+            Currently will raise NotImplementedError.
         """
-        return list(self.OUTPUT_AUDIO_FORMATS)
+        if out_stream_type == AudioStream:
+            return self.audio_h.record(name, out_dir, duration_sec)
+        else:
+            return self.video_h.record(name, out_dir, duration_sec)
 
-    ############################### PUBLIC METHODS ########################
 
-    def write(self, identifiers: List[str]) -> Tuple[bool, Dict]:
+    def write_stream(
+        self,
+        stream : Stream,
+        out_dir : str,
+        name : str = None,
+        format : str = None
+    ) -> str:
         """
-        Write the audio stream associated with the given identifiers.
-        If the output path and formats were not explicitly set, they default
-        to the input directory path and input formats.
+        Writes audio or video stream to given output directory.
 
         Args:
-            identifiers (List[str]): Unique identifiers for audio stream
+            stream: Inputted stream, of type AudioStream or VideoStream.
+            out_dir: Path of the desired output directory as a string.
+            name: File name as a string.
+            format: Audio format as a string.
 
         Returns:
-            (bool): True if all files are successfully written. False otherwise.
+            Output as type stream.
         """
-        paths = dict()
-        # List to store success values
-        is_success_list = list()
-        # Verify all identifiers
-        if not all([identifier in self.streams.keys()
-                    for identifier in identifiers]):
-            return False, paths
-        # Write all the output files
-        for name in identifiers:
-            success, output_path = self._export_audio(
-                self.streams[name].audio_segment,
-                self.streams[name].output_dir_path,
-                name,
-                self.streams[name].output_format)
-            is_success_list.append(success)
-            paths[name] = output_path
-        return all(is_success_list), paths
+        return self._get_handler(stream).write_stream(
+            stream, out_dir, name, format
+        )
 
-    def mono_to_stereo(self) -> Tuple[bool, str]:
+    def info(self, stream : Stream) -> Dict:
         """
-        Convert two mono streams into a single stereo stream.
-        The streams must have the same number of frames.
-        Only applies when there are only two streams that have been read.
-        Previous streams will be discarded and only the stereo stream will be
-        stored.
+        Accesss audio or video information
+
+        Args:
+            stream: Inputted stream, of type AudioStream or VideoStream.
 
         Returns:
-            (Tuple[bool,str]):
-                True if successful. False otherwise.
-                The string represents the unique identifier / name for the
-                stereo stream.
+            Information pertaining to the inputted stream in the form of a dictionary 
+            with different data fields.
         """
-        # Ensure that we only have two streams to combine into stereo.
-        if len(self.streams.keys()) != 2:
-            return (False, None)
-        # Obtain the audio segments
-        name_1, name_2 = self.streams.keys()
-        audio_segment_1 = self.streams[name_1].audio_segment
-        audio_segment_2 = self.streams[name_2].audio_segment
-        # Generate new file name and data for new stream.
-        stereo_name = "{}_{}_stereo".format(name_1, name_2)
-        output_dir_path = self.streams[name_1].output_dir_path
-        output_format = self.streams[name_1].output_format
-        # Attempt to combine into stereo.
-        try:
-            stereo_segment = AudioSegment.from_mono_audiosegments(
-                audio_segment_1, audio_segment_2)
-            stream = AudioStream(
-                "", self.default_input_audio_format, stereo_segment,
-                output_dir_path, output_format)
-            # Clear existing streams is successful
-            self.streams.clear()
-            self.streams[stereo_name] = stream
-            return (True, stereo_name)
-        except:
-            return (False, None)
-
-    def stereo_to_mono(self) -> Tuple[bool, Tuple[str, str]]:
-        """
-        Convert a stereo stream to two mono streams i.e. left stream and right
-        stream.
-        Only applies when there is only one stereo stream that has been
-        read.
-        Afterwards, the stereo stream is deleted and the left and right
-        streams are stored instead.
-
-        Returns:
-            (Tuple[bool, Tuple[str,str]]):
-                True if successful. False otherwise.
-                The Tuple represents the names /unique identifier of the left
-                channel stream and the right channel stream.
-        """
-        # Only works when a single stereo audio file has been read.
-        if len(self.streams.keys()) != 1:
-            return (False, (None, None))
-        # Generating names for channels
-        name, = self.streams.keys()
-        left_channel_name = name + "_left_channel_mono"
-        right_channel_name = name + "_right_channel_mono"
-        # Gathering data for new potential streams
-        audio_segment = self.streams[name].audio_segment
-        output_dir_path = self.streams[name].output_dir_path
-        output_format = self.streams[name].output_format
-        # Attempting to convert to mono.
-        try:
-            left_segment, right_segment = audio_segment.split_to_mono()
-            self.streams.clear()
-            # Creating streams for left and right channels.
-            left_stream = AudioStream(
-                "", self.default_input_audio_format, left_segment,
-                output_dir_path, output_format)
-            right_stream = AudioStream(
-                "", self.default_input_audio_format, right_segment,
-                output_dir_path, output_format)
-            self.streams[left_channel_name] = left_stream
-            self.streams[right_channel_name] = right_stream
-            return (True, (left_channel_name, right_channel_name))
-        except:
-            return (False, (None, None))
-
-    def concat(self) -> Tuple[bool, str]:
-        """
-        Combine all the streams into a single stream, one after another, in the
-        specific order in which they were read. There must be at least one
-        audio stream read before using this method.
-
-        Returns:
-            (Tuple[bool,str]):
-                True + name of the combined stream if successful.
-                False + "" otherwise.
-        """
-        # Do not do anything if no files have been read
-        if len(self.streams.keys()) == 0:
-            return (False, "")
-        # Concat all existing segments
-        combined_segment = AudioSegment.empty()
-        for stream in self.streams.values():
-            combined_segment += stream.audio_segment
-        # Generate name
-        combined_name = "_".join([name for name in self.streams.keys()])
-        combined_name += "_concatenated"
-        # Clear all existing streams
-        self.streams.clear()
-        # Store new stream
-        self.streams[combined_name] = AudioStream(
-            "", self.default_input_audio_format, combined_segment, None, None)
-        return (True, combined_name)
-
-    def overlay(self, loop_shorter_stream: bool = False) -> Tuple[bool, str]:
-        """
-        Overlays two audio streams on top of each other.
-        Clears all existing streams and only stores the overlaid stream.
-
-        Args:
-            loop_shorter_stream (bool):
-                If True, the shorter audio stream is looped i.e. starts playing
-                again after it ends. If False, silence is inserted after the
-                shorter audio stream until the longer stream finishes.
-                False by default.
-
-        Returns:
-            (Tuple[bool,str]):
-                True + name of the combined stream if successful.
-                False + "" otherwise.
-        """
-        # Only two files can be overlayed
-        if len(self.streams.keys()) != 2:
-            return (False, "")
-        # Determine the longer and shorted segments
-        segment_1, segment_2 = [stream.audio_segment
-                                for stream in self.streams.values()]
-        if segment_1.duration_seconds < segment_2.duration_seconds:
-            longer_segment, shorter_segment = segment_2, segment_1
-        else:
-            longer_segment, shorter_segment = segment_1, segment_2
-        # Combine the segments
-        if loop_shorter_stream:
-            overlaid_segment = longer_segment.overlay(
-                shorter_segment, loop=True)
-        else:
-            # Create a silent stream to cover duration difference
-            duration_difference = longer_segment.duration_seconds - \
-                shorter_segment.duration_seconds
-            silence = AudioSegment.silent(duration=duration_difference)
-            shorter_segment += silence
-            overlaid_segment = longer_segment.overlay(shorter_segment)
-        # Clear existing streams and store overlaid segment as new stream
-        overlaid_name = "_".join(self.streams.keys())
-        overlaid_name += "_overlaid"
-        self.streams.clear()
-        self.streams[overlaid_name] = AudioStream(
-            "", self.default_input_audio_format, overlaid_segment, None, None)
-        return (True, overlaid_name)
-
-    def change_volume(self, change: Dict[str, int]) -> bool:
-        """
-        Change the volume of the given file names.
-
-        Args:
-            change (Dict[str,int]):
-                Mapping from the name / unique identifier of the file to the
-                amount that the volume has to be changed in decibels.
-                Ex: 1 means no change, 2 means twice the volume, -2 means half
-                the original volume etc.
-        """
-        # Ensure that the name is a stream that has been read.
-        for name in change.keys():
-            if name not in self.streams.keys():
-                return False
-        # Applying the gain
-        for name, db_change in change.items():
-            audio_segment = self.streams[name].audio_segment
-            # Apply db change to the audio stream
-            new_segment = audio_segment.apply_gain(db_change)
-            self.streams[name].audio_segment = new_segment
-        return True
-
-    def reverse(self, names: List[str]) -> bool:
-        """
-        Reverse the audio stream with the name / identifier.
-
-        Args:
-            names (List[str]): Names of the streams to reverse. Must have
-                            been read before using this method.
-        """
-        # Ensure name is present / has been read.
-        for name in names:
-            if name not in self.streams.keys():
-                return False
-        # Reverse the appropriate streams
-        for name in names:
-            audio_segment = self.streams[name].audio_segment
-            reversed_segment = audio_segment.reverse()
-            self.streams[name].audio_segment = reversed_segment
-        return True
-
-    def chunk(self, chunks: Dict[str, int]) \
-            -> Tuple[bool, Dict[str, List[str]]]:
-        """
-        Chunks the streams with the given names / unique identifiers into
-        segments of the defined duration. If the duration of the chunk is
-        greater than the duration of the stream, it is not changed.
-        The original stream is deleted.
-        NOTE: The duration of the chunks is in seconds.
-
-        Args:
-            chunks (Dict[str,int]):
-                Mapping from name / identifier of stream to the duration of
-                each chunk in seconds.
-                The duration has to be a positive value.
-
-        Returns:
-            (Tuple[bool, Dict[str,List[str]]]):
-                True if successful. False otherwise.
-                The dictionary is a mapping from the name of stream to a list
-                containing the names of streams the original stream is chunked
-                into.
-        """
-        # All the names should be already read stream names.
-        # The chunk durations should be valid
-        for name, chunk_duration_seconds in chunks.items():
-            if name not in self.streams.keys() or \
-                    chunk_duration_seconds <= 0:
-                return (False, {})
-        # Mappings to store the new stream names and their relationships with
-        # original stream.
-        try:
-            name_mappings = dict()
-            new_streams = dict()
-            for name, chunk_duration_seconds in chunks.items():
-                audio_segment = self.streams[name].audio_segment
-                # Chunk based on the duration given.
-                if audio_segment.duration_seconds <= chunk_duration_seconds:
-                    name_mappings[name] = [name]
-                    new_streams[name] = deepcopy(self.streams[name])
-                else:
-                    chunk_names = list()
-                    duration_ms = chunk_duration_seconds * 1000
-                    for i, chunk_segment in enumerate(audio_segment[::duration_ms]):
-                        chunk_name = "{}_chunk_{}".format(name, i)
-                        new_streams[chunk_name] = AudioStream(
-                            "", self.default_input_audio_format, chunk_segment, None,
-                            "wav")
-                        chunk_names.append(chunk_name)
-                    name_mappings[name] = chunk_names
-            self.streams.clear()
-            self.streams = new_streams
-            return (True, name_mappings)
-        except Exception as e:
-            print(e)
+        return self._get_handler(stream).info(stream)
 
-    # -------------------------- PRIVATE METHODS
+    def change_volume(
+        self,
+        stream : Stream,
+        change_db : float
+    ) -> Stream:
+        """
+        Change audio or video information by given scale
+        
+        Args:
+            stream: Inputted stream, of type AudioStream or VideoStream.
+            change_db: Float value representing the decibals by which to change the volume.
+            
+        Returns:
+            The resulting stream as an instance of AudioStream or VideoStream.
+           """
+        return self._get_handler(stream).change_volume(stream, change_db)
+
+    ### Audio Methods
+    def mono_to_stereo(
+        self,
+        left_stream : AudioStream,
+        right_stream : AudioStream
+    ) -> AudioStream:
+        """
+        Converts the given mono stream to stereo.
+
+         Args: 
+            left_stream: AudioStream
+                stores the data of a mono audio file
+            right_stream: AudioStream
+                stores the data of a mono audio file 
+        
+        Returns:
+            the resulting stereo audio stream as an instance of AudioStream.
 
-    def _export_audio(
-            self, audio_segment: AudioSegment,
-        output_dir_path: str, name: str, output_format: str) \
-            -> Tuple[bool, str]:
         """
-        Export the audio stream.
+        return self.audio_h.mono_to_stereo(left_stream, right_stream)
 
-        Args:
-            audio_segment (AudioSegment): Segment to export.
-            output_dir_path (str): Directory path for the output file.
-                                Must be a valid directory path.
-            name (str): File name. Does not include extension.
-            output_format (str): Format of the output file.
-                            Must be a supported output format.
+    def stereo_to_mono(
+        self,
+        stream : AudioStream
+    ) -> List[AudioStream]:
         """
-        try:
-            if not self._is_directory(output_dir_path) or \
-                    not output_format in self.OUTPUT_AUDIO_FORMATS:
-                return False, None
-
-            output_file_path = "{}/{}.{}".format(
-                output_dir_path, name, output_format)
-            audio_segment.export(output_file_path, format=output_format)
-            return True, output_file_path
-        except Exception as e:
-            return False, None
+        Converts the given stereo stream to mono.
 
-    def _initialize_audio_stream_from_file(
-            self, input_file_path, input_format,
-            output_dir_path, output_format) -> AudioStream:
+        Args: 
+            stream: AudioStream 
+                stores the data of a stereo audio file 
+        
+        Returns:
+            a list of two mono audio streams representing the two files.
         """
-        Initializes and returns an AudioStream object by reading from input path.
+        return self.audio_h.stereo_to_mono(stream)
+
+    def concat(self, streams : List[AudioStream]) -> AudioStream:
         """
-        try:
-            audio_segment = AudioSegment.from_file(input_file_path,
-                                                   format=input_format)
-            # Output format defaults to the input format if not specified.
-            if output_format == None:
-                output_format = input_format
-            # The output path defaults to the input path directory if not specified
-            if len(input_file_path) > 0 and \
-                    output_dir_path == None and \
-                    input_file_path.find("/") != -1:
-                output_dir_path = input_file_path[:input_file_path.rfind("/")]
-            stream = AudioStream(
-                input_file_path, input_format, audio_segment, output_dir_path,
-                output_format)
-            return (True, stream)
+        Concatenates the given stream end to end, start to finish, into a single stream.
 
-        except:
-            return (False, None)
+        Args:
+            streams: List of AudioStreams of which to concatenate together
 
-    def _does_file_exist(self, file_path: str) -> bool:
+        Returns:
+            AudioStream representing the concatenated audio.
         """
-        Determines if the file exists.
+        return self.audio_h.concat(streams)
+
+    def overlay(
+        self,
+        left_stream : AudioStream,
+        right_stream : AudioStream,
+        loop_shorter_stream : bool = False
+    ) -> AudioStream:
         """
-        return os.path.exists(file_path) and os.path.isfile(file_path)
+        Overlays two audio streams on top of each other
 
-    def _is_audio_file(self, file_path: str) -> bool:
+        Args:
+            left_stream:AudioStream
+                stores one audio file data that will be overlayed 
+            right_stream:AudioStream
+                stores one audio file data that will be overlayed 
+            loop_shorter_stream: bool
+                if true, the shorter audio file will be looped until it reaches
+                the length of the longer audio file 
+        Returns:
+            AudioStream representing the overlaid audio files.
         """
-        Determine if the file exists and is of a supported audio file format.
+        return self.audio_h.overlay(
+            left_stream, right_stream,loop_shorter_stream
+        )
+
+    def reverse(self, stream : AudioStream) -> AudioStream:
         """
-        return self._does_file_exist(file_path) and \
-            self._get_file_extension(file_path).lower() in \
-            self.INPUT_AUDIO_FORMATS
+        Reverse the given audio stream in place
 
-    def _is_directory(self, dir_path: str) -> bool:
+        Args:
+            stream: AudioStream to reverse
+
+        Returns:
+            AudioStream representing the reversed audio.
         """
-        Determine if path is a directory.
+        return self.audio_h.reverse(stream)
+
+    def chunk(
+        self,
+        stream : AudioStream,
+        chunk_duration_s : float
+    ) -> List[AudioStream]:
         """
-        return os.path.isdir(dir_path)
+        Generates chunks of the given audio with the provided duration.
+
+        Args:
+            stream: AudioStream for which to generate chunks
+            chunk_duration_s: float representing the duration to make each chunk
 
-    def _get_file_extension(self, file_path: str) -> str:
+        Returns:
+            A list of AudioStreams containing each generated chunk
+        """
+        return self.audio_h.chunk(
+            stream, chunk_duration_s
+        )
+
+    ### Video Methods
+    def extract_audio(self, stream : VideoStream) -> AudioStream:
+        raise NotImplementedError
+
+    def remove_audio(self, stream : VideoStream) -> VideoStream:
+        raise NotImplementedError
+
+    def _get_handler(self, stream : Stream) -> Union[AudioHandler, VideoHandler]:
         """
-        Obtain file extension /format, which is the substring after the right-
-        most "." character.
+        Returns the handler of a given stream; either Audio or Video
+        
+        Args:
+            stream for which to generate the handler
+            
+        Returns:
+            AudioHandler or VideoHandler, depending on the type of the given stream. """
+        return self.audio_h if isinstance(stream, AudioStream) else self.video_h
+    
+    @staticmethod
+    def convert_to_16bit_wav(input_path, output_path):
+        return AudioHandler.convert_to_16bit_wav(input_path, output_path)
+
+        
+    @staticmethod 
+    def compress_to_opus(media_path:str, output_dir:str):
+        """ compress the  file stored in media_path to output_dir, 
+            with the same  file name with compressed format
+
+        Args:
+            media_path (str): the path to original file 
+            output_dir (str): the path to the directory where the compressed file 
+                              will be stored
+
+        Raises:
+            ChildProcessError: 
+            ChildProcessError: 
+            ProcessLookupError: 
+
+        Returns:
+            str: the path to the compressed file
         """
-        return os.path.splitext(file_path.strip())[1][1:]
+        return AudioHandler.compress_to_opus(media_path, output_dir)
+    
+    @staticmethod 
+    def chunk_audio_to_outpath(input_path:str, output_path:str, duration:int) -> List[str]:
+        """ given the audio path, chunking the audio into a series of audio
+            segments
+        
+        Args:
+            audiopath[str]: the file path to the audio file 
+            output_path[str]: the output of the chunked file 
+            duration[int]: the length of each chunk
+            
+        Return:
+            Union[List[str], bool]: return a list of the audio path to the 
+                                    chunked audios in order 
+        """
+        return AudioHandler.chunk_audio_to_outpath(input_path, output_path, duration)
+    
+    
+    @staticmethod 
+    def remove_prelude_silence(input_path:str, outdir:str) -> str:
+        ouput_path = os.path.join(outdir, f"{get_name(input_path)}.{get_extension(input_path)}")
+        sound = AudioSegment.from_file(input_path)
+        leading_silence = detect_leading_silence(sound)
+        trim_ed: AudioSegment = sound[leading_silence :]
+        trim_ed.export(ouput_path, "wav")
+        return ouput_path
```

### Comparing `GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_manager.py` & `GailBot-0.1a9/src/gailbot/plugins/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,276 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2021-12-02 13:13:08
-# @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2022-08-23 11:03:32
-# Standard library imports
-from typing import Dict, Any, List, Tuple
-# Local imports
-from .apply_config import ApplyConfig
-from .manager_summary import PluginManagerSummary
-from .plugin_details import PluginDetails
-from .config import PluginConfig
-from .plugin_source import PluginSource
-from .loader import PluginLoader
-from .logic import PluginPipelineLogic
-from .plugin_execution_summary import PluginExecutionSummary
-
-from gailbot.core.pipeline import Pipeline, Stream
-from gailbot.core.io import GailBotIO
+# @Date:   2023-01-08 13:22:01
+# @Last Modified by:   Jason Y. Wu
+# @Last Modified time: 2023-06-28 19:15:39
+from dataclasses import dataclass
+import toml
+import sys
+import os
+from typing import List, Union, Dict
+import validators
+from .suite import PluginSuite, MetaData
+from .loader import (
+    PluginURLLoader,
+    PluginDirectoryLoader,
+    PluginLoader,
+    PluginTOMLLoader,
+)
+from gailbot.core.utils.logger import makelogger
+from gailbot.configs import PLUGIN_CONFIG
+from gailbot.core.utils.general import (
+    make_dir,
+    subdirs_in_dir,
+    delete,
+    get_name,
+    is_directory,
+    filepaths_in_dir,
+)
+from gailbot.configs.interfaces import get_plugin_structure_config
+
+EXPECTED_STRUCTURE = get_plugin_structure_config()
+logger = makelogger("plugin_manager")
+
+
+@dataclass
+class ERROR:
+    INVALID_URL = "The given url is not supported by gailbot"
+    MISSING_CONFIG = "The plugin suite is missing a config.toml file that specifies the plugins dependencies"
+    MISSING_DOC = "The plugin suite is missing a DOCUMENT.md file"
+    MODULE_ERROR = "Fail to load import plugin module"
+    INVALID_INPUT = "The plugin suite source can only be URL, a valid Amazon S3 Bucket name, or path to directory"
+    EXCEEDS_TOML = "The plugin suite has exceeded the maximum number of .toml files. It should only contain a config.toml file that specifies the plugins dependencies."
+    INCORRECT_STRUCTURE = (
+        "The inputted plugin suite does not match the expected structure."
+    )
+
+
+class DuplicatePlugin(Exception):
+    def __str__(self) -> str:
+        return "ERROR: loading existing plugin"
 
 
 class PluginManager:
-
-    def __init__(self) -> None:
-        # Objects
-        self.loader = PluginLoader()
-        self.io = GailBotIO()
-        # Vars.
-        self.config_file_extension = "json"
-        self.pipeline_name = "plugin_pipeline"
-        self.pipeline_num_threads = 3
-
-    ############################ MODIFIERS ##################################
-
-    def register_plugins_from_directory(self, dir_path: str,
-                                        check_subdirectories: bool = True) -> int:
-        """
-        Register a plugin from the specified directory.
-        All configuration files from the directory are used to initialize all
-        plugins.
-
-        Args:
-            dir_path (str): Path to the directory.
-            check_subdirectories (bool):
-                If True, checks all subdirectories for configuration files.
-
-        Returns:
-            (int): Number of plugins loaded from directory.
+    """
+    Manage multiple plugins suites that can be registered, including
+    storing the plugin files, parsing the config files, and instantiating
+    plugin objects from files.
+    """
+
+    def __init__(
+        self, workspace: str, load_existing: bool = True, over_write: bool = True
+    ):
         """
-        if not self.io.is_directory(dir_path):
-            return 0
-        # Load all possible config files
-        _, paths = self.io.path_of_files_in_directory(
-            dir_path, [self.config_file_extension], check_subdirectories)
-        return sum([self.register_plugin_using_config_file(path) for path in paths])
+        Args:
+        workspace (str) : the path to plugin workspace
+        loading_existing: if true, load the existing plugin from plugin workspace
+        over_write: if true, overwrite the existing plugin if plugins_sources
+                    contain plugin that has already been saved in workspace
+        """
+
+        self.workspace = workspace
+        logger.info(f"get workspace {self.workspace}")
+        self._init_workspace()
+
+        self.loaders: List[PluginLoader] = [
+            PluginURLLoader(self.download_dir, self.suites_dir),
+            PluginDirectoryLoader(self.suites_dir),
+        ]
+
+        if load_existing:
+            subdirs = subdirs_in_dir(self.suites_dir, recursive=False)
+            for plugin_source in subdirs:
+                if not self.register_suite(plugin_source):
+                    logger.error(f"{get_name(plugin_source)} cannot be registered")
+        try:
+            self.register_suite(PLUGIN_CONFIG.HILAB_BUCKET)
+        except Exception as e:
+            logger.error(e, exc_info=e)
 
-    def register_plugin_using_config_file(self, config_file_path: str) -> bool:
-        """
-        Register a plugin from a configuration file directly.
+    def get_all_suites_name(self) -> List[str]:
+        """return a list of available plugin suite names"""
+        return set(self.suites.keys())
 
-        Args:
-            config_file_path (str): Path to the configuration file.
+    def is_suite(self, suite_name: str) -> bool:
+        """check if suite name is an available plugin suite"""
+        return suite_name in self.suites
 
-        Returns:
-            (bool): True if successfully loaded. False otherwise.
+    def reset_workspace(self) -> bool:
         """
-        # Generate config object and load
-        _, data = self.io.read(config_file_path)
-        return self.register_plugin_using_config_data(data)
-
-    def register_plugin_using_config_data(self, data: Dict[str, Any]) -> bool:
+        Reset all the plugins that currently exist.
+        They will be permanently deleted and will have to be re-added.
         """
-        Register a plugin using a dictionary representation of PluginConfig.
+        make_dir(self.workspace, overwrite=True)
 
-        Args:
-            data (Dict[str,Any]):
-                Mapping from all keys in PluginConfig to their values.
-
-        Returns:
-            (bool): True if successfully configured. False otherwise.
+    def register_suite(self, plugin_source: str) -> Union[List[str], str]:
+        """
+        Register a plugin suite from the given source, which can be
+        a plugin directory, a url, a conf file, or a dictionary configuration.
         """
+        registered = []
         try:
-            success, config = self._generate_config(data)
-            if not success:
-                return False
-            return self.loader.load_plugin_using_config(config)
+            for loader in self.loaders:
+                suites = loader.load(plugin_source)
+                if suites and isinstance(suites, list):
+                    for suite in suites:
+                        if isinstance(suite, PluginSuite):
+                            self.suites[suite.name] = suite
+                            registered.append(suite.name)
+                    return registered
+            return self.report_registration_err(plugin_source)
         except Exception as e:
-            print(e)
+            logger.error(e, exc_info=e)
+            return self.report_registration_err(plugin_source)
 
-    def apply_plugins(self, apply_configs: Dict[str, ApplyConfig]) \
-            -> PluginManagerSummary:
-        """
-        Apply all plugins defined by the given plugin configs.
-        The plugins must be previously registered.
+    def get_suite(self, suite_name: str) -> PluginSuite:
+        """Given a suite name, return the plugin suite object
 
         Args:
-            apply_configs (Dict[str,ApplyConfig]):
-                Mapping from plugin name to ApplyConfig.
+            suite_name (str): the name that identifies the plugin suite
 
         Returns:
-            (PluginManagerSummary): Summary for executing all plugins.
+            PluginSuite: the plugin suite object identified by suite name
         """
-        did_generate, pipeline = self._generate_execution_pipeline(
-            apply_configs)
-        if not did_generate:
-            return self._generate_summary({}, apply_configs)
-        pipeline.set_base_input(apply_configs)
-        pipeline.execute()
-        return self._generate_summary(
-            pipeline.get_execution_summary(), apply_configs)
-
-    ############################# GETTERS ###################################
+        if not self.is_suite(suite_name):
+            logger.error(f"Suite does not exist {suite_name}")
+            return None
+        return self.suites[suite_name]
+
+    def is_official_suite(self, suite_name) -> bool:
+        if not self.is_suite(suite_name):
+            logger.error(f"Suite does not exist {suite_name}")
+            return None
+        return self.suites[suite_name].is_official
+
+    def get_suite_metadata(self, suite_name: str) -> Dict[str, str]:
+        if not self.is_suite(suite_name):
+            logger.error(f"Suite does not exist {suite_name}")
+            return None
+        return self.suites[suite_name].get_meta_data()
+
+    def get_suite_dependency_graph(self, suite_name: str) -> Dict[str, List[str]]:
+        if not self.is_suite(suite_name):
+            logger.error(f"Suite does not exist {suite_name}")
+            return None
+        return self.suites[suite_name].dependency_graph()
+
+    def get_suite_documentation_path(self, suite_name) -> str:
+        if not self.is_suite(suite_name):
+            logger.error(f"Suite does not exist {suite_name}")
+            return None
+        return self.suites[suite_name].document_path
+
+    def _init_workspace(self):
+        """
+        Init workspace and load plugins from the specified sources.
+        """
+        self.suites_dir = f"{self.workspace}/suites"
+        self.download_dir = f"{self.workspace}/downloads"
+        sys.path.append(self.suites_dir)
+        self.suites: Dict[str, PluginSuite] = dict()
+
+        # Make the directory
+        make_dir(self.workspace, overwrite=False)
+        make_dir(self.suites_dir, overwrite=False)
+        make_dir(self.download_dir, overwrite=True)
 
-    def is_plugin(self, plugin_name: str) -> bool:
+    def delete_suite(self, name: str):
         """
-        Determine if the plugin is available.
-
-        Args:
-            plugin_name (str)
-
-        Returns:
-            (bool): True if the plugin is available. False otherwise.
-        """
-        return self.loader.is_plugin_loaded(plugin_name)
-
-    def get_plugin_names(self) -> List[str]:
+        given a suite name, delete the plugin suite
         """
-        Get the names of all available plugins.
+        try:
+            if self.is_suite(name):
+                delete(os.path.join(self.suites_dir, name))
+                del self.suites[name]
+                return True
+            else:
+                return False
+        except Exception as e:
+            logger.error(e, exc_info=e)
+            return False
 
-        Returns:
-            (List[str])
-        """
-        return self.loader.get_loaded_plugin_names()
+    def get_suite_path(self, name: str) -> str:
+        """given a name of the suite, return the suite path that is internally
+        managed by the suite manager
+        """
+        if self.is_suite(name):
+            path = os.path.join(self.suites_dir, name)
+            if is_directory(path):
+                return path
+            else:
+                del self.suites[name]
+                return None
+        else:
+            return None
 
-    def get_plugin_details(self, plugin_name: str) -> PluginDetails:
-        """
-        Get PluginDetails for the specified plugin if it is available.
+    def report_registration_err(self, suite: str) -> str:
+        """report plugin registration error
 
         Args:
-            plugin_name (str): Name of plugin.
+            suite (str): the path to the suite source
 
         Returns:
-            (PluginDetails)
+            str: a string that report the plugin registration error
         """
-        if not self.is_plugin(plugin_name):
-            return
-        source: PluginSource = self.loader.get_plugin(plugin_name)
-        return PluginDetails(
-            source.plugin_name, source.plugin_dependencies,
-            source.number_of_dependencies, source.plugin_file_path,
-            source.plugin_author, source.plugin_input_type,
-            source.plugin_output_type)
-
-    def get_all_plugin_details(self) -> Dict[str, PluginDetails]:
-        """
-        Get mapping from plugin name to PluginDetails for all available plugins.
-
-        Returns:
-            (Dict[str,PluginDetails])
-        """
-        details = dict()
-        plugin_names = self.loader.get_loaded_plugin_names()
-        for plugin_name in plugin_names:
-            details[plugin_name] = self.get_plugin_details(plugin_name)
-        return details
-
-    ########################### PRIVATE METHODS #############################
-
-    def _generate_config(self, data: Dict[str, Any]) \
-            -> Tuple[bool, PluginConfig]:
         try:
-            config = PluginConfig(
-                data["plugin_name"], data["plugin_dependencies"],
-                data["plugin_file_path"],
-                data["plugin_source_name"], data["plugin_class_name"])
-            return (True, config)
+            if validators.url(suite):
+                if not PluginURLLoader.is_valid_url(suite):
+                    return ERROR.INVALID_URL
+                else:
+                    return ERROR.MODULE_ERROR
+            elif is_directory(suite):
+                tomls = filepaths_in_dir(suite, ["toml"])
+                if len(tomls) == 0 or not tomls:
+                    return ERROR.MISSING_CONFIG
+                elif len(tomls) > 1:
+                    return ERROR.EXCEEDS_TOML
+                elif get_name(tomls[0]) != "config":
+                    return ERROR.MISSING_CONFIG
+                else:
+                    valid = self.validate_plugin_structure(tomls[0], EXPECTED_STRUCTURE)
+                    if valid != True:
+                        return self.validate_plugin_structure(
+                            tomls[0], EXPECTED_STRUCTURE
+                        )
+                mds = filepaths_in_dir(suite, ["md"])
+                if len(mds) == 0 or not mds:
+                    return ERROR.MISSING_DOC
+                return ERROR.MODULE_ERROR
+            else:
+                return ERROR.INVALID_INPUT
         except Exception as e:
-            print(e)
-            return (False, None)
+            logger.error(e, exc_info=e)
 
-    def _generate_execution_pipeline(
-            self, apply_configs: Dict[str, ApplyConfig]) -> Tuple[bool, Pipeline]:
-        """
-        Generate a pipeline given a mapping from plugin name to ApplyConfig.
-        All plugins must be loaded.
-        """
-        pipeline = Pipeline(self.pipeline_name, self.pipeline_num_threads)
-        pipeline.set_logic(PluginPipelineLogic())
-        for plugin_name in apply_configs.keys():
-            if not self._add_plugin_with_dependencies(
-                    pipeline, plugin_name, apply_configs):
-                return (False, None)
-        return (True, pipeline)
-
-    def _add_plugin_with_dependencies(
-            self, pipeline: Pipeline,
-            plugin_name: str, apply_configs: Dict[str, ApplyConfig]) -> bool:
-        """
-        Add a plugin and its required dependencies to the given pipeline using
-        the given ApplyConfig's.
-        All the plugins must be loaded.
-        """
-        # Plugin must be loaded.
-        if not self.loader.is_plugin_loaded(plugin_name) or \
-                not plugin_name in apply_configs:
-            return False
-        # Do not re-load component
-        if plugin_name in pipeline.get_component_names():
-            return True
-        # Load the dependencies
-        plugin_source: PluginSource = self.loader.get_plugin(plugin_name)
-        for dependency in plugin_source.plugin_dependencies:
-            if not self._add_plugin_with_dependencies(
-                    pipeline, dependency, apply_configs):
-                return False
-        # Add actual plugin
-        return pipeline.add_component(
-            plugin_name, plugin_source, plugin_source.plugin_dependencies)
-
-    def _generate_summary(self, execution_summary: Dict[str, Any],
-                          apply_configs: Dict[str, ApplyConfig]) \
-            -> PluginManagerSummary:
+    def validate_plugin_structure(self, user_suite: str, expected: Dict):
         """
-        Generate the summary for executing all plugins in the pipeline.
+        Validates the structure of the inputted plugin suite configuration
 
         Args:
-            execution_summary (Dict[str,Any]):
-                Summary obtained by executing a Pipeline
+            user_suite : str = path to the configuration file for the inputted plugin suite
+            expected : dictionary that stores the expected structure of the configuration file
+
+        Returns:
+            Error message if the plugin suite does not meet the expected format, true if it does
         """
-        try:
-            # Initializing the plugin summaries.
-            total_time_seconds = 0
-            successful_plugins = list()
-            failed_plugins = list()
-            plugin_summaries = dict()
-            # Summary only generated for plugins that were selected.
-            plugin_names = list(apply_configs.keys())
-            for plugin_name in plugin_names:
-                # Means plugin was executed and we can get summary.
-                if plugin_name in execution_summary.keys() and \
-                        execution_summary[plugin_name]["state"] == "successful":
-                    summary = execution_summary[plugin_name]
-                    stream: Stream = summary["result"]
-                    # TODO: This keeps causing issues.
-                    if stream != None:
-                        plugin_summary: PluginExecutionSummary = \
-                            stream.get_stream_data()
-                        plugin_summaries[plugin_name] = plugin_summary
-                        total_time_seconds += plugin_summary.runtime_seconds
-                        if plugin_summary.was_successful:
-                            successful_plugins.append(
-                                plugin_summary.plugin_name)
-                        else:
-                            failed_plugins.append(plugin_summary.plugin_name)
-                # Plugin was not executed.
-                else:
-                    plugin_summaries[plugin_name] = PluginExecutionSummary(
-                        plugin_name, [], {}, None, 0, False)
-                    failed_plugins.append(plugin_name)
-            return PluginManagerSummary(
-                total_time_seconds, successful_plugins, failed_plugins,
-                plugin_summaries)
-        except Exception as e:
-            print(e)
+        expected = toml.load(expected)
+        actual_config = toml.load(user_suite)
+        loader = PluginTOMLLoader()
+        if "suite_name" in actual_config:
+            validated, conf = loader.validate_config(
+                user_suite, actual_config["suite_name"]
+            )
+            if not validated:
+                return conf[0]
+        else:
+            return "Configuration is missing key 'suite_name'"
+        for section, keys in expected.items():
+            if section not in actual_config:
+                return f"{ERROR.INCORRECT_STRUCTURE} Missing section: {section}"
+            if type(keys) != str:
+                for key in keys:
+                    if key not in actual_config[section]:
+                        return f"{ERROR.INCORRECT_STRUCTURE} Missing key: {section}"
+                    if type(keys[key]) != type(actual_config[section].get(key)):
+                        logger.debug("hello")
+                        return f"{ERROR.INCORRECT_STRUCTURE} Type mismatch: {section}.{key}"
+        return True
```

### Comparing `GailBot-0.1a7/gailbot/utils/download.py` & `GailBot-0.1a9/src/gailbot/core/utils/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,76 @@
 # -*- coding: utf-8 -*-
 # @Author: Muhammad Umair
-# @Date:   2022-05-03 11:06:45
+# @Date:   2023-01-12 13:39:44
 # @Last Modified by:   Muhammad Umair
-# @Last Modified time: 2022-05-03 12:39:22
 
 import shutil
 from typing import List
-from tqdm.auto import *
+from tqdm.auto import tqdm
 import requests
 from zipfile import ZipFile
 import os
+import socket
+from .logger import makelogger
 
-# ---- GLOBALS
+logger = makelogger("download")
 
-# NOTE: These are direct download urls to the plugin suites
-URLS = [
-    "https://sites.tufts.edu/hilab/files/2022/05/ca_pkg.zip"]
 
-
-def download_from_urls(urls, download_dir, unzip=True, chunkSize=8192):
+def download_from_urls(
+    urls: List[str], download_dir: str, unzip: bool = True, chunkSize: int = 8192
+) -> List[str]:
+    """
+    Download from a list of urls and return a path to the directory containing
+    the data from each url
+    """
     # Create paths
     dataset_download_path = os.path.join(download_dir, "download")
     dataset_extract_path = download_dir
     if os.path.isdir(dataset_download_path):
         shutil.rmtree(dataset_download_path)
     os.makedirs(dataset_download_path)
     os.makedirs(dataset_extract_path, exist_ok=True)
     # Download each url as a zip file.
     extracted_paths = []
     for i, url in enumerate(urls):
         # Create a temp. dir for this specific url
         name = os.path.splitext(os.path.basename(url))[0]
-        url_temp_path = "{}.zip".format(
-            os.path.join(dataset_download_path, name))
+        url_temp_path = "{}.zip".format(os.path.join(dataset_download_path, name))
         with requests.get(url, stream=True) as r:
             r.raise_for_status()
             pbar = tqdm(
-                total=int(r.headers['Content-Length']), desc="{}".format(name))
+                total=int(r.headers.get("content-length", 0)), desc="{}".format(name)
+            )
             with open(url_temp_path, "wb+") as f:
                 for chunk in r.iter_content(chunk_size=chunkSize):
                     if chunk:  # filter out keep-alive new chunks
                         f.write(chunk)
                         pbar.update(len(chunk))
         if unzip:
-            with ZipFile(url_temp_path, 'r') as zipObj:
+            with ZipFile(url_temp_path, "r") as zipObj:
                 # Extract all the contents of zip file in different directory
                 extract_path = os.path.join(dataset_extract_path, name)
                 extracted_paths.append(extract_path)
                 if os.path.exists(extract_path):
                     shutil.rmtree(extract_path)
                 os.makedirs(extract_path)
                 zipObj.extractall(extract_path)
     # Remove the temp folders
     shutil.rmtree(dataset_download_path)
     return extracted_paths
 
 
-def download_all_plugins(download_dir: str) -> List[str]:
-    return download_from_urls(
-        urls=URLS,
-        download_dir=download_dir,
-        unzip=True)
-
-
-def download_plugin_from_url(url: str, download_dir: str) -> List[str]:
-    return download_from_urls(
-        urls=[url],
-        download_dir=download_dir,
-        unzip=True)
-
-
-# --------- Tests
-
-
-def unittest():
+def is_internet_connected() -> bool:
     """
-    Tests:
-        1. Download and extract from a url.
+    True if connected to the internet, false otherwise
     """
-    urls = [
-        "https://sites.tufts.edu/hilab/files/2022/05/ca_pkg.zip"]
-
-    download_from_urls(
-        urls=urls,
-        download_dir="./test")
-
-
-if __name__ == "__main__":
-    unittest()
+    try:
+        # connect to the host -- tells us if the host is actually
+        # reachable
+        sock = socket.create_connection(("www.google.com", 80))
+        if sock is not None:
+            print("Clossing socket")
+            sock.close
+        return True
+    except OSError:
+        pass
+    return False
```

### Comparing `GailBot-0.1a7/pyproject.toml` & `GailBot-0.1a9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,66 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "GailBot"
+authors = [
+  { name="Muhammad Umair", email="muhammad.umair@tufts.edu" },
+]
 license = {file = "LICENSE"}
-description = "An Automated Transcription System for Conversation Analysis"
+readme = "README.md"
+description = "GailBot API"
 maintainers=[
     {name="Human Interaction Lab - Tufts University", email="hilab-dev@elist.tufts.edu"}
 ]
-requires-python=">=3.8"
-
-dependencies = [
-    "pydub",
-    "sounddevice",
-    "moviepy",
-    "dacite",
-    "networkx",
-    "ibm_watson",
-    "scipy",
-    "syllables",
-    "pyyaml",
-    "lxml"
-]
-
-readme="README.md"
+requires-python=">=3.10"
 classifiers=[
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Topic :: Scientific/Engineering",
     "Operating System :: MacOS",
 ]
 
-dynamic = ["version"]
 
+dynamic = ["dependencies", "version"]
 
 
-[project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "pytest-timeout",
-    "pytest-xdist",
-]
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+version = {attr = "gailbot.__version__"}
+
+[tool.setuptools.packages.find]
+where =["src"]
+
 
 [project.urls]
 homepage = "https://github.com/mumair01/GailBot"
 source = "https://github.com/mumair01/GailBot"
-download = "https://github.com/mumair01/GailBot/releases"
 tracker = "https://github.com/mumair01/GailBot/issues"
 
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages.find]
-where =["."]
 
-[tool.setuptools.dynamic]
-version = {attr = "gailbot.__version__"}
+[project.optional-dependencies]
+dev = [
+    "pytest",
+    "pytest-cov",
+    "pytest-timeout",
+    "pytest-xdist",
+    "ipython"
+]
 
 # pyproject.toml
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra -q"
+addopts = "-rA"
+pythonpath = [
+  "src"
+]
 testpaths = [
     "tests",
 ]
 filterwarnings = [
     "ignore::DeprecationWarning"
 ]
```

