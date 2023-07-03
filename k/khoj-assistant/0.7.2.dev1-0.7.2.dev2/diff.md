# Comparing `tmp/khoj_assistant-0.7.2.dev1.tar.gz` & `tmp/khoj_assistant-0.7.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul  3 22:55:11 2023, max compression
+gzip compressed data, last modified: Mon Jul  3 23:04:32 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev1.tar` & `khoj_assistant-0.7.2.dev2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/__init__.py
--rw-r--r--   0        0        0    10727 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/configure.py
--rw-r--r--   0        0        0     5282 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    13551 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6739 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    18662 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3583 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4065 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13481 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5392 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18352 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4646 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2385 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/LICENSE
--rw-r--r--   0        0        0    23342 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/README.md
--rw-r--r--   0        0        0     2792 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/pyproject.toml
--rw-r--r--   0        0        0    25706 2023-07-03 22:55:11.000000 khoj_assistant-0.7.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10727 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/configure.py
+-rw-r--r--   0        0        0     5282 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    15023 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    13551 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6739 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19388 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3583 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4065 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5392 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18345 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4646 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2385 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/LICENSE
+-rw-r--r--   0        0        0    23342 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/README.md
+-rw-r--r--   0        0        0     2792 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0    25706 2023-07-03 23:04:32.000000 khoj_assistant-0.7.2.dev2/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev2/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/main.py` & `khoj_assistant-0.7.2.dev2/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/chat.html`

 * *Files 4% similar despite different names*

```diff
@@ -83,31 +83,35 @@
 
         window.onload = function () {
             fetch('/api/chat?client=web')
                 .then(response => response.json())
                 .then(data => {
                     if (data.detail) {
                         // If the server returns a 500 error with detail, render it as a message.
-                        renderMessage(data.detail + " You can configure Khoj chat in your <a class='inline-chat-link' href='/config'>settings</a>.", "khoj");
+                        renderMessage("Hi 👋🏾, to get started <br/>1. Get your <a class='inline-chat-link' href='https://platform.openai.com/account/api-keys'>OpenAI API key</a><br/>2. Save it in the Khoj <a class='inline-chat-link' href='/config/processor/conversation'>chat settings</a> <br/>3. Click Configure on the Khoj <a class='inline-chat-link' href='/config'>settings page</a>", "khoj");
+
+                        // Disable chat input field and update placeholder text
+                        document.getElementById("chat-input").setAttribute("disabled", "disabled");
+                        document.getElementById("chat-input").setAttribute("placeholder", "Configure Khoj to enable chat");
+                    } else {
+                        // Set welcome message on load
+                        renderMessage("Hey 👋🏾, what's up?", "khoj");
                     }
                     return data.response;
                 })
                 .then(response => {
                     // Render conversation history, if any
                     response.forEach(chat_log => {
                         renderMessageWithReference(chat_log.message, chat_log.by, chat_log.context, new Date(chat_log.created));
                     });
                 })
                 .catch(err => {
                     return;
                 });
 
-             // Set welcome message on load
-            renderMessage("Hey, what's up?", "khoj");
-
             // Fill query field with value passed in URL query parameters, if any.
             var query_via_url = new URLSearchParams(window.location.search).get("q");
             if (query_via_url) {
                 document.getElementById("chat-input").value = query_via_url;
                 chat();
             }
         }
```

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,22 @@
         }
 
         function populate_type_dropdown() {
             // Populate type dropdown field with enabled content types only
             fetch("/api/config/types")
                 .then(response => response.json())
                 .then(enabled_types => {
+                    // Show warning if no content types are enabled
+                    if (enabled_types.detail) {
+                        document.getElementById("results").innerHTML = "<div id='results-error'>To use Khoj search, setup your content plugins on the Khoj <a class='inline-chat-link' href='/config'>settings page</a>.</div>";
+                        document.getElementById("query").setAttribute("disabled", "disabled");
+                        document.getElementById("query").setAttribute("placeholder", "Configure Khoj to enable search");
+                        return [];
+                    }
+
                     document.getElementById("type").innerHTML =
                     enabled_types
                     .map(type => `<option value="${type}">${type.slice(0,1).toUpperCase() + type.slice(1)}</option>`)
                     .join('');
 
                     return enabled_types;
                 })
@@ -403,25 +411,30 @@
 
         img.avatar {
             width: 20px;
             height: 20px;
             border-radius: 50%;
         }
 
+        div#results-error,
         div.results-markdown,
         div.results-org,
         div.results-pdf {
             text-align: left;
             box-shadow: 2px 2px 2px var(--primary-hover);
             border-radius: 5px;
             padding: 10px;
             margin: 10px 0;
             border: 4px solid rgb(229, 229, 229);
         }
 
+        div#results-error {
+            box-shadow: 2px 2px 2px #FF5722;
+        }
+
         img {
             max-width: 90%;
         }
 
         div.khoj-banner-container {
             background: linear-gradient(-45deg, #FFC107, #FF9800, #FF5722, #FF9800, #FFC107);
             background-size: 400% 400%;
@@ -477,16 +490,15 @@
                 display: block;
             }
         }
 
     </style>
     <script>
         var khojBannerSubmit = document.getElementById("khoj-banner-submit");
-
-        khojBannerSubmit.addEventListener("click", function(event) {
+        khojBannerSubmit?.addEventListener("click", function(event) {
             event.preventDefault();
             var email = document.getElementById("khoj-banner-email").value;
             fetch("https://lantern.khoj.dev/beta/users/", {
                     method: "POST",
                     body: JSON.stringify({
                         email: email
                     }),
```

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev2/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev2/src/khoj/routers/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 ):
     if (
         state.processor_config is None
         or state.processor_config.conversation is None
         or state.processor_config.conversation.openai_api_key is None
     ):
         raise HTTPException(
-            status_code=500, detail="Chat processor not configured. Configure OpenAI API key on server and restart it."
+            status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
         )
 
     # Load Conversation History
     chat_session = state.processor_config.conversation.chat_session
     meta_log = state.processor_config.conversation.meta_log
 
     # If user query is empty, return chat history
```

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.2.dev2/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev2/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev2/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev2/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/.gitignore` & `khoj_assistant-0.7.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/LICENSE` & `khoj_assistant-0.7.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/README.md` & `khoj_assistant-0.7.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/pyproject.toml` & `khoj_assistant-0.7.2.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev1/PKG-INFO` & `khoj_assistant-0.7.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev1
+Version: 0.7.2.dev2
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

