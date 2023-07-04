# Comparing `tmp/chatgpt-tool-hub-0.4.5.tar.gz` & `tmp/chatgpt-tool-hub-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.4.5.tar", last modified: Sun Jun 11 16:29:23 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.4.6.tar", last modified: Tue Jul  4 16:37:52 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.4.5.tar` & `chatgpt-tool-hub-0.4.6.tar`

### file list

```diff
@@ -1,163 +1,159 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.016620 chatgpt-tool-hub-0.4.5/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.5/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-06-11 16:29:23.016401 chatgpt-tool-hub-0.4.5/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    13902 2023-05-04 15:37:21.000000 chatgpt-tool-hub-0.4.5/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.989922 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.991733 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2516 2023-05-04 17:20:51.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2874 2023-05-12 01:12:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.992380 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/all_bot_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.992991 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11410 2023-05-15 14:37:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2310 2023-05-15 15:34:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.993622 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4988 2023-05-15 14:37:53.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.994250 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.994783 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-05-15 15:34:57.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.997401 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/config.py
--rw-r--r--   0 goldfish   (502) staff       (20)      359 2023-05-12 01:00:31.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/json_utils.py
--rw-r--r--   0 goldfish   (502) staff       (20)      859 2023-05-13 16:15:44.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.998260 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.999187 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/
--rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12786 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/initialize.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-27 15:08:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/tool_engine.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.999925 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)     2766 2023-05-20 10:34:57.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.000818 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4872 2023-05-04 10:03:38.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    16231 2023-05-20 10:32:17.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/chatgpt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.001214 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/dashscope/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:59:11.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/dashscope/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      903 2023-05-04 10:14:15.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/model_factory.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.001340 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/moss/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:58:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/moss/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.002313 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.003453 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)     1395 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/all_tool_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.004246 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/
--rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2937 2023-05-05 15:15:58.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.004878 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.005445 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.005916 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/
--rw-r--r--   0 goldfish   (502) staff       (20)       60 2023-05-04 14:00:20.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1070 2023-05-04 13:53:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.006646 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5263 2023-04-26 16:51:21.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1965 2023-05-06 18:07:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.007100 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      884 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.007583 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.008421 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3142 2023-05-12 01:24:50.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.008892 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/
--rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2257 2023-05-12 01:22:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.009183 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.009721 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.010450 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/
--rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/map_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/reduce_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7304 2023-05-15 14:53:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.011122 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/
--rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/answer_user.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.011809 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-28 11:33:01.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)      916 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool_register.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.012363 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/
--rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2377 2023-04-28 11:33:15.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/text2image.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.014043 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     2397 2023-04-26 15:57:51.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5173 2023-05-05 16:21:45.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.015319 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.016124 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-06-11 16:27:47.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.990621 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     5003 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-06-11 16:29:23.016664 chatgpt-tool-hub-0.4.5/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.5/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.625126 chatgpt-tool-hub-0.4.6/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.6/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-07-04 16:37:52.624922 chatgpt-tool-hub-0.4.6/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    13902 2023-07-04 16:13:08.000000 chatgpt-tool-hub-0.4.6/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.610777 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.612067 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2516 2023-05-04 17:20:51.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2874 2023-05-12 01:12:49.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.612301 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/all_bot_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.612623 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11410 2023-05-15 14:37:49.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2310 2023-05-15 15:34:09.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.612933 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4988 2023-05-15 14:37:53.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.613263 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.613585 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-05-15 15:34:57.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.615257 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2668 2023-07-04 16:34:08.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/config.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      359 2023-05-12 01:00:31.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/json_utils.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      859 2023-05-13 16:15:44.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.615708 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.616157 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/
+-rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12786 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/initialize.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-27 15:08:27.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/tool_engine.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.616467 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2764 2023-07-04 16:31:02.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.616794 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4872 2023-05-04 10:03:38.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    16227 2023-07-02 16:26:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      941 2023-07-04 16:10:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/model_factory.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.617215 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.617860 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1395 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.618288 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2937 2023-05-05 15:15:58.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.618610 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.618929 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.619163 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/hello_tool/
+-rw-r--r--   0 goldfish   (502) staff       (20)       60 2023-05-04 14:00:20.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/hello_tool/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1070 2023-05-04 13:53:09.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/hello_tool/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.619501 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5263 2023-04-26 16:51:21.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1965 2023-05-06 18:07:09.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.619737 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      884 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.620055 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/finance_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/finance_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/finance_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.620650 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3142 2023-05-12 01:24:50.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.621134 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/
+-rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2257 2023-05-12 01:22:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.621378 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/python/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.621784 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.622298 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/
+-rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/map_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/reduce_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7381 2023-06-26 16:58:34.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.622621 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/
+-rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/answer_user.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/debug.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.622840 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-28 11:33:01.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      916 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/tool_register.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.623064 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2377 2023-04-28 11:33:15.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.623955 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2397 2023-04-26 15:57:51.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5173 2023-05-05 16:21:45.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.624276 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.624705 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-07-04 16:24:41.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-07-04 16:37:52.611465 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-07-04 16:37:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     4916 2023-07-04 16:37:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-07-04 16:37:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-07-04 16:37:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-07-04 16:37:52.000000 chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-07-04 16:37:52.625164 chatgpt-tool-hub-0.4.6/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-07-04 16:33:13.000000 chatgpt-tool-hub-0.4.6/setup.py
```

