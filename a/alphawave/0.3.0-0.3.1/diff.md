# Comparing `tmp/alphawave-0.3.0.tar.gz` & `tmp/alphawave-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.0.tar", last modified: Wed Jun 28 02:46:39 2023, max compression
+gzip compressed data, was "alphawave-0.3.1.tar", last modified: Tue Jul  4 18:57:05 2023, max compression
```

## Comparing `alphawave-0.3.0.tar` & `alphawave-0.3.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.277962 alphawave-0.3.0/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.0/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-28 02:46:39.277962 alphawave-0.3.0/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.0/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-28 02:46:30.000000 alphawave-0.3.0/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-28 02:46:39.277962 alphawave-0.3.0/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.269962 alphawave-0.3.0/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.273962 alphawave-0.3.0/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9427 2023-06-27 18:52:28.000000 alphawave-0.3.0/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.0/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.0/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-26 03:01:54.000000 alphawave-0.3.0/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.0/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.3.0/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8940 2023-06-27 16:04:31.000000 alphawave-0.3.0/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.0/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.0/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.0/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.0/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.0/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.3.0/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.0/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.0/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.273962 alphawave-0.3.0/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-28 02:46:39.000000 alphawave-0.3.0/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1758 2023-06-28 02:46:39.000000 alphawave-0.3.0/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-28 02:46:39.000000 alphawave-0.3.0/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-28 02:46:39.000000 alphawave-0.3.0/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-28 02:46:39.000000 alphawave-0.3.0/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.273962 alphawave-0.3.0/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16543 2023-06-28 02:17:08.000000 alphawave-0.3.0/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.3.0/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.3.0/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.3.0/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.0/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.0/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.3.0/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.3.0/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.3.0/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.3.0/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.0/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.0/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.0/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.3.0/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.273962 alphawave-0.3.0/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.0/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7791 2023-06-27 19:17:46.000000 alphawave-0.3.0/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.3.0/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.0/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.0/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    23229 2023-06-27 19:16:18.000000 alphawave-0.3.0/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.0/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.273962 alphawave-0.3.0/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.3.0/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.3.0/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.0/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12703 2023-06-28 02:40:52.000000 alphawave-0.3.0/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.3.0/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-28 02:46:39.277962 alphawave-0.3.0/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.0/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.0/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.3.0/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.1/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-04 18:57:05.394066 alphawave-0.3.1/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.1/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      942 2023-07-04 18:56:52.000000 alphawave-0.3.1/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-04 18:57:05.394066 alphawave-0.3.1/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.390066 alphawave-0.3.1/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10039 2023-07-04 02:40:43.000000 alphawave-0.3.1/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.1/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.1/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8159 2023-07-04 16:10:19.000000 alphawave-0.3.1/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.1/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.3.1/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.1/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.1/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.1/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.1/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.1/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.1/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.1/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.3.1/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.1/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.1/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-04 18:57:05.000000 alphawave-0.3.1/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1797 2023-07-04 18:57:05.000000 alphawave-0.3.1/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-04 18:57:05.000000 alphawave-0.3.1/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-07-04 18:57:05.000000 alphawave-0.3.1/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-04 18:57:05.000000 alphawave-0.3.1/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16350 2023-07-04 18:23:32.000000 alphawave-0.3.1/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1645 2023-07-04 15:32:04.000000 alphawave-0.3.1/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7199 2023-07-04 18:19:22.000000 alphawave-0.3.1/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.1/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.1/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.1/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.1/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1507 2023-07-01 23:27:46.000000 alphawave-0.3.1/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.1/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7943 2023-07-04 16:11:01.000000 alphawave-0.3.1/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.1/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.1/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.1/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2035 2023-07-04 17:32:53.000000 alphawave-0.3.1/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.1/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7792 2023-06-28 22:49:13.000000 alphawave-0.3.1/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.1/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.1/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.1/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    23933 2023-06-29 21:03:58.000000 alphawave-0.3.1/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.1/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.1/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1029 2023-07-03 20:25:17.000000 alphawave-0.3.1/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.1/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.1/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.1/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-04 18:57:05.394066 alphawave-0.3.1/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.1/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.1/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.3.1/tests/testSchema.py
```

### Comparing `alphawave-0.3.0/LICENSE` & `alphawave-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/PKG-INFO` & `alphawave-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.0
-Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
+Version: 0.3.1
+Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `alphawave-0.3.0/README.md` & `alphawave-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/pyproject.toml` & `alphawave-0.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
-description = "AlphaWave - a client for interfacing with Large Language Models (LLM)"
+description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
 
 
 readme = "README.md"
 
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `alphawave-0.3.0/src/alphawave/AlphaWave.py` & `alphawave-0.3.1/src/alphawave/AlphaWave.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     client: PromptCompletionClient = None
     prompt: Prompt = None
     prompt_options: PromptCompletionOptions = None
     memory: PromptMemory = VolatileMemory()
     functions: PromptFunctions = FunctionRegistry()
     history_variable: str = 'history'
     input_variable: str = 'input'
-    max_history_messages: int = 10
-    max_repair_attempts: int = 3
+    max_history_messages: int = 6
+    max_repair_attempts: int =2
     tokenizer: Tokenizer = GPT3Tokenizer()
     validator: DefaultResponseValidator = DefaultResponseValidator()
     logRepairs: bool = False
 
 def update_dataclass(instance, **kwargs):
     for key, value in kwargs.items():
         if hasattr(instance, key):
@@ -55,18 +55,18 @@
         else:
             values.append(None)
     return values
 
 class AlphaWave(AsyncIOEventEmitter):
     def __init__(self, **kwargs):
         super().__init__()
-        self.options = AlphaWaveOptions(
-        )
+        self.options = AlphaWaveOptions()
         update_dataclass(self.options, **kwargs)
         #display_dataclass(self.options)
+        
     async def completePrompt(self, input=None):
         client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, logRepairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'logRepairs'))
 
         if self.options.input_variable:
             if input:
                 memory.set(input_variable, input)
             else:
@@ -75,38 +75,42 @@
             input = ''
 
         try:
             self.emit('beforePrompt', memory, functions, tokenizer, prompt, prompt_options)
             response = await client.completePrompt(memory, functions, tokenizer, prompt, prompt_options)
             self.emit('afterPrompt', memory, functions, tokenizer, prompt, prompt_options, response)
             if response['status'] != 'success':
