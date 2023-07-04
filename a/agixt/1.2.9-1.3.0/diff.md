# Comparing `tmp/agixt-1.2.9.tar.gz` & `tmp/agixt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.9.tar", last modified: Fri Jun 16 02:42:28 2023, max compression
+gzip compressed data, was "agixt-1.3.0.tar", last modified: Tue Jul  4 09:08:48 2023, max compression
```

## Comparing `agixt-1.2.9.tar` & `agixt-1.3.0.tar`

### file list

```diff
@@ -1,210 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.232481 agixt-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 02:42:18.000000 agixt-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 02:42:18.000000 agixt-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-16 02:42:28.232481 agixt-1.2.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27140 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.204481 agixt-1.2.9/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.212481 agixt-1.2.9/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Smart Task Chain without Research.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Task Chain without Research.json
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate and Run Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate and Run Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.212481 agixt-1.2.9/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/agixt_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Get Task Description.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Title a Chain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/poe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.224481 agixt-1.2.9/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Poe.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 02:42:18.000000 agixt-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 02:42:18.000000 agixt-1.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:42:28.232481 agixt-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-16 02:42:18.000000 agixt-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.232481 agixt-1.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57091 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.393595 agixt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 09:08:37.000000 agixt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 09:08:37.000000 agixt-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-07-04 09:08:48.393595 agixt-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.377595 agixt-1.3.0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/DBConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.377595 agixt-1.3.0/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/Websearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.373595 agixt-1.3.0/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.377595 agixt-1.3.0/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.381595 agixt-1.3.0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/agixt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 09:08:37.000000 agixt-1.3.0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.377595 agixt-1.3.0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-07-04 09:08:48.000000 agixt-1.3.0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-04 09:08:48.000000 agixt-1.3.0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:08:48.000000 agixt-1.3.0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-04 09:08:48.000000 agixt-1.3.0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 09:08:48.000000 agixt-1.3.0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.381595 agixt-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.381595 agixt-1.3.0/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.385595 agixt-1.3.0/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Smart Task Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/2-Concepts/Task Chains.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.389595 agixt-1.3.0/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Custom OpenAI Style Provider.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/Poe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.393595 agixt-1.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-04 09:08:37.000000 agixt-1.3.0/docs/images/db.dbdiagram
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 09:08:37.000000 agixt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-04 09:08:37.000000 agixt-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:08:48.393595 agixt-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-04 09:08:37.000000 agixt-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:08:48.393595 agixt-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-04 09:08:37.000000 agixt-1.3.0/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 09:08:37.000000 agixt-1.3.0/tests/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    45872 2023-07-04 09:08:37.000000 agixt-1.3.0/tests/tests.ipynb
```

### Comparing `agixt-1.2.9/LICENSE` & `agixt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/PKG-INFO` & `agixt-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.9
+Version: 1.3.0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,29 +12,32 @@
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-[![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
+[![Logo](https://josh-xt.github.io/AGiXT/images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quick Start Guide](#quick-start-guide)
+    - [Downloading the docker-compose file](#downloading-the-docker-compose-file)
+    - [Editing the environment file](#editing-the-environment-file)
+    - [Running AGiXT](#running-agixt)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -60,25 +63,49 @@
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quick Start Guide
 
-To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
+To get started quickly, you can use the Docker deployment. You will need [docker and docker-compose](https://docs.docker.com/compose/install/) installed on your system. 
 
-Open a terminal and run the following commands:
+Note: If you run locally without docker, it is unsupported.  Any issues you encounter will be closed without comment. Docker is the only way we can say "it works on my machine" and have it mean anything.
+
+### Downloading the docker-compose file
+Open a terminal and run the following commands to download the docker-compose file and the example environment file:
 
 ```
-git clone https://github.com/Josh-XT/AGiXT
+mkdir AGiXT
 cd AGiXT
-./AGiXT.sh
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/.env.example
+```
+
+### Editing the environment file
+Open the `.env.example` file in a text editor, you will want to at least change the `POSTGRES_PASSWORD` if nothing else.
+
+- `POSTGRES_SERVER` is the name of the database server, this should be `db` if you are using the docker-compose file as-is.
+- `POSTGRES_DB` is the name of the database, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PORT` is the port that the database is listening on, this should be `5432` if you are using the docker-compose file as-is.
+- `POSTGRES_USER` is the username to connect to the database with, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PASSWORD` **is the password to connect to the database with, this should be changed from the example file.**
+- `UVICORN_WORKERS` is the number of workers to run the web server with, this is `6` by default, adjust this to your system's capabilities.
+- `AGIXT_HUB` is the name of the AGiXT hub, this should be `AGiXT/hub` if you want to use the [Open Source AGiXT hub.](https://github.com/AGiXT/hub) If you want to use your own fork of AGiXT hub, change this to your username and the name of your fork.
+- `AGIXT_URI` is the URI of the AGiXT hub, this should be `http://agixt:7437` if you are using the docker-compose file as-is. If hosting the AGiXT server separately, change this to the URI of your AGiXT server, otherwise leave it as-is.
+- `GITHUB_USER` is your GitHub username, this is only required if using your own AGiXT hub to pull your repository data.
+- `GITHUB_TOKEN` is your GitHub personal access token, this is only required if using your own AGiXT hub to pull your repository data.
+
+### Running AGiXT
+Once you have edited the `.env.example` file, save it as `.env` and run the following command to start AGiXT:
+```
+docker-compose up -d
 ```
 
-Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `./AGiXT.sh` again.
+Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `docker-compose up -d` again from the `AGiXT` directory.
 
 - Access the web interface at http://localhost:8501
 - Access the AGiXT API documentation at http://localhost:7437
 
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
```

### Comparing `agixt-1.2.9/agixt/Interactions.py` & `agixt-1.3.0/agixt/Interactions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import re
-import os
 import regex
 import json
 import time
-import spacy
+import logging
 from datetime import datetime
 from Agent import Agent
 from Prompts import Prompts
-from extensions.searxng import searxng
-from Chain import Chain, get_chain_responses_file_path, create_command_suggestion_chain
-from urllib.parse import urlparse
-import logging
+from Embedding import get_tokens
+from Chain import Chain
 from concurrent.futures import Future
+from agixtsdk import AGiXTSDK
+from History import log_interaction
+from Websearch import Websearch
+
+base_uri = "http://localhost:7437"
+ApiClient = AGiXTSDK(base_uri=base_uri)
+chain = Chain()
+cp = Prompts()
 
 
 class Interactions:
     def __init__(self, agent_name: str = ""):
         if agent_name != "":
             self.agent_name = agent_name
             self.agent = Agent(self.agent_name)
             self.agent_commands = self.agent.get_commands_string()
+            self.memories = self.agent.get_memories()
+            searx_instance_url = (
+                self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
+                if "SEARXNG_INSTANCE_URL" in self.agent.PROVIDER_SETTINGS
+                else ""
+            )
+            try:
+                max_tokens = self.agent.PROVIDER_SETTINGS["MAX_TOKENS"]
+            except:
+                max_tokens = 2048
+            self.websearch = Websearch(
+                agent_name=self.agent_name,
+                searx_instance_url=searx_instance_url,
+                max_tokens=max_tokens,
+            )
         else:
             self.agent_name = ""
             self.agent = None
             self.agent_commands = ""
+            self.memories = None
         self.stop_running_event = None
         self.browsed_links = []
         self.failures = 0
-        self.nlp = None
-
-    def load_spacy_model(self):
-        if not self.nlp:
-            try:
-                self.nlp = spacy.load("en_core_web_sm")
-            except:
-                spacy.cli.download("en_core_web_sm")
-                self.nlp = spacy.load("en_core_web_sm")
-        self.nlp.max_length = 99999999999999999999999
 
     def custom_format(self, string, **kwargs):
         if isinstance(string, list):
             string = "".join(str(x) for x in string)
 
         def replace(match):
             key = match.group(1)
@@ -50,98 +61,32 @@
             else:
                 return str(value)
 
         pattern = r"(?<!{){([^{}\n]+)}(?!})"
         result = re.sub(pattern, replace, string)
         return result
 
-    def get_step_response(self, chain_name, step_number):
-        base_path = os.path.join(os.getcwd(), "chains")
-        file_path = os.path.normpath(
-            os.path.join(base_path, chain_name, "responses.json")
-        )
-        if not file_path.startswith(base_path):
-            raise ValueError("Invalid path, chain name must not contain slashes.")
-        try:
-            with open(file_path, "r") as f:
-                responses = json.load(f)
-            return responses.get(str(step_number))
-        except:
-            return ""
-
-    def get_step_content(self, chain_name, prompt_content, user_input, agent_name):
-        new_prompt_content = {}
-        if isinstance(prompt_content, dict):
-            for arg, value in prompt_content.items():
-                if isinstance(value, str):
-                    if "{user_input}" in value:
-                        value = value.replace("{user_input}", user_input)
-                    if "{agent_name}" in value:
-                        value = value.replace("{agent_name}", agent_name)
-                    if "{STEP" in value:
-                        # Count how many times {STEP is in the value
-                        step_count = value.count("{STEP")
-                        for i in range(step_count):
-                            # Get the step number from value between {STEP and }
-                            new_step_number = int(value.split("{STEP")[1].split("}")[0])
-                            # get the response from the step number
-                            step_response = self.get_step_response(
-                                chain_name=chain_name, step_number=new_step_number
-                            )
-                            # replace the {STEPx} with the response
-                            value = value.replace(
-                                f"{{STEP{new_step_number}}}",
-                                f"{step_response['response']}",
-                            )
-                new_prompt_content[arg] = value
-        elif isinstance(prompt_content, str):
-            new_prompt_content = prompt_content
-            if "{user_input}" in prompt_content:
-                new_prompt_content = new_prompt_content.replace(
-                    "{user_input}", user_input
-                )
-            if "{agent_name}" in new_prompt_content:
-                new_prompt_content = new_prompt_content.replace(
-                    "{agent_name}", agent_name
-                )
-            if "{STEP" in prompt_content:
-                step_count = value.count("{STEP")
-                for i in range(step_count):
-                    # Get the step number from value between {STEP and }
-                    new_step_number = int(
-                        prompt_content.split("{STEP")[1].split("}")[0]
-                    )
-                    # get the response from the step number
-                    step_response = self.get_step_response(
-                        chain_name=chain_name, step_number=new_step_number
-                    )
-                    # replace the {STEPx} with the response
-                    new_prompt_content = prompt_content.replace(
-                        f"{{STEP{new_step_number}}}", f"{step_response['response']}"
-                    )
-            if new_prompt_content == {}:
-                new_prompt_content = prompt_content
-        return new_prompt_content
-
     async def format_prompt(
         self,
         user_input: str = "",
         top_results: int = 5,
         prompt="",
         chain_name="",
         step_number=0,
         memories=None,
         **kwargs,
     ):
-        cp = Prompts()
         if prompt == "":
             prompt = user_input
         else:
             try:
-                prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
+                prompt = cp.get_prompt(
+                    prompt_name=prompt,
+                    prompt_category=self.agent.AGENT_CONFIG["settings"]["AI_MODEL"],
+                )
             except:
                 prompt = prompt
         if top_results == 0:
             context = "None"
         else:
             try:
                 context = await memories.context_agent(
@@ -151,78 +96,103 @@
                 context = "None."
         command_list = self.agent.get_commands_string()
         if chain_name != "":
             try:
                 for arg, value in kwargs.items():
                     if "{STEP" in value:
                         # get the response from the step number
-                        step_response = self.get_step_response(
+                        step_response = chain.get_step_response(
                             chain_name=chain_name, step_number=step_number
                         )
                         # replace the {STEPx} with the response
                         value = value.replace(f"{{STEP{step_number}}}", step_response)
                         kwargs[arg] = value
             except:
                 logging.info("No args to replace.")
             if "{STEP" in prompt:
-                step_response = self.get_step_response(
+                step_response = chain.get_step_response(
                     chain_name=chain_name, step_number=step_number
                 )
                 prompt = prompt.replace(f"{{STEP{step_number}}}", step_response)
             if "{STEP" in user_input:
-                step_response = self.get_step_response(
+                step_response = chain.get_step_response(
                     chain_name=chain_name, step_number=step_number
                 )
                 user_input = user_input.replace(f"{{STEP{step_number}}}", step_response)
+        try:
+            working_directory = self.agent.AGENT_CONFIG["settings"]["WORKING_DIRECTORY"]
+        except:
+            working_directory = "./WORKSPACE"
+        if "helper_agent_name" not in kwargs:
+            if "helper_agent_name" in self.agent.AGENT_CONFIG["settings"]:
+                helper_agent_name = self.agent.AGENT_CONFIG["settings"][
+                    "helper_agent_name"
+                ]
+            else:
+                helper_agent_name = self.agent_name
         formatted_prompt = self.custom_format(
             string=prompt,
             user_input=user_input,
             agent_name=self.agent_name,
             COMMANDS=self.agent_commands,
             context=context,
             command_list=command_list,
             date=datetime.now().strftime("%B %d, %Y %I:%M %p"),
+            working_directory=working_directory,
+            helper_agent_name=helper_agent_name,
             **kwargs,
         )
 
-        if not self.nlp:
-            self.load_spacy_model()
-        tokens = len(self.nlp(formatted_prompt))
+        tokens = get_tokens(formatted_prompt)
         logging.info(f"FORMATTED PROMPT: {formatted_prompt}")
         return formatted_prompt, prompt, tokens
 
     async def run(
         self,
         user_input: str = "",
         prompt: str = "",
         context_results: int = 5,
         websearch: bool = False,
         websearch_depth: int = 3,
         learn_file: str = "",
         chain_name: str = "",
         step_number: int = 0,
         shots: int = 1,
+        disable_memory: bool = False,
         **kwargs,
     ):
-        memories = self.agent.get_memories()
+        shots = int(shots)
         if learn_file != "":
-            learning_file = await memories.mem_read_file(file_path=learn_file)
+            try:
+                learning_file = ApiClient.learn_file(file_path=learn_file)
+            except:
+                return "Failed to read file."
             if learning_file == False:
                 return "Failed to read file."
+        if websearch:
+            if user_input == "":
+                if "primary_objective" in kwargs and "task" in kwargs:
+                    search_string = f"Primary Objective: {kwargs['primary_objective']}\n\nTask: {kwargs['task']}"
+                else:
+                    search_string = ""
+            else:
+                search_string = user_input
+            if search_string != "":
+                await self.websearch.websearch_agent(
+                    user_input=search_string, depth=websearch_depth
+                )
         formatted_prompt, unformatted_prompt, tokens = await self.format_prompt(
             user_input=user_input,
             top_results=context_results,
             prompt=prompt,
             chain_name=chain_name,
             step_number=step_number,
-            memories=memories,
+            memories=self.memories,
             **kwargs,
         )
-        if websearch:
-            await self.websearch_agent(user_input=user_input, depth=websearch_depth)
         try:
             # Workaround for non-threaded providers
             run_response = await self.agent.instruct(formatted_prompt, tokens=tokens)
             self.response = (
                 run_response.result()
                 if isinstance(run_response, Future)
                 else run_response
@@ -236,32 +206,42 @@
                 self.failures == 0
                 logging.info("Failed to get a response 5 times in a row.")
                 return None
             logging.info(f"Retrying in 10 seconds...")
             time.sleep(10)
             if context_results > 0:
                 context_results = context_results - 1
-            self.response = await self.run(
-                user_input=user_input,
-                prompt=prompt,
-                context_results=context_results,
-                **kwargs,
+            self.response = ApiClient.prompt_agent(
+                agent_name=self.agent_name,
+                prompt_name=prompt,
+                prompt_args={
+                    "chain_name": chain_name,
+                    "step_number": step_number,
+                    "shots": shots,
+                    "disable_memory": disable_memory,
+                    "user_input": user_input,
+                    "context_results": context_results,
+                    **kwargs,
+                },
             )
 
         # Handle commands if the prompt contains the {COMMANDS} placeholder
         # We handle command injection that DOESN'T allow command execution by using {command_list} in the prompt
         if "{COMMANDS}" in unformatted_prompt:
             execution_response = await self.execution_agent(
                 execution_response=self.response,
                 user_input=user_input,
                 context_results=context_results,
                 **kwargs,
             )
             return_response = ""
-            if bool(self.agent.AUTONOMOUS_EXECUTION) == True:
+            if (
+                bool(self.agent.AGENT_CONFIG["settings"]["AUTONOMOUS_EXECUTION"])
+                == True
+            ):
                 try:
                     self.response = json.loads(self.response)
                     if "response" in self.response:
                         return_response = self.response["response"]
                     if "commands" in self.response:
                         if self.response["commands"] != {}:
                             return_response += (
@@ -274,235 +254,66 @@
                 except:
                     return_response = self.response
             else:
                 return_response = f"{self.response}\n\n{execution_response}"
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
-            try:
-                await memories.store_result(input=user_input, result=self.response)
-            except:
-                pass
-            if prompt == "Chat":
-                self.agent.log_interaction(role="USER", message=user_input)
+            if disable_memory == False:
+                try:
+                    await self.memories.store_result(
+                        input=user_input, result=self.response
+                    )
+                except:
+                    pass
+            if user_input != "":
+                log_interaction(
+                    agent_name=self.agent_name,
+                    conversation_name=f"{self.agent_name} History",
+                    role="USER",
+                    message=user_input,
+                )
             else:
-                self.agent.log_interaction(role="USER", message=formatted_prompt)
-            self.agent.log_interaction(role=self.agent_name, message=self.response)
+                log_interaction(
+                    agent_name=self.agent_name,
+                    conversation_name=f"{self.agent_name} History",
+                    role="USER",
+                    message=formatted_prompt,
+                )
+            log_interaction(
+                agent_name=self.agent_name,
+                conversation_name=f"{self.agent_name} History",
+                role=self.agent_name,
+                message=self.response,
+            )
 
-        if int(shots) > 1:
+        if shots > 1:
             responses = [self.response]
             for shot in range(shots - 1):
-                shot_response = await self.run(
-                    user_input=user_input,
-                    prompt=prompt,
-                    context_results=context_results,
-                    shots=shots - 1,
-                    chain_name=chain_name,
-                    step_number=step_number,
-                    **kwargs,
+                shot_response = ApiClient.prompt_agent(
+                    agent_name=self.agent_name,
+                    prompt_name=prompt,
+                    prompt_args={
+                        "chain_name": chain_name,
+                        "step_number": step_number,
+                        "user_input": user_input,
+                        "context_results": context_results,
+                        **kwargs,
+                    },
                 )
                 time.sleep(1)
                 responses.append(shot_response)
             return "\n".join(
                 [
                     f"Response {shot + 1}:\n{response}"
                     for shot, response in enumerate(responses)
                 ]
             )
         return self.response
 
-    async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
-        logging.info(step)
-        if step:
-            if "prompt_type" in step:
-                self.agent_name = step["agent_name"]
-                self.agent = Agent(self.agent_name)
-                self.agent_commands = self.agent.get_commands_string()
-                prompt_type = step["prompt_type"]
-                step_number = step["step"]
-                if "prompt_name" in step["prompt"]:
-                    prompt_name = step["prompt"]["prompt_name"]
-                else:
-                    prompt_name = ""
-                args = self.get_step_content(
-                    chain_name=chain_name,
-                    prompt_content=step["prompt"],
-                    user_input=user_input,
-                    agent_name=self.agent_name,
-                )
-                if prompt_type == "Command":
-                    return await self.agent.execute(
-                        command_name=args["command_name"],
-                        command_args=args,
-                    )
-                elif prompt_type == "Prompt":
-                    result = await self.run(
-                        user_input=user_input,
-                        prompt=prompt_name,
-                        chain_name=chain_name,
-                        step_number=step_number,
-                        **args,
-                    )
-                elif prompt_type == "Chain":
-                    result = await self.run_chain(
-                        chain_name=args["chain"],
-                        user_input=args["input"],
-                        all_responses=False,
-                    )
-        if result:
-            return result
-        else:
-            return None
-
-    async def run_chain(self, chain_name, user_input=None, all_responses=True):
-        chain = Chain()
-        file_path = get_chain_responses_file_path(chain_name=chain_name)
-        chain_data = chain.get_chain(chain_name=chain_name)
-        if chain_data == {}:
-            return f"Chain `{chain_name}` not found."
-        logging.info(f"Running chain '{chain_name}'")
-        responses = {}  # Create a dictionary to hold responses.
-        last_response = ""
-        for step_data in chain_data["steps"]:
-            if "prompt" in step_data and "step" in step_data:
-                logging.info(f"Running step {step_data['step']}")
-                step = {}
-                step_response = await self.run_chain_step(
-                    step=step_data, chain_name=chain_name, user_input=user_input
-                )  # Get the response of the current step.
-                step["response"] = step_response
-                step["agent_name"] = step_data["agent_name"]
-                step["prompt"] = step_data["prompt"]
-                step["prompt_type"] = step_data["prompt_type"]
-                last_response = step_response
-                responses[step_data["step"]] = step  # Store the response.
-                logging.info(f"Response: {step_response}")
-                # Write the responses to the json file.
-                dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-                with open(file_path, "w") as f:
-                    json.dump(responses, f)
-        if all_responses == True:
-            return responses
-        else:
-            # Return only the last response in the chain.
-            return last_response
-
-    async def smart_instruct(
-        self,
-        user_input: str = "Write a tweet about AI.",
-        shots: int = 3,
-        learn_file: str = "",
-        objective: str = None,
-        **kwargs,
-    ):
-        answers = []
-        # Do multi shots of prompt to get N different answers to be validated
-        answers.append(
-            await self.run(
-                user_input=user_input,
-                prompt="SmartInstruct-StepByStep"
-                if objective == None
-                else "SmartTask-StepByStep",
-                context_results=6,
-                websearch=True,
-                websearch_depth=3,
-                shots=shots,
-                learn_file=learn_file,
-                objective=objective,
-                **kwargs,
-            )
-        )
-        if shots > 1:
-            for i in range(shots - 1):
-                answers.append(
-                    await self.run(
-                        user_input=user_input,
-                        prompt="SmartInstruct-StepByStep"
-                        if objective == None
-                        else "SmartTask-StepByStep",
-                        context_results=6,
-                        shots=shots,
-                        objective=objective,
-                        **kwargs,
-                    )
-                )
-        answer_str = ""
-        for i, answer in enumerate(answers):
-            answer_str += f"Answer {i + 1}:\n{answer}\n\n"
-        researcher = await self.run(
-            user_input=answer_str,
-            prompt="SmartInstruct-Researcher",
-            shots=shots,
-            **kwargs,
-        )
-        resolver = await self.run(
-            user_input=researcher,
-            prompt="SmartInstruct-Resolver",
-            shots=shots,
-            **kwargs,
-        )
-        execution_response = await self.run(
-            user_input=f"{user_input}\nContext:\n{resolver}",
-            prompt="instruct",
-            **kwargs,
-        )
-        response = f"{resolver}\n\n{execution_response}"
-        return response
-
-    async def smart_chat(
-        self,
-        user_input: str = "Write a tweet about AI.",
-        shots: int = 3,
-        learn_file: str = "",
-        **kwargs,
-    ):
-        answers = []
-        answers.append(
-            await self.run(
-                user_input=user_input,
-                prompt="SmartChat-StepByStep",
-                context_results=6,
-                websearch=True,
-                websearch_depth=3,
-                shots=shots,
-                learn_file=learn_file,
-                **kwargs,
-            )
-        )
-        # Do multi shots of prompt to get N different answers to be validated
-        if shots > 1:
-            for i in range(shots - 1):
-                answers.append(
-                    await self.run(
-                        user_input=user_input,
-                        prompt="SmartChat-StepByStep",
-                        context_results=6,
-                        shots=shots,
-                        **kwargs,
-                    )
-                )
-        answer_str = ""
-        for i, answer in enumerate(answers):
-            answer_str += f"Answer {i + 1}:\n{answer}\n\n"
-        researcher = await self.run(
-            user_input=answer_str,
-            prompt="SmartChat-Researcher",
-            context_results=6,
-            shots=shots,
-            **kwargs,
-        )
-        resolver = await self.run(
-            user_input=researcher,
-            prompt="SmartChat-Resolver",
-            context_results=6,
-            shots=shots,
-            **kwargs,
-        )
-        return resolver
-
     # Worker Sub-Agents
     async def validation_agent(
         self, user_input, execution_response, context_results, **kwargs
     ):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
             cleaned_json = pattern.findall(execution_response)
@@ -516,24 +327,52 @@
             logging.info("INVALID JSON RESPONSE")
             logging.info(execution_response)
             logging.info("... Trying again.")
             if context_results != 0:
                 context_results = context_results - 1
             else:
                 context_results = 0
-            execution_response = await self.run(
-                user_input=user_input, context_results=context_results, **kwargs
+            execution_response = ApiClient.prompt_agent(
+                agent_name=self.agent_name,
+                prompt_name="JSONFormatter",
+                prompt_args={
+                    "user_input": user_input,
+                    "context_results": context_results,
+                    **kwargs,
+                },
             )
             return await self.validation_agent(
                 user_input=user_input,
                 execution_response=execution_response,
                 context_results=context_results,
                 **kwargs,
             )
 
+    def create_command_suggestion_chain(self, agent_name, command_name, command_args):
+        chains = ApiClient.get_chains()
+        chain_name = f"{agent_name} Command Suggestions"
+        if chain_name in chains:
+            step = (
+                int(ApiClient.get_chain(chain_name=chain_name)["steps"][-1]["step"]) + 1
+            )
+        else:
+            ApiClient.add_chain(chain_name=chain_name)
+            step = 1
+        ApiClient.add_step(
+            chain_name=chain_name,
+            agent_name=agent_name,
+            step_number=step,
+            prompt_type="Command",
+            prompt={
+                "command_name": command_name,
+                **command_args,
+            },
+        )
+        return f"The command has been added to a chain called '{agent_name} Command Suggestions' for you to review and execute manually."
+
     async def execution_agent(
         self, execution_response, user_input, context_results, **kwargs
     ):
         validated_response = await self.validation_agent(
             user_input=user_input,
             execution_response=execution_response,
             context_results=context_results,
@@ -549,29 +388,34 @@
                             try:
                                 if bool(self.agent.AUTONOMOUS_EXECUTION) == True:
                                     command_output = await self.agent.execute(
                                         command_name=command_name,
                                         command_args=command_args,
                                     )
                                 else:
-                                    command_output = create_command_suggestion_chain(
-                                        agent_name=self.agent_name,
-                                        command_name=command_name,
-                                        command_args=command_args,
+                                    command_output = (
+                                        self.create_command_suggestion_chain(
+                                            agent_name=self.agent_name,
+                                            command_name=command_name,
+                                            command_args=command_args,
+                                        )
                                     )
                             except Exception as e:
                                 logging.info("Command validation failed, retrying...")
-                                validate_command = await self.run(
-                                    user_input=user_input,
-                                    prompt="ValidationFailed",
-                                    command_name=command_name,
-                                    command_args=command_args,
-                                    command_output=e,
-                                    context_results=context_results,
-                                    **kwargs,
+                                validate_command = ApiClient.prompt_agent(
+                                    agent_name=self.agent_name,
+                                    prompt_name="ValidationFailed",
+                                    prompt_args={
+                                        "command_name": command_name,
+                                        "command_args": command_args,
+                                        "command_output": e,
+                                        "user_input": user_input,
+                                        "context_results": context_results,
+                                        **kwargs,
+                                    },
                                 )
                                 return await self.execution_agent(
                                     execution_response=validate_command,
                                     user_input=user_input,
                                     context_results=context_results,
                                     **kwargs,
                                 )
@@ -583,79 +427,7 @@
                 else:
                     if command_name == "None.":
                         return "\nNo commands were executed.\n"
                     else:
                         return f"\Command not recognized: `{command_name}`."
         else:
             return "\nNo commands were executed.\n"
-
-    async def websearch_agent(
-        self,
-        user_input: str = "What are the latest breakthroughs in AI?",
-        depth: int = 3,
-    ):
-        memories = self.agent.get_memories()
-
-        async def resursive_browsing(user_input, links):
-            try:
-                words = links.split()
-                links = [
-                    word for word in words if urlparse(word).scheme in ["http", "https"]
-                ]
-            except:
-                links = links
-            if links is not None:
-                for link in links:
-                    if "href" in link:
-                        try:
-                            url = link["href"]
-                        except:
-                            url = link
-                    else:
-                        url = link
-                    url = re.sub(r"^.*?(http)", r"http", url)
-                    # Check if url is an actual url
-                    if url.startswith("http"):
-                        logging.info(f"Scraping: {url}")
-                        if url not in self.browsed_links:
-                            self.browsed_links.append(url)
-                            (
-                                collected_data,
-                                link_list,
-                            ) = await memories.read_website(url)
-                            if link_list is not None:
-                                if len(link_list) > 0:
-                                    if len(link_list) > 5:
-                                        link_list = link_list[:3]
-                                    try:
-                                        pick_a_link = await self.run(
-                                            user_input=user_input,
-                                            prompt="Pick-a-Link",
-                                            links=link_list,
-                                        )
-                                        if not pick_a_link.startswith("None"):
-                                            await resursive_browsing(
-                                                user_input, pick_a_link
-                                            )
-                                    except:
-                                        logging.info(
-                                            f"Issues reading {url}. Moving on..."
-                                        )
-
-        results = await self.run(user_input=user_input, prompt="WebSearch")
-        results = results.split("\n")
-        for result in results:
-            search_string = result.lstrip("0123456789. ")
-            try:
-                searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
-            except:
-                searx_server = ""
-            try:
-                links = await searxng(SEARXNG_INSTANCE_URL=searx_server).search(
-                    search_string
-                )
-                if len(links) > depth:
-                    links = links[:depth]
-            except:
-                links = None
-            if links is not None:
-                await resursive_browsing(user_input, links)
```

### Comparing `agixt-1.2.9/agixt/Memories.py` & `agixt-1.3.0/agixt/Memories.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List
-import spacy
 import os
 from hashlib import sha256
-from Embedding import Embedding
+from Embedding import Embedding, get_tokens, nlp
 from datetime import datetime
 from collections import Counter
 import pandas as pd
 import docx2txt
 import pdfplumber
 from playwright.async_api import async_playwright
 from semantic_kernel.connectors.memory.chroma import ChromaMemoryStore
@@ -23,35 +22,25 @@
 
 class Memories:
     def __init__(self, agent_name: str = "AGiXT", agent_config=None):
         self.agent_name = agent_name
         self.agent_config = agent_config
         self.chroma_client = None
         self.collection = None
-        self.nlp = None
         self.chunk_size = 128
         memories_dir = os.path.join(os.getcwd(), "agents", self.agent_name, "memories")
         self.chroma_client = ChromaMemoryStore(
             persist_directory=memories_dir,
             client_settings=Settings(
                 chroma_db_impl="chromadb.db.duckdb.PersistentDuckDB",
                 persist_directory=memories_dir,
                 anonymized_telemetry=False,
             ),
         )
 
-    def load_spacy_model(self):
-        if not self.nlp:
-            try:
-                self.nlp = spacy.load("en_core_web_sm")
-            except:
-                spacy.cli.download("en_core_web_sm")
-                self.nlp = spacy.load("en_core_web_sm")
-        self.nlp.max_length = 99999999999999999999999
-
     async def get_embedder(self):
         embedder, chunk_size = await Embedding(
             AGENT_CONFIG=self.agent_config
         ).get_embedder()
         return embedder, chunk_size
 
     async def get_collection(self):
@@ -70,51 +59,43 @@
                 memories = await self.chroma_client.get_collection_async(
                     collection_name="memories"
                 )
             return memories
         except Exception as e:
             raise RuntimeError(f"Unable to initialize chroma client: {e}")
 
-    async def store_memory(
-        self, content: str, description: str = None, external_source_name: str = None
-    ):
-        embedder, chunk_size = await self.get_embedder()
-        collection = await self.get_collection()
-        record = MemoryRecord(
-            is_reference=False,
-            id=sha256((content + datetime.now().isoformat()).encode()).hexdigest(),
-            text=content,
-            timestamp=datetime.now().isoformat(),
-            description=description,
-            external_source_name=external_source_name,  # URL or File path
-            embedding=await embedder(content),
-        )
-
-        try:
-            await self.chroma_client.upsert_async(
-                collection_name="memories",
-                record=record,
-            )
-            self.chroma_client._client.persist()
-        except Exception as e:
-            logging.info(f"Failed to store memory: {e}")
-
     async def store_result(
         self, input: str, result: str, external_source_name: str = None
     ):
         if result:
+            embedder, chunk_size = await self.get_embedder()
+            collection = await self.get_collection()
             if not isinstance(result, str):
                 result = str(result)
-            chunks = await self.chunk_content(result, input)
+            chunks = await self.chunk_content(content=result, chunk_size=chunk_size)
             for chunk in chunks:
-                await self.store_memory(
-                    content=chunk,
+                record = MemoryRecord(
+                    is_reference=False,
+                    id=sha256(
+                        (chunk + datetime.now().isoformat()).encode()
+                    ).hexdigest(),
+                    text=chunk,
+                    timestamp=datetime.now().isoformat(),
                     description=input,
-                    external_source_name=external_source_name,
+                    external_source_name=external_source_name,  # URL or File path
+                    embedding=await embedder(chunk),
+                    additional_metadata=chunk,
                 )
+                try:
+                    await self.chroma_client.upsert_async(
+                        collection_name="memories",
+                        record=record,
+                    )
+                except Exception as e:
+                    logging.info(f"Failed to store memory: {e}")
 
     async def context_agent(self, query: str, top_results_num: int) -> List[str]:
         embedder, chunk_size = await self.get_embedder()
         collection = await self.get_collection()
         if collection == None:
             return []
         results = await self.chroma_client.get_nearest_matches_async(
@@ -122,63 +103,47 @@
             embedding=await embedder(query),
             limit=top_results_num,
             min_relevance_score=0.1,
         )
         context = []
         for memory, score in results:
             context.append(memory._text)
-        trimmed_context = await self.trim_context(context)
-        logging.info(f"CONTEXT: {trimmed_context}")
-        context_str = "\n".join(trimmed_context)
-        response = f"Context: {context_str}\n\n"
-        return response
-
-    async def trim_context(self, context: List[str]) -> List[str]:
-        embedder, chunk_size = await self.get_embedder()
-        if not self.nlp:
-            self.load_spacy_model()
         trimmed_context = []
         total_tokens = 0
         for item in context:
-            item_tokens = len(self.nlp(item))
+            item_tokens = get_tokens(item)
             if total_tokens + item_tokens <= chunk_size:
                 trimmed_context.append(item)
                 total_tokens += item_tokens
             else:
                 break
-        return trimmed_context
-
-    def get_keywords(self, query: str):
-        """Extract keywords from a query using Spacy's part-of-speech tagging."""
-        if not self.nlp:
-            self.load_spacy_model()
-        doc = self.nlp(query)
-        keywords = [
-            token.text for token in doc if token.pos_ in {"NOUN", "PROPN", "VERB"}
-        ]
-        return set(keywords)
+        logging.info(f"Context Injected: {trimmed_context}")
+        context_str = "\n".join(trimmed_context)
+        response = (
+            f"The user's input causes you remember these things:\n {context_str} \n\n"
+        )
+        return response
 
     def score_chunk(self, chunk: str, keywords: set):
         """Score a chunk based on the number of query keywords it contains."""
         chunk_counter = Counter(chunk.split())
         score = sum(chunk_counter[keyword] for keyword in keywords)
         return score
 
     async def chunk_content(
-        self, content: str, query: str, overlap: int = 2
+        self, content: str, chunk_size: int, overlap: int = 2
     ) -> List[str]:
-        embedder, chunk_size = await self.get_embedder()
-        if not self.nlp:
-            self.load_spacy_model()
-        doc = self.nlp(content)
+        doc = nlp(content)
         sentences = list(doc.sents)
         content_chunks = []
         chunk = []
         chunk_len = 0
-        keywords = self.get_keywords(query)
+        keywords = [
+            token.text for token in doc if token.pos_ in {"NOUN", "PROPN", "VERB"}
+        ]
 
         for i, sentence in enumerate(sentences):
             sentence_tokens = len(sentence)
             if chunk_len + sentence_tokens > chunk_size and chunk:
                 chunk_text = " ".join(token.text for token in chunk)
                 content_chunks.append(
                     (self.score_chunk(chunk_text, keywords), chunk_text)
@@ -192,15 +157,15 @@
             chunk_text = " ".join(token.text for token in chunk)
             content_chunks.append((self.score_chunk(chunk_text, keywords), chunk_text))
 
         # Sort the chunks by their score in descending order before returning them
         content_chunks.sort(key=lambda x: x[0], reverse=True)
         return [chunk_text for score, chunk_text in content_chunks]
 
-    async def mem_read_file(self, file_path: str):
+    async def read_file(self, file_path: str):
         base_path = os.path.join(os.getcwd(), "WORKSPACE")
         file_path = os.path.normpath(os.path.join(base_path, file_path))
         if not file_path.startswith(base_path):
             raise Exception("Path given not allowed")
         try:
             # If file extension is pdf, convert to text
             if file_path.endswith(".pdf"):
@@ -213,15 +178,17 @@
             elif file_path.endswith(".doc") or file_path.endswith(".docx"):
                 content = docx2txt.process(file_path)
             # TODO: If file is an image, classify it in text.
             # Otherwise just read the file
             else:
                 with open(file_path, "r") as f:
                     content = f.read()
-            await self.store_result(input=file_path, result=content)
+            await self.store_result(
+                input=file_path, result=content, external_source_name=file_path
+            )
             return True
         except:
             return False
 
     async def read_website(self, url):
         try:
             async with async_playwright() as p:
@@ -240,11 +207,13 @@
                     link_list.append((title, href))
 
                 await browser.close()
                 soup = BeautifulSoup(content, "html.parser")
                 text_content = soup.get_text()
                 text_content = " ".join(text_content.split())
                 if text_content:
-                    await self.store_result(input=url, result=text_content)
+                    await self.store_result(
+                        input=url, result=text_content, external_source_name=url
+                    )
                 return text_content, link_list
         except:
             return None, None
```

### Comparing `agixt-1.2.9/agixt/app.py` & `agixt-1.3.0/agixt/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,54 @@
 import uvicorn
+import os
+import logging
+import base64
+import string
+import random
+import time
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
+from DBConnection import DBConnection
+
+db = DBConnection()
+try:
+    db.engine.execute("SELECT 1 FROM agent LIMIT 1")
+    migrated = True
+except Exception as e:
+    migrated = False
+    # Check if migration.txt exists
+    if os.path.exists("migration.txt"):
+        while os.path.exists("migration.txt"):
+            time.sleep(2)
+    else:
+        # Create migration.txt
+        with open("migration.txt", "w") as f:
+            f.write("1")
+        from Hub import import_agixt_hub
+
+        import_agixt_hub()
+        os.remove("migration.txt")
+
+if migrated == True:
+    from Hub import import_agixt_hub
+
+    import_agixt_hub()
+
 from Interactions import Interactions
 from Agent import Agent, add_agent, delete_agent, rename_agent, get_agents
 from Chain import Chain
 from Prompts import Prompts
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options, get_providers
-from Embedding import get_embedding_providers
+from Embedding import get_embedding_providers, get_tokens
 from Extensions import Extensions
-import os
-import logging
-import base64
+from History import get_conversation, delete_history, delete_message
+
+os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
     version = f.read().strip()
 
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO"),
@@ -44,20 +76,16 @@
 
 
 class AgentNewName(BaseModel):
     new_name: str
 
 
 class AgentPrompt(BaseModel):
-    user_input: str
     prompt_name: str
     prompt_args: dict
-    websearch: bool
-    websearch_depth: int
-    context_results: int
 
 
 class Objective(BaseModel):
     objective: str
 
 
 class Prompt(BaseModel):
@@ -68,22 +96,54 @@
     prompt_name: str
 
 
 class PromptList(BaseModel):
     prompts: List[str]
 
 
+class Completions(BaseModel):
+    # Everything in this class except prompt, n, and model (agent_name) are unused currently.
+    prompt: str
+    max_tokens: int = 100
+    temperature: float = 0.9
+    top_p: float = 1.0
+    n: int = 1
+    stream: bool = False
+    logprobs: int = None
+    stop: List[str] = None
+    presence_penalty: float = 0.0
+    frequency_penalty: float = 0.0
+    best_of: int = 1
+    echo: bool = False
+    user: str = None
+    model: str = None  # Model is actually the agent_name
+    stop_sequence: List[str] = None
+    metadata: Dict[str, str] = None
+
+
 class ChainNewName(BaseModel):
     new_name: str
 
 
 class ChainName(BaseModel):
     chain_name: str
 
 
+class ChainData(BaseModel):
+    chain_name: str
+    steps: Dict[str, Any]
+
+
+class RunChain(BaseModel):
+    prompt: str
+    agent_override: Optional[str] = ""
+    all_responses: Optional[bool] = False
+    from_step: Optional[int] = 1
+
+
 class StepInfo(BaseModel):
     step_number: int
     agent_name: str
     prompt_type: str
     prompt: dict
 
 
@@ -135,14 +195,20 @@
 
 
 class AgentSettings(BaseModel):
     agent_name: str
     settings: Dict[str, Any]
 
 
+class AgentConfig(BaseModel):
+    agent_name: str
+    settings: Dict[str, Any]
+    commands: Dict[str, Any]
+
+
 class AgentCommands(BaseModel):
     agent_name: str
     commands: Dict[str, Any]
 
 
 @app.get("/api/provider", tags=["Provider"])
 async def getproviders():
@@ -163,14 +229,23 @@
 
 
 @app.post("/api/agent", tags=["Agent"])
 async def addagent(agent: AgentSettings) -> Dict[str, str]:
     return add_agent(agent_name=agent.agent_name, provider_settings=agent.settings)
 
 
+@app.post("/api/agent/import", tags=["Agent"])
+async def import_agent(agent: AgentConfig) -> Dict[str, str]:
+    return add_agent(
+        agent_name=agent.agent_name,
+        provider_settings=agent.settings,
+        commands=agent.commands,
+    )
+
+
 @app.patch("/api/agent/{agent_name}", tags=["Agent"])
 async def renameagent(agent_name: str, new_name: AgentNewName) -> ResponseMessage:
     rename_agent(agent_name=agent_name, new_name=new_name.new_name)
     return ResponseMessage(message="Agent renamed.")
 
 
 @app.put("/api/agent/{agent_name}", tags=["Agent"])
@@ -192,15 +267,15 @@
     if not file_path.startswith(base_path):
         raise Exception("Path given not allowed")
     file_content = base64.b64decode(file.file_content)
     with open(file_path, "wb") as f:
         f.write(file_content)
     try:
         memories = Agent(agent_name=agent_name).get_memories()
-        await memories.mem_read_file(file_path=file_path)
+        await memories.read_file(file_path=file_path)
         try:
             os.remove(file_path)
         except Exception:
             pass
         return ResponseMessage(message="Agent learned the content from the file.")
     except Exception as e:
         try:
@@ -246,110 +321,176 @@
 async def get_agentconfig(agent_name: str):
     agent_config = Agent(agent_name=agent_name).get_agent_config()
     return {"agent": agent_config}
 
 
 @app.get("/api/{agent_name}/chat", tags=["Agent"])
 async def get_chat_history(agent_name: str):
-    chat_history = Agent(agent_name=agent_name).get_history()
+    chat_history = get_conversation(agent_name=agent_name)
+    if chat_history is None:
+        chat_history = []
+    if "interactions" in chat_history:
+        chat_history = chat_history["interactions"]
     return {"chat_history": chat_history}
 
 
 @app.delete("/api/agent/{agent_name}/history", tags=["Agent"])
-async def delete_history(agent_name: str) -> ResponseMessage:
-    Agent(agent_name=agent_name).delete_history()
+async def delete_conversation_history(agent_name: str) -> ResponseMessage:
+    delete_history(agent_name=agent_name, conversation_name=f"{agent_name} History")
     return ResponseMessage(message=f"History for agent {agent_name} deleted.")
 
 
 @app.delete("/api/agent/{agent_name}/history/message", tags=["Agent"])
 async def delete_history_message(
     agent_name: str, message: ResponseMessage
 ) -> ResponseMessage:
-    Agent(agent_name=agent_name).delete_history_message(message.message)
+    delete_message(
+        agent_name=agent_name,
+        message=message.message,
+        conversation_name=f"{agent_name} History",
+    )
     return ResponseMessage(message=f"Message deleted.")
 
 
 @app.delete("/api/agent/{agent_name}/memory", tags=["Agent"])
 async def wipe_agent_memories(agent_name: str) -> ResponseMessage:
     Agent(agent_name=agent_name).wipe_agent_memories()
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
-@app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
-async def instruct(agent_name: str, prompt: Prompt):
-    agent = Interactions(agent_name=agent_name)
-    response = await agent.run(
-        user_input=prompt.prompt,
-        prompt="instruct",
-    )
-    return {"response": str(response)}
-
-
 @app.post("/api/agent/{agent_name}/prompt", tags=["Agent"])
 async def prompt_agent(agent_name: str, agent_prompt: AgentPrompt):
     agent = Interactions(agent_name=agent_name)
     response = await agent.run(
         prompt=agent_prompt.prompt_name,
-        websearch=agent_prompt.websearch,
-        websearch_depth=agent_prompt.websearch_depth,
-        context_results=agent_prompt.context_results,
         **agent_prompt.prompt_args,
     )
     return {"response": str(response)}
 
 
-@app.post("/api/agent/{agent_name}/smartinstruct/{shots}", tags=["Agent"])
-async def smartinstruct(agent_name: str, shots: int, prompt: Prompt):
-    agent = Interactions(agent_name=agent_name)
-    response = await agent.smart_instruct(user_input=prompt.prompt, shots=int(shots))
-    return {"response": str(response)}
-
-
-@app.post("/api/agent/{agent_name}/chat", tags=["Agent"])
-async def chat(agent_name: str, prompt: Prompt):
-    agent = Interactions(agent_name=agent_name)
+@app.post("/api/v1/completions", tags=["Agent"])
+async def completion(prompt: Completions):
+    # prompt.model is the agent name
+    agent = Interactions(agent_name=prompt.model)
+    agent_config = Agent(agent_name=prompt.model).get_agent_config()
+    if "settings" in agent_config:
+        if "AI_MODEL" in agent_config["settings"]:
+            model = agent_config["settings"]["AI_MODEL"]
+        else:
+            model = "undefined"
+    else:
+        model = "undefined"
     response = await agent.run(
-        user_input=prompt.prompt, prompt="Chat", context_results=6
+        user_input=prompt.prompt,
+        prompt="Custom Input",
+        context_results=3,
+        shots=prompt.n,
     )
-    return {"response": str(response)}
+    characters = string.ascii_letters + string.digits
+    prompt_tokens = get_tokens(prompt.prompt)
+    completion_tokens = get_tokens(response)
+    total_tokens = int(prompt_tokens) + int(completion_tokens)
+    random_chars = "".join(random.choice(characters) for _ in range(15))
+    res_model = {
+        "id": f"cmpl-{random_chars}",
+        "object": "text_completion",
+        "created": int(time.time()),
+        "model": model,
+        "choices": [
+            {
+                "text": response,
+                "index": 0,
+                "logprobs": None,
+                "finish_reason": "stop",
+            }
+        ],
+        "usage": {
+            "prompt_tokens": prompt_tokens,
+            "completion_tokens": completion_tokens,
+            "total_tokens": total_tokens,
+        },
+    }
+    return res_model
 
 
-@app.post("/api/agent/{agent_name}/smartchat/{shots}", tags=["Agent"])
-async def smartchat(agent_name: str, shots: int, prompt: Prompt):
-    agent = Interactions(agent_name=agent_name)
-    response = await agent.smart_chat(user_input=prompt.prompt, shots=shots)
-    return {"response": str(response)}
+@app.post("/api/v1/chat/completions", tags=["Agent"])
+async def chat_completion(prompt: Completions):
+    # prompt.model is the agent name
+    agent = Interactions(agent_name=prompt.model)
+    agent_config = Agent(agent_name=prompt.model).get_agent_config()
+    if "settings" in agent_config:
+        if "AI_MODEL" in agent_config["settings"]:
+            model = agent_config["settings"]["AI_MODEL"]
+        else:
+            model = "undefined"
+    else:
+        model = "undefined"
+    response = await agent.run(
+        user_input=prompt.prompt,
+        prompt="Custom Input",
+        context_results=3,
+        shots=prompt.n,
+    )
+    characters = string.ascii_letters + string.digits
+    prompt_tokens = get_tokens(prompt.prompt)
+    completion_tokens = get_tokens(response)
+    total_tokens = int(prompt_tokens) + int(completion_tokens)
+    random_chars = "".join(random.choice(characters) for _ in range(15))
+    res_model = {
+        "id": f"chatcmpl-{random_chars}",
+        "object": "chat.completion",
+        "created": int(time.time()),
+        "model": model,
+        "choices": [
+            {
+                "index": 0,
+                "message": [
+                    {
+                        "role": "assistant",
+                        "content": response,
+                    },
+                ],
+                "finish_reason": "stop",
+            }
+        ],
+        "usage": {
+            "prompt_tokens": prompt_tokens,
+            "completion_tokens": completion_tokens,
+            "total_tokens": total_tokens,
+        },
+    }
+    return res_model
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
     agent = Agent(agent_name=agent_name)
-    return {"commands": agent.agent_config["commands"]}
+    return {"commands": agent.AGENT_CONFIG["commands"]}
 
 
 @app.patch("/api/agent/{agent_name}/command", tags=["Agent"])
 async def toggle_command(
     agent_name: str, payload: ToggleCommandPayload
 ) -> ResponseMessage:
     agent = Agent(agent_name=agent_name)
     try:
         if payload.command_name == "*":
-            for each_command_name in agent.agent_config["commands"]:
-                agent.agent_config["commands"][each_command_name] = payload.enable
+            for each_command_name in agent.AGENT_CONFIG["commands"]:
+                agent.AGENT_CONFIG["commands"][each_command_name] = payload.enable
 
             agent.update_agent_config(
-                new_config=agent.agent_config["commands"], config_key="commands"
+                new_config=agent.AGENT_CONFIG["commands"], config_key="commands"
             )
             return ResponseMessage(
                 message=f"All commands enabled for agent '{agent_name}'."
             )
         else:
-            agent.agent_config["commands"][payload.command_name] = payload.enable
+            agent.AGENT_CONFIG["commands"][payload.command_name] = payload.enable
             agent.update_agent_config(
-                new_config=agent.agent_config["commands"], config_key="commands"
+                new_config=agent.AGENT_CONFIG["commands"], config_key="commands"
             )
             return ResponseMessage(
                 message=f"Command '{payload.command_name}' toggled for agent '{agent_name}'."
             )
     except Exception as e:
         logging.info(e)
         raise HTTPException(
@@ -362,44 +503,55 @@
 async def get_chains():
     chains = Chain().get_chains()
     return chains
 
 
 @app.get("/api/chain/{chain_name}", tags=["Chain"])
 async def get_chain(chain_name: str):
-    try:
-        chain_data = Chain().get_chain(chain_name=chain_name)
-        return {"chain": chain_data}
-    except:
-        raise HTTPException(status_code=404, detail="Chain not found")
+    # try:
+    chain_data = Chain().get_chain(chain_name=chain_name)
+    return {"chain": chain_data}
+    # except:
+    #    raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.get("/api/chain/{chain_name}/responses", tags=["Chain"])
 async def get_chain_responses(chain_name: str):
     try:
         chain_data = Chain().get_step_response(chain_name=chain_name, step_number="all")
         return {"chain": chain_data}
     except:
         raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
-async def run_chain(chain_name: str, user_input: Prompt):
-    chain_response = await Interactions(agent_name="").run_chain(
-        chain_name=chain_name, user_input=user_input.prompt
+async def run_chain(chain_name: str, user_input: RunChain):
+    chain_response = await Chain().run_chain(
+        chain_name=chain_name,
+        user_input=user_input.prompt,
+        agent_override=user_input.agent_override,
+        all_responses=user_input.all_responses,
+        from_step=user_input.from_step,
     )
     return chain_response
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
     Chain().add_chain(chain_name=chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
 
 
+@app.post("/api/chain/import", tags=["Chain"])
+async def importchain(chain: ChainData) -> ResponseMessage:
+    print(chain)
+    response = Chain().import_chain(chain_name=chain.chain_name, steps=chain.steps)
+    return ResponseMessage(message=response)
+
+
 @app.put("/api/chain/{chain_name}", tags=["Chain"])
 async def rename_chain(chain_name: str, new_name: ChainNewName) -> ResponseMessage:
     Chain().rename_chain(chain_name=chain_name, new_name=new_name.new_name)
     return ResponseMessage(
         message=f"Chain '{chain_name}' renamed to '{new_name.new_name}'."
     )
 
@@ -498,15 +650,17 @@
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' updated.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.get("/api/prompt/{prompt_name}/args", tags=["Prompt"])
 async def get_prompt_arg(prompt_name: str):
-    return {"prompt_args": Prompts().get_prompt_args(prompt_name)}
+    prompt_name = prompt_name.replace("%20", " ")
+    prompt = Prompts().get_prompt(prompt_name=prompt_name)
+    return {"prompt_args": Prompts().get_prompt_args(prompt)}
 
 
 @app.get("/api/extensions/settings", tags=["Extensions"])
 async def get_extension_settings():
     try:
         return {"extension_settings": Extensions().get_extension_settings()}
     except Exception:
@@ -516,12 +670,13 @@
 @app.get("/api/extensions/{command_name}/args", tags=["Extension"])
 async def get_command_args(command_name: str):
     return {"command_args": Extensions().get_command_args(command_name=command_name)}
 
 
 @app.get("/api/extensions", tags=["Extension"])
 async def get_extensions():
-    return {"extensions": Extensions().get_extensions()}
+    extensions = Extensions().get_extensions()
+    return {"extensions": extensions}
 
 
 if __name__ == "__main__":
     uvicorn.run(app, host="0.0.0.0", port=7437)
```

### Comparing `agixt-1.2.9/agixt/provider/azure.py` & `agixt-1.3.0/agixt/provider/azure.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         openai.api_type = "azure"
         openai.api_base = AZURE_OPENAI_ENDPOINT
         openai.api_version = "2023-05-15"
         openai.api_key = AZURE_API_KEY
         self.requirements = ["openai"]
         self.DEPLOYMENT_ID = DEPLOYMENT_ID
         self.AZURE_API_KEY = AZURE_API_KEY
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.AI_TOP_P = AI_TOP_P
-        self.MAX_TOKENS = MAX_TOKENS
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "gpt-35-turbo"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.AI_TOP_P = AI_TOP_P if AI_TOP_P else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 4096
         self.AZURE_EMBEDDER_DEPLOYMENT_ID = AZURE_EMBEDDER_DEPLOYMENT_ID
 
     async def instruct(self, prompt: str, tokens: int = 0) -> str:
         num_retries = 3
         messages = [{"role": "system", "content": prompt}]
         for _ in range(num_retries):
             try:
```

### Comparing `agixt-1.2.9/agixt/provider/chatgpt.py` & `agixt-1.3.0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/agixt/provider/claude.py` & `agixt-1.3.0/agixt/provider/claude.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
         ANTHROPIC_API_KEY: str = "",
         MAX_TOKENS: int = 75000,
         AI_MODEL: str = "claude-v1-100k",
         AI_TEMPERATURE: float = 0.7,
         **kwargs,
     ):
         self.ANTHROPIC_API_KEY = ANTHROPIC_API_KEY
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 75000
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "claude-v1-100k"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
 
     async def instruct(self, prompt):
         try:
             c = anthropic.Client(api_key=self.ANTHROPIC_API_KEY)
             return c.completion(
                 prompt=f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}",
                 stop_sequences=[anthropic.HUMAN_PROMPT],
```

### Comparing `agixt-1.2.9/agixt/provider/fastchat.py` & `agixt-1.3.0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/agixt/provider/gpt4all.py` & `agixt-1.3.0/agixt/provider/gpt4all.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         MAX_TOKENS: int = 2000,
         AI_MODEL: str = "default",
         AI_TEMPERATURE: float = 0.7,
         **kwargs,
     ):
         self.model = GPT4All(model=MODEL_NAME)
         self.model.open()
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 2000
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "default"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
         # TODO: Need to research to add temperature, no obvious flag.
 
     async def instruct(self, prompt):
         try:
             return self.model.prompt(prompt)
         except Exception as e:
             return f"GPT4ALL Error: {e}"
```

### Comparing `agixt-1.2.9/agixt/provider/gpugpt4all.py` & `agixt-1.3.0/agixt/provider/gpugpt4all.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         **kwargs,
     ):
         try:
             self.max_tokens = int(MAX_TOKENS)
         except:
             self.max_tokens = 2000
         self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
         # GPT4All will just download the model, maybe save it in our workspace?
         self.model = GPT4All(llama_path=MODEL_PATH)
         self.config = {
             "num_beams": 2,
             "min_new_tokens": 10,
             "max_length": 100,
             "repetition_penalty": 2.0,
```

### Comparing `agixt-1.2.9/agixt/provider/huggingchat.py` & `agixt-1.3.0/agixt/provider/huggingchat.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,22 @@
         AI_TEMPERATURE: float = 0.7,
         MAX_TOKENS: int = 2000,
         AI_MODEL: str = "openassistant",
         HUGGINGCHAT_COOKIE_PATH: str = "./huggingchat-cookies.json",
         **kwargs,
     ):
         self.requirements = []
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.MAX_TOKENS = int(MAX_TOKENS)
-        self.AI_MODEL = AI_MODEL
-        self.HUGGINGCHAT_COOKIE_PATH = HUGGINGCHAT_COOKIE_PATH
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.MAX_TOKENS = int(MAX_TOKENS) if MAX_TOKENS else 2000
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "openassistant"
+        self.HUGGINGCHAT_COOKIE_PATH = (
+            HUGGINGCHAT_COOKIE_PATH
+            if HUGGINGCHAT_COOKIE_PATH
+            else "./huggingchat-cookies.json"
+        )
 
     async def instruct(self, prompt: str, tokens: int = 0) -> str:
         try:
             chatbot = hugchat.ChatBot(cookie_path=self.HUGGINGCHAT_COOKIE_PATH)
             id = chatbot.new_conversation()
             response = chatbot.chat(
                 text=prompt,
```

### Comparing `agixt-1.2.9/agixt/provider/huggingface.py` & `agixt-1.3.0/agixt/provider/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
         AI_MODEL: str = "gpt2",
         AI_TEMPERATURE: float = 0.7,
         MAX_TOKENS: int = 4096,
         **kwargs,
     ):
         self.HUGGINGFACE_API_KEY = HUGGINGFACE_API_KEY
         self.HUGGINGFACE_API_URL = HUGGINGFACE_API_URL
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.MAX_TOKENS = MAX_TOKENS
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "gpt2"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 4096
 
     async def instruct(self, prompt: str, tokens: int = 0) -> str:
         num_retries = 3
         headers = {"Authorization": f"Bearer {self.HUGGINGFACE_API_KEY}"}
         payload = {
             "inputs": prompt,
             "max_tokens": int(self.MAX_TOKENS),
```

### Comparing `agixt-1.2.9/agixt/provider/kobold.py` & `agixt-1.3.0/agixt/provider/kobold.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,16 @@
         MAX_TOKENS: int = 2000,
         AI_TEMPERATURE: float = 0.7,
         AI_MODEL: str = "default",
         **kwargs,
     ):
         self.requirements = []
         self.AI_PROVIDER_URI = AI_PROVIDER_URI
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_TEMPERATURE = AI_TEMPERATURE
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 2000
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
         self.AI_MODEL = AI_MODEL
 
     async def instruct(self, prompt, tokens: int = 0):
         try:
             max_tokens = int(self.MAX_TOKENS - tokens)
         except:
             max_tokens = 2000
```

### Comparing `agixt-1.2.9/agixt/provider/llamacpp.py` & `agixt-1.3.0/agixt/provider/llamacpp.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,21 +21,21 @@
         GPU_LAYERS: int = 0,
         BATCH_SIZE: int = 2048,
         THREADS: int = 0,
         STOP_SEQUENCE: str = "</s>",
         **kwargs,
     ):
         self.requirements = ["llama-cpp-python"]
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_MODEL = AI_MODEL
-        self.GPU_LAYERS = GPU_LAYERS
-        self.BATCH_SIZE = BATCH_SIZE
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 2048
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "default"
+        self.GPU_LAYERS = GPU_LAYERS if GPU_LAYERS else 0
+        self.BATCH_SIZE = BATCH_SIZE if BATCH_SIZE else 2048
         self.THREADS = THREADS if THREADS != 0 else None
-        self.STOP_SEQUENCE = STOP_SEQUENCE
+        self.STOP_SEQUENCE = STOP_SEQUENCE if STOP_SEQUENCE else "</s>"
         self.MODEL_PATH = MODEL_PATH
         if self.MODEL_PATH:
             try:
                 self.MAX_TOKENS = int(self.MAX_TOKENS)
             except:
                 self.MAX_TOKENS = 2048
```

### Comparing `agixt-1.2.9/agixt/provider/llamacppapi.py` & `agixt-1.3.0/agixt/provider/llamacppapi.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,22 +8,24 @@
         AI_PROVIDER_URI: str = "http://localhost:8000",
         MAX_TOKENS: int = 2048,
         AI_TEMPERATURE: float = 0.7,
         AI_MODEL: str = "default",
         STOP_SEQUENCE: str = "</s>",
         **kwargs,
     ):
-        self.AI_PROVIDER_URI = AI_PROVIDER_URI
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_MODEL = AI_MODEL
-        self.STOP_SEQUENCE = STOP_SEQUENCE
-        self.MAX_TOKENS = int(self.MAX_TOKENS)
+        self.AI_PROVIDER_URI = (
+            AI_PROVIDER_URI if AI_PROVIDER_URI else "http://localhost:8000"
+        )
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 2048
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "default"
+        self.STOP_SEQUENCE = STOP_SEQUENCE if STOP_SEQUENCE else "</s>"
+        self.MAX_TOKENS = int(self.MAX_TOKENS) if self.MAX_TOKENS else 2048
 
-    def instruct(self, prompt, tokens: int = 0):
+    async def instruct(self, prompt, tokens: int = 0):
         params = {
             "prompt": prompt,
             "temperature": float(self.AI_TEMPERATURE),
             "stop": self.STOP_SEQUENCE,
             "seed": random.randint(1, 1000000000),
         }
         response = requests.post(f"{self.AI_PROVIDER_URI}/v1/completions", json=params)
```

### Comparing `agixt-1.2.9/agixt/provider/openai.py` & `agixt-1.3.0/agixt/provider/openai.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 import openai
+import time
+import logging
 
 
 class OpenaiProvider:
     def __init__(
         self,
         OPENAI_API_KEY: str = "",
-        AI_MODEL: str = "gpt-3.5-turbo",
+        AI_MODEL: str = "gpt-3.5-turbo-16k-0613",
         AI_TEMPERATURE: float = 0.7,
         AI_TOP_P: float = 0.7,
-        MAX_TOKENS: int = 4096,
-        **kwargs
+        MAX_TOKENS: int = 16384,
+        API_URI: str = "https://api.openai.com/v1",
+        **kwargs,
     ):
         self.requirements = ["openai"]
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.AI_TOP_P = AI_TOP_P
-        self.MAX_TOKENS = MAX_TOKENS
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "gpt-3.5-turbo-16k-0613"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.AI_TOP_P = AI_TOP_P if AI_TOP_P else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 16384
+        self.API_URI = API_URI
+        openai.api_base = self.API_URI
         openai.api_key = OPENAI_API_KEY
 
     async def instruct(self, prompt, tokens: int = 0):
         max_new_tokens = int(self.MAX_TOKENS) - tokens
-        if not self.AI_MODEL.startswith("gpt-"):
-            # Use completion API
-            response = openai.Completion.create(
-                engine=self.AI_MODEL,
-                prompt=prompt,
-                temperature=float(self.AI_TEMPERATURE),
-                max_tokens=max_new_tokens,
-                top_p=float(self.AI_TOP_P),
-                frequency_penalty=0,
-                presence_penalty=0,
-            )
-            return response.choices[0].text.strip()
-        else:
-            # Use chat completion API
-            messages = [{"role": "system", "content": prompt}]
-            response = openai.ChatCompletion.create(
-                model=self.AI_MODEL,
-                messages=messages,
-                temperature=float(self.AI_TEMPERATURE),
-                max_tokens=max_new_tokens,
-                top_p=float(self.AI_TOP_P),
-                n=1,
-                stop=None,
-            )
-            return response.choices[0].message.content.strip()
+        try:
+            if not self.AI_MODEL.startswith("gpt-"):
+                # Use completion API
+                response = openai.Completion.create(
+                    engine=self.AI_MODEL,
+                    prompt=prompt,
+                    temperature=float(self.AI_TEMPERATURE),
+                    max_tokens=max_new_tokens,
+                    top_p=float(self.AI_TOP_P),
+                    frequency_penalty=0,
+                    presence_penalty=0,
+                )
+                return response.choices[0].text.strip()
+            else:
+                # Use chat completion API
+                messages = [{"role": "system", "content": prompt}]
+                response = openai.ChatCompletion.create(
+                    model=self.AI_MODEL,
+                    messages=messages,
+                    temperature=float(self.AI_TEMPERATURE),
+                    max_tokens=max_new_tokens,
+                    top_p=float(self.AI_TOP_P),
+                    n=1,
+                    stop=None,
+                )
+                return response.choices[0].message.content.strip()
+        except Exception as e:
+            logging.info(f"OpenAI API Error: {e}")
+            time.sleep(3)
+            return await self.instruct(prompt=prompt, tokens=tokens)
```

### Comparing `agixt-1.2.9/agixt/provider/poe.py` & `agixt-1.3.0/agixt/provider/poe.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/agixt/provider/runpod.py` & `agixt-1.3.0/agixt/provider/runpod.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,20 @@
         API_KEY: str = "",
         MAX_TOKENS: int = 2000,
         AI_TEMPERATURE: float = 0.7,
         AI_MODEL: str = "",
         **kwargs,
     ):
         self.requirements = []
-        self.AI_PROVIDER_URI = AI_PROVIDER_URI
-        self.MAX_TOKENS = MAX_TOKENS
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.AI_MODEL = AI_MODEL
+        self.AI_PROVIDER_URI = (
+            AI_PROVIDER_URI if AI_PROVIDER_URI else "https://api.runpod.io"
+        )
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 2000
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "default"
         self.API_KEY = API_KEY
 
     @threaded
     async def instruct(self, prompt, tokens: int = 0):
         headers = {"Authorization": f"Bearer {self.API_KEY}"}
         max_new_tokens = int(self.MAX_TOKENS) - tokens
```

### Comparing `agixt-1.2.9/agixt/provider/transformer.py` & `agixt-1.3.0/agixt/provider/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,25 @@
         T5Tokenizer,
     )
 
 
 class TransformerProvider:
     def __init__(
         self,
-        MODEL_PATH: str = "HuggingFaceH4/starchat-alpha",
+        MODEL_PATH: str = "HuggingFaceH4/starchat-beta",
         AI_TEMPERATURE: float = 0.7,
         MAX_TOKENS: int = 4096,
         AI_MODEL: str = "starchat",
         **kwargs,
     ):
         self.requirements = ["transformers", "accelerate"]
-        self.AI_MODEL = AI_MODEL
-        self.AI_TEMPERATURE = AI_TEMPERATURE
-        self.MAX_TOKENS = MAX_TOKENS
-        self.MODEL_PATH = MODEL_PATH
+        self.AI_MODEL = AI_MODEL if AI_MODEL else "starchat"
+        self.AI_TEMPERATURE = AI_TEMPERATURE if AI_TEMPERATURE else 0.7
+        self.MAX_TOKENS = MAX_TOKENS if MAX_TOKENS else 4096
+        self.MODEL_PATH = MODEL_PATH if MODEL_PATH else "HuggingFaceH4/starchat-beta"
 
     async def instruct(self, prompt, tokens: int = 0):
         max_new_tokens = int(self.MAX_TOKENS) - tokens
         try:
             model_path = self.MODEL_PATH
             if "chatglm" in model_path:
                 tokenizer = AutoTokenizer.from_pretrained(
```

### Comparing `agixt-1.2.9/agixt.egg-info/PKG-INFO` & `agixt-1.3.0/agixt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.9
+Version: 1.3.0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -12,29 +12,32 @@
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-[![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
+[![Logo](https://josh-xt.github.io/AGiXT/images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quick Start Guide](#quick-start-guide)
+    - [Downloading the docker-compose file](#downloading-the-docker-compose-file)
+    - [Editing the environment file](#editing-the-environment-file)
+    - [Running AGiXT](#running-agixt)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -60,25 +63,49 @@
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quick Start Guide
 
-To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
+To get started quickly, you can use the Docker deployment. You will need [docker and docker-compose](https://docs.docker.com/compose/install/) installed on your system. 
 
-Open a terminal and run the following commands:
+Note: If you run locally without docker, it is unsupported.  Any issues you encounter will be closed without comment. Docker is the only way we can say "it works on my machine" and have it mean anything.
+
+### Downloading the docker-compose file
+Open a terminal and run the following commands to download the docker-compose file and the example environment file:
 
 ```
-git clone https://github.com/Josh-XT/AGiXT
+mkdir AGiXT
 cd AGiXT
-./AGiXT.sh
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/.env.example
+```
+
+### Editing the environment file
+Open the `.env.example` file in a text editor, you will want to at least change the `POSTGRES_PASSWORD` if nothing else.
+
+- `POSTGRES_SERVER` is the name of the database server, this should be `db` if you are using the docker-compose file as-is.
+- `POSTGRES_DB` is the name of the database, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PORT` is the port that the database is listening on, this should be `5432` if you are using the docker-compose file as-is.
+- `POSTGRES_USER` is the username to connect to the database with, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PASSWORD` **is the password to connect to the database with, this should be changed from the example file.**
+- `UVICORN_WORKERS` is the number of workers to run the web server with, this is `6` by default, adjust this to your system's capabilities.
+- `AGIXT_HUB` is the name of the AGiXT hub, this should be `AGiXT/hub` if you want to use the [Open Source AGiXT hub.](https://github.com/AGiXT/hub) If you want to use your own fork of AGiXT hub, change this to your username and the name of your fork.
+- `AGIXT_URI` is the URI of the AGiXT hub, this should be `http://agixt:7437` if you are using the docker-compose file as-is. If hosting the AGiXT server separately, change this to the URI of your AGiXT server, otherwise leave it as-is.
+- `GITHUB_USER` is your GitHub username, this is only required if using your own AGiXT hub to pull your repository data.
+- `GITHUB_TOKEN` is your GitHub personal access token, this is only required if using your own AGiXT hub to pull your repository data.
+
+### Running AGiXT
+Once you have edited the `.env.example` file, save it as `.env` and run the following command to start AGiXT:
+```
+docker-compose up -d
 ```
 
-Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `./AGiXT.sh` again.
+Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `docker-compose up -d` again from the `AGiXT` directory.
 
 - Access the web interface at http://localhost:8501
 - Access the AGiXT API documentation at http://localhost:7437
 
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
```

### Comparing `agixt-1.2.9/docs/1-Getting started/Screenshots.md` & `agixt-1.3.0/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/1-Getting started/Support.md` & `agixt-1.3.0/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.3.0/docs/2-Concepts/0-Core Concepts.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 ## Chat
 Chatting with an AI is like having a conversation with a friend, but your friend is a computer. You can talk about all sorts of topics, ask questions, and get responses. The AI doesn't just do one thing and stop; it keeps the conversation going. It's more interactive and open-ended than just giving an instruction.
 
 ## Smart Chat
 "Smart Chat" is an advanced feature of the AGiXT software that integrates artificial intelligence with web research to deliver highly accurate and contextually relevant responses to user prompts. It initiates with user interaction, followed by strategic web searches conducted by an AI agent. The agent then scrapes and analyses data from the web, recursively learning and exploring until it gathers enough information. This knowledge is then used to generate potential task solutions, which are evaluated and refined through multiple AI modules. The result is a carefully crafted solution that not only addresses the user's original prompt but also incorporates the most recent and pertinent data from the web, ensuring a comprehensive and informed response.
 
-## Task
-A task is like a project or a big job that needs to be done. It's more complicated than a simple instruction and may involve multiple steps. For example, planning a trip involves many tasks, like booking flights, choosing hotels, and creating an itinerary. When you ask an AI to perform a task, you're asking it to figure out and complete all these steps for you. It's like having a personal assistant who can take care of complex projects on your behalf.
-
-## Smart Task
-The Smart Task process is an intelligent system that dynamically manages tasks through a series of AI-driven agents. It starts with a user-defined objective, which is then broken down into subtasks by the Task Agent. These subtasks are methodically executed using a loop structure that employs a Smart Instruct process. This process involves a suite of agents including a Web Search Agent for information gathering, an Instruction Agent for generating potential solutions, a Research Agent for analyzing these solutions, a Solution Agent for determining the best course of action, and finally an Execution Agent for carrying out the necessary commands. The task list is continually reprioritized to optimize efficiency and prevent redundancy. The final output of the Smart Task process is a comprehensive solution to the user's initial objective, encompassing an explanation from the Solution Agent and the results of the executed commands from the Execution Agent. The Smart Task process exemplifies an innovative application of AI in task management, demonstrating a high level of responsiveness to user input and adaptability to evolving task requirements.
-
 ## Chains
 Imagine a chain of dominoes. When you knock over the first one, it sets off a series of actions, with each domino affecting the next. In AI, a chain is a series of steps or commands that are linked together. The output of one step becomes the input for the next. This allows you to create complex workflows, where the AI performs a series of actions in a specific order, like a recipe. It's a way of automating processes, so you can get the AI to do more complex jobs without needing to supervise every step.
 
+## Task Chains
+
+Think of Task Chains as a roadmap for a journey. When you plan a trip, you don't just decide on the destination, you also plan the route you'll take, the stops you'll make, and the sights you'll see along the way. In the world of AI, a Task Chain is a sequence of steps or tasks that the AI needs to perform to reach a user-defined objective. Each step in the chain is a task that needs to be completed for the overall objective to be achieved. The AI follows this roadmap, executing each task in the chain in the order they appear, and using the output of one task as the input for the next. This allows the AI to handle complex objectives that require multiple steps to complete.
+
+## Smart Task Chains
+
+Smart Task Chains are an advanced feature of the AGiXT software that takes Task Chains to the next level. Imagine a Task Chain as a roadmap, but now, each stop along the way is thoroughly researched and planned out before you even set off on your journey. That's what Smart Task Chains do. They start with a user-defined objective and generate a Task Chain to achieve it. But instead of blindly following the chain, each step in the chain is treated as a Smart Instruct. This means that before the AI attempts each task, it first conducts a thorough research using web search, formulates strategies, evaluates them, and fine-tunes the best possible solution. This ensures that each step in the chain is not just completed, but completed in the best possible way. Smart Task Chains represent a combination of strategic planning and efficient execution, providing a comprehensive, intelligent, and reliable approach to achieving complex objectives.
```

### Comparing `agixt-1.2.9/docs/2-Concepts/Agents.md` & `agixt-1.3.0/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Chains.md` & `agixt-1.3.0/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Chat.md` & `agixt-1.3.0/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Commands.md` & `agixt-1.3.0/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Instructions.md` & `agixt-1.3.0/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Prompts.md` & `agixt-1.3.0/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Smart Chat.md` & `agixt-1.3.0/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Smart Instruct.md` & `agixt-1.3.0/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/2-Concepts/Smart Task.md` & `agixt-1.3.0/docs/2-Concepts/Smart Task Chains.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Smart Tasks
-The Smart Task process is an intelligent system that dynamically manages tasks through a series of AI-driven agents. It starts with a user-defined objective, which is then broken down into subtasks by the Task Agent. These subtasks are methodically executed using a loop structure that employs a Smart Instruct process. This process involves a suite of agents including a Web Search Agent for information gathering, an Instruction Agent for generating potential solutions, a Research Agent for analyzing these solutions, a Solution Agent for determining the best course of action, and finally an Execution Agent for carrying out the necessary commands. The task list is continually reprioritized to optimize efficiency and prevent redundancy. The final output of the Smart Task process is a comprehensive solution to the user's initial objective, encompassing an explanation from the Solution Agent and the results of the executed commands from the Execution Agent. The Smart Task process exemplifies an innovative application of AI in task management, demonstrating a high level of responsiveness to user input and adaptability to evolving task requirements.
+# Smart Task Chains
+
+Smart Task Chains are an advanced feature of the AGiXT software that enhances the functionality of Task Chains. In a Smart Task Chain, each task in the chain is treated as a Smart Instruct. This means that before the AI attempts each task, it first conducts a thorough research using web search, formulates strategies, evaluates them, and fine-tunes the best possible solution. This ensures that each step in the chain is not just completed, but completed in the best possible way.
 
 ## Important Notice About Small Context Models!
-Small context models are not good at doing things like this.  A small context model is anything with less than 4000 max tokens, and even at 4000 tokens, depending on the complexity of your task, it may not be enough. See [Core Concepts](https://josh-xt.github.io/AGiXT/2-Concepts/0-Core%20Concepts.html) for more information.
+
+Small context models may struggle with complex Smart Task Chains. A small context model is anything with less than 4000 max tokens, and even at 4000 tokens, depending on the complexity of your task, it may not be enough. See Core Concepts for more information.
 
 ## Overview
-1. **Task Definition:** The user provides the LLM with a specific task to accomplish. This task serves as the objective that the LLM will work towards.
 
-2. **Task Breakdown:** The Task Agent, an AI component, analyzes the main task and generates a list of subtasks necessary for its completion. 
+1. **Objective Acquisition:** The process begins with the user providing the initial objective. This objective serves as the base for the entire process, determining the direction of the subsequent steps.
+
+2. **Task Breakdown:** The Task Agent AI takes the initial objective and breaks it down into a sequence of tasks. These tasks are generated based on the AI's understanding of the objective and its knowledge about the steps needed to accomplish it.
 
-3. **Task Execution Loop:** The Task Agent enters a loop where it utilizes a Smart Instruct process for each subtask. 
+3. **Smart Instruct Integration:** Each task in the chain is treated as a Smart Instruct. This means that before the AI attempts each task, it first conducts a thorough research using web search, formulates strategies, evaluates them, and fine-tunes the best possible solution.
 
-4. **Task Prioritization:** After the completion of each subtask, the AI reevaluates and reprioritizes the remaining tasks. This helps in minimizing redundancy and overlapping work.
+4. **Task Execution:** The Execution Agent then executes each task in the chain in the order they appear. It checks after each execution to ensure the output matches the expected results. The agent repeats this process until the objective is accomplished as intended.
 
-5. **Loop Continuation:** The process continues, looping back to the Smart Instruct step until all the tasks in the list are completed.
+5. **Final Output:** The process culminates with the delivery of the final output. This includesboth the detailed explanation from the Task Agent on how the objective was accomplished, as well as the specific task outputs from the Execution Agent. The user is thus provided with a comprehensive view of the objective completion process.
 
-Within this process, the Smart Instruct system is responsible for completing individual tasks. See the [Smart Instruct Documentation](https://josh-xt.github.io/AGiXT/2-Concepts/Smart%20Instruct.html) for more information.
+This process ultimately leverages AI's ability to research, analyze, plan, and execute tasks, creating a robust and intelligent system for task completion. Smart Task Chains represent a combination of strategic planning and efficient execution, providing a comprehensive, intelligent, and reliable approach to achieving complex objectives.
```

### Comparing `agixt-1.2.9/docs/3-Providers/Anthropic Claude.md` & `agixt-1.3.0/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/Azure OpenAI.md` & `agixt-1.3.0/docs/3-Providers/Azure OpenAI.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 1. Set `AI_PROVIDER` to `azure`.
 2. Set `AZURE_API_KEY` to your Azure OpenAI API key.
 3. Set `DEPLOYMENT_ID` to your Azure OpenAI deployment ID for your primary model.
 4. Set `EMBEDDER_DEPLOYMENT_ID` to your Azure OpenAI deployment ID for your embedder model.
 5. Set `AZURE_OPENAI_ENDPOINT` to your Azure OpenAI endpoint.
 6. Choose your `AI_MODEL`.  Enter `gpt-3.5-turbo`, `gpt-4`, `gpt-4-32k`, or any other model you may have access to.
 7. Set `AI_TEMPERATURE` to a value between 0 and 1. The higher the value, the more creative the output.
-8. Set `MAX_TOKENS` to the maximum number of tokens to generate. The higher the value, the longer the output.  The maximum for `gpt-3.5-turbo` is 4096, `gpt-4` is 8192, `gpt-4-32k` is 32768.
+8. Set `MAX_TOKENS` to the maximum number of tokens to generate. The higher the value, the longer the output.  The maximum for `gpt-3.5-turbo` is 4096, `gpt-4` is 8192, `gpt-4-32k` is 32768, `gpt-3.5-turbo-16k` is 16000.
```

### Comparing `agixt-1.2.9/docs/3-Providers/ChatGPT.md` & `agixt-1.3.0/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/FastChat.md` & `agixt-1.3.0/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.3.0/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/GPT4ALL.md` & `agixt-1.3.0/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/GPT4Free.md` & `agixt-1.3.0/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/Google Bard.md` & `agixt-1.3.0/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.3.0/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/HuggingChat.md` & `agixt-1.3.0/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/Microsoft Bing.md` & `agixt-1.3.0/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.3.0/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files 27% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 ### Start provider locally
 1. Setup `text-generation-webui` from above
 1. Make sure `--api` and `--listen` (when running `AGiXT` in docker) are present
 1. `AI_PROVIDER_URI` is now `http://localhost:5000` or `http://172.x.x.x` (docker)
 
 ### Create Agent 
 1. Create a new agent
-1. Set `AI_PROVIDER` to `oobabooga`.
-1. Set `AI_PROVIDER_URI` to the URI of your Oobabooga server.
+2. Set `AI_PROVIDER` to `oobabooga`.
+3. Set `AI_PROVIDER_URI` to the URI of your Oobabooga server.
+4. Set `PROMPT_PREFIX` and `PROMPT_SUFFIX` if your model requires it.  For example, for models like Vicuna, you will want to enter the `PROMPT_PREFIX` to `User: ` and `PROMPT_SUFFIX` to `\nAssistant: `.
+5. Review and set any of the other settings as you see fit from the agent settings page.
```

### Comparing `agixt-1.2.9/docs/3-Providers/OpenAI.md` & `agixt-1.3.0/docs/3-Providers/OpenAI.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 
 ## Quick Start Guide
 ### Update your agent settings
 1. Set `AI_PROVIDER` to `openai`.
 2. Set `OPENAI_API_KEY` to your OpenAI API key.
 3. Set `AI_MODEL` to `gpt-3.5-turbo` for ChatGPT.
 4. Set `AI_TEMPERATURE` to a value between 0 and 1. The higher the value, the more creative the output.
-5. Set `MAX_TOKENS` to the maximum number of tokens to generate. The higher the value, the longer the output.  The maximum for `gpt-3.5-turbo` is 4000, `gpt-4` is 8000.
+5. Set `MAX_TOKENS` to the maximum number of tokens to generate. The higher the value, the longer the output.  The maximum for `gpt-3.5-turbo` is 4000, `gpt-4` is 8000, `gpt-3.5-turbo-16k` is 16000.
```

### Comparing `agixt-1.2.9/docs/3-Providers/Poe.md` & `agixt-1.3.0/docs/3-Providers/Poe.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/llamacpp API.md` & `agixt-1.3.0/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/3-Providers/llamacpp.md` & `agixt-1.3.0/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/README.md` & `agixt-1.3.0/docs/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 [![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html) [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-[![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
+[![Logo](https://josh-xt.github.io/AGiXT/images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quick Start Guide](#quick-start-guide)
+    - [Downloading the docker-compose file](#downloading-the-docker-compose-file)
+    - [Editing the environment file](#editing-the-environment-file)
+    - [Running AGiXT](#running-agixt)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -50,25 +53,49 @@
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quick Start Guide
 
-To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
+To get started quickly, you can use the Docker deployment. You will need [docker and docker-compose](https://docs.docker.com/compose/install/) installed on your system. 
 
-Open a terminal and run the following commands:
+Note: If you run locally without docker, it is unsupported.  Any issues you encounter will be closed without comment. Docker is the only way we can say "it works on my machine" and have it mean anything.
+
+### Downloading the docker-compose file
+Open a terminal and run the following commands to download the docker-compose file and the example environment file:
 
 ```
-git clone https://github.com/Josh-XT/AGiXT
+mkdir AGiXT
 cd AGiXT
-./AGiXT.sh
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/.env.example
+```
+
+### Editing the environment file
+Open the `.env.example` file in a text editor, you will want to at least change the `POSTGRES_PASSWORD` if nothing else.
+
+- `POSTGRES_SERVER` is the name of the database server, this should be `db` if you are using the docker-compose file as-is.
+- `POSTGRES_DB` is the name of the database, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PORT` is the port that the database is listening on, this should be `5432` if you are using the docker-compose file as-is.
+- `POSTGRES_USER` is the username to connect to the database with, this should be `postgres` if you are using the docker-compose file as-is.
+- `POSTGRES_PASSWORD` **is the password to connect to the database with, this should be changed from the example file.**
+- `UVICORN_WORKERS` is the number of workers to run the web server with, this is `6` by default, adjust this to your system's capabilities.
+- `AGIXT_HUB` is the name of the AGiXT hub, this should be `AGiXT/hub` if you want to use the [Open Source AGiXT hub.](https://github.com/AGiXT/hub) If you want to use your own fork of AGiXT hub, change this to your username and the name of your fork.
+- `AGIXT_URI` is the URI of the AGiXT hub, this should be `http://agixt:7437` if you are using the docker-compose file as-is. If hosting the AGiXT server separately, change this to the URI of your AGiXT server, otherwise leave it as-is.
+- `GITHUB_USER` is your GitHub username, this is only required if using your own AGiXT hub to pull your repository data.
+- `GITHUB_TOKEN` is your GitHub personal access token, this is only required if using your own AGiXT hub to pull your repository data.
+
+### Running AGiXT
+Once you have edited the `.env.example` file, save it as `.env` and run the following command to start AGiXT:
+```
+docker-compose up -d
 ```
 
-Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `./AGiXT.sh` again.
+Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `docker-compose up -d` again from the `AGiXT` directory.
 
 - Access the web interface at http://localhost:8501
 - Access the AGiXT API documentation at http://localhost:7437
 
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
```

### Comparing `agixt-1.2.9/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.3.0/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/AGiXT-gradient-light.svg` & `agixt-1.3.0/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/AGiXT.png` & `agixt-1.3.0/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/AGiXT.svg` & `agixt-1.3.0/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.3.0/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/AGiXTwhiteborder.svg` & `agixt-1.3.0/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.3.0/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Smart Instruct.drawio` & `agixt-1.3.0/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Smart Instruct.drawio.svg` & `agixt-1.3.0/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Smart Tasks.drawio` & `agixt-1.3.0/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Smart Tasks.drawio.svg` & `agixt-1.3.0/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/docs/images/Untitled Diagram.drawio` & `agixt-1.3.0/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/setup.py` & `agixt-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/tests/test-commands.ipynb` & `agixt-1.3.0/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.9/tests/tests.ipynb` & `agixt-1.3.0/tests/tests.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897736458970221%*

 * *Differences: {"'cells'": '{5: {\'outputs\': {0: {\'text\': ["Providers: [\'gpt4free\', \'azure\', \'chatgpt\', '*

 * *            "'runpod', 'poe', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'agixt', "*

 * *            "'transformer', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', "*

 * *            '\'llamacpp\', \'gpugpt4all\', \'custom\', \'bard\']\\n"]}}, \'source\': {delete: [1, '*

 * *            '0]}}, 7: {\'source\': {insert: [(3, \'print(f"Settings for {provider_name}:", '*

 * *            "provider_setting […]*

```diff
@@ -5,14 +5,38 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Tests for AGiXT API Client\n"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Add a 60 second delay before we start so that the server has time to start up\n",
+                "import time\n",
+                "\n",
+                "time.sleep(60)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 151,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from agixtsdk import AGiXTSDK\n",
+                "\n",
+                "base_uri = \"http://localhost:7437\"\n",
+                "ApiClient = AGiXTSDK(base_uri=base_uri)\n"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Agents\n"
             ]
         },
@@ -31,22 +55,19 @@
             "execution_count": 152,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "The history saving thread hit an unexpected error (OperationalError('attempt to write a readonly database')).History will not be written to the database.\n",
-                        "Providers: ['gpt4free', 'azure', 'chatgpt', 'runpod', 'poe', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'transformer', 'bing', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', 'bard']\n"
+                        "Providers: ['gpt4free', 'azure', 'chatgpt', 'runpod', 'poe', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'agixt', 'transformer', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', 'custom', 'bard']\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_providers()\n",
                 "providers = ApiClient.get_providers()\n",
                 "print(\"Providers:\", providers)\n"
             ]
         },
         {
             "attachments": {},
@@ -68,20 +89,18 @@
                     "output_type": "stream",
                     "text": [
                         "Settings for gpt4free: {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_provider_settings()\n",
                 "provider_name = \"gpt4free\"\n",
                 "provider_settings = ApiClient.get_provider_settings(provider_name=provider_name)\n",
-                "print(f\"Settings for {provider_name}:\", provider_settings)"
+                "print(f\"Settings for {provider_name}:\", provider_settings)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -100,19 +119,17 @@
                     "output_type": "stream",
                     "text": [
                         "Embed Providers: ['azure', 'cohere', 'default', 'embed_text', 'get_embedder', 'google_palm', 'google_vertex', 'large_local', 'llamacpp', 'openai']\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_embed_providers()\n",
                 "embed_providers = ApiClient.get_embed_providers()\n",
-                "print(\"Embed Providers:\", embed_providers)"
+                "print(\"Embed Providers:\", embed_providers)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -131,16 +148,14 @@
                     "output_type": "stream",
                     "text": [
                         "Extension Settings response: {'macostts': {'USE_MAC_OS_TTS': False}, 'file_system': {'WORKING_DIRECTORY': './WORKSPACE', 'WORKING_DIRECTORY_RESTRICTED': True}, 'huggingface': {'HUGGINGFACE_API_KEY': '', 'HUGGINGFACE_AUDIO_TO_TEXT_MODEL': 'facebook/wav2vec2-large-960h-lv60-self', 'WORKING_DIRECTORY': './WORKSPACE'}, 'discord': {'DISCORD_API_KEY': '', 'DISCORD_COMMAND_PREFIX': '/AGiXT'}, 'dalle': {'HUGGINGFACE_API_KEY': '', 'OPENAI_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'briantts': {'USE_BRIAN_TTS': True}, 'google': {'GOOGLE_API_KEY': ''}, 'microsoft_365': {'MICROSOFT_365_CLIENT_ID': '', 'MICROSOFT_365_CLIENT_SECRET': '', 'MICROSOFT_365_REDIRECT_URI': ''}, 'github': {'GITHUB_USERNAME': '', 'GITHUB_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'gtts': {'USE_GTTS': False}, 'elevenlabs': {'ELEVENLABS_API_KEY': '', 'ELEVENLABS_VOICE': 'Josh'}, 'sendgrid_email': {'SENDGRID_API_KEY': '', 'SENDGRID_EMAIL': ''}, 'searxng': {'SEARXNG_INSTANCE_URL': ''}, 'twitter': {'TW_CONSUMER_KEY': '', 'TW_CONSUMER_SECRET': '', 'TW_ACCESS_TOKEN': '', 'TW_ACCESS_TOKEN_SECRET': ''}}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_extension_settings()\n",
                 "ext_settings_resp = ApiClient.get_extension_settings()\n",
                 "print(\"Extension Settings response:\", ext_settings_resp)\n"
             ]
         },
         {
             "attachments": {},
@@ -155,21 +170,19 @@
             "execution_count": 156,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Extensions response: [['Scrape Text with Playwright', 'scrape_text_with_playwright', {'url': None}], ['Scrape Links with Playwright', 'scrape_links_with_playwright', {'url': None}], ['Speak with MacOS TTS', 'speak_with_macos_speech', {'text': None, 'voice_index': 0}], ['Evaluate Code', 'evaluate_code', {'code': None, 'agent': 'AGiXT'}], ['Analyze Pull Request', 'analyze_pull_request', {'pr_url': None, 'agent': 'AGiXT'}], ['Perform Automated Testing', 'perform_automated_testing', {'test_url': None, 'agent': 'AGiXT'}], ['Run CI-CD Pipeline', 'run_ci_cd_pipeline', {'repo_url': None, 'agent': 'AGiXT'}], ['Improve Code', 'improve_code', {'suggestions': None, 'code': None, 'agent': 'AGiXT'}], ['Write Tests', 'write_tests', {'code': None, 'focus': None, 'agent': 'AGiXT'}], ['Create a new command', 'create_command', {'function_description': None, 'agent': 'AGiXT'}], ['Describe Image', 'describe_image', {'image_url': None}], ['Ask AI Agent Bing', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bing', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent tester', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent tester', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent gpt4free', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent gpt4free', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Bard', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bard', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Vicuna', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Vicuna', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent OpenAI', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent OpenAI', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent azure', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent azure', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent ChatGPT', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent ChatGPT', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent new_agent', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent new_agent', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Guanaco', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Guanaco', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Write to File', 'write_to_file', {'filename': None, 'text': None}], ['Read File', 'read_file', {'filename': None}], ['Search Files', 'search_files', {'directory': None}], ['Append to File', 'append_to_file', {'filename': None, 'text': None}], ['Execute Python File', 'execute_python_file', {'file': None}], ['Delete File', 'delete_file', {'filename': None}], ['Execute Shell', 'execute_shell', {'command_line': None}], ['Read Audio from File', 'read_audio_from_file', {'audio_path': None}], ['Read Audio', 'read_audio', {'audio': None}], ['Generate Image with Stable Diffusion', 'generate_image_with_hf', {'prompt': None, 'filename': None}], ['Speak with TTS with BrianTTS', 'speak_with_briantts', {'text': None}], ['Clone Github Repository', 'clone_repo', {'repo_url': None, 'clone_path': None}], ['Get Datetime', 'get_datetime', {}], ['Speak with TTS Using Elevenlabs', 'speak_with_elevenlabs', {'text': None, 'voice_index': 0}], ['Use The Search Engine', 'search', {'query': None}], ['Create Task Chain', 'create_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}], ['Create Smart Task Chain', 'create_smart_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}]]\n"
+                        "Extensions response: [{'extension_name': 'Web Playwright', 'description': 'Web Playwright', 'settings': [], 'commands': [{'friendly_name': 'Scrape Text with Playwright', 'command_name': 'scrape_text_with_playwright', 'command_args': {'url': ''}}, {'friendly_name': 'Scrape Links with Playwright', 'command_name': 'scrape_links_with_playwright', 'command_args': {'url': ''}}]}, {'extension_name': 'Agixt Actions', 'description': 'Agixt Actions', 'settings': [], 'commands': [{'friendly_name': 'Create Task Chain', 'command_name': 'create_task_chain', 'command_args': {'agent': '', 'primary_objective': '', 'numbered_list_of_tasks': '', 'short_chain_description': '', 'smart_chain': False, 'researching': False}}, {'friendly_name': 'Generate Extension from OpenAPI', 'command_name': 'generate_openapi_chain', 'command_args': {'agent': '', 'extension_name': '', 'openapi_json_url': ''}}, {'friendly_name': 'Generate Agent Helper Chain', 'command_name': 'generate_helper_chain', 'command_args': {'user_agent': '', 'helper_agent': '', 'task_in_question': ''}}, {'friendly_name': 'Ask for Help or Further Clarification to Complete Task', 'command_name': 'ask_for_help', 'command_args': {'your_agent_name': '', 'your_task': ''}}, {'friendly_name': 'Create a new command', 'command_name': 'create_command', 'command_args': {'function_description': '', 'agent': 'AGiXT'}}, {'friendly_name': 'Describe Image', 'command_name': 'describe_image', 'command_args': {'image_url': ''}}, {'friendly_name': 'Execute Python Code', 'command_name': 'execute_python_code', 'command_args': {'code': ''}}, {'friendly_name': 'Get Python Code from Response', 'command_name': 'get_python_code_from_response', 'command_args': {'response': ''}}]}, {'extension_name': 'Macostts', 'description': 'Macostts', 'settings': ['USE_MAC_OS_TTS'], 'commands': [{'friendly_name': 'Speak with MacOS TTS', 'command_name': 'speak_with_macos_speech', 'command_args': {'text': '', 'voice_index': 0}}]}, {'extension_name': 'File System', 'description': 'File System', 'settings': ['WORKING_DIRECTORY', 'WORKING_DIRECTORY_RESTRICTED'], 'commands': [{'friendly_name': 'Write to File', 'command_name': 'write_to_file', 'command_args': {'filename': '', 'text': ''}}, {'friendly_name': 'Read File', 'command_name': 'read_file', 'command_args': {'filename': ''}}, {'friendly_name': 'Search Files', 'command_name': 'search_files', 'command_args': {'directory': ''}}, {'friendly_name': 'Append to File', 'command_name': 'append_to_file', 'command_args': {'filename': '', 'text': ''}}, {'friendly_name': 'Execute Python File', 'command_name': 'execute_python_file', 'command_args': {'file': ''}}, {'friendly_name': 'Delete File', 'command_name': 'delete_file', 'command_args': {'filename': ''}}, {'friendly_name': 'Execute Shell', 'command_name': 'execute_shell', 'command_args': {'command_line': ''}}, {'friendly_name': 'Indent String for Python Code', 'command_name': 'indent_string', 'command_args': {'string': '', 'indents': 1}}, {'friendly_name': 'Generate Commands Dictionary', 'command_name': 'generate_commands_dict', 'command_args': {'python_file_content': ''}}]}, {'extension_name': 'Huggingface', 'description': 'Huggingface', 'settings': ['HUGGINGFACE_API_KEY', 'HUGGINGFACE_AUDIO_TO_TEXT_MODEL', 'WORKING_DIRECTORY'], 'commands': [{'friendly_name': 'Read Audio from File', 'command_name': 'read_audio_from_file', 'command_args': {'audio_path': ''}}, {'friendly_name': 'Read Audio', 'command_name': 'read_audio', 'command_args': {'audio': ''}}, {'friendly_name': 'Generate Image with Stable Diffusion', 'command_name': 'generate_image_with_hf', 'command_args': {'prompt': '', 'filename': ''}}]}, {'extension_name': 'Discord', 'description': 'Discord', 'settings': ['DISCORD_API_KEY', 'DISCORD_COMMAND_PREFIX'], 'commands': []}, {'extension_name': 'Dalle', 'description': 'Dalle', 'settings': ['HUGGINGFACE_API_KEY', 'OPENAI_API_KEY', 'WORKING_DIRECTORY'], 'commands': []}, {'extension_name': 'Briantts', 'description': 'Briantts', 'settings': ['USE_BRIAN_TTS'], 'commands': [{'friendly_name': 'Speak with TTS with BrianTTS', 'command_name': 'speak_with_briantts', 'command_args': {'text': ''}}]}, {'extension_name': 'Google', 'description': 'Google', 'settings': ['GOOGLE_API_KEY'], 'commands': []}, {'extension_name': 'Microsoft 365', 'description': 'Microsoft 365', 'settings': ['MICROSOFT_365_CLIENT_ID', 'MICROSOFT_365_CLIENT_SECRET', 'MICROSOFT_365_REDIRECT_URI'], 'commands': []}, {'extension_name': 'Github', 'description': 'Github', 'settings': ['GITHUB_USERNAME', 'GITHUB_API_KEY', 'WORKING_DIRECTORY'], 'commands': [{'friendly_name': 'Clone Github Repository', 'command_name': 'clone_repo', 'command_args': {'repo_url': ''}}]}, {'extension_name': 'Gtts', 'description': 'Gtts', 'settings': ['USE_GTTS'], 'commands': []}, {'extension_name': 'Times', 'description': 'Times', 'settings': [], 'commands': [{'friendly_name': 'Get Datetime', 'command_name': 'get_datetime', 'command_args': {}}]}, {'extension_name': 'Elevenlabs', 'description': 'Elevenlabs', 'settings': ['ELEVENLABS_API_KEY', 'ELEVENLABS_VOICE'], 'commands': [{'friendly_name': 'Speak with TTS Using Elevenlabs', 'command_name': 'speak_with_elevenlabs', 'command_args': {'text': '', 'voice_index': 0}}]}, {'extension_name': 'Sendgrid Email', 'description': 'Sendgrid Email', 'settings': ['SENDGRID_API_KEY', 'SENDGRID_EMAIL'], 'commands': []}, {'extension_name': 'Searxng', 'description': 'Searxng', 'settings': ['SEARXNG_INSTANCE_URL'], 'commands': [{'friendly_name': 'Use The Search Engine', 'command_name': 'search', 'command_args': {'query': ''}}]}, {'extension_name': 'Twitter', 'description': 'Twitter', 'settings': ['TW_CONSUMER_KEY', 'TW_CONSUMER_SECRET', 'TW_ACCESS_TOKEN', 'TW_ACCESS_TOKEN_SECRET'], 'commands': []}]\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_extensions()\n",
                 "ext = ApiClient.get_extensions()\n",
                 "print(\"Extensions response:\", ext)\n"
             ]
         },
         {
             "attachments": {},
@@ -186,21 +199,19 @@
             "execution_count": 157,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agents: [{'name': 'Bing', 'status': False}, {'name': 'tester', 'status': False}, {'name': 'gpt4free', 'status': False}, {'name': 'Bard', 'status': False}, {'name': 'Vicuna', 'status': False}, {'name': 'OpenAI', 'status': False}, {'name': 'azure', 'status': False}, {'name': 'ChatGPT', 'status': False}, {'name': 'new_agent', 'status': False}, {'name': 'Guanaco', 'status': False}]\n"
+                        "Agents: [{'name': 'gpt4free', 'status': False}, {'name': 'OobaStarchat', 'status': False}]\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_agents()\n",
                 "agents = ApiClient.get_agents()\n",
                 "print(\"Agents:\", agents)\n"
             ]
         },
         {
             "attachments": {},
@@ -222,24 +233,21 @@
                     "output_type": "stream",
                     "text": [
                         "Add agent response: {'message': 'Agent test_agent created.'}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test add_agent()\n",
                 "agent_name = \"test_agent\"\n",
                 "provider_name = \"gpt4free\"\n",
                 "# Gets a list of the provider setting defaults\n",
                 "# We'll use defaults for the provider instead of defining anything for the tests.\n",
-                "provider_settings = ApiClient.get_provider_settings(provider_name=provider_name)\n",
-                "add_agent_resp = ApiClient.add_agent(agent_name=agent_name, settings=provider_settings)\n",
-                "print(\"Add agent response:\", add_agent_resp)"
+                "add_agent_resp = ApiClient.add_agent(agent_name=agent_name, settings={})\n",
+                "print(\"Add agent response:\", add_agent_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -258,23 +266,21 @@
                     "output_type": "stream",
                     "text": [
                         "Rename agent response: {'message': 'Agent renamed.'}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test rename_agent()\n",
                 "agent_name = \"test_agent\"\n",
                 "new_agent_name = \"new_agent\"\n",
                 "rename_agent_resp = ApiClient.rename_agent(\n",
                 "    agent_name=agent_name, new_name=new_agent_name\n",
                 ")\n",
-                "print(\"Rename agent response:\", rename_agent_resp)"
+                "print(\"Rename agent response:\", rename_agent_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -288,21 +294,19 @@
             "execution_count": 160,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': '0.7', 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
+                        "Config for new_agent: {'commands': None, 'settings': {'provider': 'gpt4free', 'embedder': 'default', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': '0.7', 'MAX_TOKENS': '4096', 'AUTONOMOUS_EXECUTION': False}, 'enabled_commands': []}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_agentconfig()\n",
                 "agent_name = \"new_agent\"\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
                 "print(f\"Config for {agent_name}:\", agent_config)\n"
             ]
         },
         {
@@ -321,21 +325,19 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent settings response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
+                        "New config for new_agent: {'commands': None, 'settings': {'provider': 'gpt4free', 'embedder': 'default', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': '0.7', 'MAX_TOKENS': '4096', 'AUTONOMOUS_EXECUTION': False}, 'enabled_commands': []}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test update_agent_settings()\n",
                 "agent_name = \"new_agent\"\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
                 "agent_settings = agent_config[\"settings\"]\n",
                 "# We'll just change the AI_TEMPERATURE setting for the test\n",
                 "agent_settings[\"AI_TEMPERATURE\"] = 0.5\n",
                 "update_agent_settings_resp = ApiClient.update_agent_settings(\n",
@@ -361,21 +363,19 @@
             "execution_count": 162,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Commands: {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}\n"
+                        "Commands: {}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_commands()\n",
                 "agent_name = \"new_agent\"\n",
                 "commands = ApiClient.get_commands(agent_name=agent_name)\n",
                 "print(\"Commands:\", commands)\n"
             ]
         },
         {
@@ -431,22 +431,20 @@
                     "output_type": "stream",
                     "text": [
                         "Chat response: The capital of France is Paris.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test chat()\n",
                 "agent_name = \"new_agent\"\n",
                 "chat_resp = ApiClient.chat(\n",
                 "    agent_name=agent_name, prompt=\"What is the capital of France?\"\n",
                 ")\n",
-                "print(\"Chat response:\", chat_resp)"
+                "print(\"Chat response:\", chat_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -460,55 +458,66 @@
             "execution_count": 165,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agent prompt response: Dragons, mighty beasts of fire\n",
-                        "With scales gleaming bright and higher\n",
-                        "Their breath scorching the earth and skies\n",
-                        "As they soar amidst the sunrise\n",
+                        "Agent prompt response: In ancient realms where legends thrive,\n",
+                        "Where fire breathes and scales arrive,\n",
+                        "The mighty dragons take to the skies,\n",
+                        "With wings that soar and tales that mesmerize.\n",
+                        "\n",
+                        "Oh, magnificent creatures of ancient lore,\n",
+                        "Fierce and powerful, forevermore,\n",
+                        "Their eyes ablaze with wisdom's light,\n",
+                        "Guiding souls through day and night.\n",
                         "\n",
-                        "Their wings spread wide, they glide with grace\n",
-                        "Through mountains and valleys they embrace\n",
-                        "Their eyes ablaze with ancient power\n",
-                        "As they guard their hoard with valour\n",
+                        "A dance of flames in the moonlit air,\n",
+                        "Their serpentine bodies, beyond compare,\n",
+                        "Through misty peaks and valleys deep,\n",
+                        "They guard their secrets, their treasures to keep.\n",
                         "\n",
-                        "Fierce and proud, they rule with might\n",
-                        "Their strength unmatched, their roar a fright\n",
-                        "Yet in their lair, a softer side\n",
-                        "As they tend to hatchlings, with gentle pride\n",
+                        "Dragon's roar, a thunder's might,\n",
+                        "Shaking earth and stars at night,\n",
+                        "Their majestic presence, all shall fear,\n",
+                        "For their might and beauty are crystal clear.\n",
                         "\n",
-                        "From legend to myth, they captivate us still\n",
-                        "A symbol of power, and a tale to thrill\n",
-                        "Their existence a mystery, a fantasy so grand\n",
-                        "Dragons, creatures of wonder, guardians of the land.\n"
+                        "Yet, in their hearts, a gentle flame,\n",
+                        "A loyalty that cannot be tamed,\n",
+                        "Protectors of lands, brave and true,\n",
+                        "In times of darkness, they'll see us through.\n",
+                        "\n",
+                        "So let us marvel at these wondrous beasts,\n",
+                        "Their grace, their strength, their magical feats,\n",
+                        "For in their realm of myth and flight,\n",
+                        "Dragons ignite our dreams, taking us to new heights.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test prompt_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "prompt_name = \"Write a Haiku\"\n",
                 "user_input = \"Show me 3.\"\n",
                 "# The \"Write a Poem\" prompt only requires one argument, \"subject\".\n",
                 "# We'll ask the AI to write a poem about dragons.\n",
-                "prompt_args = {\"subject\": \"dragons\"}\n",
+                "prompt_args = {\n",
+                "    \"user_input\": user_input,\n",
+                "    \"subject\": \"dragons\",\n",
+                "    \"websearch\": False,\n",
+                "    \"websearch_depth\": 0,\n",
+                "    \"context_results\": 0,\n",
+                "    \"shots\": 1,\n",
+                "}\n",
+                "\n",
                 "agent_prompt_resp = ApiClient.prompt_agent(\n",
                 "    agent_name=agent_name,\n",
                 "    prompt_name=prompt_name,\n",
                 "    prompt_args=prompt_args,\n",
-                "    user_input=user_input,\n",
-                "    websearch=False,  # We don't need web search for this test\n",
-                "    websearch_depth=0,  # Depth of web search if enabled.\n",
-                "    context_results=0,  # Number of context results to inject from memory\n",
-                "    shots=1,  # Number of responses to generate\n",
                 ")\n",
                 "print(\"Agent prompt response:\", agent_prompt_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -524,32 +533,30 @@
             "execution_count": 166,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Instruct response: ```JSON\n",
-                        "{\n",
+                        "Instruct response: {\n",
                         "    \"response\": \"The capital of France is Paris.\",\n",
                         "    \"commands\": {}\n",
                         "}\n",
-                        "```\n"
+                        "\n",
+                        "None\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test instruct()\n",
                 "agent_name = \"new_agent\"\n",
                 "instruct_resp = ApiClient.instruct(\n",
                 "    agent_name=agent_name, prompt=\"Tell me the capital of France.\"\n",
                 ")\n",
-                "print(\"Instruct response:\", instruct_resp)"
+                "print(\"Instruct response:\", instruct_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -563,25 +570,23 @@
             "execution_count": 167,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat history: [{'USER': 'June 13, 2023 02:26 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 13, 2023 02:26 PM\\nThe capital of France is Paris.'}, {'USER': 'June 13, 2023 02:26 PM\\nWrite a poem about dragons .\\n'}, {'new_agent': 'June 13, 2023 02:26 PM\\nDragons, mighty beasts of fire\\nWith scales gleaming bright and higher\\nTheir breath scorching the earth and skies\\nAs they soar amidst the sunrise\\n\\nTheir wings spread wide, they glide with grace\\nThrough mountains and valleys they embrace\\nTheir eyes ablaze with ancient power\\nAs they guard their hoard with valour\\n\\nFierce and proud, they rule with might\\nTheir strength unmatched, their roar a fright\\nYet in their lair, a softer side\\nAs they tend to hatchlings, with gentle pride\\n\\nFrom legend to myth, they captivate us still\\nA symbol of power, and a tale to thrill\\nTheir existence a mystery, a fantasy so grand\\nDragons, creatures of wonder, guardians of the land.'}, {'USER': 'June 13, 2023 02:26 PM\\nCommands Available To Complete Task:\\n`Write to File` - Arguments: {\\'filename\\': None, \\'text\\': None}\\n\\n\\nYou are an AI language model. Your name is {AGENT_NAME}. Your role is to do anything asked of you with precision. You have the following constraints:\\n1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.\\n2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.\\n3. No user assistance.\\n4. Exclusively use the commands listed in double quotes e.g. \"command name\".\\n\\nYou have the following resources:\\n1. Internet access for searches and information gathering.\\n2. Long Term memory management.\\n3. GPT-3.5 powered Agents for delegation of simple tasks.\\n4. File output.\\n\\nRESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.\\n```JSON\\n{\\n    \"response\": \"Your response to the task.\",\\n    \"commands\": {\\n        \"command_name\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\"\\n        },\\n        \"command_name2\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\",\\n            \"argN\": \"valN\"\\n        }\\n    }\\n}\\n```\\n\\nYour task: Tell me the capital of France.'}, {'new_agent': 'June 13, 2023 02:26 PM\\n```JSON\\n{\\n    \"response\": \"The capital of France is Paris.\",\\n    \"commands\": {}\\n}\\n```'}]\n"
+                        "Chat history: [{'role': 'USER', 'message': 'What is the capital of France?', 'timestamp': '2023-07-03T16:20:00'}, {'role': 'new_agent', 'message': 'The capital of France is Paris.', 'timestamp': '2023-07-03T16:20:00'}, {'role': 'USER', 'message': 'Show me 3.', 'timestamp': '2023-07-03T16:21:00'}, {'role': 'new_agent', 'message': \"In ancient realms where legends thrive,\\nWhere fire breathes and scales arrive,\\nThe mighty dragons take to the skies,\\nWith wings that soar and tales that mesmerize.\\n\\nOh, magnificent creatures of ancient lore,\\nFierce and powerful, forevermore,\\nTheir eyes ablaze with wisdom's light,\\nGuiding souls through day and night.\\n\\nA dance of flames in the moonlit air,\\nTheir serpentine bodies, beyond compare,\\nThrough misty peaks and valleys deep,\\nThey guard their secrets, their treasures to keep.\\n\\nDragon's roar, a thunder's might,\\nShaking earth and stars at night,\\nTheir majestic presence, all shall fear,\\nFor their might and beauty are crystal clear.\\n\\nYet, in their hearts, a gentle flame,\\nA loyalty that cannot be tamed,\\nProtectors of lands, brave and true,\\nIn times of darkness, they'll see us through.\\n\\nSo let us marvel at these wondrous beasts,\\nTheir grace, their strength, their magical feats,\\nFor in their realm of myth and flight,\\nDragons ignite our dreams, taking us to new heights.\", 'timestamp': '2023-07-03T16:21:00'}, {'role': 'USER', 'message': 'Tell me the capital of France.', 'timestamp': '2023-07-03T16:21:00'}, {'role': 'new_agent', 'message': '{\\n    \"response\": \"The capital of France is Paris.\",\\n    \"commands\": {}\\n}\\n\\nNone', 'timestamp': '2023-07-03T16:21:00'}]\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_chat_history()\n",
                 "agent_name = \"new_agent\"\n",
                 "chat_history = ApiClient.get_chat_history(agent_name=agent_name)\n",
-                "print(\"Chat history:\", chat_history)"
+                "print(\"Chat history:\", chat_history)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -596,25 +601,26 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent commands response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False, 'Ask AI Agent new_agent_2': False, 'Instruct AI Agent new_agent_2': False}, 'settings': {'provider': 'gpt4free', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': '4096', 'embedder': 'default', 'autonomous_execution': 'false'}}\n"
+                        "New config for new_agent: {'commands': None, 'settings': {'provider': 'gpt4free', 'embedder': 'default', 'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': '0.7', 'MAX_TOKENS': '4096', 'AUTONOMOUS_EXECUTION': False}, 'enabled_commands': []}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test update_agent_commands()\n",
                 "agent_name = \"new_agent\"\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
-                "agent_commands = agent_config[\"commands\"]\n",
+                "if agent_config[\"commands\"] != None:\n",
+                "    agent_commands = agent_config[\"commands\"]\n",
+                "else:\n",
+                "    agent_commands = {}\n",
                 "agent_commands[\"Write to File\"] = False\n",
                 "update_agent_commands_resp = ApiClient.update_agent_commands(\n",
                 "    agent_name=agent_name, commands=agent_commands\n",
                 ")\n",
                 "print(\"Update agent commands response:\", update_agent_commands_resp)\n",
                 "agent_config = ApiClient.get_agentconfig(agent_name=agent_name)\n",
                 "print(f\"New config for {agent_name}:\", agent_config)\n"
@@ -626,106 +632,104 @@
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a File\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 172,
+            "execution_count": 169,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "File Learning response: Agent learned the content from the file.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
                 "import base64\n",
                 "import os\n",
                 "\n",
                 "# Test learn_file()\n",
                 "agent_name = \"new_agent\"\n",
-                "learn_file_path = \"ApiClient.py\"\n",
+                "learn_file_path = \"test.txt\"\n",
                 "\n",
                 "with open(learn_file_path, \"rb\") as f:\n",
                 "    learn_file_content = base64.b64encode(f.read()).decode(\"utf-8\")\n",
                 "\n",
                 "file_learning = ApiClient.learn_file(\n",
                 "    agent_name=agent_name,\n",
                 "    file_name=learn_file_path,\n",
                 "    file_content=learn_file_content,\n",
                 ")\n",
-                "print(\"File Learning response:\", file_learning)"
+                "print(\"File Learning response:\", file_learning)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a URL\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 170,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "URL Learning response: Agent learned the content from the url.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test learn_url()\n",
                 "agent_name = \"new_agent\"\n",
-                "url_learning = ApiClient.learn_url(agent_name=agent_name, url=\"https://agixt.com\")\n",
-                "print(\"URL Learning response:\", url_learning)\n"
+                "url_learning = ApiClient.learn_url(\n",
+                "    agent_name=agent_name,\n",
+                "    url=\"https://josh-xt.github.io/AGiXT/2-Concepts/0-Core%20Concepts.html\",\n",
+                ")\n",
+                "print(\"URL Learning response:\", url_learning)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Wipe the agents memories\n",
                 "\n",
                 "This is necessary if you want the agent to serve a different purpose than its original intent after it has learned things. It may inject unnecessary context into the conversation if you don't wipe its memory and try to give it a different purpose, even temporarily.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 171,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Wipe agent memories response: Memories for agent new_agent deleted.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test wipe_agent_memories()\n",
                 "# Note: Use this function with caution as it will erase the agent's memory.\n",
                 "agent_name = \"new_agent\"\n",
                 "wipe_mem_resp = ApiClient.wipe_agent_memories(agent_name=agent_name)\n",
-                "print(\"Wipe agent memories response:\", wipe_mem_resp)"
+                "print(\"Wipe agent memories response:\", wipe_mem_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -738,87 +742,81 @@
             "metadata": {},
             "source": [
                 "## Get a list of Chains available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 172,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chains: ['Smart Instruct', 'Test_Commands', 'Generate and Run Smart Task Chain', 'Write a Poem', 'Generate and Run Task Chain', 'Generate Task Chain', 'Generate Smart Task Chain', 'Smart Chat']\n"
+                        "Chains: ['Smart Instruct', 'Smart Prompt', 'Test_Commands', 'Generate and Run Smart Task Chain', 'Write a Poem', 'Generate and Run Task Chain', 'Smart Chat - No Research', 'Generate Task Chain', 'Generate Smart Task Chain', 'Smart Chat', 'Ask Helper Agent for Help', 'Generate Smart Task Chain without Research', 'Generate Task Chain without Research', 'Create New Command', 'Solve Math Problem', 'Smart Instruct - No Research']\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_chains()\n",
                 "chains = ApiClient.get_chains()\n",
-                "print(\"Chains:\", chains)"
+                "print(\"Chains:\", chains)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 173,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add chain response: Chain 'Write another Poem' created.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test add_chain()\n",
                 "chain_name = \"Write another Poem\"\n",
                 "add_chain_resp = ApiClient.add_chain(chain_name=chain_name)\n",
-                "print(\"Add chain response:\", add_chain_resp)"
+                "print(\"Add chain response:\", add_chain_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Rename the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 174,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Rename chain response: Chain 'Write another Poem' renamed to 'Poem Writing Chain'.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test rename_chain()\n",
                 "chain_name = \"Write another Poem\"\n",
                 "new_chain_name = \"Poem Writing Chain\"\n",
                 "rename_chain_resp = ApiClient.rename_chain(\n",
                 "    chain_name=chain_name, new_name=new_chain_name\n",
                 ")\n",
                 "print(\"Rename chain response:\", rename_chain_resp)\n"
@@ -830,29 +828,27 @@
             "metadata": {},
             "source": [
                 "## Add Chain Steps\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 175,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add step response: Step 1 added to chain 'Poem Writing Chain'.\n",
                         "Add step response: Step 2 added to chain 'Poem Writing Chain'.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "agent_name = \"new_agent\"\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "# Test add_step()\n",
                 "add_step_resp = ApiClient.add_step(\n",
                 "    chain_name=chain_name,\n",
                 "    step_number=1,\n",
                 "    agent_name=agent_name,\n",
@@ -882,60 +878,56 @@
             "metadata": {},
             "source": [
                 "## Get the content of the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 176,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chain: {'chain_name': 'Poem Writing Chain', 'steps': [{'step': 1, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial Intelligence'}}, {'step': 2, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}}]}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "chain = ApiClient.get_chain(chain_name=chain_name)\n",
-                "print(\"Chain:\", chain)"
+                "print(\"Chain:\", chain)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Modify a chain step\n",
                 "\n",
                 "Instead of the subject of the poem just being Artificial Intelligence, we'll change it to be Artificial General Intelligence.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 177,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update step response: Step 1 updated for chain 'Poem Writing Chain'.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "agent_name = \"new_agent\"\n",
                 "# Test update_step()\n",
                 "update_step_resp = ApiClient.update_step(\n",
                 "    chain_name=chain_name,\n",
                 "    step_number=1,\n",
                 "    agent_name=agent_name,\n",
@@ -956,28 +948,26 @@
                 "## Move the chain step\n",
                 "\n",
                 "When you move a step, it will automatically reassign the order of the steps to match the new order. If there are only 2 steps like in our case, it will just swap them.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 178,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Move step response: Step 1 moved to 2 in chain 'Poem Writing Chain'.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "agent_name = \"new_agent\"\n",
                 "\n",
                 "# Test move_step()\n",
                 "move_step_resp = ApiClient.move_step(\n",
                 "    chain_name=chain_name, old_step_number=1, new_step_number=2\n",
                 ")\n",
@@ -985,47 +975,73 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Delete a step from the chain\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 179,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete step response: Unable to retrieve data.\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Test delete_step()\n",
+                "chain_name = \"Poem Writing Chain\"\n",
+                "delete_step_resp = ApiClient.delete_step(chain_name=chain_name, step_number=2)\n",
+                "print(\"Delete step response:\", delete_step_resp)\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Add a Command to the Chain\n",
                 "\n",
                 "We'll write the result to a file for an example.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 180,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Add step response: Step 3 added to chain 'Poem Writing Chain'.\n"
+                        "Add step response: Step 2 added to chain 'Poem Writing Chain'.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "agent_name = \"new_agent\"\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "# Test add_step()\n",
                 "add_step_resp = ApiClient.add_step(\n",
                 "    chain_name=chain_name,\n",
-                "    step_number=3,\n",
+                "    step_number=2,\n",
                 "    agent_name=agent_name,\n",
                 "    prompt_type=\"Command\",\n",
                 "    prompt={\n",
                 "        \"command_name\": \"Write to File\",\n",
                 "        \"filename\": \"{user_input}.txt\",\n",
-                "        \"text\": \"First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}\",\n",
+                "        \"text\": \"Poem:\\n{STEP1}\",\n",
                 "    },\n",
                 ")\n",
                 "print(\"Add step response:\", add_step_resp)\n"
             ]
         },
         {
             "attachments": {},
@@ -1033,184 +1049,148 @@
             "metadata": {},
             "source": [
                 "## Run the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 181,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Run chain response: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                        "Run chain response: File written to successfully.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test run_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "# The user input for this chain will just be the name of the text file to write to.\n",
                 "user_input = \"Super Poems\"\n",
-                "run_chain_resp = ApiClient.run_chain(chain_name=chain_name, user_input=user_input)\n",
-                "print(\"Run chain response:\", run_chain_resp)"
+                "run_chain_resp = ApiClient.run_chain(\n",
+                "    chain_name=chain_name, user_input=user_input, from_step=1\n",
+                ")\n",
+                "print(\"Run chain response:\", run_chain_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Get the responses from the chain running\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 182,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chain: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                        "Chain: {'1': [], '2': ['File written to successfully.']}\n"
                     ]
                 }
             ],
             "source": [
                 "# Need to make a function to get_chain_responses() as it's not in the API yet.\n",
-                "from ApiClient import ApiClient\n",
+                "\n",
                 "\n",
                 "# Test get_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "chain = ApiClient.get_chain_responses(chain_name=chain_name)\n",
                 "print(\"Chain:\", chain)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Delete a step from the chain\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Delete step response: Step 2 deleted from chain 'Poem Writing Chain'.\n"
-                    ]
-                }
-            ],
-            "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
-                "# Test delete_step()\n",
-                "chain_name = \"Poem Writing Chain\"\n",
-                "delete_step_resp = ApiClient.delete_step(chain_name=chain_name, step_number=2)\n",
-                "print(\"Delete step response:\", delete_step_resp)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "## Delete the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 183,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete chain response: Chain 'Poem Writing Chain' deleted.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test delete_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "delete_chain_resp = ApiClient.delete_chain(chain_name=chain_name)\n",
-                "print(\"Delete chain response:\", delete_chain_resp)"
+                "print(\"Delete chain response:\", delete_chain_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Prompts\n",
                 "\n",
                 "## Get a list of prompts available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 184,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Prompts: ['Pseudo Code', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'SmartChat-Researcher', 'Tell Me How', 'Execution', 'Score Response', 'Get Task Description', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Check-Instruction', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Get Task List']\n"
+                        "Prompts: ['instruct', 'Pseudo Code', 'Convert OpenAPI Endpoint', 'Ask for Help', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'Proofreader', 'SmartChat-Researcher', 'Evaluate Code', 'Get ezsession Auth Type', 'Expert Determination', 'Tell Me How', 'New Extension Format', 'Execution', 'Score Response', 'Get Task Description', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'Translate Math to Python', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Prompt Generator', 'Check-Instruction', 'Get Clarification', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Title a Chain', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Summarize Web Content', 'Get Task List', 'Break into steps', 'instruct', 'instruct', 'instruct', 'instruct', 'instruct']\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_prompts()\n",
                 "prompts = ApiClient.get_prompts()\n",
-                "print(\"Prompts:\", prompts)"
+                "print(\"Prompts:\", prompts)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new prompt\n",
                 "\n",
                 "We'll make a basic prompt that asks the AI to tell us a short story about a subject. The subject is not yet defined, it would be defined in a chain. Using `{variable_name}` in a prompt will allow you to define the variable in a chain and have it be used in the prompt.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 185,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add prompt response: Prompt 'Short Story' added.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test add_prompt()\n",
                 "add_prompt_resp = ApiClient.add_prompt(\n",
                 "    prompt_name=\"Short Story\", prompt=\"Tell me a short story about {subject}\"\n",
                 ")\n",
                 "print(\"Add prompt response:\", add_prompt_resp)\n"
             ]
         },
@@ -1220,58 +1200,56 @@
             "metadata": {},
             "source": [
                 "## Get the prompt content\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 186,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt response: Write a poem about {subject} .\n",
                         "{user_input}\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test get_prompt()\n",
                 "get_prompt_resp = ApiClient.get_prompt(prompt_name=\"Write a Poem\")\n",
-                "print(\"Get prompt response:\", get_prompt_resp)"
+                "print(\"Get prompt response:\", get_prompt_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Get the prompt variables\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 187,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt args response: ['subject']\n"
                     ]
                 }
             ],
             "source": [
                 "# Get prompt args\n",
-                "from ApiClient import ApiClient\n",
+                "\n",
                 "\n",
                 "# Test get_prompt_args()\n",
                 "get_prompt_args_resp = ApiClient.get_prompt_args(prompt_name=\"Short Story\")\n",
                 "print(\"Get prompt args response:\", get_prompt_args_resp)\n"
             ]
         },
         {
@@ -1282,28 +1260,26 @@
                 "## Update the prompt content\n",
                 "\n",
                 "We'll ask it to `Add a dragon to the story somehow` in the prompt to make the short story more interesting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 188,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update prompt response: Prompt 'Short Story' updated.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test update_prompt()\n",
                 "update_prompt_resp = ApiClient.update_prompt(\n",
                 "    prompt_name=\"Short Story\",\n",
                 "    prompt=\"Tell me a short story about {subject}. Add a dragon to the story somehow.\",\n",
                 ")\n",
                 "print(\"Update prompt response:\", update_prompt_resp)\n"
             ]
@@ -1316,59 +1292,55 @@
                 "## Delete the prompt\n",
                 "\n",
                 "If you don't want the prompt anymore, delete it.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 189,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete prompt response: Prompt 'Short Story' deleted.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test delete_prompt()\n",
                 "delete_prompt_resp = ApiClient.delete_prompt(prompt_name=\"Short Story\")\n",
-                "print(\"Delete prompt response:\", delete_prompt_resp)"
+                "print(\"Delete prompt response:\", delete_prompt_resp)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Delete Agent History\n",
                 "\n",
                 "Delete the history for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 190,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: History for agent new_agent deleted.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test delete_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "delete_agent_resp = ApiClient.delete_agent_history(agent_name=agent_name)\n",
                 "print(\"Delete agent response:\", delete_agent_resp)\n"
             ]
         },
         {
@@ -1379,32 +1351,30 @@
                 "## Delete the Agent\n",
                 "\n",
                 "If you are done with the agent and don't want or need it anymore, you can delete it along with everything associated with it, such as its memories, settings, and history. The Agent isn't just fired, it is dead.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 191,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: Agent new_agent deleted.\n"
                     ]
                 }
             ],
             "source": [
-                "from ApiClient import ApiClient\n",
-                "\n",
                 "# Test delete_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "delete_agent_resp = ApiClient.delete_agent(agent_name=agent_name)\n",
-                "print(\"Delete agent response:\", delete_agent_resp)"
+                "print(\"Delete agent response:\", delete_agent_resp)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