### Comparing `chatgpt-tool-hub-0.4.5/LICENSE` & `chatgpt-tool-hub-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/PKG-INFO` & `chatgpt-tool-hub-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.5
+Version: 0.4.6
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.5/README.md` & `chatgpt-tool-hub-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app_factory.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/app_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/lite_app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/apps/victorinox.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/chat_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/bots/qa_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/calculate_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 from chatgpt_tool_hub.common.log import LOG
 
 
 # refer to https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
-def count_message_tokens(messages, model: str = "gpt-3.5-turbo"):
-    """Returns the number of tokens used by a list of messages."""
+
+def count_message_tokens(messages, model="gpt-3.5-turbo-0613"):
     import tiktoken
+
+    if model.startswith("gpt-35"):
+        model = model.replace("gpt-35-", "gpt-3.5-")
+
+    """Return the number of tokens used by a list of messages."""
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         LOG.debug("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model == "gpt-3.5-turbo":
-        return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
-    elif model == "gpt-4":
-        return count_message_tokens(messages, model="gpt-4-0314")
+    if model in {
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k-0613",
+        "gpt-4-0314",
+        "gpt-4-32k-0314",
+        "gpt-4-0613",
+        "gpt-4-32k-0613",
+        }:
+        tokens_per_message = 3
+        tokens_per_name = 1
     elif model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         tokens_per_name = -1  # if there's a name, the role is omitted
-    elif model == "gpt-4-0314":
-        tokens_per_message = 3
-        tokens_per_name = 1
+    elif "gpt-3.5-turbo" in model:
+        LOG.debug("Warning: gpt-3.5-turbo may update over time. Returning num tokens assuming gpt-3.5-turbo-0613.")
+        return count_message_tokens(messages, model="gpt-3.5-turbo-0613")
+    elif "gpt-4" in model:
+        LOG.debug("Warning: gpt-4 may update over time. Returning num tokens assuming gpt-4-0613.")
+        return count_message_tokens(messages, model="gpt-4-0613")
     else:
-        LOG.warn(f"count_message_tokens() is not implemented for model {model}. "
-                 f"Returning num tokens assuming gpt-3.5-turbo-0301.")
-        return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
+        raise NotImplementedError(
+            f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
+        )
     num_tokens = 0
     for message in messages:
         num_tokens += tokens_per_message
         for key, value in message.items():
             num_tokens += len(encoding.encode(value))
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
 
-def count_string_tokens(string: str, model_name: str = "gpt-3.5-turbo") -> int:
+def count_string_tokens(string: str, model_name: str = "gpt-35-turbo") -> int:
     """
     Returns the number of tokens in a text string.
 
     Args:
     string (str): The text string.
-    model_name (str): The name of the encoding to use. (e.g., "gpt-3.5-turbo")
+    model_name (str): The name of the encoding to use. (e.g., "gpt-35-turbo")
 
     Returns:
     int: The number of tokens in the text string.
     """
     import tiktoken
+
+    if model_name.startswith("gpt-35"):
+        model_name = model_name.replace("gpt-35-", "gpt-3.5-")
+
     encoding = tiktoken.encoding_for_model(model_name)
     return len(encoding.encode(string))
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/json_utils.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/log.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/log.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/utils.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/common/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/bot.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/bot.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/initialize.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/initialize.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/tool_engine.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/engine/tool_engine.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/__init__.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from chatgpt_tool_hub.common.cache import BaseCache
 from chatgpt_tool_hub.common.constants import openai_default_api_base
 from chatgpt_tool_hub.common.utils import get_from_dict_or_env
 
 verbose: bool = False
 llm_cache: Optional[BaseCache] = None
 
-# default for gpt-3.5
+# default for gpt-35
 ALL_MAX_TOKENS_NUM = 4000
 
 # token manage strategy
 BOT_PROMPT = 1000
 MEMORY_MAX_TOKENS_NUM = 600
 BOT_SCRATCHPAD_MAX_TOKENS_NUM = ALL_MAX_TOKENS_NUM - BOT_PROMPT - MEMORY_MAX_TOKENS_NUM - 200
 
@@ -22,15 +22,15 @@
     MEMORY_MAX_TOKENS_NUM = memory_max_tokens_num
     BOT_SCRATCHPAD_MAX_TOKENS_NUM = ALL_MAX_TOKENS_NUM - BOT_PROMPT - MEMORY_MAX_TOKENS_NUM - 200
 
 
 def build_model_params(kwargs: dict) -> dict:
     _api_key = get_from_dict_or_env(kwargs, "llm_api_key", "LLM_API_KEY")
     _proxy = get_from_dict_or_env(kwargs, "proxy", "PROXY", "")
-    _model = get_from_dict_or_env(kwargs, "model_name", "MODEL_NAME", "gpt-3.5-turbo")
+    _model = get_from_dict_or_env(kwargs, "model_name", "MODEL_NAME", "gpt-35-turbo")
     _timeout = get_from_dict_or_env(kwargs, "request_timeout", "REQUEST_TIMEOUT", 120)
     _llm_api_base_url = get_from_dict_or_env(kwargs, "llm_api_base_url", "LLM_API_BASE_URL", openai_default_api_base)
     _deployment_id = get_from_dict_or_env(kwargs, "deployment_id", "DEPLOYMENT_ID", "")
 
     # tool llm need them
     os.environ["LLM_API_KEY"] = str(_api_key)
     if _proxy and not _proxy.startswith("http://") and not _proxy.startswith("https://"):
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,20 @@
     Any parameters that are valid to be passed to the openai.create call can be passed
     in, even if not explicitly saved on this class.
 
     Example:
         .. code-block:: python
 
             from lib.chat_models import ChatOpenAI
-            openai = ChatOpenAI(model_name="gpt-3.5-turbo")
+            openai = ChatOpenAI(model_name="gpt-35-turbo")
     """
 
     client: Any  #: :meta private:
     """Model name to use."""
-    model_name: str = "gpt-3.5-turbo"
+    model_name: str = "gpt-35-turbo"
     """Holds any model parameters valid for `create` call not explicitly specified."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """llm api base url"""
     llm_api_base_url: str = openai_default_api_base
     """a key to call llm api server"""
     llm_api_key: Optional[str] = None
     """Timeout in seconds for the OpenAPI request."""
@@ -363,42 +363,42 @@
             import tiktoken
         except ImportError:
             raise ValueError(
                 "Could not import tiktoken python package. "
                 "This is needed in order to calculate get_num_tokens. "
                 "Please it install it with `pip install tiktoken`."
             )
-        # create a GPT-3.5-Turbo encoder instance
+        # create a gpt-35-Turbo encoder instance
         enc = tiktoken.encoding_for_model(self.model_name)
 
-        # encode the text using the GPT-3.5-Turbo encoder
+        # encode the text using the gpt-35-Turbo encoder
         tokenized_text = enc.encode(text)
 
         # calculate the number of tokens in the encoded text
         return len(tokenized_text)
 
     def get_num_tokens_from_messages(
-        self, messages: List[BaseMessage], model: str = "gpt-3.5-turbo-0301"
+        self, messages: List[BaseMessage], model: str = "gpt-35-turbo"
     ) -> int:
-        """Calculate num tokens for gpt-3.5-turbo with tiktoken package."""
+        """Calculate num tokens for gpt-35-turbo with tiktoken package."""
         try:
             import tiktoken
         except ImportError:
             raise ValueError(
                 "Could not import tiktoken python package. "
                 "This is needed in order to calculate get_num_tokens. "
                 "Please it install it with `pip install tiktoken`."
             )
 
         """Returns the number of tokens used by a list of messages."""
         try:
             encoding = tiktoken.encoding_for_model(model)
         except KeyError:
             encoding = tiktoken.get_encoding("cl100k_base")
-        if model != "gpt-3.5-turbo-0301":
+        if not model.startswith("gpt-35-turbo"):
             raise NotImplementedError(
                 f"get_num_tokens_from_messages() is not presently implemented "
                 f"for model {model}."
                 "See https://github.com/openai/openai-python/blob/main/chatml.md for "
                 "information on how messages are converted to tokens."
             )
         num_tokens = 0
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/model_factory.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/models/model_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
     def __init__(self):
         self.available_models_prefix = {
             "text-davinci": "chatgpt",
             "gpt-3.5-turbo": "chatgpt",
             "gpt-4": "chatgpt",
             "gpt-4-32k": "chatgpt",
+            "gpt-35-turbo": "chatgpt",
         }
         pass
 
     def match_model(self, name: str) -> str:
         for k, v in self.available_models_prefix.items():
             if name.startswith(k):
                 return v
         return ""
 
     def create_llm_model(self, **model_kwargs):
-        _model = get_from_dict_or_env(model_kwargs, "model_name", "MODEL_NAME", "gpt-3.5-turbo")
+        _model = get_from_dict_or_env(model_kwargs, "model_name", "MODEL_NAME", "gpt-35-turbo")
         match_llm_model = self.match_model(_model)
         if match_llm_model == "chatgpt":
             return ChatOpenAI(**model_kwargs)
         else:
             raise NotImplementedError("implement me!")
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/__init__.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/arxiv_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/hello_tool/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/load_tools.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/docs_prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/meteo/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/__init__.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/finance_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/morning_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/news_api/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/searxng_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/map_prompt.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/map_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/summary/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,19 +138,21 @@
         with open(file_path, "r") as f:
             source_text = f.read()
 
         _text = source_text
         ctn = 0
         while get_token_num(_text) >= self.max_segment_length:
             ctn += 1
-            if ctn > 8:
+            if ctn > 3:
                 LOG.warning(f"[summary] 我已经map-reduce {ctn}轮了，但是文本量还是很长，避免死循环我帮你关掉了~")
+                break
             # map
             _clip_text_list = _clipper.clip(_text, self.message_num)
             # async call llm to get summary of each clip_text
+            # TODO need stop when receive reset signal
             map_text_list = asyncio.run(self._acall(self.map_bot, _clip_text_list))
             map_text = _clipper.seperator.join(map_text_list)
 
             LOG.debug(f"[summary] round:{ctn}, map_list: {map_text}")
             # reduce
             _clip_summary_list = _clipper.clip(map_text, self.message_num)
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/answer_user.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/answer_user.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/debug.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/system/debug.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool_register.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/tool_register.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/text2image.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/visual_dl/text2image.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/browser.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/get.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/get.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/post.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/web_requests/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.5
+Version: 0.4.6
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.4.6/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,14 @@
 chatgpt_tool_hub/engine/tool_engine.py
 chatgpt_tool_hub/models/__init__.py
 chatgpt_tool_hub/models/base.py
 chatgpt_tool_hub/models/model_factory.py
 chatgpt_tool_hub/models/chatgpt/__init__.py
 chatgpt_tool_hub/models/chatgpt/base.py
 chatgpt_tool_hub/models/chatgpt/chatgpt.py
-chatgpt_tool_hub/models/dashscope/__init__.py
-chatgpt_tool_hub/models/moss/__init__.py
 chatgpt_tool_hub/prompts/__init__.py
 chatgpt_tool_hub/prompts/base.py
 chatgpt_tool_hub/prompts/chat.py
 chatgpt_tool_hub/prompts/prompt.py
 chatgpt_tool_hub/tools/__init__.py
 chatgpt_tool_hub/tools/all_tool_list.py
 chatgpt_tool_hub/tools/base_tool.py
```

### Comparing `chatgpt-tool-hub-0.4.5/setup.py` & `chatgpt-tool-hub-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     install_requires=[
         'pydantic~=1.10.7',
         'pyopenssl',
         'pyyaml~=6.0',
         'lxml',
         'beautifulsoup4~=4.12.0',
         "tenacity~=8.2.2",
-        "openai~=0.27.2",
-        "tiktoken~=0.3.2",
+        "openai~=0.27.4",
+        "tiktoken~=0.4.0",
         "arxiv",
         "wikipedia",
         "wolframalpha",
         'aiohttp~=3.8.4',
         'requests~=2.28.2',
         "google-api-python-client",
         "SQLAlchemy~=2.0.7",
```