+                #print(f'***** Alphawave client completePrompt failure {response}')
                 return response
 
             if not isinstance(response['message'], dict):
+                #print(f'***** Alphawave making sure message is a dict with key content')
                 response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
 
             self.emit('beforeValidation', memory, functions, tokenizer, response, max_repair_attempts)
+            #print(f'***** Alphawave before validation ')
             validation = validator.validate_response(memory, functions, tokenizer, response, max_repair_attempts)
             self.emit('afterValidation', memory, functions, tokenizer, response, max_repair_attempts, validation)
             if 'coroutine' in str(type(validation)).lower():
                 validation = await validation
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
-
+                    #print(f"***** Alphawave post validation picking up value {response}\n note response['message']['content'] must exist!")
+        
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
                 return response
 
             if self.options.logRepairs:
                 print(Colorize.title('REPAIRING RESPONSE:'))
                 print(Colorize.output(memory))
             fork = MemoryFork(memory)
-            self.addInputToHistory(fork, history_variable, input)
-            self.addResponseToHistory(fork, history_variable, response['message'])
+            #self.addInputToHistory(fork, history_variable, input)
+            #self.addResponseToHistory(fork, history_variable, response['message'])
 
             if self.options.logRepairs:
                 print(Colorize.output(response['message']['content']))
 
             self.emit('beforeRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
             repair = self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
             if 'coroutine' in str(type(repair)).lower():
@@ -136,16 +140,20 @@
             history.append({'role': 'user', 'content': input})
             if len(history) > self.options.max_history_messages:
                 history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     def addResponseToHistory(self, memory, variable, message):
         if variable:
+            # first check if we have a assistant prompt as last message in history
             history = memory.get(variable) or []
-            history.append(message)
+            if len(history) == 0 or len(history[-1]['content']) > 0:
+                history.append(message)
+            else:
+                history[-1]['content']=message
             if len(history) > self.options.max_history_messages:
                 history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     async def repairResponse(self, fork, functions, tokenizer, response, validation, remaining_attempts):
         client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
 
@@ -192,7 +200,9 @@
                 repair_response['message']['content'] = validation['value']
 
             return repair_response
 
         # Try next attempt
         remaining_attempts -= 1
         return await self.repairResponse(fork, functions, tokenizer, repair_response, validation, remaining_attempts)
+
+
```

### Comparing `alphawave-0.3.0/src/alphawave/Colorize.py` & `alphawave-0.3.1/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.1/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.1/src/alphawave/TOMLResponseValidator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,153 @@
-from jsonschema import validate, ValidationError
+import toml
+from toml import TomlDecodeError
+from cerberus import Validator
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptMemory, Tokenizer
 from alphawave.alphawaveTypes import PromptResponse, Validation, PromptResponseValidator
-from alphawave.Response import Response
 from pyee import AsyncIOEventEmitter
-import json
-import ast
+import sys
 import traceback
 import re
 
-def extract_json_template(schema, p=True):
-    template = {}
-    if schema is not None and "properties" in schema:
-        for key, value in schema["properties"].items():
-            if "type" in value:
-                if value["type"] == "object":
-                    template[key] = extract_json_template(value, p=False)
-                elif value["type"] == "array":
-                    if "items" in value:
-                        template[key] = [extract_json_template(value["items"], p=False)]
-                    else:
-                        template[key] = {}
-                else:
-                    template[key] = '<'+key+'>'
-            elif "$ref" in value:
-                ref = value["$ref"]
-                ref_schema = schema
-                for part in ref.split("/")[1:]:
-                    ref_schema = ref_schema[part]
-                template[key] = extract_json_template(ref_schema, p=False)
-
-    return template
 
-class JSONResponseValidator(PromptResponseValidator):
-    def __init__(self, schema=None, missing_json_feedback='Invalid JSON. return valid JSON.'):
+class TOMLResponseValidator(PromptResponseValidator):
+    def __init__(self, schema=None, missing_toml_feedback="Response was not formatted as expected. "):
         self.schema = schema
-        self.missing_json_feedback = missing_json_feedback
-
-    def parse_dict(self, s):
-        if s is None:
-            return s
-        # Try to parse as JSON
+        self.missing_toml_feedback = missing_toml_feedback
+        self.validator = Validator(schema)
         try:
-            return json.loads(s)
-        except json.JSONDecodeError:
-            pass
+            self.feedback_schema = self.extract_toml_template(schema)
+        except Exception as e:
+            traceback.print_exc()
+        #print(f'***** TOMLResponseValidator feedback {self.feedback_schema}')
         
-        # Try to parse as a Python literal
-        try:
-            return ast.literal_eval(s)
-        except (SyntaxError, ValueError):
-            pass
-
-        # Try to repair common errors and parse again
-        s = s.strip()
-        if not (s.startswith('{') and s.endswith('}')):
-            s = '{' + s + '}'
-        s = re.sub(r'([{,]\s*)(\w+)(\s*:)', r'\1"\2"\3', s)  # add quotes around keys
-        #s = s.replace("'", '"')  # replace single quotes with double quotes
-
-        # Try to parse the repaired string
-        try:
-            y = json.loads(s)
-            return y
-        except json.JSONDecodeError:
+    def find_toml(self, s):
+        if s is None:
             return s
+        # Look for [RESPONSE] ... [STOP]
+
+        s = re.sub('\n+', '\n', s)
+        cleaned_s = ""
+        for char in s:
+            if ord(char) >= 10:
+                cleaned_s += char
+        s = cleaned_s
+        s = s.replace('\\*', '*')
+        s = s.replace('\\+', '+')
+        s = s.replace('\\-', '-')
+        s = s.replace('\\/', '/')
+        s = s.replace('RESPONSE:', '[RESPONSE]')
+        start = s.find('[RESPONSE]')
+        if start < 0:
+            #print(f'***** find_toml no start')
+            return ''
+        end = s[start:].find('[STOP]')
+        if end < 0:
+            end = (s[start+1:]).find('[')
+        if end < 0:
+            #print(f'***** find_toml {start} no end\n{s[start:]}')
+            return s[start:]
+        else:
+            #print(f'***** find_toml {start}, {end}\n{s[start:start+end-1]}')
+            return s[start:start+end-1]
 
+    def extract_toml_template(self,schema, prefix=None):
+        if prefix is None:  ### top level
+            #print(f'\n***** template extract input\n{schema}')
+            template = '[RESPONSE]\n'
+        else:
+            template = ''
+        if schema is not None and type(schema) == dict:
+            for item in schema:
+                value = schema[item]
+                if prefix is None:
+                    key = item
+                else:
+                    key = prefix+"."+item
+                if type(value) == dict:
+                    if 'type' in value and value['type'] == 'dict':
+                        #print(f'\n***** template dict {key},{value}')
+                        # recurse on nested structure
+                        if 'schema' in value:
+                            subtemplate = self.extract_toml_template(value['schema'], key)
+                            template = template+subtemplate
+                        elif 'keysrules' in value:
+                            template = template+key+"={}\n"
+                    elif 'meta' in value:
+                        template = template+key+'="'+value['meta']+'"\n'
+                    elif 'type' in value:
+                        template = template+key+'="'+value['type']+'"\n'
+                else:
+                    template = template+key+'='+value+'\n'
+                    
+        if prefix is None:
+            template += '[STOP]\n'
+        #print(f'\n***** template extract \n{template}')
+        return template
+                
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts: int) -> Validation:
         message = response['message']
         
         text = message if isinstance(message, str) else message.get('content', '')
