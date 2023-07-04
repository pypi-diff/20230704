# Comparing `tmp/GailBot-0.1a6.dev0.tar.gz` & `tmp/GailBot-0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GailBot-0.1a6.dev0.tar", last modified: Tue Aug 23 18:54:03 2022, max compression
+gzip compressed data, was "GailBot-0.1a7.tar", last modified: Tue Aug 23 19:14:23 2022, max compression
```

## Comparing `GailBot-0.1a6.dev0.tar` & `GailBot-0.1a7.tar`

### file list

```diff
@@ -1,167 +1,96 @@
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.521354 GailBot-0.1a6.dev0/
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.473784 GailBot-0.1a6.dev0/GailBot.egg-info/
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13421 2022-08-23 18:54:03.000000 GailBot-0.1a6.dev0/GailBot.egg-info/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4808 2022-08-23 18:54:03.000000 GailBot-0.1a6.dev0/GailBot.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)        1 2022-08-23 18:54:03.000000 GailBot-0.1a6.dev0/GailBot.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)      135 2022-08-23 18:54:03.000000 GailBot-0.1a6.dev0/GailBot.egg-info/requires.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)       19 2022-08-23 18:54:03.000000 GailBot-0.1a6.dev0/GailBot.egg-info/top_level.txt
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1078 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/LICENSE
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13421 2022-08-23 18:54:03.520850 GailBot-0.1a6.dev0/PKG-INFO
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11324 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/README.md
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.474766 GailBot-0.1a6.dev0/gailbot/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      458 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10680 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/controller.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.475070 GailBot-0.1a6.dev0/gailbot/core/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.475885 GailBot-0.1a6.dev0/gailbot/core/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      330 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2256 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/engine.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1369 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/engines.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.477044 GailBot-0.1a6.dev0/gailbot/core/engines/google/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      228 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/google/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8825 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/google/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3526 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/google/google.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.479491 GailBot-0.1a6.dev0/gailbot/core/engines/watson/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      214 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    12029 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/acoustic_model.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    17536 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/core.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    17514 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/language_model.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    13114 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/recognition_results.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6370 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/recognize_callback.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    26034 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/engines/watson/watson.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.481622 GailBot-0.1a6.dev0/gailbot/core/io/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      204 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    23318 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/audio.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    18783 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/general.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    25569 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/io.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6128 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/shell.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11533 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/io/video.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.483887 GailBot-0.1a6.dev0/gailbot/core/network/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     7626 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/WS_factory.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6587 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/WS_interface.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1810 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/WS_models.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11779 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/WS_protocol.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      184 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4737 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/network.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11452 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/network/request.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.486063 GailBot-0.1a6.dev0/gailbot/core/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      131 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/pipeline/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2948 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/pipeline/component.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3829 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/pipeline/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    16013 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/pipeline/pipeline.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1142 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/core/pipeline/stream.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.486500 GailBot-0.1a6.dev0/gailbot/plugin/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      164 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.491229 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      365 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      427 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/apply_config.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1207 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/config.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3914 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/loader.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3932 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      585 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/manager_summary.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1503 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      396 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_details.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      344 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_execution_summary.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     9994 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      524 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_source.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      279 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/plugins.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.491722 GailBot-0.1a6.dev0/gailbot/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.494271 GailBot-0.1a6.dev0/gailbot/services/objects/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      354 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/objects/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2365 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/objects/gailbot_settings.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2854 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/objects/settings.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3233 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/objects/source.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      406 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/objects/utt.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.495602 GailBot-0.1a6.dev0/gailbot/services/organizer_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      210 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/organizer_service/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    10333 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/organizer_service/organizer_service.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5485 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/organizer_service/source_loader.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.498736 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      263 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4718 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/logic.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5930 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/output_stage.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      901 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/payload.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4108 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/pipeline_service.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5014 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/plugins_stage.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3903 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/services/pipeline_service/transcription_stage.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.501016 GailBot-0.1a6.dev0/gailbot/utils/
--rw-r--r--   0 muhammadumair   (501) staff       (20)       17 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/utils/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2785 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/utils/download.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     2025 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/utils/manager.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1714 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/utils/models.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     5674 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/gailbot/utils/threads.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1447 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/pyproject.toml
--rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2022-08-23 18:54:03.521454 GailBot-0.1a6.dev0/setup.cfg
--rw-r--r--   0 muhammadumair   (501) staff       (20)      230 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/setup.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.501429 GailBot-0.1a6.dev0/tests/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.502184 GailBot-0.1a6.dev0/tests/controller/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/controller/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6309 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/controller/test_controller.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.502966 GailBot-0.1a6.dev0/tests/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/engines/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      342 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/engines/test_engines.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.503709 GailBot-0.1a6.dev0/tests/gailbot_io/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/gailbot_io/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      280 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/gailbot_io/test_gailbot_io.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.504440 GailBot-0.1a6.dev0/tests/network/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/network/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      280 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/network/test_network.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.505326 GailBot-0.1a6.dev0/tests/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/pipeline/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      289 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/pipeline/test_pipeline.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.506131 GailBot-0.1a6.dev0/tests/plugin_manager/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/plugin_manager/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      307 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/plugin_manager/test_plugin_manager.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.507496 GailBot-0.1a6.dev0/tests/services/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/services/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      324 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/services/organizer_service.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      315 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/services/pipeline_service.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.509000 GailBot-0.1a6.dev0/tests/tests_old/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1495 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/conftest.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.509504 GailBot-0.1a6.dev0/tests/tests_old/py_test/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.512467 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4337 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/google_core_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3485 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/google_engine_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)      961 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/watson_am_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     9196 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/watson_core_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6139 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/watson_engine_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6077 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/engines/watson_lm_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.514672 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11552 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/audio_io_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    11839 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/general_io_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    38502 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/io_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1850 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/shell_io_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3903 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/io/video_io_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.515686 GailBot-0.1a6.dev0/tests/tests_old/py_test/network/
--rw-r--r--   0 muhammadumair   (501) staff       (20)     9697 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/network/WSInterface_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/network/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     6801 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/network/network_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     8473 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/network/request_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.516000 GailBot-0.1a6.dev0/tests/tests_old/py_test/organizer_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/organizer_service/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.517016 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1926 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline/component_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)    18312 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline/pipeline_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.517367 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline_service/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/pipeline_service/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.518436 GailBot-0.1a6.dev0/tests/tests_old/py_test/plugin_manager/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/plugin_manager/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1131 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/plugin_manager/loader_test.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     3588 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/plugin_manager/plugin_manager_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.518974 GailBot-0.1a6.dev0/tests/tests_old/py_test/shared_models/
--rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/shared_models/__init__.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.519615 GailBot-0.1a6.dev0/tests/tests_old/py_test/transcription/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      243 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/transcription/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1638 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/py_test/transcription/transcription_test.py
-drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 18:54:03.520414 GailBot-0.1a6.dev0/tests/tests_old/pypi/
--rw-r--r--   0 muhammadumair   (501) staff       (20)      162 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/pypi/__init__.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1626 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/pypi/main.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4986 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/pypi/vardefs.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     1080 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/utils.py
--rw-r--r--   0 muhammadumair   (501) staff       (20)     4992 2022-08-23 18:53:45.000000 GailBot-0.1a6.dev0/tests/tests_old/vardefs.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.765103 GailBot-0.1a7/
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.736847 GailBot-0.1a7/GailBot.egg-info/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13416 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2721 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        1 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      135 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/requires.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       13 2022-08-23 19:14:23.000000 GailBot-0.1a7/GailBot.egg-info/top_level.txt
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1078 2022-08-23 19:13:38.000000 GailBot-0.1a7/LICENSE
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13416 2022-08-23 19:14:23.764765 GailBot-0.1a7/PKG-INFO
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11324 2022-08-23 19:13:38.000000 GailBot-0.1a7/README.md
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.738372 GailBot-0.1a7/gailbot/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      455 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10680 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/controller.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.738846 GailBot-0.1a7/gailbot/core/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.740171 GailBot-0.1a7/gailbot/core/engines/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      330 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2256 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/engine.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1369 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/engines.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.741466 GailBot-0.1a7/gailbot/core/engines/google/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      228 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     8825 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/core.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3526 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/google/google.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.744864 GailBot-0.1a7/gailbot/core/engines/watson/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      214 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    12029 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/acoustic_model.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    17536 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/core.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    17514 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/language_model.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    13114 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/recognition_results.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     6370 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/recognize_callback.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    26034 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/engines/watson/watson.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.747771 GailBot-0.1a7/gailbot/core/io/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      204 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    23318 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/audio.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    18783 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/general.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    25569 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/io.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     6128 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/shell.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11533 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/io/video.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.751164 GailBot-0.1a7/gailbot/core/network/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     7626 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_factory.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     6587 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_interface.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1810 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_models.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11779 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/WS_protocol.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      184 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4737 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/network.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    11452 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/network/request.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.753091 GailBot-0.1a7/gailbot/core/pipeline/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      131 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2948 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/component.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3829 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/logic.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    16013 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/pipeline.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1142 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/core/pipeline/stream.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.753587 GailBot-0.1a7/gailbot/plugin/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      164 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.757888 GailBot-0.1a7/gailbot/plugin/plugin_manager/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      365 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      427 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/apply_config.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1207 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/config.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3914 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/loader.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3932 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/logic.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      585 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/manager_summary.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1503 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      396 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_details.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      344 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_execution_summary.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     9994 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_manager.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      524 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_source.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      279 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/plugins.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.758229 GailBot-0.1a7/gailbot/services/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/__init__.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.760200 GailBot-0.1a7/gailbot/services/objects/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      354 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2365 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/gailbot_settings.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2854 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/settings.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3233 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/source.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      406 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/objects/utt.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.761158 GailBot-0.1a7/gailbot/services/organizer_service/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      210 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)    10333 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/organizer_service.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5485 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/organizer_service/source_loader.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.763127 GailBot-0.1a7/gailbot/services/pipeline_service/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      263 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4718 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/logic.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5930 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/output_stage.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      901 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/payload.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     4108 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/pipeline_service.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5014 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/plugins_stage.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     3903 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/services/pipeline_service/transcription_stage.py
+drwxr-xr-x   0 muhammadumair   (501) staff       (20)        0 2022-08-23 19:14:23.764375 GailBot-0.1a7/gailbot/utils/
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       17 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/__init__.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2785 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/download.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     2025 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/manager.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1714 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/models.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     5674 2022-08-23 19:13:38.000000 GailBot-0.1a7/gailbot/utils/threads.py
+-rw-r--r--   0 muhammadumair   (501) staff       (20)     1447 2022-08-23 19:13:38.000000 GailBot-0.1a7/pyproject.toml
+-rw-r--r--   0 muhammadumair   (501) staff       (20)       38 2022-08-23 19:14:23.765216 GailBot-0.1a7/setup.cfg
+-rw-r--r--   0 muhammadumair   (501) staff       (20)      230 2022-08-23 19:13:38.000000 GailBot-0.1a7/setup.py
```

### Comparing `GailBot-0.1a6.dev0/GailBot.egg-info/PKG-INFO` & `GailBot-0.1a7/GailBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.1a6.dev0
+Version: 0.1a7
 Summary: An Automated Transcription System for Conversation Analysis
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
         Copyright (c) 2022 Human Interaction Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `GailBot-0.1a6.dev0/LICENSE` & `GailBot-0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/PKG-INFO` & `GailBot-0.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.1a6.dev0
+Version: 0.1a7
 Summary: An Automated Transcription System for Conversation Analysis
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
         Copyright (c) 2022 Human Interaction Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `GailBot-0.1a6.dev0/README.md` & `GailBot-0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/controller.py` & `GailBot-0.1a7/gailbot/controller.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/engine.py` & `GailBot-0.1a7/gailbot/core/engines/engine.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/engines.py` & `GailBot-0.1a7/gailbot/core/engines/engines.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/google/core.py` & `GailBot-0.1a7/gailbot/core/engines/google/core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/google/google.py` & `GailBot-0.1a7/gailbot/core/engines/google/google.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/acoustic_model.py` & `GailBot-0.1a7/gailbot/core/engines/watson/acoustic_model.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/core.py` & `GailBot-0.1a7/gailbot/core/engines/watson/core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/language_model.py` & `GailBot-0.1a7/gailbot/core/engines/watson/language_model.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/recognition_results.py` & `GailBot-0.1a7/gailbot/core/engines/watson/recognition_results.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/recognize_callback.py` & `GailBot-0.1a7/gailbot/core/engines/watson/recognize_callback.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/engines/watson/watson.py` & `GailBot-0.1a7/gailbot/core/engines/watson/watson.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/io/audio.py` & `GailBot-0.1a7/gailbot/core/io/audio.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/io/general.py` & `GailBot-0.1a7/gailbot/core/io/general.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/io/io.py` & `GailBot-0.1a7/gailbot/core/io/io.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/io/shell.py` & `GailBot-0.1a7/gailbot/core/io/shell.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/io/video.py` & `GailBot-0.1a7/gailbot/core/io/video.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/WS_factory.py` & `GailBot-0.1a7/gailbot/core/network/WS_factory.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/WS_interface.py` & `GailBot-0.1a7/gailbot/core/network/WS_interface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/WS_models.py` & `GailBot-0.1a7/gailbot/core/network/WS_models.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/WS_protocol.py` & `GailBot-0.1a7/gailbot/core/network/WS_protocol.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/network.py` & `GailBot-0.1a7/gailbot/core/network/network.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/network/request.py` & `GailBot-0.1a7/gailbot/core/network/request.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/pipeline/component.py` & `GailBot-0.1a7/gailbot/core/pipeline/component.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/pipeline/logic.py` & `GailBot-0.1a7/gailbot/core/pipeline/logic.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/pipeline/pipeline.py` & `GailBot-0.1a7/gailbot/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/core/pipeline/stream.py` & `GailBot-0.1a7/gailbot/core/pipeline/stream.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/config.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/config.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/loader.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/loader.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/logic.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/logic.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/manager_summary.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/manager_summary.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_manager.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/plugin/plugin_manager/plugin_source.py` & `GailBot-0.1a7/gailbot/plugin/plugin_manager/plugin_source.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/objects/gailbot_settings.py` & `GailBot-0.1a7/gailbot/services/objects/gailbot_settings.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/objects/settings.py` & `GailBot-0.1a7/gailbot/services/objects/settings.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/objects/source.py` & `GailBot-0.1a7/gailbot/services/objects/source.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/organizer_service/organizer_service.py` & `GailBot-0.1a7/gailbot/services/organizer_service/organizer_service.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/organizer_service/source_loader.py` & `GailBot-0.1a7/gailbot/services/organizer_service/source_loader.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/logic.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/logic.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/output_stage.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/output_stage.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/payload.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/payload.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/pipeline_service.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/plugins_stage.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/plugins_stage.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/services/pipeline_service/transcription_stage.py` & `GailBot-0.1a7/gailbot/services/pipeline_service/transcription_stage.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/utils/download.py` & `GailBot-0.1a7/gailbot/utils/download.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/utils/manager.py` & `GailBot-0.1a7/gailbot/utils/manager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/utils/models.py` & `GailBot-0.1a7/gailbot/utils/models.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/gailbot/utils/threads.py` & `GailBot-0.1a7/gailbot/utils/threads.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.1a6.dev0/pyproject.toml` & `GailBot-0.1a7/pyproject.toml`

 * *Files identical despite different names*