-
-        # Parse the response text
-        parsed=[]
+        #print(f'***** TOMLResponseValidator raw input type {type(text)}\n{text}\n')
         try:
-            parsed = Response.parse_all_objects(text)
+            toml_extract = self.find_toml(text)
         except Exception as e:
-            raise e
-        if len(parsed) == 0:
-            template = extract_json_template(self.schema)
-            #print(f'***** JSONResponseValidator failure len(parsed) == 0')
+            traceback.print_exc()
+        #print(f'\n***** TOMLResponseValidator toml_extract \n{toml_extract}\n')
+        if toml_extract == '':
+            #print(f'***** TOMLResponseValidator failure no toml', file=sys.stderr)
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': self.missing_json_feedback+f' using this template: {template} '
+                'feedback': self.missing_toml_feedback+f' using this template:\n{self.feedback_schema}'
             }
 
         # Validate the response against the schema
+        errors = None
+        try:
+            response_as_dict = toml.loads(toml_extract)
+            #print(f'\n***** TOMLResponseValidator as_dict \n{response_as_dict}\n')
+        except TomlDecodeError as e:
+            #print(f'***** TOMLResponseValidator TomlDecodeError {str(e)}\n{toml_extract}')
+            return {
+                'type': 'Validation',
+                'valid': False,
+                'feedback': self.missing_toml_feedback+f' e fixes:\n{str(e)}. respond using this format:\n{self.feedback_schema} '
+            }
+
         if self.schema:
-            errors = None
-            for i in range(len(parsed) - 1, -1, -1):
-                obj = parsed[i]
-                try:
-                    try:
-                        obj = self.parse_dict(obj) if type(obj) == str else obj
-                    except Exception as e:
-                        pass
-                    validate(obj, self.schema)
-                    #print(f'***** JSONResponseValidator validation passed!')
+            try:
+                #print(f'***** TOMLResponseValidator validate input against \n{self.schema}')
+                v = Validator(self.schema)
+                validation_result = v.validate(response_as_dict['RESPONSE'])
+                if validation_result:
+                    #print(f'***** TOMLResponseValidator validation passed!')
                     return {
                         'type': 'Validation',
                         'valid': True,
-                        'value': obj
+                        'value': response_as_dict['RESPONSE']
                     }
-                except ValidationError as e:
-                    path = str(list(e.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
-                    if not errors:
-                        errors = e
-                    template = extract_json_template(self.schema)
-                    #print(f'***** JSONResponseValidator ValidationError exception {str(e)}')
+                else:
+                    #print(f'***** TOMLResponseValidator schema validation failed {v._errors}\n{response_as_dict}\n')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}. respond using this template: {template} '
+                        'feedback': self.missing_toml_feedback+f'Apply these fixes:\n{v._errors} response template:\n{self.feedback_schema}\n'
                     }
-                except Exception as e:
-                    template = extract_json_template(self.schema)
-                    #print(f'***** JSONResponseValidator validator generic exception {str(e)}')
-                    return {
-                        'type': 'Validation',
-                        'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}. respond using this template: {template} '
-                    }      
+            except Exception as e:
+                #print(f'***** TOMLResponseValidator validator exception {str(e)}')
+                return {
+                    'type': 'Validation',
+                    'valid': False,
+                    'feedback': self.missing_toml_feedback+f'Repair and respond using this template:\n{self.feedback_schema} '
+                }      
     
         else:
             # Return the last object
-            #print(f'***** JSONResponseValidator exit last object {parsed[-1]}')
+            #print(f'***** TOMLResponseValidator exit last object {response_as_dict}')
             return {
                 'type': 'Validation',
                 'valid': True,
-                'value': parsed[-1]
+                'value': response_as_dict['RESPONSE']
             }
 
-    def get_error_fix(self, error: ValidationError) -> str:
-        # Get argument as a string
-        arg = error.validator
-        path = str(list(error.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
-        
-        switcher = {
-            'type': f'convert "{path}" value to a {error.validator_value}' if len(path)> 0 else '',
-            'anyOf': f'convert "{path}" to one of the allowed types: {error.validator_value}',
-            'additionalProperties': f'remove the "{arg}" field from "{path}"',
-            'required': f"add the {error.validator_value} fields to {path if len(path)>0 else 'response'}",
-            'format': f'change the "{path}" field to be a {error.validator_value}',
-            'uniqueItems': f'remove all duplicate items from "{error.path}"',
-            'enum': f'change the "{path}" value to be one of these values: {arg}',
-            'const': f'change the "{path}" value to be {arg}',
-        }
-
-        return switcher[arg] if arg in switcher else error.message
-
```

### Comparing `alphawave-0.3.0/src/alphawave/MemoryFork.py` & `alphawave-0.3.1/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/OSClient.py` & `alphawave-0.3.1/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/OpenAIClient.py` & `alphawave-0.3.1/src/alphawave/OpenAIClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,13 +150,13 @@
         }
         self.addRequestHeaders(requestHeaders, self.options)
         jsonbody = asdict(body)
         keys = list(jsonbody.keys())
         for key in keys:
             if jsonbody[key] is None:
                 del jsonbody[key]
-        print(jsonbody)
+
         result = self._session.post(url, json=jsonbody, headers=requestHeaders)
         if result.status_code < 300:
             completion = result.json().get('choices')[0]
         return result
```

### Comparing `alphawave-0.3.0/src/alphawave/RepairTestClient.py` & `alphawave-0.3.1/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/Response.py` & `alphawave-0.3.1/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/TestClient.py` & `alphawave-0.3.1/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/TestClientTest.py` & `alphawave-0.3.1/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.1/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/internalTypes.py` & `alphawave-0.3.1/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave/jsonParser.py` & `alphawave-0.3.1/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.1/src/alphawave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.0
-Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
+Version: 0.3.1
+Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `alphawave-0.3.0/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.1/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
 src/alphawave/RepairTestClient.py
 src/alphawave/Response.py
+src/alphawave/TOMLResponseValidator.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/__init__.py
 src/alphawave/alphawaveTypes.py
 src/alphawave/internalTypes.py
 src/alphawave/jsonParser.py
 src/alphawave.egg-info/PKG-INFO
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/Agent.py` & `alphawave-0.3.1/src/alphawave_agents/Agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from alphawave.AlphaWave import AlphaWave, AlphaWaveOptions
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, Validation, PromptResponseValidator
 from alphawave.JSONResponseValidator import JSONResponseValidator
 
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand, CommandSchema
 from alphawave_agents.AgentCommandValidator import AgentCommandValidator
 import promptrix.Utilities
-from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchema
+from alphawave_agents.agentTypes import Command, AgentThought
 from alphawave_agents.AgentCommandSection import AgentCommandSection
 
 from typing import Dict, Any
 from pydantic import BaseModel, Field
 import traceback
 
 class AgentCommandSchema(BaseModel):
@@ -40,25 +40,15 @@
         "input": {
             "type": "string",
             "description": "input for command",
         }
     }
     required: list[str] = ["input"]
 
-PromptInstructionSection = TemplateSection(\
-"""
-Reason step by step how to answer the users query below.
-Return a JSON object with your thoughts and the next command to perform, using the following format and available commands.
-Response Format:
 
-{\"reasoning\":\"<reflections on how to construct an answerto the user query>\",\"plan\":\"concise plan for constructing answer\",\"command\":{\"name\":\"<command name of next action to perform>\",\"input\":{\"<key>\":\"<value>\"}}</s>"
-"""
-                                              , 'system')
-OneShot = [UserMessage('What is 3 + 4?'),
-           AssistantMessage('{"reasoning":"I\' not good at math, I\'ll use the math command", "command":{"name":"math", "input":{"code":3+4"}}')]
 
 @dataclass
 class AgentOptions:
     client: PromptCompletionClient
     context_variable: Optional[str] = None
     prompt: Union[str, list[str], PromptSection] = None
     prompt_options: PromptCompletionOptions = None
@@ -71,15 +61,15 @@
     max_history_messages: Optional[int] = None
     max_repair_attempts: Optional[int] = None
     max_steps: Optional[int] = None
     memory: Optional[PromptMemory] = None
     retry_invalid_responses: Optional[bool] = None
     step_delay: Optional[int] = None
     tokenizer: Optional[Tokenizer] = None
-
+    syntax: Optional[str] = 'JSON'
 
 @dataclass
 class ConfiguredAgentOptions:
     agent_variable: str = None
     client: PromptCompletionClient = None
     context_variable: str = None
     functions: PromptFunctions = None
@@ -92,20 +82,40 @@
     max_steps: int = 5
     memory: PromptMemory = None
     prompt: Union[str, list[str], PromptSection] = None
     prompt_options: PromptCompletionOptions = None
     retry_invalid_responses: bool = False
     step_delay: int = 5
     tokenizer: Tokenizer = None
+    syntax: Optional[str] = 'JSON'
 
-def update_dataclass(instance, **kwargs):
-    for key, value in kwargs.items():
+def update_dataclass(instance, source):
+    for key, value in source.items():
         if key in instance and value is not None:
             instance[key] =  value
 
+##
+PromptInstructionSectionJSON = TemplateSection(\
+"""
+Reason about the user query following these instructions.
+If the answer is available from fact or reasoning, respond with the answer using the finalAnswer command
+Otherwise, reason step by step about the query, the available information, and the set of commands listed earlier, and select a command to perform.
+The ONLY commands available are the commands listed.
+Return a JSON object with your reasoning and the next command to perform, with arguments, using the format shown above for that command
+"""
+                                              , 'system')
+
+PromptInstructionSectionTOML = TemplateSection(\
+"""
+Reason about the user query following these instructions.
+If the answer is available from fact or reasoning, respond with the answer using the finalAnswer command.
+Otherwise, reason step by step about the query, the available information, and the set of commands listed above, and select a command to perform.
+Return your reasoning and the next command to perform, with arguments, using the format provided above for that command.
+"""
+                                              , 'system')
 
 @dataclass
 class AgentCommandInput:
     agentId: str
     input: str
 
 
@@ -134,16 +144,18 @@
             'max_steps': 5,
             'memory': VolatileMemory(),
             'prompt': None,
             'prompt_options': None,
             'retry_invalid_responses': False,
             'step_delay': 5,
             'tokenizer': GPT3Tokenizer(),
+            'syntax': 'JSON'
         }
-        update_dataclass(self._options, **asdict(options))
+        update_dataclass(self._options, options.__dict__)
+        #self._options = self._options.__dict__
         self._events: EventEmitter = AsyncIOEventEmitter()
 
     @property
     def client(self):
         return self._options.client
 
     @property
@@ -183,62 +195,44 @@
     async def completeTask(self, input: Optional[str] = None, agentId: Optional[str] = None, executeInitialThought: bool = False):
       try:
         # Initialize the input to the next step
         stepInput = input if input is not None else self.memory.get(self.options['input_variable'])
         # Dispatch to child agent if needed
         step = 0
         state = self.get_agent_state(agentId)
-        if 'child' in state and state['child'] is not None:
-            childAgent = self.getCommand(state['child'].title)
-            
-            response = await childAgent.completeTask(input, state['child'].agentId)
-            if response.status != 'success':
-                return response
-
-            # Delete child and save state
-            del state.child
-            self.setAgentState(state, agentId)
-
-            # Use agents response as input to the next step
-            # We don't know how many steps the child agent took, so we'll just assume it took one
-            stepInput = response.message
-            step = 1
-            executeInitialThought = False
-
         # Start main task loop
         while step < self.options['max_steps']:
-            # Wait for step delay
-            
-            if step > 0 and self.options['step_delay'] > 0:
+            # Wait for step delay to prevent gpt overrun
+            if step > 0 and self._options['step_delay'] > 0:
                 sys.stdout.flush()
-                await asyncio.sleep(self.options['step_delay']/1000)
-
+                await asyncio.sleep(self._options['step_delay']/1000)
             # Execute next step
+            #print(f'***** Agent completeTask calling execute_next_step {stepInput}')
             result = await self.execute_next_step(stepInput, agentId, executeInitialThought)
-            if isinstance(result, str):
+            if isinstance(result, str): ## weird way to determining valid result!
                 stepInput = result
             else:
                 return result
 
             step += 1
             executeInitialThought = False
-
         # Return too many steps
         return {
             "type": "TaskResponse",
             "status": "too_many_steps",
             "message": "The current task has taken too many steps."
         }
       except Exception as e:
         traceback.print_exc()
         pass
 
     # Agent as Commands
     async def execute(self, input: AgentCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer):
         # Initialize the agents state
+        #print(f'***** Agent execute input {input}')
         agentId = input.agentId
         state = self.get_agent_state(agentId)
         state['context'] = input.input
         self.set_agent_state(state, agentId)
 
         # Start the task
         return await self.completeTask(None, agentId)
@@ -256,50 +250,50 @@
 
     def get_agent_history_variable(self, agentId: Optional[str] = None):
         return f"{self._options['history_variable']}-{agentId}" if agentId else self._options['history_variable']
 
 
     async def execute_next_step(self, input: Optional[str] = None, agent_id: Optional[str] = None, execute_initial_thought: bool = False):
         try:
+            #print(f'***** Agent execute_next_step input {input}')
             state = self.get_agent_state(agent_id)
-
             # Create agents prompt section
             if isinstance(self._options['prompt'], list):
                 agent_prompt = TemplateSection('\n'.join(self._options['prompt']), 'system')
             elif isinstance(self._options['prompt'], dict):
                 agent_prompt = self._options['prompt']
             else:
                 agent_prompt = TemplateSection(self._options['prompt'], 'system')
             
             # Ensure the context variable is set
             if 'context' in state:
                 self.memory.set(self.options['context_variable'], state['context'])
 
             # Create prompt
             history_variable = self.get_agent_history_variable(agent_id)
-            sections = [agent_prompt]
-            sections.append(AgentCommandSection(self._commands))
-            pis = PromptInstructionSection
-            sections.append(pis)
-            if OneShot is not None:
-                prompt = Prompt([
-                    GroupSection(sections, 'system'),
-                    OneShot[0], OneShot[1],
-                    ConversationHistory(history_variable, 1.0, True)
-                ])
-            else:
+            try:
+                sections = [agent_prompt]
+                sections.append(AgentCommandSection(self._commands, one_shot=True, syntax=self._options['syntax']))
+                
+                if self._options['syntax'] == 'JSON':
+                    pis = PromptInstructionSectionJSON
+                else:
+                    pis = PromptInstructionSectionTOML
+                    
+                sections.append(pis)
                 prompt = Prompt([
                     GroupSection(sections, 'system'),
                     ConversationHistory(history_variable, 1.0, True)
                 ])
-            if input:
-                prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
-                # Ensure input variable is set otherwise the history will be wrong.
-                self.memory.set(self.options['input_variable'], input)
-
+                if input:
+                    prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
+                    # Ensure input variable is set otherwise the history will be wrong.
+                    self.memory.set(self.options['input_variable'], input)
+            except Exception as e:
+                tracebak.print_exc()
 
             if execute_initial_thought and self._options['initial_thought']:
                 # Just use initial thought as response
                 # - This is used when agents are being called as commands.
                 response = {
                     'status': 'success',
                     'message': {'role': 'assistant', 'content': self._options['initial_thought']}
@@ -309,17 +303,18 @@
                 if state['totalSteps'] == 0 and self._options['initial_thought']:
                     history = self.memory.get(history_variable) or []
                     message = {'role': 'assistant', 'content': json.dumps(self._options['initial_thought'])}
                     history.append(message)
                     self.memory.set(history_variable, history)
 
                 # Create command validator
-                validator = AgentCommandValidator(self._commands, self._options['prompt_options']['model'])
+                validator = AgentCommandValidator(self._commands, self._options['client'], self._options['prompt_options'].model, self._options['syntax'], memory=self.memory, history_variable=history_variable)
 
                 # Create a wave for the prompt
+                ### this is the ONLY wave call in Agent. 
                 wave = AlphaWave(
                     client = self._options['client'],
                     prompt = prompt,
                     prompt_options = self._options['prompt_options'],
                     functions = self._options['functions'],
                     history_variable = history_variable,
                     input_variable = self._options['input_variable'],
@@ -346,20 +341,23 @@
                         'message': response['message']
                     }
 
             # Get agents thought and execute command
             message = response['message']
             thought = message['content']
             self._events.emit('newThought', thought)
+            #print(f'***** Agent execute_next_step calling execute_command state {state}, thought {thought}')
+
             result = await self.execute_command(state, thought)
 
             # Check for task result and error
             task_response = result if isinstance(result, dict) and result.get('type') == 'TaskResponse' else None
             if task_response:
                 if task_response['status'] in ['error', 'invalid_response', 'rate_limited', 'too_many_steps', 'too_long']:
+                    #print(f'***** Agent execute_next_step fail {task_response}')
                     return task_response
 
             # Update history
             history = self.memory.get(history_variable) or []
             if input:
                 #history.append({'role': 'user', 'content': input})
                 pass
@@ -367,45 +365,30 @@
             self.memory.set(history_variable, history)
 
             # Save the agents state
             state['totalSteps'] += 1
             self.set_agent_state(state, agent_id)
 
             # Return result
-            return task_response if task_response else Utilities.to_string(self.tokenizer, result)
+            return_msg = task_response if task_response else Utilities.to_string(self.tokenizer, result)
+            #print(f'***** Agent execute_next_step returning {return_msg}')
+            return return_msg
         except Exception as err:
+            traceback_printexc()
             return {
                 'type': "TaskResponse",
                 'status': "error",
                 'message': str(err)
             }
 
     async def execute_command(self, state: AgentState, thought: AgentThought):
         # Get command
-        command_name = thought['command']['input']['name'] if thought['command']['name'] == 'character' else thought['command']['name']
+        command_name = thought['command']
         command = self._commands.get(command_name, None) or {}
-        input = thought['command']['input'] or {}
-        if isinstance(command, Agent):
-            # Pass control to child agent
-            agentId = str(uuid4())
-            childAgent = command
-            response = await childAgent.execute(input['input'], self.memory, self.functions, self.tokenizer)
-            if response.status == 'success':
-                # Just return the response message since agent completed without additional input
-                return response.message
-            elif response.status == 'input_needed':
-                # Remember that we're talking to the agent
-                state.child = {
-                    'title': command_name,
-                    'agentId': agentId
-                }
-                return response
-            else:
-                # Return the response since the agent failed
-                return response
-        else:
-            # Execute command and return result
-            response = command.execute(input, self.memory, self.functions, self.tokenizer)
-            if 'coroutine' in str(type(response)).lower():
-                return await response
-            return response
+        input = thought['inputs'] or {}
+        # Execute command and return result
+        #print(f'***** Agent execute_command  {command_name}, {input}')
+        response = command.execute(input, self.memory, self.functions, self.tokenizer)
+        if 'coroutine' in str(type(response)).lower():
+            return await response
+        return response
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.1/src/alphawave_agents/AskCommand.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     properties= {
         'question': {
             'type': "string",
             'description': "question to ask"
         }
     },
     required= ["question"],
-    returns= "users answer"
+    returns= "answer"
 )
 
 
 class AskCommandInput:
     def __init__(self, question: str):
         self.question = question
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.1/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.1/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.1/tests/testSchema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from typing import Dict, Optional
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, asdict, field
-from promptrix.promptrixTypes import PromptMemory, Tokenizer, PromptFunctions
-from alphawave_agents.agentTypes import TaskResponse
-from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
+from promptrix.promptrixTypes import PromptMemory, PromptFunctions, Tokenizer
+from promptrix.Prompt import Prompt
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
-
+from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
+from alphawave_agents.agentTypes import TaskResponse
+from dataclasses import dataclass, asdict
 
 @dataclass
 class CommandSchema(sbcCommandSchema):
-    schema_type: str = "object"
-    title: str = "finalAnswer"
-    description: str = "show answer to the user"
-    properties: dict = field(default_factory=lambda: {
-        "answer": {
-            "type": "string",
-            "description": "final answer"
-        }
-    })
-    required: list[str] = field(default_factory=lambda: ["answer"])
-    returns: str = "a followup task or question"
-
-@dataclass
-class FinalAnswerCommandInput:
-    answer:str
+    schema_type: str
+    title: str
+    description: str
+    properties: Dict[str,Dict[str,str]]
+    required: list[str]
+    returns: str
 
-class FinalAnswerCommand(SchemaBasedCommand):
-    def __init__(self, title: Optional[str] = None, description: Optional[str] = None):
-        super().__init__(CommandSchema(), title, description)
 
-    def execute(self, input: FinalAnswerCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
-        print(f'\nAnswer: \n{input}\n')
-        return {
-            "type": "TaskResponse",
-            "status": "input_needed",
-            "message": "input['answer']"
+schema = CommandSchema(
+    schema_type="object",
+    title= "ask",
+    description= "ask the user a question and wait for their response",
+    properties= {
+        'question': {
+            'type': "string",
+            'description': "question to ask"
         }
+    },
+    required= ["question"],
+    returns= "users answer"
+)
+print('AskCommand',asdict(schema))
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.1/src/alphawave_agents/MathCommand.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,15 @@
     properties: Dict[str,Dict[str,str]]
     required: list[str]
     returns: str
 
 @dataclass
 class MathCommandInput:
     code:str
-"""
-class TaskResponse:
-    def __init__(self, response_type: str, status: str, message: str):
-        self.type = response_type
-        self.status = status
-        self.message = message
-"""
+
 schema = CommandSchema(
     schema_type="object",
     title="math",
     description="execute some python code to calculate a value",
     properties={
         "code": {
             "type": "string",
@@ -41,12 +35,17 @@
 class MathCommand(SchemaBasedCommand):
 
     def __init__(self, title = None, description = None):
         super().__init__(schema, title, description)
 
     def execute(self, input: MathCommandInput, memory: Any, functions: Any, tokenizer: Any) -> Any:
         try:
-            return eval(input['code'])
+            exp = input['code']
+            exp = exp.replace('\\*', '*')
+            exp = exp.replace('\\+', '+')
+            exp = exp.replace('\\-', '-')
+            exp = exp.replace('\\/', '/')
+            return eval(exp)
         except Exception as err:
             message = str(err)
             return asdict(TaskResponse('TaskResponse', 'error', message))
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.1/src/alphawave_agents/PromptCommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         self.client = client
         self.prompt = prompt
         self.prompt_options = options.prompt_options
 
     async def execute(self, input: Dict[str, Any], memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> Union[TaskResponse, str]:
         # Fork memory and copy the input into the fork
         fork = MemoryFork(memory)
+        if type(input) != dict:
+            print (f'***** PromptCommand execute input not dict\n{input}\n')
         for key, value in input.items():
             fork.set(key, value)
 
         # Create a wave and send it
         options = AlphaWaveOptions()
         update_dataclass(options, **self.options.__dict__)
         update_dataclass(options, memory=fork, functions= functions, tokenizer= tokenizer)
```

### Comparing `alphawave-0.3.0/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.1/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.1/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.1/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.1/src/alphawave_pyexts/LLMClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         prime=''
         for msg_idx, msg in enumerate(messages):
             #print(msg_idx, msg)
             role = msg['role']
             ### conv.system is a prompt msg, and will be inserted as the first entry by conv.get_prompt()
             if role.lower() == 'system' and msg_idx==0:
                 if len(conv.system)>0:
-                    prime = msg['content']+' '+conv.system
+                    prime = conv.system+'\n'+msg['content']
                 else:
                     prime = msg['content']
                 if len(conv.roles)>2:
                     conv.append_message(conv.roles[2], prime)
                     prime=''
             elif role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
                 role_index = 0
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.1/src/alphawave_pyexts/SearchCommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,14 @@
                     for item in response:
                         if type(item) == dict and 'url' in item:
                             sc_urls.append(item['url'])
                         if type(item) == dict and 'text' in item:
                             sc_text += '\n'+(item['text'])
                     sc_text = sc_text[:max(len(sc_text)-1, self.max_chars)]
                 if self.return_urls:
-                    return {'status':'success', 'message':{'text': sc_text, 'urls':sc_urls}}
+                    return {'type':'TaskResponse','status':'success', 'message':{'text': sc_text, 'urls':sc_urls}}
                 else:
-                    return {'status':'success', 'message':sc_text}
+                    return {'type':'TaskResponse','status':'success', 'message':sc_text}
                     
         except Exception as err:
             message = str(err)
             return asdict(TaskResponse('TaskResponse', 'error', message))
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/chat.py` & `alphawave-0.3.1/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.1/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.1/src/alphawave_pyexts/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,27 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n\n",
     )
 )
 
+# OpenLLama default template (copy of alpaca_
+register_conv_template(
+    Conversation(
+        name="openllama",
+        system="",
+        roles=("### Instruction", "### Response"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n\n",
+    )
+)
+
 # Dolly V2 default template
 register_conv_template(
     Conversation(
         name="dolly_v2",
         system="",
         roles=("### Instruction", "### Response"),
         messages=(),
@@ -659,14 +672,27 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n",
     )
 )
 
+# Pygmalion template
+register_conv_template(
+    Conversation(
+        name="pygmalion",
+        system="Samanatha's Persona: a young, flirty, chatty women. She loves to hang out  with friends, go to movies, or just snuggle on the sofa. <START>\n",
+        roles=("You", "Samanath"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n",
+    )
+)
+
 # tigerbot template
 register_conv_template(
     Conversation(
         name="tigerbot",
         system="A chat between a curious user and an artificial intelligence assistant. "
         "The assistant gives helpful, detailed, and polite answers to the user's questions.",
         roles=("### Instruction", "### Response"),
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/handler.py` & `alphawave-0.3.1/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.1/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             options = Options()
             options.page_load_strategy = 'eager'
             options.add_argument("--headless")
             result = ''
             with webdriver.Chrome(options=options) as dr:
-                #print(f'*****setting page load timeout {timeout}')
+                #print(f'*****setting page load timeout {timeout} {url}')
                 dr.set_page_load_timeout(timeout)
                 try:
                     dr.get(url)
                     response = dr.page_source
                     result =  await response_text_extract(query_phrase, keywords, keyword_weights, url, response, int(time.time()-start_time),
                                                           client, model, memory, functions, tokenizer, max_chars)
                 except selenium.common.exceptions.TimeoutException:
@@ -90,27 +90,27 @@
                        # no sense starting if not much time left
                        and ((search_level==DEEP_SEARCH and len(full_text) < 9600 and len(in_process) < 8 and time.time() - start_time < 42)
                             or (search_level==NORMAL_SEARCH and len(full_text) < 6400 and len(in_process) < 7 and time.time()-start_time < 36)
                             or (search_level==QUICK_SEARCH  and len(full_text) < 4800 and len(in_process) < 6 and time.time()-start_time < 24))):
                     url = urls[0]
                     urls = urls[1:]
                     # set timeout so we don't wait for a slow site forever
-                    timeout = 12-int(time.time()-start_time)
+                    timeout = 24-int(time.time()-start_time)
                     if search_level==NORMAL_SEARCH:
-                        timeout = timeout+4
+                        timeout = timeout+8
                     future = executor.submit(process_url, query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars)
                     in_process.append(future)
                 # Process the responses as they arrive
                 for future in in_process:
                     if future.done():
                         in_process.remove(future)
                         try:
-                            result, url = await asyncio.wait_for(future.result(), timeout=(max (1, (12-(time.time()-start_time)))))
+                            result, url = await asyncio.wait_for(future.result(), timeout=(max (1, (32-(time.time()-start_time)))))
                         except asyncio.TimeoutError:
-                            print('timeout')
+                            #print(f'timeout ')
                             continue
                         if 'coroutine' in str(type(result)).lower():
                             result = await result
                         if len(result) > 0:
                             site = ut.extract_site(url)
                             domain = ut.extract_domain(url)
                             response.append({'source':ut.extract_domain(url), 'url':url, 'text':result})
@@ -191,44 +191,59 @@
 
 def log_url_process(site, reason, raw_text, extract_text, gpt_text):
     return
 
 
 async def llm_tldr (text, query, client, model, memory, functions, tokenizer, max_chars):
     text = text[:max_chars] # make sure we don't run over token limit
-    prompt = Prompt([UserMessage('Analyze the following Text to identify if there is any content relevant to the query {{$query}}, Respond using this JSON template:\n\n{"relevant": True if there is any text found in the input that is relevant to the query, False otherwise>, "tldr": <relevant content found in Text, rewritten as needed for coherence, or "" if nothing found>}\n\nText:\n\n{{$input}}\n\n. ')])
+    prompt = Prompt([UserMessage('Analyze the following Text to identify if there is any content relevant to the query {{$query}}, Respond using this JSON template:\n\n{"relevant": "Yes" if there is any text found in the input that is relevant to the query, "No" otherwise>, "tldr": "<relevant content found in Text, rewritten coherence>"}\n\nText:\n{{$input}}\n. ')])
     response_text=''
     completion = None
     schema = {
-        'schema_type':'object',
-        'title':'tldr',
-        'description':'extract query-relevant text',
-        'properties':{
-            'relevant': {
-                'type': 'boolean',
-                'description': 'True if there is any text found in the input that is relevant to the query, otherwise False'
+        "schema_type":"object",
+        "title":"tldr",
+        "description":"extract query-relevant text",
+        "properties":{
+            "relevant": {
+                "type": "string",
+                "description": "Yes if any relevant text, otherwise No"
             },
-            'tldr': {
-                'type': 'string',
-                'description': 'relevant extract from Text, or empty string'
+            "tldr": {
+                "type": "string",
+                "description": "relevant extract from Text, or empty string"
             }
         },
-        'required':['relevant', 'tldr'],
-        'returns':"extract"
+        "required":["relevant", "tldr"],
+        "returns":"extract"
     }
     
     options = PromptCompletionOptions(completion_type='chat', model=model)
     # don't clutter primary memory with tldr stuff
     fork = MemoryFork(memory)
     response = await ut.run_wave(client, {'input':text, 'query':query}, prompt, options, fork, functions, tokenizer, validator=JSONResponseValidator(schema))
+    #print(f'\n***** google llm_tldr processing \n{response}')
     if type(response) == dict and 'status' in response and response['status'] == 'success'and 'message' in response:
         message = response['message']
-        if type(message) == dict and 'content' in message and type(message['content']) == dict:
+        if type(message) != dict:
+            try:
+                message = json.loads(message)
+            except Exception as e:
+                if message.find('tldr')> 0:
+                    return message[message.find('tldr'):]
+                else:
+                    return ''
+        if 'content' in message:
             content = message['content']
-            if 'relevant' in content and content['relevant'] == True:
+            if type(content) !=  dict:
+                try:
+                    content = json.loads(content.strip())
+                except Exception as e:
+                    return ''
+            if 'relevant' in content and 'yes' in str(content['relevant']).lower() and 'tldr' in content:
+                #print(f"***** google llm_tldr\n{content['tldr']}\n")
                 return content['tldr']
     return ''
     
 
 async def response_text_extract(query_phrase, keywords, keyword_weights, url, response, get_time, client, model, memory, functions, tokenizer, max_chars):
     curr=time.time()
     extract_text = ''
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.1/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   try:
     #
     fork = MemoryFork(memory)
     query_phrase, keywords = await ut.get_search_phrase_and_keywords(client, query_string, model, fork, functions, tokenizer)
 
     google_text=\
       await gs.search_google(query_string, gs.QUICK_SEARCH, query_phrase, keywords, client, model, fork, functions, tokenizer, max_chars)
+    print(f'***** search_service result {google_text}')
     return google_text
   except:
     traceback.print_exc()
   return ''
 
 if __name__ == '__main__' :
   while True:
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.1/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.1/src/alphawave_pyexts/serverUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       self.stop_strs = stop_strs
       self.tokenizer=tokenizer
       self.prompt_len=len(prompt)
       self.prompt=True
       
       if stop_strs is not None and isinstance(stop_strs, Iterable):
         for stop_wd in stop_strs:
-          print(f'***** stop wd pre encode {stop_wd}')
+          #print(f'***** stop wd pre encode {stop_wd}')
           if stop_wd is not None:
             tokens = tokenizer.encode(stop_wd)
             self.stop_ids.append(tokens)
       print(f'***** stop_id tokens {self.prompt_len}, {self.stop_ids} ')
       
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
       # don't process prompt
@@ -47,15 +47,15 @@
         if len(input_ids[0]) >= len(stop_id):
           if input_ids[0][:-len(stop_id)] == stop_id:
             print(f'***** stopping on token {stop_id}')
             return True
       input_str = self.tokenizer.decode(input_ids[0], skip_special_tokens=True)
       for stop_str in self.stop_strs:
         if len(input_str)>self.prompt_len and stop_str in input_str[self.prompt_len:]:
-          print(f'***** stopping on string {stop_str}, {input_str}')
+          print(f'***** stopping on string {stop_str}, \n{input_str[self.prompt_len:]}')
           return True
       return False
     
 class MyStreamer(TextIteratorStreamer):
   def __init__(self, tokenizer, stop_event=None, skip_prompt=True):
     super(TextIteratorStreamer, self).__init__(tokenizer, skip_prompt)
     self.stop_event = stop_event
```

### Comparing `alphawave-0.3.0/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.1/src/alphawave_pyexts/utilityV2.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,25 +146,30 @@
           'description': 'list of named-entities found'
         }
       },
       'required':['Phrase', 'Keywords', 'NamedEntities'],
       'returns':"query answer"
     }
 
-    options = PromptCompletionOptions(completion_type='chat', model=model)
-    response = await run_wave(client, {'input':query_string}, prompt, options, memory, functions, tokenizer, validator=JSONResponseValidator(schema))
-
-    if type(response) == dict and 'status' in response and response['status'] == 'success':
-        content = response['message']['content']
-        if type(content) == dict:
-            phrase = content['Phrase']
-            keywords = content['Keywords']
-            return phrase, keywords
-    else:
-        return response, []
+    phrase = ''; keywords = []
+    try:
+        options = PromptCompletionOptions(completion_type='chat', model=model)
+        response = await run_wave(client, {'input':query_string}, prompt, options, memory, functions, tokenizer, validator=JSONResponseValidator(schema))
+        
+        if type(response) == dict and 'status' in response and response['status'] == 'success':
+            content = response['message']['content']
+            if type(content) == dict:
+                if 'Phrase' in content:
+                    phrase = content['Phrase']
+                if 'Keywords' in content:
+                    keywords = content['Keywords']
+                return phrase, keywords
+    except Exception as e:
+        traceback.print_exc()
+    return phrase, keywords
 
 
 def reform(elements):
   #reformulates text extracted from a webpage by unstructured.partition_html into larger keyword-rankable chunks
   texts = [] # a list of text_strings, each of at most *max* chars, separated on '\n' when splitting an element is needed
   paragraphs = []
   total_elem_len = 0
```

### Comparing `alphawave-0.3.0/tests/testOSClient.py` & `alphawave-0.3.1/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.0/tests/testOpenAiClient.py` & `alphawave-0.3.1/tests/testOpenAiClient.py`

 * *Files identical despite different names*

