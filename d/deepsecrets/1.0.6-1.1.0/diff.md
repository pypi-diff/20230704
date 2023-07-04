# Comparing `tmp/deepsecrets-1.0.6.tar.gz` & `tmp/deepsecrets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.0.6.tar", max compression
+gzip compressed data, was "deepsecrets-1.1.0.tar", max compression
```

## Comparing `deepsecrets-1.0.6.tar` & `deepsecrets-1.1.0.tar`

### file list

```diff
@@ -1,146 +1,150 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.6/LICENSE
--rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.6/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.6/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.6/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.6/deepsecrets/__main__.py
--rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.6/deepsecrets/cli.py
--rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.6/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.6/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.6/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.6/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.0.6/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.0.6/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.6/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.6/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7459 2023-06-26 13:33:19.902788 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     4034 2023-06-26 13:33:19.226359 deepsecrets-1.0.6/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.6/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.6/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.6/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.6/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.6/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.6/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.6/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.6/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.6/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.6/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.6/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.6/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0    10200 2023-06-26 13:42:04.228723 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     6581 2023-06-27 14:19:02.007570 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     5885 2023-06-27 14:19:01.181294 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6481 2023-06-26 13:42:02.632935 deepsecrets-1.0.6/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     1841 2023-06-26 16:37:09.047505 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.6/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.6/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.6/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0     1060 2023-06-26 16:37:08.518447 deepsecrets-1.0.6/deepsecrets/core/utils/guess_filetype.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.6/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.6/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.0.6/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.6/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.6/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1646 2023-06-27 14:19:34.187662 deepsecrets-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 deepsecrets-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.1.0/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.1.0/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-07-04 12:10:29.237681 deepsecrets-1.1.0/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.1.0/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     7633 2023-07-04 11:57:11.643286 deepsecrets-1.1.0/deepsecrets/cli.py
+-rw-r--r--   0        0        0     2256 2023-07-03 10:00:00.045463 deepsecrets-1.1.0/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.1.0/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.1.0/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.1.0/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.1.0/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.1.0/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.1.0/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.1.0/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.1.0/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7355 2023-06-28 16:55:39.241507 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      797 2023-06-28 18:04:12.582631 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-07-04 13:26:48.391130 deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     3886 2023-06-28 16:55:38.707373 deepsecrets-1.1.0/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.1.0/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.1.0/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.1.0/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.1.0/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.1.0/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.1.0/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.1.0/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      281 2023-06-28 18:04:11.970796 deepsecrets-1.1.0/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-07-04 13:26:47.808614 deepsecrets-1.1.0/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8594 2023-07-04 09:53:49.065871 deepsecrets-1.1.0/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5166 2023-07-04 09:53:48.500643 deepsecrets-1.1.0/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.1.0/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.1.0/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10945 2023-07-04 12:01:13.022231 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-06-28 17:29:54.564568 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1371 2023-06-28 18:14:23.816502 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      556 2023-06-28 18:14:23.216059 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7398 2023-06-28 18:18:53.090440 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     7425 2023-07-04 13:39:06.736554 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     3845 2023-06-28 18:18:52.403328 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     6529 2023-07-04 13:39:05.813218 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-06-28 17:29:53.978332 deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.1.0/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6862 2023-07-04 12:01:12.367278 deepsecrets-1.1.0/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3487 2023-07-03 09:28:55.083680 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5474 2023-07-04 09:56:49.777143 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     2681 2023-06-30 18:34:33.195619 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5265 2023-07-03 12:07:13.918625 deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/lexer_finder.cpython-311.pyc
+-rw-r--r--   0        0        0     1759 2023-07-03 09:28:54.438041 deepsecrets-1.1.0/deepsecrets/core/utils/cpu.py
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.1.0/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3022 2023-07-04 09:56:48.933550 deepsecrets-1.1.0/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.1.0/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0     1538 2023-06-30 18:34:31.705561 deepsecrets-1.1.0/deepsecrets/core/utils/guess_filetype.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.1.0/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2810 2023-07-03 12:07:13.137522 deepsecrets-1.1.0/deepsecrets/core/utils/lexer_finder.py
+-rw-r--r--   0        0        0     2669 2023-07-04 14:27:00.175183 deepsecrets-1.1.0/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.1.0/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.1.0/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5823 2023-07-04 11:57:19.417209 deepsecrets-1.1.0/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3333 2023-07-04 11:57:18.653455 deepsecrets-1.1.0/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1709 2023-07-03 11:58:13.505921 deepsecrets-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 deepsecrets-1.1.0/PKG-INFO
```

### Comparing `deepsecrets-1.0.6/LICENSE` & `deepsecrets-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/README.md` & `deepsecrets-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/__init__.py` & `deepsecrets-1.1.0/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/cli.py` & `deepsecrets-1.1.0/deepsecrets/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,30 +13,33 @@
 from deepsecrets.core.rulesets.false_findings import FalseFindingsBuilder
 from deepsecrets.core.rulesets.hashed_secrets import HashedSecretsRulesetBuilder
 from deepsecrets.core.rulesets.regex import RegexRulesetBuilder
 from deepsecrets.core.utils.fs import get_abspath, get_path_inside_package
 from deepsecrets.scan_modes.cli import CliScanMode
 
 DISABLED = 'disabled'
+FINDINGS_DETECTED_RETURN_CODE = 66
 
 
 class DeepSecretsCliTool:
     argparser: argparse.ArgumentParser
 
     def __init__(self, args: List[str]):
         self.args = args
         self._build_argparser()
 
     def say_hello(self) -> None:
-        bar = '―'
+        bar = '-'
         logger.info('')
-        logger.info(f' {bar*20} DeepSecrets {bar*20}')
-        logger.info(f'  A better tool for secrets search')
-        logger.info('  version 1.0')
+        logger.info(f'{" "*8}{bar*25} DeepSecrets {bar*25}')
+        logger.info(f'{" "*10}A better tool for secret scanning')
+        logger.info(f'{" "*10}version 1.1')
         logger.info(f'')
+        logger.info(f'{" "*8}{bar*63}')
+
 
     def _build_argparser(self) -> None:
         parser = argparse.ArgumentParser(
             prog=MODULE_NAME,
             description='DeepSecrets - a better tool for secrets search',
             formatter_class=RawTextHelpFormatter,
         )
@@ -102,32 +105,51 @@
         parser.add_argument(
             '-v',
             '--verbose',
             action='store_true',
             help='Verbose mode',
         )
 
+        parser.add_argument(
+            '--reflect-findings-in-return-code',
+            action='store_true',
+            help='Return code of 66 if any findings are detected during scan',
+        )
+
+        parser.add_argument(
+            '--process-count',
+            type=int,
+            default=0,
+            help='Number of processes in a pool for file analysis (one process per file)\n'
+            'Default: number of processor cores of your machine or cpu limit of your container from cgroup.\n'
+            'If all checks are failed the fallback value is 4'
+        )
+
         parser.add_argument('--outfile', required=True, type=str)
         parser.add_argument('--outformat', default='json', type=str, choices=['json'])
         self.argparser = parser
 
     def parse_arguments(self) -> None:
         user_args = self.argparser.parse_args(args=self.args[1:])
         self.say_hello()
 
         if user_args.verbose:
             set_logging_level(logging.DEBUG)
 
         self.config = Config()
         self.config.set_workdir(user_args.target_dir)
+        self.config.set_process_count(user_args.process_count)
         self.config.output = Output(type=user_args.outformat, path=user_args.outfile)
 
+        if user_args.reflect_findings_in_return_code:
+            self.config.return_code_if_findings = True
+
         EXCLUDE_PATHS_BUILTIN = get_path_inside_package('rules/excluded_paths.json')
         if user_args.excluded_paths is not None:
-            rules = [rule.replace('built-in', EXCLUDE_PATHS_BUILTIN) for rule in user_args.regex_rules]
+            rules = [rule.replace('built-in', EXCLUDE_PATHS_BUILTIN) for rule in user_args.excluded_paths]
             self.config.set_global_exclusion_paths(rules)
 
         self.config.engines = []
 
         REGEX_BUILTIN_RULESET = get_path_inside_package('rules/regexes.json')
         if user_args.regex_rules is not None:
             rules = [rule.replace('built-in', REGEX_BUILTIN_RULESET) for rule in user_args.regex_rules]
@@ -147,23 +169,29 @@
         if conf_false_findings_ruleset is not None:
             self.config.add_ruleset(FalseFindingsBuilder, conf_false_findings_ruleset)
 
     def start(self) -> None:  # pragma: nocover
         try:
             self.parse_arguments()
         except Exception as e:
-            logger.error(e)
+            logger.exception(e)
             sys.exit(1)
 
-        logger.info(f'Starting scan against {self.config.workdir_path}...')
+        logger.info(f'Starting scan against {self.config.workdir_path} using {self.config.process_count} processes...')
+        if self.config.return_code_if_findings is True:
+            logger.info(f'[!] The tool will return code of {FINDINGS_DETECTED_RETURN_CODE} if any findings are detected\n')
+
         logger.info(80 * '=')
         findings: List[Finding] = CliScanMode(config=self.config).run()
         logger.info(80 * '=')
         logger.info('Scanning finished')
         logger.info(f'{len(findings)} potential secrets found')
         report_path = get_abspath(self.config.output.path)
 
         logger.info(f'Writing report to {report_path}')
         with open(report_path, 'w+') as f:
             json.dump(FindingResponse.from_list(findings), f)
 
         logger.info('Done')
+
+        if len(findings) > 0 and self.config.return_code_if_findings:
+            sys.exit(FINDINGS_DETECTED_RETURN_CODE)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `deepsecrets-1.0.6/deepsecrets/config.py` & `deepsecrets-1.1.0/deepsecrets/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,59 @@
 from typing import Dict, List, Type
 
 from pydantic import BaseModel
+from deepsecrets.core.utils.cpu import CpuHelper
 
 from deepsecrets.core.utils.exceptions import FileNotFoundException
 from deepsecrets.core.utils.fs import get_abspath, path_exists
 
+FALLBACK_PROCESS_COUNT = 4
 
 class Output(BaseModel):
     type: str
     path: str
 
 
 class Config:
     workdir_path: str
     engines: List[Type] = []
     rulesets: Dict[Type, List[str]] = {}
     global_exclusion_paths: List[str] = []
     output: Output
+    process_count: int
+    return_code_if_findings: bool
 
     def __init__(self) -> None:
         self.engines = []
         self.rulesets = {}
         self.global_exclusion_paths = []
+        self.return_code_if_findings = False
+        # equals to CPU count
+        self.process_count = FALLBACK_PROCESS_COUNT
 
     def _set_path(self, path: str, field: str) -> None:
         if not path_exists(path):
             raise FileNotFoundException(f'{field} path does not exist ({path})')
         setattr(self, field, get_abspath(path))
 
     def set_workdir(self, path: str) -> None:
         self._set_path(path, 'workdir_path')
+    
+    def set_process_count(self, count: int):
+        if count > 0:
+            self.process_count = count
+            return
+        
+        count = CpuHelper().get_limit()
+        if count > 0:
+            self.process_count = count
+            return
+        
+        self.process_count = FALLBACK_PROCESS_COUNT
+
 
     def set_global_exclusion_paths(self, paths: List[str]) -> None:
         for path in paths:
             if not path_exists(path):
                 raise FileNotFoundException(f'global_exclusion_path does not exist ({path})')
             self.global_exclusion_paths.append(path)
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.1.0/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.1.0/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/regex.py` & `deepsecrets-1.1.0/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.1.0/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.1.0/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.1.0/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0x9f939964 (Mon Jun 26 13:33:19 2023 UTC)
-files sz: 4034
+moddate:  0x0a669c64 (Wed Jun 28 16:55:38 2023 UTC)
+files sz: 3886
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a036d045a046d055a0501
-      00640064036c066d075a070100640064046c086d095a090100640064056c
-      0a6d0b5a0b010002004700640684006407a6020000ab0200000000000000
-      005a0c64015300
+      00640064036c066d075a070100640064046c086d095a0901000200470064
+      0584006406a6020000ab0200000000000000005a0a64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (regex)
                  8 STORE_NAME               1 (re)
    
@@ -39,292 +38,279 @@
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('get_abspath',))
                 46 IMPORT_NAME              8 (deepsecrets.core.utils.fs)
                 48 IMPORT_FROM              9 (get_abspath)
                 50 STORE_NAME               9 (get_abspath)
                 52 POP_TOP
    
-     6          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               5 (('FileTypeGuesser',))
-                58 IMPORT_NAME             10 (deepsecrets.core.utils.guess_filetype)
-                60 IMPORT_FROM             11 (FileTypeGuesser)
-                62 STORE_NAME              11 (FileTypeGuesser)
-                64 POP_TOP
-   
-     9          66 PUSH_NULL
-                68 LOAD_BUILD_CLASS
-                70 LOAD_CONST               6 (<code object File, file "/app/deepsecrets/core/model/file.py", line 9>)
-                72 MAKE_FUNCTION            0
-                74 LOAD_CONST               7 ('File')
-                76 PRECALL                  2
-                80 CALL                     2
-                90 STORE_NAME              12 (File)
-                92 LOAD_CONST               1 (None)
-                94 RETURN_VALUE
+     8          54 PUSH_NULL
+                56 LOAD_BUILD_CLASS
+                58 LOAD_CONST               5 (<code object File, file "/app/deepsecrets/core/model/file.py", line 8>)
+                60 MAKE_FUNCTION            0
+                62 LOAD_CONST               6 ('File')
+                64 PRECALL                  2
+                68 CALL                     2
+                78 STORE_NAME              10 (File)
+                80 LOAD_CONST               1 (None)
+                82 RETURN_VALUE
    consts
       0
       None
       ('Dict', 'Optional', 'Tuple')
       ('logger',)
       ('get_abspath',)
-      ('FileTypeGuesser',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
             00000064035a056503650464043c0000006506650464053c00000069005a
             076508650665096506650666021900000000000000000066021900000000
             0000000000650464063c00000069005a0a65086506650366021900000000
-            0000000000650464073c000000650b650464083c000000650c6503190000
-            00000000000000650464093c000000650c65031900000000000000000065
-            04640a3c000000090009000900641e640265036401650c65031900000000
-            00000000006404650c650319000000000000000000640c650c6508190000
-            00000000000000640d640b660a640e84055a0d640d650c65031900000000
-            00000000006602640f84045a0e640d650c65031900000000000000000066
-            02641084045a0f641f641184045a10640d65036602641284045a11641365
-            06640d650c6506190000000000000000006604641484045a126413650664
-            0d650c6506190000000000000000006604641584045a1364166506640d65
-            0c6503190000000000000000006604641784045a1464186506640d650c65
-            03190000000000000000006604641984045a156420641a6503641b650c65
-            096506650666021900000000000000000019000000000000000000640d65
-            0c6509650665066602190000000000000000001900000000000000000066
-            06641c84055a16640d65036602641d84045a17640b5300
-           9           0 RESUME                   0
+            0000000000650464073c000000650b650464083c0000006503650464093c
+            000000650c6503190000000000000000006504640a3c0000000900090009
+            00641e640265036401650c6503190000000000000000006404650c650319
+            000000000000000000640c650c650819000000000000000000640d640b66
+            0a640e84055a0d640d65036602640f84045a0e640d650c65031900000000
+            00000000006602641084045a0f641f641184045a10640d65036602641284
+            045a1164136506640d650c6506190000000000000000006604641484045a
+            1264136506640d650c6506190000000000000000006604641584045a1364
+            166506640d650c6503190000000000000000006604641784045a14641865
+            06640d650c6503190000000000000000006604641984045a156420641a65
+            03641b650c65096506650666021900000000000000000019000000000000
+            000000640d650c6509650665066602190000000000000000001900000000
+            00000000006606641c84055a16640d65036602641d84045a17640b5300
+           8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('File')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          10          12 LOAD_NAME                3 (str)
+           9          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('relative_path')
                       18 STORE_SUBSCR
          
-          11          22 LOAD_NAME                3 (str)
+          10          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('path')
                       28 STORE_SUBSCR
          
-          12          32 LOAD_CONST               3 ('')
+          11          32 LOAD_CONST               3 ('')
                       34 STORE_NAME               5 (content)
                       36 LOAD_NAME                3 (str)
                       38 LOAD_NAME                4 (__annotations__)
                       40 LOAD_CONST               4 ('content')
                       42 STORE_SUBSCR
          
-          13          46 LOAD_NAME                6 (int)
+          12          46 LOAD_NAME                6 (int)
                       48 LOAD_NAME                4 (__annotations__)
                       50 LOAD_CONST               5 ('length')
                       52 STORE_SUBSCR
          
-          14          56 BUILD_MAP                0
+          13          56 BUILD_MAP                0
                       58 STORE_NAME               7 (line_offsets)
                       60 LOAD_NAME                8 (Dict)
                       62 LOAD_NAME                6 (int)
                       64 LOAD_NAME                9 (Tuple)
                       66 LOAD_NAME                6 (int)
                       68 LOAD_NAME                6 (int)
                       70 BUILD_TUPLE              2
                       72 BINARY_SUBSCR
                       82 BUILD_TUPLE              2
                       84 BINARY_SUBSCR
                       94 LOAD_NAME                4 (__annotations__)
                       96 LOAD_CONST               6 ('line_offsets')
                       98 STORE_SUBSCR
          
-          15         102 BUILD_MAP                0
+          14         102 BUILD_MAP                0
                      104 STORE_NAME              10 (line_contents_cache)
                      106 LOAD_NAME                8 (Dict)
                      108 LOAD_NAME                6 (int)
                      110 LOAD_NAME                3 (str)
                      112 BUILD_TUPLE              2
                      114 BINARY_SUBSCR
                      124 LOAD_NAME                4 (__annotations__)
                      126 LOAD_CONST               7 ('line_contents_cache')
                      128 STORE_SUBSCR
          
-          16         132 LOAD_NAME               11 (bool)
+          15         132 LOAD_NAME               11 (bool)
                      134 LOAD_NAME                4 (__annotations__)
                      136 LOAD_CONST               8 ('empty')
                      138 STORE_SUBSCR
          
-          17         142 LOAD_NAME               12 (Optional)
-                     144 LOAD_NAME                3 (str)
-                     146 BINARY_SUBSCR
-                     156 LOAD_NAME                4 (__annotations__)
-                     158 LOAD_CONST               9 ('extension')
-                     160 STORE_SUBSCR
+          16         142 LOAD_NAME                3 (str)
+                     144 LOAD_NAME                4 (__annotations__)
+                     146 LOAD_CONST               9 ('name')
+                     148 STORE_SUBSCR
+         
+          17         152 LOAD_NAME               12 (Optional)
+                     154 LOAD_NAME                3 (str)
+                     156 BINARY_SUBSCR
+                     166 LOAD_NAME                4 (__annotations__)
+                     168 LOAD_CONST              10 ('extension')
+                     170 STORE_SUBSCR
          
-          18         164 LOAD_NAME               12 (Optional)
-                     166 LOAD_NAME                3 (str)
-                     168 BINARY_SUBSCR
-                     178 LOAD_NAME                4 (__annotations__)
-                     180 LOAD_CONST              10 ('guessed_extension')
-                     182 STORE_SUBSCR
+          22         174 NOP
          
-          23         186 NOP
+          23         176 NOP
          
-          24         188 NOP
+          24         178 NOP
          
-          25         190 NOP
+          19         180 LOAD_CONST              30 ((None, None, None))
+                     182 LOAD_CONST               2 ('path')
          
-          20         192 LOAD_CONST              30 ((None, None, None))
-                     194 LOAD_CONST               2 ('path')
+          21         184 LOAD_NAME                3 (str)
          
-          22         196 LOAD_NAME                3 (str)
+          19         186 LOAD_CONST               1 ('relative_path')
          
-          20         198 LOAD_CONST               1 ('relative_path')
+          22         188 LOAD_NAME               12 (Optional)
+                     190 LOAD_NAME                3 (str)
+                     192 BINARY_SUBSCR
          
-          23         200 LOAD_NAME               12 (Optional)
-                     202 LOAD_NAME                3 (str)
-                     204 BINARY_SUBSCR
+          19         202 LOAD_CONST               4 ('content')
          
-          20         214 LOAD_CONST               4 ('content')
+          23         204 LOAD_NAME               12 (Optional)
+                     206 LOAD_NAME                3 (str)
+                     208 BINARY_SUBSCR
          
-          24         216 LOAD_NAME               12 (Optional)
-                     218 LOAD_NAME                3 (str)
-                     220 BINARY_SUBSCR
+          19         218 LOAD_CONST              12 ('offsets')
          
-          20         230 LOAD_CONST              12 ('offsets')
+          24         220 LOAD_NAME               12 (Optional)
+                     222 LOAD_NAME                8 (Dict)
+                     224 BINARY_SUBSCR
          
-          25         232 LOAD_NAME               12 (Optional)
-                     234 LOAD_NAME                8 (Dict)
-                     236 BINARY_SUBSCR
+          19         234 LOAD_CONST              13 ('return')
          
-          20         246 LOAD_CONST              13 ('return')
+          25         236 LOAD_CONST              11 (None)
          
-          26         248 LOAD_CONST              11 (None)
+          19         238 BUILD_TUPLE             10
+                     240 LOAD_CONST              14 (<code object __init__, file "/app/deepsecrets/core/model/file.py", line 19>)
+                     242 MAKE_FUNCTION            5 (defaults, annotations)
+                     244 STORE_NAME              13 (__init__)
          
-          20         250 BUILD_TUPLE             10
-                     252 LOAD_CONST              14 (<code object __init__, file "/app/deepsecrets/core/model/file.py", line 20>)
-                     254 MAKE_FUNCTION            5 (defaults, annotations)
-                     256 STORE_NAME              13 (__init__)
+          54         246 LOAD_CONST              13 ('return')
+                     248 LOAD_NAME                3 (str)
+                     250 BUILD_TUPLE              2
+                     252 LOAD_CONST              15 (<code object _get_name, file "/app/deepsecrets/core/model/file.py", line 54>)
+                     254 MAKE_FUNCTION            4 (annotations)
+                     256 STORE_NAME              14 (_get_name)
          
-          57         258 LOAD_CONST              13 ('return')
+          59         258 LOAD_CONST              13 ('return')
                      260 LOAD_NAME               12 (Optional)
                      262 LOAD_NAME                3 (str)
                      264 BINARY_SUBSCR
                      274 BUILD_TUPLE              2
-                     276 LOAD_CONST              15 (<code object _get_extension, file "/app/deepsecrets/core/model/file.py", line 57>)
+                     276 LOAD_CONST              16 (<code object _get_extension, file "/app/deepsecrets/core/model/file.py", line 59>)
                      278 MAKE_FUNCTION            4 (annotations)
-                     280 STORE_NAME              14 (_get_extension)
+                     280 STORE_NAME              15 (_get_extension)
+         
+          66         282 LOAD_CONST              31 (('return', None))
+                     284 LOAD_CONST              17 (<code object _calc_offsets, file "/app/deepsecrets/core/model/file.py", line 66>)
+                     286 MAKE_FUNCTION            4 (annotations)
+                     288 STORE_NAME              16 (_calc_offsets)
+         
+          75         290 LOAD_CONST              13 ('return')
+                     292 LOAD_NAME                3 (str)
+                     294 BUILD_TUPLE              2
+                     296 LOAD_CONST              18 (<code object _get_contents, file "/app/deepsecrets/core/model/file.py", line 75>)
+                     298 MAKE_FUNCTION            4 (annotations)
+                     300 STORE_NAME              17 (_get_contents)
+         
+          82         302 LOAD_CONST              19 ('position')
+                     304 LOAD_NAME                6 (int)
+                     306 LOAD_CONST              13 ('return')
+                     308 LOAD_NAME               12 (Optional)
+                     310 LOAD_NAME                6 (int)
+                     312 BINARY_SUBSCR
+                     322 BUILD_TUPLE              4
+                     324 LOAD_CONST              20 (<code object get_line_number, file "/app/deepsecrets/core/model/file.py", line 82>)
+                     326 MAKE_FUNCTION            4 (annotations)
+                     328 STORE_NAME              18 (get_line_number)
+         
+          85         330 LOAD_CONST              19 ('position')
+                     332 LOAD_NAME                6 (int)
+                     334 LOAD_CONST              13 ('return')
+                     336 LOAD_NAME               12 (Optional)
+                     338 LOAD_NAME                6 (int)
+                     340 BINARY_SUBSCR
+                     350 BUILD_TUPLE              4
+                     352 LOAD_CONST              21 (<code object _get_line_number_for_position, file "/app/deepsecrets/core/model/file.py", line 85>)
+                     354 MAKE_FUNCTION            4 (annotations)
+                     356 STORE_NAME              19 (_get_line_number_for_position)
+         
+          92         358 LOAD_CONST              22 ('line_number')
+                     360 LOAD_NAME                6 (int)
+                     362 LOAD_CONST              13 ('return')
+                     364 LOAD_NAME               12 (Optional)
+                     366 LOAD_NAME                3 (str)
+                     368 BINARY_SUBSCR
+                     378 BUILD_TUPLE              4
+                     380 LOAD_CONST              23 (<code object get_line_contents, file "/app/deepsecrets/core/model/file.py", line 92>)
+                     382 MAKE_FUNCTION            4 (annotations)
+                     384 STORE_NAME              20 (get_line_contents)
+         
+         102         386 LOAD_CONST              24 ('span_end')
+                     388 LOAD_NAME                6 (int)
+                     390 LOAD_CONST              13 ('return')
+                     392 LOAD_NAME               12 (Optional)
+                     394 LOAD_NAME                3 (str)
+                     396 BINARY_SUBSCR
+                     406 BUILD_TUPLE              4
+                     408 LOAD_CONST              25 (<code object get_full_line_for_position, file "/app/deepsecrets/core/model/file.py", line 102>)
+                     410 MAKE_FUNCTION            4 (annotations)
+                     412 STORE_NAME              21 (get_full_line_for_position)
          
-          64         282 LOAD_CONST              13 ('return')
-                     284 LOAD_NAME               12 (Optional)
-                     286 LOAD_NAME                3 (str)
-                     288 BINARY_SUBSCR
-                     298 BUILD_TUPLE              2
-                     300 LOAD_CONST              16 (<code object _try_guess_extension, file "/app/deepsecrets/core/model/file.py", line 64>)
-                     302 MAKE_FUNCTION            4 (annotations)
-                     304 STORE_NAME              15 (_try_guess_extension)
-         
-          67         306 LOAD_CONST              31 (('return', None))
-                     308 LOAD_CONST              17 (<code object _calc_offsets, file "/app/deepsecrets/core/model/file.py", line 67>)
-                     310 MAKE_FUNCTION            4 (annotations)
-                     312 STORE_NAME              16 (_calc_offsets)
-         
-          76         314 LOAD_CONST              13 ('return')
-                     316 LOAD_NAME                3 (str)
-                     318 BUILD_TUPLE              2
-                     320 LOAD_CONST              18 (<code object _get_contents, file "/app/deepsecrets/core/model/file.py", line 76>)
-                     322 MAKE_FUNCTION            4 (annotations)
-                     324 STORE_NAME              17 (_get_contents)
-         
-          83         326 LOAD_CONST              19 ('position')
-                     328 LOAD_NAME                6 (int)
-                     330 LOAD_CONST              13 ('return')
-                     332 LOAD_NAME               12 (Optional)
-                     334 LOAD_NAME                6 (int)
-                     336 BINARY_SUBSCR
-                     346 BUILD_TUPLE              4
-                     348 LOAD_CONST              20 (<code object get_line_number, file "/app/deepsecrets/core/model/file.py", line 83>)
-                     350 MAKE_FUNCTION            4 (annotations)
-                     352 STORE_NAME              18 (get_line_number)
-         
-          86         354 LOAD_CONST              19 ('position')
-                     356 LOAD_NAME                6 (int)
-                     358 LOAD_CONST              13 ('return')
-                     360 LOAD_NAME               12 (Optional)
-                     362 LOAD_NAME                6 (int)
-                     364 BINARY_SUBSCR
-                     374 BUILD_TUPLE              4
-                     376 LOAD_CONST              21 (<code object _get_line_number_for_position, file "/app/deepsecrets/core/model/file.py", line 86>)
-                     378 MAKE_FUNCTION            4 (annotations)
-                     380 STORE_NAME              19 (_get_line_number_for_position)
-         
-          93         382 LOAD_CONST              22 ('line_number')
-                     384 LOAD_NAME                6 (int)
-                     386 LOAD_CONST              13 ('return')
-                     388 LOAD_NAME               12 (Optional)
-                     390 LOAD_NAME                3 (str)
-                     392 BINARY_SUBSCR
-                     402 BUILD_TUPLE              4
-                     404 LOAD_CONST              23 (<code object get_line_contents, file "/app/deepsecrets/core/model/file.py", line 93>)
-                     406 MAKE_FUNCTION            4 (annotations)
-                     408 STORE_NAME              20 (get_line_contents)
-         
-         103         410 LOAD_CONST              24 ('span_end')
-                     412 LOAD_NAME                6 (int)
-                     414 LOAD_CONST              13 ('return')
-                     416 LOAD_NAME               12 (Optional)
+         109         414 LOAD_CONST              32 ((None,))
+                     416 LOAD_CONST              26 ('str')
                      418 LOAD_NAME                3 (str)
-                     420 BINARY_SUBSCR
-                     430 BUILD_TUPLE              4
-                     432 LOAD_CONST              25 (<code object get_full_line_for_position, file "/app/deepsecrets/core/model/file.py", line 103>)
-                     434 MAKE_FUNCTION            4 (annotations)
-                     436 STORE_NAME              21 (get_full_line_for_position)
-         
-         110         438 LOAD_CONST              32 ((None,))
-                     440 LOAD_CONST              26 ('str')
-                     442 LOAD_NAME                3 (str)
-                     444 LOAD_CONST              27 ('between')
-                     446 LOAD_NAME               12 (Optional)
-                     448 LOAD_NAME                9 (Tuple)
-                     450 LOAD_NAME                6 (int)
-                     452 LOAD_NAME                6 (int)
-                     454 BUILD_TUPLE              2
-                     456 BINARY_SUBSCR
-                     466 BINARY_SUBSCR
-                     476 LOAD_CONST              13 ('return')
-                     478 LOAD_NAME               12 (Optional)
-                     480 LOAD_NAME                9 (Tuple)
-                     482 LOAD_NAME                6 (int)
-                     484 LOAD_NAME                6 (int)
-                     486 BUILD_TUPLE              2
-                     488 BINARY_SUBSCR
-                     498 BINARY_SUBSCR
-                     508 BUILD_TUPLE              6
-                     510 LOAD_CONST              28 (<code object get_span_for_string, file "/app/deepsecrets/core/model/file.py", line 110>)
-                     512 MAKE_FUNCTION            5 (defaults, annotations)
-                     514 STORE_NAME              22 (get_span_for_string)
-         
-         124         516 LOAD_CONST              13 ('return')
-                     518 LOAD_NAME                3 (str)
-                     520 BUILD_TUPLE              2
-                     522 LOAD_CONST              29 (<code object __repr__, file "/app/deepsecrets/core/model/file.py", line 124>)
-                     524 MAKE_FUNCTION            4 (annotations)
-                     526 STORE_NAME              23 (__repr__)
-                     528 LOAD_CONST              11 (None)
-                     530 RETURN_VALUE
+                     420 LOAD_CONST              27 ('between')
+                     422 LOAD_NAME               12 (Optional)
+                     424 LOAD_NAME                9 (Tuple)
+                     426 LOAD_NAME                6 (int)
+                     428 LOAD_NAME                6 (int)
+                     430 BUILD_TUPLE              2
+                     432 BINARY_SUBSCR
+                     442 BINARY_SUBSCR
+                     452 LOAD_CONST              13 ('return')
+                     454 LOAD_NAME               12 (Optional)
+                     456 LOAD_NAME                9 (Tuple)
+                     458 LOAD_NAME                6 (int)
+                     460 LOAD_NAME                6 (int)
+                     462 BUILD_TUPLE              2
+                     464 BINARY_SUBSCR
+                     474 BINARY_SUBSCR
+                     484 BUILD_TUPLE              6
+                     486 LOAD_CONST              28 (<code object get_span_for_string, file "/app/deepsecrets/core/model/file.py", line 109>)
+                     488 MAKE_FUNCTION            5 (defaults, annotations)
+                     490 STORE_NAME              22 (get_span_for_string)
+         
+         123         492 LOAD_CONST              13 ('return')
+                     494 LOAD_NAME                3 (str)
+                     496 BUILD_TUPLE              2
+                     498 LOAD_CONST              29 (<code object __repr__, file "/app/deepsecrets/core/model/file.py", line 123>)
+                     500 MAKE_FUNCTION            4 (annotations)
+                     502 STORE_NAME              23 (__repr__)
+                     504 LOAD_CONST              11 (None)
+                     506 RETURN_VALUE
          consts
             'File'
             'relative_path'
             'path'
             ''
             'content'
             'length'
             'line_offsets'
             'line_contents_cache'
             'empty'
+            'name'
             'extension'
-            'guessed_extension'
             None
             'offsets'
             'return'
             code
                argcount  : 5
                nlocals   : 6
                stacksize : 4
@@ -338,77 +324,76 @@
                   000000a6000000ab0000000000000000007c005f0500000000000000006e
                   2b2300740e000000000000000000002400721e7d05741100000000000000
                   0000006a0900000000000000006401a6010000ab01000000000000000001
                   00590064007d057e056e0864007d057e0577017700780359007701741500
                   0000000000000000007c006a050000000000000000a6010000ab01000000
                   00000000007c005f0b00000000000000007c00a00c000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007c005f0d00
-                  000000000000007c006a0d000000000000000080197c00a00e0000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007c
-                  005f0f00000000000000007c006a0b000000000000000064026b02000000
-                  00720264036e0164047c005f1000000000000000007c0481077c047c005f
-                  0000000000000000007c006a100000000000000000732e74150000000000
-                  00000000007c006a000000000000000000a6010000ab0100000000000000
-                  0064026b020000000072187c00a011000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000000100640053006400530064
-                  005300
-                20           0 RESUME                   0
+                  000000000000007c00a00e00000000000000000000000000000000000000
+                  00a6000000ab0000000000000000007c005f0f00000000000000007c006a
+                  0b000000000000000064026b0200000000720264036e0164047c005f1000
+                  000000000000007c0481077c047c005f0000000000000000007c006a1000
+                  00000000000000732e7415000000000000000000007c006a000000000000
+                  000000a6010000ab01000000000000000064026b020000000072187c00a0
+                  110000000000000000000000000000000000000000a6000000ab00000000
+                  00000000000100640053006400530064005300
+                19           0 RESUME                   0
                
-                27           2 BUILD_MAP                0
+                26           2 BUILD_MAP                0
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (line_offsets)
                
-                28          16 BUILD_MAP                0
+                27          16 BUILD_MAP                0
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (line_contents_cache)
                
-                30          30 LOAD_FAST                1 (path)
+                29          30 LOAD_FAST                1 (path)
                             32 POP_JUMP_FORWARD_IF_NONE    20 (to 74)
                
-                31          34 LOAD_GLOBAL              5 (NULL + get_abspath)
+                30          34 LOAD_GLOBAL              5 (NULL + get_abspath)
                             46 LOAD_FAST                1 (path)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               3 (path)
                
-                33     >>   74 LOAD_FAST                2 (relative_path)
+                32     >>   74 LOAD_FAST                2 (relative_path)
                             76 POP_JUMP_FORWARD_IF_NONE     2 (to 82)
                             78 LOAD_FAST                2 (relative_path)
                             80 JUMP_FORWARD             6 (to 94)
                        >>   82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (path)
                        >>   94 LOAD_FAST                0 (self)
                             96 STORE_ATTR               4 (relative_path)
                
-                35         106 LOAD_FAST                3 (content)
+                34         106 LOAD_FAST                3 (content)
                            108 POP_JUMP_FORWARD_IF_NONE     8 (to 126)
                
-                36         110 LOAD_FAST                3 (content)
+                35         110 LOAD_FAST                3 (content)
                            112 LOAD_FAST                0 (self)
                            114 STORE_ATTR               5 (content)
                            124 JUMP_FORWARD            70 (to 266)
                
-                38     >>  126 NOP
+                37     >>  126 NOP
                
-                39         128 LOAD_FAST                0 (self)
+                38         128 LOAD_FAST                0 (self)
                            130 LOAD_METHOD              6 (_get_contents)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 LOAD_FAST                0 (self)
                            168 STORE_ATTR               5 (content)
                            178 JUMP_FORWARD            43 (to 266)
                        >>  180 PUSH_EXC_INFO
                
-                40         182 LOAD_GLOBAL             14 (Exception)
+                39         182 LOAD_GLOBAL             14 (Exception)
                            194 CHECK_EXC_MATCH
                            196 POP_JUMP_FORWARD_IF_FALSE    30 (to 258)
                            198 STORE_FAST               5 (e)
                
-                41         200 LOAD_GLOBAL             17 (NULL + logger)
+                40         200 LOAD_GLOBAL             17 (NULL + logger)
                            212 LOAD_ATTR                9 (error)
                            222 LOAD_CONST               1 ('Error during fetching file contents')
                            224 PRECALL                  1
                            228 CALL                     1
                            238 POP_TOP
                            240 POP_EXCEPT
                            242 LOAD_CONST               0 (None)
@@ -416,188 +401,199 @@
                            246 DELETE_FAST              5 (e)
                            248 JUMP_FORWARD             8 (to 266)
                        >>  250 LOAD_CONST               0 (None)
                            252 STORE_FAST               5 (e)
                            254 DELETE_FAST              5 (e)
                            256 RERAISE                  1
                
-                40     >>  258 RERAISE                  0
+                39     >>  258 RERAISE                  0
                        >>  260 COPY                     3
                            262 POP_EXCEPT
                            264 RERAISE                  1
                
-                43     >>  266 LOAD_GLOBAL             21 (NULL + len)
+                42     >>  266 LOAD_GLOBAL             21 (NULL + len)
                            278 LOAD_FAST                0 (self)
                            280 LOAD_ATTR                5 (content)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 LOAD_FAST                0 (self)
                            306 STORE_ATTR              11 (length)
                
-                45         316 LOAD_FAST                0 (self)
-                           318 LOAD_METHOD             12 (_get_extension)
+                44         316 LOAD_FAST                0 (self)
+                           318 LOAD_METHOD             12 (_get_name)
                            340 PRECALL                  0
                            344 CALL                     0
                            354 LOAD_FAST                0 (self)
-                           356 STORE_ATTR              13 (extension)
+                           356 STORE_ATTR              13 (name)
                
-                46         366 LOAD_FAST                0 (self)
-                           368 LOAD_ATTR               13 (extension)
-                           378 POP_JUMP_FORWARD_IF_NOT_NONE    25 (to 430)
-               
-                47         380 LOAD_FAST                0 (self)
-                           382 LOAD_METHOD             14 (_try_guess_extension)
-                           404 PRECALL                  0
-                           408 CALL                     0
-                           418 LOAD_FAST                0 (self)
-                           420 STORE_ATTR              15 (guessed_extension)
-               
-                49     >>  430 LOAD_FAST                0 (self)
-                           432 LOAD_ATTR               11 (length)
-                           442 LOAD_CONST               2 (0)
-                           444 COMPARE_OP               2 (==)
-                           450 POP_JUMP_FORWARD_IF_FALSE     2 (to 456)
-                           452 LOAD_CONST               3 (True)
-                           454 JUMP_FORWARD             1 (to 458)
-                       >>  456 LOAD_CONST               4 (False)
-                       >>  458 LOAD_FAST                0 (self)
-                           460 STORE_ATTR              16 (empty)
-               
-                51         470 LOAD_FAST                4 (offsets)
-                           472 POP_JUMP_FORWARD_IF_NONE     7 (to 488)
-               
-                52         474 LOAD_FAST                4 (offsets)
-                           476 LOAD_FAST                0 (self)
-                           478 STORE_ATTR               0 (line_offsets)
-               
-                54     >>  488 LOAD_FAST                0 (self)
-                           490 LOAD_ATTR               16 (empty)
-                           500 POP_JUMP_FORWARD_IF_TRUE    46 (to 594)
-                           502 LOAD_GLOBAL             21 (NULL + len)
-                           514 LOAD_FAST                0 (self)
-                           516 LOAD_ATTR                0 (line_offsets)
-                           526 PRECALL                  1
-                           530 CALL                     1
-                           540 LOAD_CONST               2 (0)
-                           542 COMPARE_OP               2 (==)
-                           548 POP_JUMP_FORWARD_IF_FALSE    24 (to 598)
-               
-                55         550 LOAD_FAST                0 (self)
-                           552 LOAD_METHOD             17 (_calc_offsets)
-                           574 PRECALL                  0
-                           578 CALL                     0
-                           588 POP_TOP
-                           590 LOAD_CONST               0 (None)
-                           592 RETURN_VALUE
-               
-                54     >>  594 LOAD_CONST               0 (None)
-                           596 RETURN_VALUE
-                       >>  598 LOAD_CONST               0 (None)
-                           600 RETURN_VALUE
+                45         366 LOAD_FAST                0 (self)
+                           368 LOAD_METHOD             14 (_get_extension)
+                           390 PRECALL                  0
+                           394 CALL                     0
+                           404 LOAD_FAST                0 (self)
+                           406 STORE_ATTR              15 (extension)
+               
+                46         416 LOAD_FAST                0 (self)
+                           418 LOAD_ATTR               11 (length)
+                           428 LOAD_CONST               2 (0)
+                           430 COMPARE_OP               2 (==)
+                           436 POP_JUMP_FORWARD_IF_FALSE     2 (to 442)
+                           438 LOAD_CONST               3 (True)
+                           440 JUMP_FORWARD             1 (to 444)
+                       >>  442 LOAD_CONST               4 (False)
+                       >>  444 LOAD_FAST                0 (self)
+                           446 STORE_ATTR              16 (empty)
+               
+                48         456 LOAD_FAST                4 (offsets)
+                           458 POP_JUMP_FORWARD_IF_NONE     7 (to 474)
+               
+                49         460 LOAD_FAST                4 (offsets)
+                           462 LOAD_FAST                0 (self)
+                           464 STORE_ATTR               0 (line_offsets)
+               
+                51     >>  474 LOAD_FAST                0 (self)
+                           476 LOAD_ATTR               16 (empty)
+                           486 POP_JUMP_FORWARD_IF_TRUE    46 (to 580)
+                           488 LOAD_GLOBAL             21 (NULL + len)
+                           500 LOAD_FAST                0 (self)
+                           502 LOAD_ATTR                0 (line_offsets)
+                           512 PRECALL                  1
+                           516 CALL                     1
+                           526 LOAD_CONST               2 (0)
+                           528 COMPARE_OP               2 (==)
+                           534 POP_JUMP_FORWARD_IF_FALSE    24 (to 584)
+               
+                52         536 LOAD_FAST                0 (self)
+                           538 LOAD_METHOD             17 (_calc_offsets)
+                           560 PRECALL                  0
+                           564 CALL                     0
+                           574 POP_TOP
+                           576 LOAD_CONST               0 (None)
+                           578 RETURN_VALUE
+               
+                51     >>  580 LOAD_CONST               0 (None)
+                           582 RETURN_VALUE
+                       >>  584 LOAD_CONST               0 (None)
+                           586 RETURN_VALUE
                ExceptionTable:
                  128 to 176 -> 180 [0]
                  180 to 198 -> 260 [1] lasti
                  200 to 238 -> 250 [1] lasti
                  250 to 258 -> 260 [1] lasti
                consts
                   None
                   'Error during fetching file contents'
                   0
                   True
                   False
-               names      ('line_offsets', 'line_contents_cache', 'get_abspath', 'path', 'relative_path', 'content', '_get_contents', 'Exception', 'logger', 'error', 'len', 'length', '_get_extension', 'extension', '_try_guess_extension', 'guessed_extension', 'empty', '_calc_offsets')
+               names      ('line_offsets', 'line_contents_cache', 'get_abspath', 'path', 'relative_path', 'content', '_get_contents', 'Exception', 'logger', 'error', 'len', 'length', '_get_name', 'name', '_get_extension', 'extension', 'empty', '_calc_offsets')
                varnames   ('self', 'path', 'relative_path', 'content', 'offsets', 'e')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '__init__'
-               firstlineno 20
+               firstlineno 19
                lnotab
                   0x02070e010e02040128022002040110020201360112013aff0803320232
-                  010e013202280204010e023e012cff
+                  013201280204010e023e012cff
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000006401a6010000ab0100000000000000007d017c01640219
+                  000000000000000000a00100000000000000000000000000000000000000
+                  006403a6010000ab01000000000000000064041900000000000000000053
+                  00
+                54           0 RESUME                   0
+               
+                55           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (path)
+                            14 LOAD_METHOD              1 (split)
+                            36 LOAD_CONST               1 ('/')
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 STORE_FAST               1 (by_slash)
+               
+                56          54 LOAD_FAST                1 (by_slash)
+                            56 LOAD_CONST               2 (-1)
+                            58 BINARY_SUBSCR
+                            68 LOAD_METHOD              1 (split)
+                            90 LOAD_CONST               3 ('.')
+                            92 PRECALL                  1
+                            96 CALL                     1
+                           106 LOAD_CONST               4 (0)
+                           108 BINARY_SUBSCR
+                           118 RETURN_VALUE
+               consts
+                  None
+                  '/'
+                  -1
+                  '.'
+                  0
+               names      ('path', 'split')
+               varnames   ('self', 'by_slash')
+               freevars   ()
+               cellvars   ()
+               filename   '/app/deepsecrets/core/model/file.py'
+               name       '_get_name'
+               firstlineno 54
+               lnotab 0x02013401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab0100000000000000007d017405000000
                   000000000000007c01a6010000ab01000000000000000064026b02000000
                   007202640053007c016403190000000000000000005300
-                57           0 RESUME                   0
+                59           0 RESUME                   0
                
-                58           2 LOAD_FAST                0 (self)
+                60           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (path)
                             14 LOAD_METHOD              1 (split)
                             36 LOAD_CONST               1 ('.')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (by_dot)
                
-                59          54 LOAD_GLOBAL              5 (NULL + len)
+                61          54 LOAD_GLOBAL              5 (NULL + len)
                             66 LOAD_FAST                1 (by_dot)
                             68 PRECALL                  1
                             72 CALL                     1
                             82 LOAD_CONST               2 (1)
                             84 COMPARE_OP               2 (==)
                             90 POP_JUMP_FORWARD_IF_FALSE     2 (to 96)
                
-                60          92 LOAD_CONST               0 (None)
+                62          92 LOAD_CONST               0 (None)
                             94 RETURN_VALUE
                
-                62     >>   96 LOAD_FAST                1 (by_dot)
+                64     >>   96 LOAD_FAST                1 (by_dot)
                             98 LOAD_CONST               3 (-1)
                            100 BINARY_SUBSCR
                            110 RETURN_VALUE
                consts
                   None
                   '.'
                   1
                   -1
                names      ('path', 'split', 'len')
                varnames   ('self', 'by_dot')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_extension'
-               firstlineno 57
+               firstlineno 59
                lnotab 0x0201340126010402
             code
                argcount  : 1
-               nlocals   : 1
-               stacksize : 3
-               flags     : 3
-               code
-                  0x9700740100000000000000000000a6000000ab000000000000000000a0
-                  0100000000000000000000000000000000000000007c006a020000000000
-                  000000a6010000ab0100000000000000005300
-                64           0 RESUME                   0
-               
-                65           2 LOAD_GLOBAL              1 (NULL + FileTypeGuesser)
-                            14 PRECALL                  0
-                            18 CALL                     0
-                            28 LOAD_METHOD              1 (guess)
-                            50 LOAD_FAST                0 (self)
-                            52 LOAD_ATTR                2 (content)
-                            62 PRECALL                  1
-                            66 CALL                     1
-                            76 RETURN_VALUE
-               consts
-                  None
-               names      ('FileTypeGuesser', 'guess', 'content')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/app/deepsecrets/core/model/file.py'
-               name       '_try_guess_extension'
-               firstlineno 64
-               lnotab 0x0201
-            code
-               argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
                   0x9700640184007401000000000000000000006a01000000000000000064
                   027c006a020000000000000000a6020000ab0200000000000000004400a6
                   000000ab0000000000000000007d017407000000000000000000007c01a6
@@ -605,106 +601,106 @@
                   0400000000720e7c017c0264047a0a00001900000000000000000064047a
                   0000006e0164037d047c047c0366027c006a0400000000000000007c0264
                   047a0000003c0000008c2b740b000000000000000000007c006a04000000
                   0000000000a6010000ab01000000000000000064036b0200000000721e7c
                   006a06000000000000000064036b0400000000721564037c006a06000000
                   000000000066027c006a04000000000000000064043c0000006400530064
                   00530064005300
-                67           0 RESUME                   0
+                66           0 RESUME                   0
                
-                68           2 LOAD_CONST               1 (<code object <listcomp>, file "/app/deepsecrets/core/model/file.py", line 68>)
+                67           2 LOAD_CONST               1 (<code object <listcomp>, file "/app/deepsecrets/core/model/file.py", line 67>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_GLOBAL              1 (NULL + re)
                             18 LOAD_ATTR                1 (finditer)
                             28 LOAD_CONST               2 ('\n')
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (content)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 GET_ITER
                             58 PRECALL                  0
                             62 CALL                     0
                             72 STORE_FAST               1 (line_breaks)
                
-                69          74 LOAD_GLOBAL              7 (NULL + enumerate)
+                68          74 LOAD_GLOBAL              7 (NULL + enumerate)
                             86 LOAD_FAST                1 (line_breaks)
                             88 PRECALL                  1
                             92 CALL                     1
                            102 GET_ITER
                        >>  104 FOR_ITER                42 (to 190)
                            106 UNPACK_SEQUENCE          2
                            110 STORE_FAST               2 (i)
                            112 STORE_FAST               3 (lb)
                
-                70         114 LOAD_FAST                2 (i)
+                69         114 LOAD_FAST                2 (i)
                            116 LOAD_CONST               3 (0)
                            118 COMPARE_OP               4 (>)
                            124 POP_JUMP_FORWARD_IF_FALSE    14 (to 154)
                            126 LOAD_FAST                1 (line_breaks)
                            128 LOAD_FAST                2 (i)
                            130 LOAD_CONST               4 (1)
                            132 BINARY_OP               10 (-)
                            136 BINARY_SUBSCR
                            146 LOAD_CONST               4 (1)
                            148 BINARY_OP                0 (+)
                            152 JUMP_FORWARD             1 (to 156)
                        >>  154 LOAD_CONST               3 (0)
                        >>  156 STORE_FAST               4 (start)
                
-                71         158 LOAD_FAST                4 (start)
+                70         158 LOAD_FAST                4 (start)
                            160 LOAD_FAST                3 (lb)
                            162 BUILD_TUPLE              2
                            164 LOAD_FAST                0 (self)
                            166 LOAD_ATTR                4 (line_offsets)
                            176 LOAD_FAST                2 (i)
                            178 LOAD_CONST               4 (1)
                            180 BINARY_OP                0 (+)
                            184 STORE_SUBSCR
                            188 JUMP_BACKWARD           43 (to 104)
                
-                73     >>  190 LOAD_GLOBAL             11 (NULL + len)
+                72     >>  190 LOAD_GLOBAL             11 (NULL + len)
                            202 LOAD_FAST                0 (self)
                            204 LOAD_ATTR                4 (line_offsets)
                            214 PRECALL                  1
                            218 CALL                     1
                            228 LOAD_CONST               3 (0)
                            230 COMPARE_OP               2 (==)
                            236 POP_JUMP_FORWARD_IF_FALSE    30 (to 298)
                            238 LOAD_FAST                0 (self)
                            240 LOAD_ATTR                6 (length)
                            250 LOAD_CONST               3 (0)
                            252 COMPARE_OP               4 (>)
                            258 POP_JUMP_FORWARD_IF_FALSE    21 (to 302)
                
-                74         260 LOAD_CONST               3 (0)
+                73         260 LOAD_CONST               3 (0)
                            262 LOAD_FAST                0 (self)
                            264 LOAD_ATTR                6 (length)
                            274 BUILD_TUPLE              2
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (line_offsets)
                            288 LOAD_CONST               4 (1)
                            290 STORE_SUBSCR
                            294 LOAD_CONST               0 (None)
                            296 RETURN_VALUE
                
-                73     >>  298 LOAD_CONST               0 (None)
+                72     >>  298 LOAD_CONST               0 (None)
                            300 RETURN_VALUE
                        >>  302 LOAD_CONST               0 (None)
                            304 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c01a000000000000000000000000000000000
                         0000000000a6000000ab00000000000000000091028c175300
-                      68           0 RESUME                   0
+                      67           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_FAST                1 (i)
                                   12 LOAD_METHOD              0 (start)
                                   34 PRECALL                  0
@@ -715,70 +711,70 @@
                      consts
                      names      ('start',)
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   '/app/deepsecrets/core/model/file.py'
                      name       '<listcomp>'
-                     firstlineno 68
+                     firstlineno 67
                      lnotab 0x
                   '\n'
                   0
                   1
                names      ('re', 'finditer', 'content', 'enumerate', 'line_offsets', 'len', 'length')
                varnames   ('self', 'line_breaks', 'i', 'lb', 'start')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_calc_offsets'
-               firstlineno 67
+               firstlineno 66
                lnotab 0x0201480128012c012002460126ff
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab01000000000000000035007d017c01a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d027c02640119
                   00000000000000000064026b030000000072057c0264027a0d00007d027c
                   026302640064006400a6020000ab02000000000000000001005300230031
                   0073047702780359007701010059000100010064005300
-                76           0 RESUME                   0
+                75           0 RESUME                   0
                
-                77           2 LOAD_GLOBAL              1 (NULL + open)
+                76           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (path)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 BEFORE_WITH
                             42 STORE_FAST               1 (f)
                
-                78          44 LOAD_FAST                1 (f)
+                77          44 LOAD_FAST                1 (f)
                             46 LOAD_METHOD              2 (read)
                             68 PRECALL                  0
                             72 CALL                     0
                             82 STORE_FAST               2 (raw)
                
-                79          84 LOAD_FAST                2 (raw)
+                78          84 LOAD_FAST                2 (raw)
                             86 LOAD_CONST               1 (-1)
                             88 BINARY_SUBSCR
                             98 LOAD_CONST               2 ('\n')
                            100 COMPARE_OP               3 (!=)
                            106 POP_JUMP_FORWARD_IF_FALSE     5 (to 118)
                
-                80         108 LOAD_FAST                2 (raw)
+                79         108 LOAD_FAST                2 (raw)
                            110 LOAD_CONST               2 ('\n')
                            112 BINARY_OP               13 (+=)
                            116 STORE_FAST               2 (raw)
                
-                81     >>  118 LOAD_FAST                2 (raw)
+                80     >>  118 LOAD_FAST                2 (raw)
                
-                77         120 SWAP                     2
+                76         120 SWAP                     2
                            122 LOAD_CONST               0 (None)
                            124 LOAD_CONST               0 (None)
                            126 LOAD_CONST               0 (None)
                            128 PRECALL                  2
                            132 CALL                     2
                            142 POP_TOP
                            144 RETURN_VALUE
@@ -805,28 +801,28 @@
                   '\n'
                names      ('open', 'path', 'read')
                varnames   ('self', 'f', 'raw')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_contents'
-               firstlineno 76
+               firstlineno 75
                lnotab 0x02012a01280118010a0102fc
             'position'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01ac
                   01a6010000ab0100000000000000005300
-                83           0 RESUME                   0
+                82           0 RESUME                   0
                
-                84           2 LOAD_FAST                0 (self)
+                83           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_get_line_number_for_position)
                             26 LOAD_FAST                1 (position)
                             28 KW_NAMES                 1
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RETURN_VALUE
                consts
@@ -834,174 +830,174 @@
                   ('position',)
                names      ('_get_line_number_for_position',)
                varnames   ('self', 'position')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_line_number'
-               firstlineno 83
+               firstlineno 82
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab00000000000000000044005d155c0200007d
                   027d037c036401190000000000000000007c016b000000000072018c127c
                   0263020100530064005300
-                86           0 RESUME                   0
+                85           0 RESUME                   0
                
-                87           2 LOAD_FAST                0 (self)
+                86           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (line_offsets)
                             14 LOAD_METHOD              1 (items)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 GET_ITER
                        >>   52 FOR_ITER                21 (to 96)
                             54 UNPACK_SEQUENCE          2
                             58 STORE_FAST               2 (linum)
                             60 STORE_FAST               3 (offsets)
                
-                88          62 LOAD_FAST                3 (offsets)
+                87          62 LOAD_FAST                3 (offsets)
                             64 LOAD_CONST               1 (1)
                             66 BINARY_SUBSCR
                             76 LOAD_FAST                1 (position)
                             78 COMPARE_OP               0 (<)
                             84 POP_JUMP_FORWARD_IF_FALSE     1 (to 88)
                
-                89          86 JUMP_BACKWARD           18 (to 52)
+                88          86 JUMP_BACKWARD           18 (to 52)
                
-                90     >>   88 LOAD_FAST                2 (linum)
+                89     >>   88 LOAD_FAST                2 (linum)
                             90 SWAP                     2
                             92 POP_TOP
                             94 RETURN_VALUE
                
-                91     >>   96 LOAD_CONST               0 (None)
+                90     >>   96 LOAD_CONST               0 (None)
                             98 RETURN_VALUE
                consts
                   None
                   1
                names      ('line_offsets', 'items')
                varnames   ('self', 'position', 'linum', 'offsets')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_line_number_for_position'
-               firstlineno 86
+               firstlineno 85
                lnotab 0x02013c01180102010801
             'line_number'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c018002640053007c017c006a000000000000000000760172397c
                   006a0100000000000000007c006a0200000000000000007c011900000000
                   00000000006401190000000000000000007c006a0200000000000000007c
                   011900000000000000000064021900000000000000000085021900000000
                   00000000007c006a0000000000000000007c013c0000007c006a00000000
                   00000000007c01190000000000000000005300
-                93           0 RESUME                   0
+                92           0 RESUME                   0
                
-                94           2 LOAD_FAST                1 (line_number)
+                93           2 LOAD_FAST                1 (line_number)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 10)
                
-                95           6 LOAD_CONST               0 (None)
+                94           6 LOAD_CONST               0 (None)
                              8 RETURN_VALUE
                
-                97     >>   10 LOAD_FAST                1 (line_number)
+                96     >>   10 LOAD_FAST                1 (line_number)
                             12 LOAD_FAST                0 (self)
                             14 LOAD_ATTR                0 (line_contents_cache)
                             24 CONTAINS_OP              1
                             26 POP_JUMP_FORWARD_IF_FALSE    57 (to 142)
                
-                98          28 LOAD_FAST                0 (self)
+                97          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                1 (content)
                
-                99          40 LOAD_FAST                0 (self)
+                98          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                2 (line_offsets)
                             52 LOAD_FAST                1 (line_number)
                             54 BINARY_SUBSCR
                             64 LOAD_CONST               1 (0)
                             66 BINARY_SUBSCR
                             76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                2 (line_offsets)
                             88 LOAD_FAST                1 (line_number)
                             90 BINARY_SUBSCR
                            100 LOAD_CONST               2 (1)
                            102 BINARY_SUBSCR
                            112 BUILD_SLICE              2
                
-                98         114 BINARY_SUBSCR
+                97         114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 LOAD_ATTR                0 (line_contents_cache)
                            136 LOAD_FAST                1 (line_number)
                            138 STORE_SUBSCR
                
-               101     >>  142 LOAD_FAST                0 (self)
+               100     >>  142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                0 (line_contents_cache)
                            154 LOAD_FAST                1 (line_number)
                            156 BINARY_SUBSCR
                            166 RETURN_VALUE
                consts
                   None
                   0
                   1
                names      ('line_contents_cache', 'content', 'line_offsets')
                varnames   ('self', 'line_number')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_line_contents'
-               firstlineno 93
+               firstlineno 92
                lnotab 0x02010401040212010c014aff1c03
             'span_end'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007d027c028002640053007c00a001000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000005300
-               103           0 RESUME                   0
+               102           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               103           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_get_line_number_for_position)
                             26 LOAD_FAST                1 (span_end)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               2 (linum)
                
-               105          44 LOAD_FAST                2 (linum)
+               104          44 LOAD_FAST                2 (linum)
                             46 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 52)
                
-               106          48 LOAD_CONST               0 (None)
+               105          48 LOAD_CONST               0 (None)
                             50 RETURN_VALUE
                
-               108     >>   52 LOAD_FAST                0 (self)
+               107     >>   52 LOAD_FAST                0 (self)
                             54 LOAD_METHOD              1 (get_line_contents)
                             76 LOAD_FAST                2 (linum)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 RETURN_VALUE
                consts
                   None
                names      ('_get_line_number_for_position', 'get_line_contents')
                varnames   ('self', 'span_end', 'linum')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_full_line_for_position'
-               firstlineno 103
+               firstlineno 102
                lnotab 0x02012a0104010402
             'str'
             'between'
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 5
@@ -1016,77 +1012,77 @@
                   00000064056406a6020000ab0200000000000000007d0474050000000000
                   00000000006a0500000000000000007c047c03a6020000ab020000000000
                   0000007d057c0544005d397d067c06a00600000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d077c026401190000
                   000000000000007c076401190000000000000000007a0000007c02640119
                   0000000000000000007c076402190000000000000000007a000000660263
                   020100530064005300
-               110           0 RESUME                   0
+               109           0 RESUME                   0
                
-               111           2 LOAD_FAST                2 (between)
+               110           2 LOAD_FAST                2 (between)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     9 (to 24)
                
-               112           6 LOAD_CONST               1 (0)
+               111           6 LOAD_CONST               1 (0)
                              8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (length)
                             20 BUILD_TUPLE              2
                             22 STORE_FAST               2 (between)
                
-               114     >>   24 LOAD_FAST                0 (self)
+               113     >>   24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                1 (content)
                             36 LOAD_FAST                2 (between)
                             38 LOAD_CONST               1 (0)
                             40 BINARY_SUBSCR
                             50 LOAD_FAST                2 (between)
                             52 LOAD_CONST               2 (1)
                             54 BINARY_SUBSCR
                             64 BUILD_SLICE              2
                             66 BINARY_SUBSCR
                             76 STORE_FAST               3 (search_window)
                
-               116          78 LOAD_GLOBAL              5 (NULL + re)
+               115          78 LOAD_GLOBAL              5 (NULL + re)
                             90 LOAD_ATTR                3 (escape)
                            100 LOAD_FAST                1 (str)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 STORE_FAST               4 (pattern)
                
-               117         118 LOAD_FAST                4 (pattern)
+               116         118 LOAD_FAST                4 (pattern)
                            120 LOAD_METHOD              4 (replace)
                            142 LOAD_CONST               3 ('\\\n')
                            144 LOAD_CONST               4 ('\n')
                            146 PRECALL                  2
                            150 CALL                     2
                            160 LOAD_METHOD              4 (replace)
                            182 LOAD_CONST               5 ('\\\t')
                            184 LOAD_CONST               6 ('\t')
                            186 PRECALL                  2
                            190 CALL                     2
                            200 STORE_FAST               4 (pattern)
                
-               118         202 LOAD_GLOBAL              5 (NULL + re)
+               117         202 LOAD_GLOBAL              5 (NULL + re)
                            214 LOAD_ATTR                5 (finditer)
                            224 LOAD_FAST                4 (pattern)
                            226 LOAD_FAST                3 (search_window)
                            228 PRECALL                  2
                            232 CALL                     2
                            242 STORE_FAST               5 (detects)
                
-               119         244 LOAD_FAST                5 (detects)
+               118         244 LOAD_FAST                5 (detects)
                            246 GET_ITER
                            248 FOR_ITER                57 (to 364)
                            250 STORE_FAST               6 (detect)
                
-               120         252 LOAD_FAST                6 (detect)
+               119         252 LOAD_FAST                6 (detect)
                            254 LOAD_METHOD              6 (span)
                            276 PRECALL                  0
                            280 CALL                     0
                            290 STORE_FAST               7 (span)
                
-               121         292 LOAD_FAST                2 (between)
+               120         292 LOAD_FAST                2 (between)
                            294 LOAD_CONST               1 (0)
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                7 (span)
                            308 LOAD_CONST               1 (0)
                            310 BINARY_SUBSCR
                            320 BINARY_OP                0 (+)
                            324 LOAD_FAST                2 (between)
@@ -1097,15 +1093,15 @@
                            342 BINARY_SUBSCR
                            352 BINARY_OP                0 (+)
                            356 BUILD_TUPLE              2
                            358 SWAP                     2
                            360 POP_TOP
                            362 RETURN_VALUE
                
-               122     >>  364 LOAD_CONST               0 (None)
+               121     >>  364 LOAD_CONST               0 (None)
                            366 RETURN_VALUE
                consts
                   None
                   0
                   1
                   '\\\n'
                   '\n'
@@ -1113,53 +1109,53 @@
                   '\t'
                names      ('length', 'content', 're', 'escape', 'replace', 'finditer', 'span')
                varnames   ('self', 'str', 'between', 'search_window', 'pattern', 'detects', 'detect', 'span')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_span_for_string'
-               firstlineno 110
+               firstlineno 109
                lnotab 0x0201040112023602280154012a01080128014801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               124           0 RESUME                   0
+               123           0 RESUME                   0
                
-               125           2 LOAD_FAST                0 (self)
+               124           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (path)
                             14 RETURN_VALUE
                consts
                   None
                names      ('path',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '__repr__'
-               firstlineno 124
+               firstlineno 123
                lnotab 0x0201
             (None, None, None)
             ('return', None)
             (None,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'content', 'int', 'line_offsets', 'Dict', 'Tuple', 'line_contents_cache', 'bool', 'Optional', '__init__', '_get_extension', '_try_guess_extension', '_calc_offsets', '_get_contents', 'get_line_number', '_get_line_number_for_position', 'get_line_contents', 'get_full_line_for_position', 'get_span_for_string', '__repr__')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'content', 'int', 'line_offsets', 'Dict', 'Tuple', 'line_contents_cache', 'bool', 'Optional', '__init__', '_get_name', '_get_extension', '_calc_offsets', '_get_contents', 'get_line_number', '_get_line_number_for_position', 'get_line_contents', 'get_full_line_for_position', 'get_span_for_string', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/model/file.py'
          name       'File'
-         firstlineno 9
+         firstlineno 8
          lnotab
-            0x0c010a010a010e010a012e011e010a01160116050201020102fb040202
-            fe02030efd02040efc02050efb020602fa08251807180308090c071c031c
+            0x0c010a010a010e010a012e011e010a010a0116050201020102fb040202
+            fe02030efd02040efc02050efb020602fa08230c05180708090c071c031c
             071c0a1c074e0e
       'File'
-   names      ('regex', 're', 'typing', 'Dict', 'Optional', 'Tuple', 'deepsecrets', 'logger', 'deepsecrets.core.utils.fs', 'get_abspath', 'deepsecrets.core.utils.guess_filetype', 'FileTypeGuesser', 'File')
+   names      ('regex', 're', 'typing', 'Dict', 'Optional', 'Tuple', 'deepsecrets', 'logger', 'deepsecrets.core.utils.fs', 'get_abspath', 'File')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/model/file.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080114020c010c010c03
+   lnotab 0x00ff0201080114020c010c03
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x7e403d64 (Mon Apr 17 12:50:06 2023 UTC)
+moddate:  0x171ea464 (Tue Jul  4 13:26:47 2023 UTC)
 files sz: 2007
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/file.py` & `deepsecrets-1.1.0/deepsecrets/core/model/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import regex as re
 from typing import Dict, Optional, Tuple
 
 from deepsecrets import logger
 from deepsecrets.core.utils.fs import get_abspath
-from deepsecrets.core.utils.guess_filetype import FileTypeGuesser
 
 
 class File:
     relative_path: str
     path: str
     content: str = ''
     length: int
     line_offsets: Dict[int, Tuple[int, int]] = {}
     line_contents_cache: Dict[int, str] = {}
     empty: bool
+    name: str
     extension: Optional[str]
-    guessed_extension: Optional[str]
 
     def __init__(
         self,
         path: str,
         relative_path: Optional[str] = None,
         content: Optional[str] = None,
         offsets: Optional[Dict] = None,
@@ -38,35 +37,35 @@
             try:
                 self.content = self._get_contents()
             except Exception as e:
                 logger.error('Error during fetching file contents')
 
         self.length = len(self.content)
 
+        self.name = self._get_name()
         self.extension = self._get_extension()
-        if self.extension is None:
-            self.guessed_extension = self._try_guess_extension()
-
         self.empty = True if self.length == 0 else False
 
         if offsets is not None:
             self.line_offsets = offsets
 
         if not self.empty and len(self.line_offsets) == 0:
             self._calc_offsets()
 
+    def _get_name(self) -> str:
+        by_slash = self.path.split('/')
+        return by_slash[-1].split('.')[0]
+
+
     def _get_extension(self) -> Optional[str]:
         by_dot = self.path.split('.')
         if len(by_dot) == 1:
             return None
 
         return by_dot[-1]
-    
-    def _try_guess_extension(self) -> Optional[str]:
-        return FileTypeGuesser().guess(self.content)
 
     def _calc_offsets(self) -> None:
         line_breaks = [i.start() for i in re.finditer('\n', self.content)]
         for i, lb in enumerate(line_breaks):
             start = line_breaks[i - 1] + 1 if i > 0 else 0
             self.line_offsets[i + 1] = (start, lb)
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/finding.py` & `deepsecrets-1.1.0/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.1.0/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/model/token.py` & `deepsecrets-1.1.0/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,188 +1,194 @@
 magic:    0xa70d0d0a
-moddate:  0x22418864 (Tue Jun 13 10:12:50 2023 UTC)
-files sz: 5157
+moddate:  0x2ceca364 (Tue Jul  4 09:53:48 2023 UTC)
+files sz: 5166
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c025a02640064036c036d
-      045a046d055a050100640064046c066d065a060100640064056c076d085a
-      080100640064066c096d0a5a0a0100640064076c0b6d0c5a0c6d0d5a0d6d
-      0e5a0e6d0f5a0f6d105a100100640064026c115a12640064086c136d145a
-      140100640064096c156d165a166d175a176d185a1801006400640a6c196d
-      1a5a1a01006400640b6c1b6d1c5a1c6d1d5a1d01006400640c6c1e6d1f5a
-      1f01006400640d6c206d215a2101006400640e6c226d235a230100640064
-      0f6c246d255a250100640064106c266d275a270100020047006411840064
-      12a6020000ab0200000000000000005a28641365146414650d6415652964
-      16650e651c190000000000000000006608641784045a2a64025300
+      0x9700640064016c005a00640064026c016d025a020100640064016c035a
+      03640064036c046d055a056d065a060100640064046c076d075a07010064
+      0064056c086d095a090100640064066c0a6d0b5a0b0100640064076c0c6d
+      0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a110100640064016c125a1364
+      0064086c146d155a150100640064096c166d175a176d185a186d195a1901
+      006400640a6c1a6d1b5a1b01006400640b6c1c6d1d5a1d6d1e5a1e010064
+      00640c6c1f6d205a2001006400640d6c216d225a2201006400640e6c236d
+      245a2401006400640f6c256d265a260100640064106c276d285a28010002
+      004700641184006412a6020000ab0200000000000000005a296413651564
+      14650e6415652a6416650f651d190000000000000000006608641784045a
+      2b64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('get_context',))
-                 6 IMPORT_NAME              0 (multiprocessing)
-                 8 IMPORT_FROM              1 (get_context)
-                10 STORE_NAME               1 (get_context)
-                12 POP_TOP
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (logging)
+                 8 STORE_NAME               0 (logging)
    
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (None)
-                18 IMPORT_NAME              2 (os)
-                20 STORE_NAME               2 (os)
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('get_context',))
+                14 IMPORT_NAME              1 (multiprocessing)
+                16 IMPORT_FROM              2 (get_context)
+                18 STORE_NAME               2 (get_context)
+                20 POP_TOP
    
      3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('abstractmethod', 'abstractstaticmethod'))
-                26 IMPORT_NAME              3 (abc)
-                28 IMPORT_FROM              4 (abstractmethod)
-                30 STORE_NAME               4 (abstractmethod)
-                32 IMPORT_FROM              5 (abstractstaticmethod)
-                34 STORE_NAME               5 (abstractstaticmethod)
-                36 POP_TOP
+                24 LOAD_CONST               1 (None)
+                26 IMPORT_NAME              3 (os)
+                28 STORE_NAME               3 (os)
    
-     4          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               4 (('datetime',))
-                42 IMPORT_NAME              6 (datetime)
-                44 IMPORT_FROM              6 (datetime)
-                46 STORE_NAME               6 (datetime)
-                48 POP_TOP
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('abstractmethod', 'abstractstaticmethod'))
+                34 IMPORT_NAME              4 (abc)
+                36 IMPORT_FROM              5 (abstractmethod)
+                38 STORE_NAME               5 (abstractmethod)
+                40 IMPORT_FROM              6 (abstractstaticmethod)
+                42 STORE_NAME               6 (abstractstaticmethod)
+                44 POP_TOP
    
-     5          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               5 (('partial',))
-                54 IMPORT_NAME              7 (functools)
-                56 IMPORT_FROM              8 (partial)
-                58 STORE_NAME               8 (partial)
-                60 POP_TOP
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('datetime',))
+                50 IMPORT_NAME              7 (datetime)
+                52 IMPORT_FROM              7 (datetime)
+                54 STORE_NAME               7 (datetime)
+                56 POP_TOP
    
-     6          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               6 (('Pool',))
-                66 IMPORT_NAME              9 (multiprocessing.pool)
-                68 IMPORT_FROM             10 (Pool)
-                70 STORE_NAME              10 (Pool)
-                72 POP_TOP
+     6          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('partial',))
+                62 IMPORT_NAME              8 (functools)
+                64 IMPORT_FROM              9 (partial)
+                66 STORE_NAME               9 (partial)
+                68 POP_TOP
    
-     7          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               7 (('Any', 'Callable', 'List', 'Optional', 'Type'))
-                78 IMPORT_NAME             11 (typing)
-                80 IMPORT_FROM             12 (Any)
-                82 STORE_NAME              12 (Any)
-                84 IMPORT_FROM             13 (Callable)
-                86 STORE_NAME              13 (Callable)
-                88 IMPORT_FROM             14 (List)
-                90 STORE_NAME              14 (List)
-                92 IMPORT_FROM             15 (Optional)
-                94 STORE_NAME              15 (Optional)
-                96 IMPORT_FROM             16 (Type)
-                98 STORE_NAME              16 (Type)
-               100 POP_TOP
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('Pool',))
+                74 IMPORT_NAME             10 (multiprocessing.pool)
+                76 IMPORT_FROM             11 (Pool)
+                78 STORE_NAME              11 (Pool)
+                80 POP_TOP
    
-     8         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               2 (None)
-               106 IMPORT_NAME             17 (regex)
-               108 STORE_NAME              18 (re)
+     8          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               7 (('Any', 'Callable', 'List', 'Optional', 'Type'))
+                86 IMPORT_NAME             12 (typing)
+                88 IMPORT_FROM             13 (Any)
+                90 STORE_NAME              13 (Any)
+                92 IMPORT_FROM             14 (Callable)
+                94 STORE_NAME              14 (Callable)
+                96 IMPORT_FROM             15 (List)
+                98 STORE_NAME              15 (List)
+               100 IMPORT_FROM             16 (Optional)
+               102 STORE_NAME              16 (Optional)
+               104 IMPORT_FROM             17 (Type)
+               106 STORE_NAME              17 (Type)
+               108 POP_TOP
    
-    10         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               8 (('DotWiz',))
-               114 IMPORT_NAME             19 (dotwiz)
-               116 IMPORT_FROM             20 (DotWiz)
-               118 STORE_NAME              20 (DotWiz)
-               120 POP_TOP
+     9         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               1 (None)
+               114 IMPORT_NAME             18 (regex)
+               116 STORE_NAME              19 (re)
    
-    12         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST               9 (('PLATFORM', 'PROFILER_ON', 'logger'))
-               126 IMPORT_NAME             21 (deepsecrets)
-               128 IMPORT_FROM             22 (PLATFORM)
-               130 STORE_NAME              22 (PLATFORM)
-               132 IMPORT_FROM             23 (PROFILER_ON)
-               134 STORE_NAME              23 (PROFILER_ON)
-               136 IMPORT_FROM             24 (logger)
-               138 STORE_NAME              24 (logger)
-               140 POP_TOP
+    11         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               8 (('DotWiz',))
+               122 IMPORT_NAME             20 (dotwiz)
+               124 IMPORT_FROM             21 (DotWiz)
+               126 STORE_NAME              21 (DotWiz)
+               128 POP_TOP
    
-    13         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              10 (('Config',))
-               146 IMPORT_NAME             25 (deepsecrets.config)
-               148 IMPORT_FROM             26 (Config)
-               150 STORE_NAME              26 (Config)
-               152 POP_TOP
+    13         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST               9 (('PLATFORM', 'PROFILER_ON', 'logger'))
+               134 IMPORT_NAME             22 (deepsecrets)
+               136 IMPORT_FROM             23 (PLATFORM)
+               138 STORE_NAME              23 (PLATFORM)
+               140 IMPORT_FROM             24 (PROFILER_ON)
+               142 STORE_NAME              24 (PROFILER_ON)
+               144 IMPORT_FROM             25 (logger)
+               146 STORE_NAME              25 (logger)
+               148 POP_TOP
    
-    14         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST              11 (('Finding', 'FindingMerger'))
-               158 IMPORT_NAME             27 (deepsecrets.core.model.finding)
-               160 IMPORT_FROM             28 (Finding)
-               162 STORE_NAME              28 (Finding)
-               164 IMPORT_FROM             29 (FindingMerger)
-               166 STORE_NAME              29 (FindingMerger)
-               168 POP_TOP
+    14         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST              10 (('Config',))
+               154 IMPORT_NAME             26 (deepsecrets.config)
+               156 IMPORT_FROM             27 (Config)
+               158 STORE_NAME              27 (Config)
+               160 POP_TOP
    
-    15         170 LOAD_CONST               0 (0)
-               172 LOAD_CONST              12 (('ExcludePathRule',))
-               174 IMPORT_NAME             30 (deepsecrets.core.model.rules.exlcuded_path)
-               176 IMPORT_FROM             31 (ExcludePathRule)
-               178 STORE_NAME              31 (ExcludePathRule)
-               180 POP_TOP
+    15         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST              11 (('Finding', 'FindingMerger'))
+               166 IMPORT_NAME             28 (deepsecrets.core.model.finding)
+               168 IMPORT_FROM             29 (Finding)
+               170 STORE_NAME              29 (Finding)
+               172 IMPORT_FROM             30 (FindingMerger)
+               174 STORE_NAME              30 (FindingMerger)
+               176 POP_TOP
    
-    16         182 LOAD_CONST               0 (0)
-               184 LOAD_CONST              13 (('ExcludedPathsBuilder',))
-               186 IMPORT_NAME             32 (deepsecrets.core.rulesets.excluded_paths)
-               188 IMPORT_FROM             33 (ExcludedPathsBuilder)
-               190 STORE_NAME              33 (ExcludedPathsBuilder)
-               192 POP_TOP
+    16         178 LOAD_CONST               0 (0)
+               180 LOAD_CONST              12 (('ExcludePathRule',))
+               182 IMPORT_NAME             31 (deepsecrets.core.model.rules.exlcuded_path)
+               184 IMPORT_FROM             32 (ExcludePathRule)
+               186 STORE_NAME              32 (ExcludePathRule)
+               188 POP_TOP
    
-    17         194 LOAD_CONST               0 (0)
-               196 LOAD_CONST              14 (('FalseFindingsBuilder',))
-               198 IMPORT_NAME             34 (deepsecrets.core.rulesets.false_findings)
-               200 IMPORT_FROM             35 (FalseFindingsBuilder)
-               202 STORE_NAME              35 (FalseFindingsBuilder)
-               204 POP_TOP
+    17         190 LOAD_CONST               0 (0)
+               192 LOAD_CONST              13 (('ExcludedPathsBuilder',))
+               194 IMPORT_NAME             33 (deepsecrets.core.rulesets.excluded_paths)
+               196 IMPORT_FROM             34 (ExcludedPathsBuilder)
+               198 STORE_NAME              34 (ExcludedPathsBuilder)
+               200 POP_TOP
    
-    18         206 LOAD_CONST               0 (0)
-               208 LOAD_CONST              15 (('FileAnalyzer',))
-               210 IMPORT_NAME             36 (deepsecrets.core.utils.file_analyzer)
-               212 IMPORT_FROM             37 (FileAnalyzer)
-               214 STORE_NAME              37 (FileAnalyzer)
-               216 POP_TOP
+    18         202 LOAD_CONST               0 (0)
+               204 LOAD_CONST              14 (('FalseFindingsBuilder',))
+               206 IMPORT_NAME             35 (deepsecrets.core.rulesets.false_findings)
+               208 IMPORT_FROM             36 (FalseFindingsBuilder)
+               210 STORE_NAME              36 (FalseFindingsBuilder)
+               212 POP_TOP
    
-    19         218 LOAD_CONST               0 (0)
-               220 LOAD_CONST              16 (('get_abspath',))
-               222 IMPORT_NAME             38 (deepsecrets.core.utils.fs)
-               224 IMPORT_FROM             39 (get_abspath)
-               226 STORE_NAME              39 (get_abspath)
-               228 POP_TOP
+    19         214 LOAD_CONST               0 (0)
+               216 LOAD_CONST              15 (('FileAnalyzer',))
+               218 IMPORT_NAME             37 (deepsecrets.core.utils.file_analyzer)
+               220 IMPORT_FROM             38 (FileAnalyzer)
+               222 STORE_NAME              38 (FileAnalyzer)
+               224 POP_TOP
    
-    22         230 PUSH_NULL
-               232 LOAD_BUILD_CLASS
-               234 LOAD_CONST              17 (<code object ScanMode, file "/app/deepsecrets/core/modes/iscan_mode.py", line 22>)
-               236 MAKE_FUNCTION            0
-               238 LOAD_CONST              18 ('ScanMode')
-               240 PRECALL                  2
-               244 CALL                     2
-               254 STORE_NAME              40 (ScanMode)
+    20         226 LOAD_CONST               0 (0)
+               228 LOAD_CONST              16 (('get_abspath',))
+               230 IMPORT_NAME             39 (deepsecrets.core.utils.fs)
+               232 IMPORT_FROM             40 (get_abspath)
+               234 STORE_NAME              40 (get_abspath)
+               236 POP_TOP
    
-   143         256 LOAD_CONST              19 ('bundle')
-               258 LOAD_NAME               20 (DotWiz)
-               260 LOAD_CONST              20 ('runner')
-               262 LOAD_NAME               13 (Callable)
-               264 LOAD_CONST              21 ('file')
-               266 LOAD_NAME               41 (str)
-               268 LOAD_CONST              22 ('return')
-               270 LOAD_NAME               14 (List)
-               272 LOAD_NAME               28 (Finding)
-               274 BINARY_SUBSCR
-               284 BUILD_TUPLE              8
-               286 LOAD_CONST              23 (<code object pool_wrapper, file "/app/deepsecrets/core/modes/iscan_mode.py", line 143>)
-               288 MAKE_FUNCTION            4 (annotations)
-               290 STORE_NAME              42 (pool_wrapper)
-               292 LOAD_CONST               2 (None)
-               294 RETURN_VALUE
+    23         238 PUSH_NULL
+               240 LOAD_BUILD_CLASS
+               242 LOAD_CONST              17 (<code object ScanMode, file "/app/deepsecrets/core/modes/iscan_mode.py", line 23>)
+               244 MAKE_FUNCTION            0
+               246 LOAD_CONST              18 ('ScanMode')
+               248 PRECALL                  2
+               252 CALL                     2
+               262 STORE_NAME              41 (ScanMode)
+   
+   142         264 LOAD_CONST              19 ('bundle')
+               266 LOAD_NAME               21 (DotWiz)
+               268 LOAD_CONST              20 ('runner')
+               270 LOAD_NAME               14 (Callable)
+               272 LOAD_CONST              21 ('file')
+               274 LOAD_NAME               42 (str)
+               276 LOAD_CONST              22 ('return')
+               278 LOAD_NAME               15 (List)
+               280 LOAD_NAME               29 (Finding)
+               282 BINARY_SUBSCR
+               292 BUILD_TUPLE              8
+               294 LOAD_CONST              23 (<code object pool_wrapper, file "/app/deepsecrets/core/modes/iscan_mode.py", line 142>)
+               296 MAKE_FUNCTION            4 (annotations)
+               298 STORE_NAME              43 (pool_wrapper)
+               300 LOAD_CONST               1 (None)
+               302 RETURN_VALUE
    consts
       0
-      ('get_context',)
       None
+      ('get_context',)
       ('abstractmethod', 'abstractstaticmethod')
       ('datetime',)
       ('partial',)
       ('Pool',)
       ('Any', 'Callable', 'List', 'Optional', 'Type')
       ('DotWiz',)
       ('PLATFORM', 'PROFILER_ON', 'logger')
@@ -206,145 +212,145 @@
             0884055a0d6407650e6602640984045a0f64076505651019000000000000
             0000006602640a84045a1164076505650619000000000000000000660264
             0b84045a12640c6506640765136604640d84045a1465156415640e8404a6
             000000ab0000000000000000005a16640765176602640f84045a18651964
             10650c64076505651019000000000000000000660464118404a6000000ab
             0000000000000000005a1a64126505651019000000000000000000640765
             056510190000000000000000006604641384045a1b64065300
-          22           0 RESUME                   0
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ScanMode')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          23          12 LOAD_NAME                3 (Config)
+          24          12 LOAD_NAME                3 (Config)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('config')
                       18 STORE_SUBSCR
          
-          24          22 LOAD_NAME                5 (List)
+          25          22 LOAD_NAME                5 (List)
                       24 LOAD_NAME                6 (str)
                       26 BINARY_SUBSCR
                       36 LOAD_NAME                4 (__annotations__)
                       38 LOAD_CONST               2 ('filepaths')
                       40 STORE_SUBSCR
          
-          25          44 BUILD_LIST               0
+          26          44 BUILD_LIST               0
                       46 STORE_NAME               7 (path_exclusion_rules)
                       48 LOAD_NAME                5 (List)
                       50 LOAD_NAME                8 (ExcludePathRule)
                       52 BINARY_SUBSCR
                       62 LOAD_NAME                4 (__annotations__)
                       64 LOAD_CONST               3 ('path_exclusion_rules')
                       66 STORE_SUBSCR
          
-          26          70 LOAD_NAME                9 (FileAnalyzer)
+          27          70 LOAD_NAME                9 (FileAnalyzer)
                       72 LOAD_NAME                4 (__annotations__)
                       74 LOAD_CONST               4 ('file_analyzer')
                       76 STORE_SUBSCR
          
-          27          80 LOAD_NAME               10 (Type)
+          28          80 LOAD_NAME               10 (Type)
                       82 LOAD_NAME                4 (__annotations__)
                       84 LOAD_CONST               5 ('pool_engine')
                       86 STORE_SUBSCR
          
-          29          90 LOAD_CONST              20 ((None,))
+          30          90 LOAD_CONST              20 ((None,))
                       92 LOAD_CONST               1 ('config')
                       94 LOAD_NAME                3 (Config)
                       96 LOAD_CONST               5 ('pool_engine')
                       98 LOAD_NAME               11 (Optional)
                      100 LOAD_NAME               12 (Any)
                      102 BINARY_SUBSCR
                      112 LOAD_CONST               7 ('return')
                      114 LOAD_CONST               6 (None)
                      116 BUILD_TUPLE              6
-                     118 LOAD_CONST               8 (<code object __init__, file "/app/deepsecrets/core/modes/iscan_mode.py", line 29>)
+                     118 LOAD_CONST               8 (<code object __init__, file "/app/deepsecrets/core/modes/iscan_mode.py", line 30>)
                      120 MAKE_FUNCTION            5 (defaults, annotations)
                      122 STORE_NAME              13 (__init__)
          
-          42         124 LOAD_CONST               7 ('return')
+          43         124 LOAD_CONST               7 ('return')
                      126 LOAD_NAME               14 (int)
                      128 BUILD_TUPLE              2
-                     130 LOAD_CONST               9 (<code object _get_process_count_for_runner, file "/app/deepsecrets/core/modes/iscan_mode.py", line 42>)
+                     130 LOAD_CONST               9 (<code object _get_process_count_for_runner, file "/app/deepsecrets/core/modes/iscan_mode.py", line 43>)
                      132 MAKE_FUNCTION            4 (annotations)
                      134 STORE_NAME              15 (_get_process_count_for_runner)
          
-          49         136 LOAD_CONST               7 ('return')
+          51         136 LOAD_CONST               7 ('return')
                      138 LOAD_NAME                5 (List)
                      140 LOAD_NAME               16 (Finding)
                      142 BINARY_SUBSCR
                      152 BUILD_TUPLE              2
-                     154 LOAD_CONST              10 (<code object run, file "/app/deepsecrets/core/modes/iscan_mode.py", line 49>)
+                     154 LOAD_CONST              10 (<code object run, file "/app/deepsecrets/core/modes/iscan_mode.py", line 51>)
                      156 MAKE_FUNCTION            4 (annotations)
                      158 STORE_NAME              17 (run)
          
-          79         160 LOAD_CONST               7 ('return')
+          78         160 LOAD_CONST               7 ('return')
                      162 LOAD_NAME                5 (List)
                      164 LOAD_NAME                6 (str)
                      166 BINARY_SUBSCR
                      176 BUILD_TUPLE              2
-                     178 LOAD_CONST              11 (<code object _get_files_list, file "/app/deepsecrets/core/modes/iscan_mode.py", line 79>)
+                     178 LOAD_CONST              11 (<code object _get_files_list, file "/app/deepsecrets/core/modes/iscan_mode.py", line 78>)
                      180 MAKE_FUNCTION            4 (annotations)
                      182 STORE_NAME              18 (_get_files_list)
          
-          99         184 LOAD_CONST              12 ('path')
+          98         184 LOAD_CONST              12 ('path')
                      186 LOAD_NAME                6 (str)
                      188 LOAD_CONST               7 ('return')
                      190 LOAD_NAME               19 (bool)
                      192 BUILD_TUPLE              4
-                     194 LOAD_CONST              13 (<code object _path_included, file "/app/deepsecrets/core/modes/iscan_mode.py", line 99>)
+                     194 LOAD_CONST              13 (<code object _path_included, file "/app/deepsecrets/core/modes/iscan_mode.py", line 98>)
                      196 MAKE_FUNCTION            4 (annotations)
                      198 STORE_NAME              20 (_path_included)
          
-         107         200 LOAD_NAME               21 (abstractmethod)
+         106         200 LOAD_NAME               21 (abstractmethod)
          
-         108         202 LOAD_CONST              21 (('return', None))
-                     204 LOAD_CONST              14 (<code object prepare_for_scan, file "/app/deepsecrets/core/modes/iscan_mode.py", line 107>)
+         107         202 LOAD_CONST              21 (('return', None))
+                     204 LOAD_CONST              14 (<code object prepare_for_scan, file "/app/deepsecrets/core/modes/iscan_mode.py", line 106>)
                      206 MAKE_FUNCTION            4 (annotations)
          
-         107         208 PRECALL                  0
+         106         208 PRECALL                  0
                      212 CALL                     0
          
-         108         222 STORE_NAME              22 (prepare_for_scan)
+         107         222 STORE_NAME              22 (prepare_for_scan)
          
-         111         224 LOAD_CONST               7 ('return')
+         110         224 LOAD_CONST               7 ('return')
                      226 LOAD_NAME               23 (DotWiz)
                      228 BUILD_TUPLE              2
-                     230 LOAD_CONST              15 (<code object analyzer_bundle, file "/app/deepsecrets/core/modes/iscan_mode.py", line 111>)
+                     230 LOAD_CONST              15 (<code object analyzer_bundle, file "/app/deepsecrets/core/modes/iscan_mode.py", line 110>)
                      232 MAKE_FUNCTION            4 (annotations)
                      234 STORE_NAME              24 (analyzer_bundle)
          
-         118         236 LOAD_NAME               25 (abstractstaticmethod)
+         117         236 LOAD_NAME               25 (abstractstaticmethod)
          
-         119         238 LOAD_CONST              16 ('file')
+         118         238 LOAD_CONST              16 ('file')
                      240 LOAD_NAME               12 (Any)
                      242 LOAD_CONST               7 ('return')
                      244 LOAD_NAME                5 (List)
                      246 LOAD_NAME               16 (Finding)
                      248 BINARY_SUBSCR
                      258 BUILD_TUPLE              4
-                     260 LOAD_CONST              17 (<code object _per_file_analyzer, file "/app/deepsecrets/core/modes/iscan_mode.py", line 118>)
+                     260 LOAD_CONST              17 (<code object _per_file_analyzer, file "/app/deepsecrets/core/modes/iscan_mode.py", line 117>)
                      262 MAKE_FUNCTION            4 (annotations)
          
-         118         264 PRECALL                  0
+         117         264 PRECALL                  0
                      268 CALL                     0
          
-         119         278 STORE_NAME              26 (_per_file_analyzer)
+         118         278 STORE_NAME              26 (_per_file_analyzer)
          
-         122         280 LOAD_CONST              18 ('results')
+         121         280 LOAD_CONST              18 ('results')
                      282 LOAD_NAME                5 (List)
                      284 LOAD_NAME               16 (Finding)
                      286 BINARY_SUBSCR
                      296 LOAD_CONST               7 ('return')
                      298 LOAD_NAME                5 (List)
                      300 LOAD_NAME               16 (Finding)
                      302 BINARY_SUBSCR
                      312 BUILD_TUPLE              4
-                     314 LOAD_CONST              19 (<code object filter_false_positives, file "/app/deepsecrets/core/modes/iscan_mode.py", line 122>)
+                     314 LOAD_CONST              19 (<code object filter_false_positives, file "/app/deepsecrets/core/modes/iscan_mode.py", line 121>)
                      316 MAKE_FUNCTION            4 (annotations)
                      318 STORE_NAME              27 (filter_false_positives)
                      320 LOAD_CONST               6 (None)
                      322 RETURN_VALUE
          consts
             'ScanMode'
             'config'
@@ -364,54 +370,54 @@
                   03000000000000000000006402a6010000ab0100000000000000006a0200
                   000000000000007c005f0300000000000000006e14740400000000000000
                   0000007c005f0300000000000000006e077c027c005f0300000000000000
                   007c017c005f0400000000000000007c00a0050000000000000000000000
                   000000000000000000a6000000ab0000000000000000007c005f06000000
                   00000000007c00a0070000000000000000000000000000000000000000a6
                   000000ab000000000000000000010064005300
-                29           0 RESUME                   0
+                30           0 RESUME                   0
                
-                30           2 LOAD_FAST                2 (pool_engine)
+                31           2 LOAD_FAST                2 (pool_engine)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE    50 (to 106)
                
-                31           6 LOAD_GLOBAL              0 (PLATFORM)
+                32           6 LOAD_GLOBAL              0 (PLATFORM)
                             18 LOAD_CONST               1 ('Darwin')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE    26 (to 80)
                
-                32          28 LOAD_GLOBAL              3 (NULL + get_context)
+                33          28 LOAD_GLOBAL              3 (NULL + get_context)
                             40 LOAD_CONST               2 ('fork')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_ATTR                2 (Pool)
                             66 LOAD_FAST                0 (self)
                             68 STORE_ATTR               3 (pool_engine)
                             78 JUMP_FORWARD            20 (to 120)
                
-                34     >>   80 LOAD_GLOBAL              4 (Pool)
+                35     >>   80 LOAD_GLOBAL              4 (Pool)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               3 (pool_engine)
                            104 JUMP_FORWARD             7 (to 120)
                
-                36     >>  106 LOAD_FAST                2 (pool_engine)
+                37     >>  106 LOAD_FAST                2 (pool_engine)
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               3 (pool_engine)
                
-                38     >>  120 LOAD_FAST                1 (config)
+                39     >>  120 LOAD_FAST                1 (config)
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (config)
                
-                39         134 LOAD_FAST                0 (self)
+                40         134 LOAD_FAST                0 (self)
                            136 LOAD_METHOD              5 (_get_files_list)
                            158 PRECALL                  0
                            162 CALL                     0
                            172 LOAD_FAST                0 (self)
                            174 STORE_ATTR               6 (filepaths)
                
-                40         184 LOAD_FAST                0 (self)
+                41         184 LOAD_FAST                0 (self)
                            186 LOAD_METHOD              7 (prepare_for_scan)
                            208 PRECALL                  0
                            212 CALL                     0
                            222 POP_TOP
                            224 LOAD_CONST               0 (None)
                            226 RETURN_VALUE
                consts
@@ -420,245 +426,248 @@
                   'fork'
                names      ('PLATFORM', 'get_context', 'Pool', 'pool_engine', 'config', '_get_files_list', 'filepaths', 'prepare_for_scan')
                varnames   ('self', 'config', 'pool_engine')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       '__init__'
-               firstlineno 29
+               firstlineno 30
                lnotab 0x02010401160134021a020e020e013201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x970064017d017401000000000000000000007c006a0100000000000000
-                  00a6010000ab0100000000000000007d027c0264026b0200000000720264
-                  0253007c027c016b050000000072027c016e017c025300
-                42           0 RESUME                   0
-               
-                43           2 LOAD_CONST               1 (15)
-                             4 STORE_FAST               1 (base)
-               
-                44           6 LOAD_GLOBAL              1 (NULL + len)
-                            18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (filepaths)
-                            30 PRECALL                  1
-                            34 CALL                     1
-                            44 STORE_FAST               2 (file_count)
-               
-                45          46 LOAD_FAST                2 (file_count)
-                            48 LOAD_CONST               2 (0)
-                            50 COMPARE_OP               2 (==)
-                            56 POP_JUMP_FORWARD_IF_FALSE     2 (to 62)
-               
-                46          58 LOAD_CONST               2 (0)
-                            60 RETURN_VALUE
-               
-                47     >>   62 LOAD_FAST                2 (file_count)
-                            64 LOAD_FAST                1 (base)
-                            66 COMPARE_OP               5 (>=)
-                            72 POP_JUMP_FORWARD_IF_FALSE     2 (to 78)
-                            74 LOAD_FAST                1 (base)
-                            76 JUMP_FORWARD             1 (to 80)
-                       >>   78 LOAD_FAST                2 (file_count)
-                       >>   80 RETURN_VALUE
+                  0x97007c006a0000000000000000006a0100000000000000007d01740500
+                  0000000000000000007c006a030000000000000000a6010000ab01000000
+                  00000000007d027c0264016b02000000007202640153007c027c016b0500
+                  00000072027c016e017c025300
+                43           0 RESUME                   0
+               
+                44           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (config)
+                            14 LOAD_ATTR                1 (process_count)
+                            24 STORE_FAST               1 (limit)
+               
+                46          26 LOAD_GLOBAL              5 (NULL + len)
+                            38 LOAD_FAST                0 (self)
+                            40 LOAD_ATTR                3 (filepaths)
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 STORE_FAST               2 (file_count)
+               
+                47          66 LOAD_FAST                2 (file_count)
+                            68 LOAD_CONST               1 (0)
+                            70 COMPARE_OP               2 (==)
+                            76 POP_JUMP_FORWARD_IF_FALSE     2 (to 82)
+               
+                48          78 LOAD_CONST               1 (0)
+                            80 RETURN_VALUE
+               
+                49     >>   82 LOAD_FAST                2 (file_count)
+                            84 LOAD_FAST                1 (limit)
+                            86 COMPARE_OP               5 (>=)
+                            92 POP_JUMP_FORWARD_IF_FALSE     2 (to 98)
+                            94 LOAD_FAST                1 (limit)
+                            96 JUMP_FORWARD             1 (to 100)
+                       >>   98 LOAD_FAST                2 (file_count)
+                       >>  100 RETURN_VALUE
                consts
                   None
-                  15
                   0
-               names      ('len', 'filepaths')
-               varnames   ('self', 'base', 'file_count')
+               names      ('config', 'process_count', 'len', 'filepaths')
+               varnames   ('self', 'limit', 'file_count')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       '_get_process_count_for_runner'
-               firstlineno 42
-               lnotab 0x0201040128010c010401
+               firstlineno 43
+               lnotab 0x0201180228010c010401
             code
                argcount  : 1
                nlocals   : 9
                stacksize : 8
                flags     : 3
                code
                   0x970067007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d027c00a001000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d037c0364
-                  016b020000000072027c01530074040000000000000000000072347c006a
-                  03000000000000000044005d2b7d047c01a0040000000000000000000000
+                  016b020000000072027c01530074040000000000000000000072357c006a
+                  03000000000000000044005d2c7d047c01a0040000000000000000000000
                   0000000000000000007c00a0050000000000000000000000000000000000
-                  0000007c04ac02a6010000ab010000000000000000a6010000ab01000000
-                  000000000001008c2c6e8c7c00a006000000000000000000000000000000
-                  00000000007c03ac03a6010000ab01000000000000000035007d057c05a0
-                  070000000000000000000000000000000000000000741100000000000000
-                  0000007412000000000000000000007c027c006a050000000000000000a6
-                  030000ab0300000000000000007c006a030000000000000000a6020000ab
-                  0200000000000000007d06640064006400a6020000ab0200000000000000
-                  0001006e0b23003100730477027803590077010100590001000100741500
-                  0000000000000000007c06a6010000ab01000000000000000044005d1a7d
-                  077c0773018c057c01a00400000000000000000000000000000000000000
-                  007c07a6010000ab01000000000000000001008c1b741700000000000000
-                  0000007c01a6010000ab010000000000000000a00c000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000007d087c00a0
-                  0d00000000000000000000000000000000000000007c08a6010000ab0100
-                  000000000000007d087c085300
-                49           0 RESUME                   0
+                  0000007c047c02ac02a6020000ab020000000000000000a6010000ab0100
+                  0000000000000001008c2d6e8c7c00a00600000000000000000000000000
+                  000000000000007c03ac03a6010000ab01000000000000000035007d057c
+                  05a007000000000000000000000000000000000000000074110000000000
+                  00000000007412000000000000000000007c027c006a0500000000000000
+                  00a6030000ab0300000000000000007c006a030000000000000000a60200
+                  00ab0200000000000000007d06640064006400a6020000ab020000000000
+                  00000001006e0b2300310073047702780359007701010059000100010074
+                  15000000000000000000007c06a6010000ab01000000000000000044005d
+                  1a7d077c0773018c057c01a0040000000000000000000000000000000000
+                  0000007c07a6010000ab01000000000000000001008c1b74170000000000
+                  00000000007c01a6010000ab010000000000000000a00c00000000000000
+                  00000000000000000000000000a6000000ab0000000000000000007d087c
+                  00a00d00000000000000000000000000000000000000007c08a6010000ab
+                  0100000000000000007d087c085300
+                51           0 RESUME                   0
                
-                50           2 BUILD_LIST               0
+                52           2 BUILD_LIST               0
                              4 STORE_FAST               1 (final)
                
-                52           6 LOAD_FAST                0 (self)
+                54           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (analyzer_bundle)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 STORE_FAST               2 (bundle)
                
-                53          46 LOAD_FAST                0 (self)
+                55          46 LOAD_FAST                0 (self)
                             48 LOAD_METHOD              1 (_get_process_count_for_runner)
                             70 PRECALL                  0
                             74 CALL                     0
                             84 STORE_FAST               3 (proc_count)
                
-                54          86 LOAD_FAST                3 (proc_count)
+                56          86 LOAD_FAST                3 (proc_count)
                             88 LOAD_CONST               1 (0)
                             90 COMPARE_OP               2 (==)
                             96 POP_JUMP_FORWARD_IF_FALSE     2 (to 102)
                
-                55          98 LOAD_FAST                1 (final)
+                57          98 LOAD_FAST                1 (final)
                            100 RETURN_VALUE
                
-                57     >>  102 LOAD_GLOBAL              4 (PROFILER_ON)
-                           114 POP_JUMP_FORWARD_IF_FALSE    52 (to 220)
+                59     >>  102 LOAD_GLOBAL              4 (PROFILER_ON)
+                           114 POP_JUMP_FORWARD_IF_FALSE    53 (to 222)
                
-                58         116 LOAD_FAST                0 (self)
+                60         116 LOAD_FAST                0 (self)
                            118 LOAD_ATTR                3 (filepaths)
                            128 GET_ITER
-                       >>  130 FOR_ITER                43 (to 218)
+                       >>  130 FOR_ITER                44 (to 220)
                            132 STORE_FAST               4 (file)
                
-                59         134 LOAD_FAST                1 (final)
+                61         134 LOAD_FAST                1 (final)
                            136 LOAD_METHOD              4 (extend)
                            158 LOAD_FAST                0 (self)
                            160 LOAD_METHOD              5 (_per_file_analyzer)
                            182 LOAD_FAST                4 (file)
-                           184 KW_NAMES                 2
-                           186 PRECALL                  1
-                           190 CALL                     1
-                           200 PRECALL                  1
-                           204 CALL                     1
-                           214 POP_TOP
-                           216 JUMP_BACKWARD           44 (to 130)
-               
-                58     >>  218 JUMP_FORWARD           140 (to 500)
+                           184 LOAD_FAST                2 (bundle)
+                           186 KW_NAMES                 2
+                           188 PRECALL                  2
+                           192 CALL                     2
+                           202 PRECALL                  1
+                           206 CALL                     1
+                           216 POP_TOP
+                           218 JUMP_BACKWARD           45 (to 130)
+               
+                60     >>  220 JUMP_FORWARD           140 (to 502)
+               
+                63     >>  222 LOAD_FAST                0 (self)
+                           224 LOAD_METHOD              6 (pool_engine)
+                           246 LOAD_FAST                3 (proc_count)
+                           248 KW_NAMES                 3
+                           250 PRECALL                  1
+                           254 CALL                     1
+                           264 BEFORE_WITH
+                           266 STORE_FAST               5 (pool)
+               
+                64         268 LOAD_FAST                5 (pool)
+                           270 LOAD_METHOD              7 (map)
+               
+                65         292 LOAD_GLOBAL             17 (NULL + partial)
+                           304 LOAD_GLOBAL             18 (pool_wrapper)
+                           316 LOAD_FAST                2 (bundle)
+                           318 LOAD_FAST                0 (self)
+                           320 LOAD_ATTR                5 (_per_file_analyzer)
+                           330 PRECALL                  3
+                           334 CALL                     3
+               
+                66         344 LOAD_FAST                0 (self)
+                           346 LOAD_ATTR                3 (filepaths)
+               
+                64         356 PRECALL                  2
+                           360 CALL                     2
+                           370 STORE_FAST               6 (per_file_findings)
                
-                61     >>  220 LOAD_FAST                0 (self)
-                           222 LOAD_METHOD              6 (pool_engine)
-                           244 LOAD_FAST                3 (proc_count)
-                           246 KW_NAMES                 3
-                           248 PRECALL                  1
-                           252 CALL                     1
-                           262 BEFORE_WITH
-                           264 STORE_FAST               5 (pool)
-               
-                62         266 LOAD_FAST                5 (pool)
-                           268 LOAD_METHOD              7 (map)
-               
-                63         290 LOAD_GLOBAL             17 (NULL + partial)
-                           302 LOAD_GLOBAL             18 (pool_wrapper)
-                           314 LOAD_FAST                2 (bundle)
-                           316 LOAD_FAST                0 (self)
-                           318 LOAD_ATTR                5 (_per_file_analyzer)
-                           328 PRECALL                  3
-                           332 CALL                     3
-               
-                64         342 LOAD_FAST                0 (self)
-                           344 LOAD_ATTR                3 (filepaths)
-               
-                62         354 PRECALL                  2
-                           358 CALL                     2
-                           368 STORE_FAST               6 (per_file_findings)
-               
-                61         370 LOAD_CONST               0 (None)
-                           372 LOAD_CONST               0 (None)
+                63         372 LOAD_CONST               0 (None)
                            374 LOAD_CONST               0 (None)
-                           376 PRECALL                  2
-                           380 CALL                     2
-                           390 POP_TOP
-                           392 JUMP_FORWARD            11 (to 416)
-                       >>  394 PUSH_EXC_INFO
-                           396 WITH_EXCEPT_START
-                           398 POP_JUMP_FORWARD_IF_TRUE     4 (to 408)
-                           400 RERAISE                  2
-                       >>  402 COPY                     3
-                           404 POP_EXCEPT
-                           406 RERAISE                  1
-                       >>  408 POP_TOP
-                           410 POP_EXCEPT
-                           412 POP_TOP
+                           376 LOAD_CONST               0 (None)
+                           378 PRECALL                  2
+                           382 CALL                     2
+                           392 POP_TOP
+                           394 JUMP_FORWARD            11 (to 418)
+                       >>  396 PUSH_EXC_INFO
+                           398 WITH_EXCEPT_START
+                           400 POP_JUMP_FORWARD_IF_TRUE     4 (to 410)
+                           402 RERAISE                  2
+                       >>  404 COPY                     3
+                           406 POP_EXCEPT
+                           408 RERAISE                  1
+                       >>  410 POP_TOP
+                           412 POP_EXCEPT
                            414 POP_TOP
+                           416 POP_TOP
                
-                70     >>  416 LOAD_GLOBAL             21 (NULL + list)
-                           428 LOAD_FAST                6 (per_file_findings)
-                           430 PRECALL                  1
-                           434 CALL                     1
-                           444 GET_ITER
-                       >>  446 FOR_ITER                26 (to 500)
-                           448 STORE_FAST               7 (file_findings)
-               
-                71         450 LOAD_FAST                7 (file_findings)
-                           452 POP_JUMP_FORWARD_IF_TRUE     1 (to 456)
-               
-                72         454 JUMP_BACKWARD            5 (to 446)
-               
-                73     >>  456 LOAD_FAST                1 (final)
-                           458 LOAD_METHOD              4 (extend)
-                           480 LOAD_FAST                7 (file_findings)
-                           482 PRECALL                  1
-                           486 CALL                     1
-                           496 POP_TOP
-                           498 JUMP_BACKWARD           27 (to 446)
-               
-                75     >>  500 LOAD_GLOBAL             23 (NULL + FindingMerger)
-                           512 LOAD_FAST                1 (final)
-                           514 PRECALL                  1
-                           518 CALL                     1
-                           528 LOAD_METHOD             12 (merge)
-                           550 PRECALL                  0
-                           554 CALL                     0
-                           564 STORE_FAST               8 (fin)
-               
-                76         566 LOAD_FAST                0 (self)
-                           568 LOAD_METHOD             13 (filter_false_positives)
-                           590 LOAD_FAST                8 (fin)
-                           592 PRECALL                  1
-                           596 CALL                     1
-                           606 STORE_FAST               8 (fin)
+                69     >>  418 LOAD_GLOBAL             21 (NULL + list)
+                           430 LOAD_FAST                6 (per_file_findings)
+                           432 PRECALL                  1
+                           436 CALL                     1
+                           446 GET_ITER
+                       >>  448 FOR_ITER                26 (to 502)
+                           450 STORE_FAST               7 (file_findings)
+               
+                70         452 LOAD_FAST                7 (file_findings)
+                           454 POP_JUMP_FORWARD_IF_TRUE     1 (to 458)
+               
+                71         456 JUMP_BACKWARD            5 (to 448)
+               
+                72     >>  458 LOAD_FAST                1 (final)
+                           460 LOAD_METHOD              4 (extend)
+                           482 LOAD_FAST                7 (file_findings)
+                           484 PRECALL                  1
+                           488 CALL                     1
+                           498 POP_TOP
+                           500 JUMP_BACKWARD           27 (to 448)
+               
+                74     >>  502 LOAD_GLOBAL             23 (NULL + FindingMerger)
+                           514 LOAD_FAST                1 (final)
+                           516 PRECALL                  1
+                           520 CALL                     1
+                           530 LOAD_METHOD             12 (merge)
+                           552 PRECALL                  0
+                           556 CALL                     0
+                           566 STORE_FAST               8 (fin)
+               
+                75         568 LOAD_FAST                0 (self)
+                           570 LOAD_METHOD             13 (filter_false_positives)
+                           592 LOAD_FAST                8 (fin)
+                           594 PRECALL                  1
+                           598 CALL                     1
+                           608 STORE_FAST               8 (fin)
                
-                77         608 LOAD_FAST                8 (fin)
-                           610 RETURN_VALUE
+                76         610 LOAD_FAST                8 (fin)
+                           612 RETURN_VALUE
                ExceptionTable:
-                 264 to 368 -> 394 [1] lasti
-                 394 to 400 -> 402 [3] lasti
-                 408 to 408 -> 402 [3] lasti
+                 266 to 370 -> 396 [1] lasti
+                 396 to 402 -> 404 [3] lasti
+                 410 to 410 -> 404 [3] lasti
                consts
                   None
                   0
-                  ('file',)
+                  ('file', 'bundle')
                   ('processes',)
                names      ('analyzer_bundle', '_get_process_count_for_runner', 'PROFILER_ON', 'filepaths', 'extend', '_per_file_analyzer', 'pool_engine', 'map', 'partial', 'pool_wrapper', 'list', 'FindingMerger', 'merge', 'filter_false_positives')
                varnames   ('self', 'final', 'bundle', 'proc_count', 'file', 'pool', 'per_file_findings', 'file_findings', 'fin')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       'run'
-               firstlineno 49
+               firstlineno 51
                lnotab
-                  0x02010402280128010c0104020e01120154ff02032e01180134010cfe10
-                  ff2e092201040102012c0242012a01
+                  0x02010402280128010c0104020e01120156ff02032e01180134010cfe10
+                  ff2e062201040102012c0242012a01
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 6
                flags     : 3
                code
                   0x970067007d017c006a000000000000000000733e740300000000000000
@@ -673,49 +682,49 @@
                   000000a00b00000000000000000000000000000000000000007c047c07a6
                   020000ab0200000000000000007d087c08a00c0000000000000000000000
                   0000000000000000007c006a0200000000000000006a0900000000000000
                   009b0064019d026402a6020000ab0200000000000000007d097c00a00d00
                   000000000000000000000000000000000000007c09a6010000ab01000000
                   000000000073018c5b7c01a00e0000000000000000000000000000000000
                   0000007c08a6010000ab01000000000000000001008c718c7a7c015300
-                79           0 RESUME                   0
+                78           0 RESUME                   0
                
-                80           2 BUILD_LIST               0
+                79           2 BUILD_LIST               0
                              4 STORE_FAST               1 (flist)
                
-                81           6 LOAD_FAST                0 (self)
+                80           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (path_exclusion_rules)
                             18 POP_JUMP_FORWARD_IF_TRUE    62 (to 144)
                
-                82          20 LOAD_GLOBAL              3 (NULL + ExcludedPathsBuilder)
+                81          20 LOAD_GLOBAL              3 (NULL + ExcludedPathsBuilder)
                             32 PRECALL                  0
                             36 CALL                     0
                             46 STORE_FAST               2 (excl_paths_builder)
                
-                83          48 LOAD_FAST                0 (self)
+                82          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                2 (config)
                             60 LOAD_ATTR                3 (global_exclusion_paths)
                             70 GET_ITER
                        >>   72 FOR_ITER                23 (to 120)
                             74 STORE_FAST               3 (path)
                
-                84          76 LOAD_FAST                2 (excl_paths_builder)
+                83          76 LOAD_FAST                2 (excl_paths_builder)
                             78 LOAD_METHOD              4 (with_rules_from_file)
                            100 LOAD_FAST                3 (path)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 POP_TOP
                            118 JUMP_BACKWARD           24 (to 72)
                
-                86     >>  120 LOAD_FAST                2 (excl_paths_builder)
+                85     >>  120 LOAD_FAST                2 (excl_paths_builder)
                            122 LOAD_ATTR                5 (rules)
                            132 LOAD_FAST                0 (self)
                            134 STORE_ATTR               0 (path_exclusion_rules)
                
-                88     >>  144 LOAD_GLOBAL             13 (NULL + os)
+                87     >>  144 LOAD_GLOBAL             13 (NULL + os)
                            156 LOAD_ATTR                7 (walk)
                            166 LOAD_GLOBAL             17 (NULL + get_abspath)
                            178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                2 (config)
                            190 LOAD_ATTR                9 (workdir_path)
                            200 PRECALL                  1
                            204 CALL                     1
@@ -724,73 +733,73 @@
                            228 GET_ITER
                        >>  230 FOR_ITER               121 (to 474)
                            232 UNPACK_SEQUENCE          3
                            236 STORE_FAST               4 (fpath)
                            238 STORE_FAST               5 (_)
                            240 STORE_FAST               6 (files)
                
-                89         242 LOAD_FAST                6 (files)
+                88         242 LOAD_FAST                6 (files)
                            244 GET_ITER
                        >>  246 FOR_ITER               112 (to 472)
                            248 STORE_FAST               7 (filename)
                
-                90         250 LOAD_GLOBAL             12 (os)
+                89         250 LOAD_GLOBAL             12 (os)
                            262 LOAD_ATTR               10 (path)
                            272 LOAD_METHOD             11 (join)
                            294 LOAD_FAST                4 (fpath)
                            296 LOAD_FAST                7 (filename)
                            298 PRECALL                  2
                            302 CALL                     2
                            312 STORE_FAST               8 (full_path)
                
-                91         314 LOAD_FAST                8 (full_path)
+                90         314 LOAD_FAST                8 (full_path)
                            316 LOAD_METHOD             12 (replace)
                            338 LOAD_FAST                0 (self)
                            340 LOAD_ATTR                2 (config)
                            350 LOAD_ATTR                9 (workdir_path)
                            360 FORMAT_VALUE             0
                            362 LOAD_CONST               1 ('/')
                            364 BUILD_STRING             2
                            366 LOAD_CONST               2 ('')
                            368 PRECALL                  2
                            372 CALL                     2
                            382 STORE_FAST               9 (rel_path)
                
-                92         384 LOAD_FAST                0 (self)
+                91         384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD             13 (_path_included)
                            408 LOAD_FAST                9 (rel_path)
                            410 PRECALL                  1
                            414 CALL                     1
                            424 POP_JUMP_FORWARD_IF_TRUE     1 (to 428)
                
-                93         426 JUMP_BACKWARD           91 (to 246)
+                92         426 JUMP_BACKWARD           91 (to 246)
                
-                95     >>  428 LOAD_FAST                1 (flist)
+                94     >>  428 LOAD_FAST                1 (flist)
                            430 LOAD_METHOD             14 (append)
                            452 LOAD_FAST                8 (full_path)
                            454 PRECALL                  1
                            458 CALL                     1
                            468 POP_TOP
                            470 JUMP_BACKWARD          113 (to 246)
                
-                89     >>  472 JUMP_BACKWARD          122 (to 230)
+                88     >>  472 JUMP_BACKWARD          122 (to 230)
                
-                97     >>  474 LOAD_FAST                1 (flist)
+                96     >>  474 LOAD_FAST                1 (flist)
                            476 RETURN_VALUE
                consts
                   None
                   '/'
                   ''
                names      ('path_exclusion_rules', 'ExcludedPathsBuilder', 'config', 'global_exclusion_paths', 'with_rules_from_file', 'rules', 'os', 'walk', 'get_abspath', 'workdir_path', 'path', 'join', 'replace', '_path_included', 'append')
                varnames   ('self', 'flist', 'excl_paths_builder', 'path', 'fpath', '_', 'files', 'filename', 'full_path', 'rel_path')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       '_get_files_list'
-               firstlineno 79
+               firstlineno 78
                lnotab
                   0x020104010e011c011c012c02180262010801400146012a0102022cfa02
                   08
             'path'
             code
                argcount  : 2
                nlocals   : 2
@@ -800,49 +809,49 @@
                   0x870197007c006a00000000000000000081187403000000000000000000
                   007c006a000000000000000000a6010000ab01000000000000000064016b
                   020000000072026402530074050000000000000000000088016601640384
                   087c006a0000000000000000004400a6000000ab000000000000000000a6
                   010000ab01000000000000000072026404530064025300
                              0 MAKE_CELL                1 (path)
                
-                99           2 RESUME                   0
+                98           2 RESUME                   0
                
-               100           4 LOAD_FAST                0 (self)
+                99           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (path_exclusion_rules)
                             16 POP_JUMP_FORWARD_IF_NONE    24 (to 66)
                             18 LOAD_GLOBAL              3 (NULL + len)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                0 (path_exclusion_rules)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_CONST               1 (0)
                             58 COMPARE_OP               2 (==)
                             64 POP_JUMP_FORWARD_IF_FALSE     2 (to 70)
                
-               101     >>   66 LOAD_CONST               2 (True)
+               100     >>   66 LOAD_CONST               2 (True)
                             68 RETURN_VALUE
                
-               103     >>   70 LOAD_GLOBAL              5 (NULL + any)
+               102     >>   70 LOAD_GLOBAL              5 (NULL + any)
                             82 LOAD_CLOSURE             1 (path)
                             84 BUILD_TUPLE              1
-                            86 LOAD_CONST               3 (<code object <genexpr>, file "/app/deepsecrets/core/modes/iscan_mode.py", line 103>)
+                            86 LOAD_CONST               3 (<code object <genexpr>, file "/app/deepsecrets/core/modes/iscan_mode.py", line 102>)
                             88 MAKE_FUNCTION            8 (closure)
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                0 (path_exclusion_rules)
                            102 GET_ITER
                            104 PRECALL                  0
                            108 CALL                     0
                            118 PRECALL                  1
                            122 CALL                     1
                            132 POP_JUMP_FORWARD_IF_FALSE     2 (to 138)
                
-               104         134 LOAD_CONST               4 (False)
+               103         134 LOAD_CONST               4 (False)
                            136 RETURN_VALUE
                
-               105     >>  138 LOAD_CONST               2 (True)
+               104     >>  138 LOAD_CONST               2 (True)
                            140 RETURN_VALUE
                consts
                   None
                   0
                   True
                   code
                      argcount  : 1
@@ -851,15 +860,15 @@
                      flags     : 51
                      code
                         0x95014b00010097007c005d197d017c01a0000000000000000000000000
                         0000000000000000008902a6010000ab0100000000000000005600970101
                         008c1a64005300
                                    0 COPY_FREE_VARS           1
                      
-                     103           2 RETURN_GENERATOR
+                     102           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                25 (to 62)
                                   12 STORE_FAST               1 (excl_rule)
                                   14 LOAD_FAST                1 (excl_rule)
                                   16 LOAD_METHOD              0 (match)
@@ -876,102 +885,102 @@
                         None
                      names      ('match',)
                      varnames   ('.0', 'excl_rule')
                      freevars   ('path',)
                      cellvars   ()
                      filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                      name       '<genexpr>'
-                     firstlineno 103
+                     firstlineno 102
                      lnotab 0x
                   False
                names      ('path_exclusion_rules', 'len', 'any')
                varnames   ('self', 'path')
                freevars   ()
                cellvars   ('path',)
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       '_path_included'
-               firstlineno 99
+               firstlineno 98
                lnotab 0x04013e01040240010401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               107           0 RESUME                   0
+               106           0 RESUME                   0
                
-               109           2 LOAD_CONST               0 (None)
+               108           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       'prepare_for_scan'
-               firstlineno 107
+               firstlineno 106
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c006a0100000000000000006a0200
                   000000000000007c006a0300000000000000006900ac01a6030000ab0300
                   000000000000005300
-               111           0 RESUME                   0
+               110           0 RESUME                   0
                
-               112           2 LOAD_GLOBAL              1 (NULL + DotWiz)
+               111           2 LOAD_GLOBAL              1 (NULL + DotWiz)
                
-               113          14 LOAD_FAST                0 (self)
+               112          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (config)
                             26 LOAD_ATTR                2 (workdir_path)
                
-               114          36 LOAD_FAST                0 (self)
+               113          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (path_exclusion_rules)
                
-               115          48 BUILD_MAP                0
+               114          48 BUILD_MAP                0
                
-               112          50 KW_NAMES                 1
+               111          50 KW_NAMES                 1
                             52 PRECALL                  3
                             56 CALL                     3
                             66 RETURN_VALUE
                consts
                   None
                   ('workdir', 'path_exclusion_rules', 'engines')
                names      ('DotWiz', 'config', 'workdir_path', 'path_exclusion_rules')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       'analyzer_bundle'
-               firstlineno 111
+               firstlineno 110
                lnotab 0x02010c0116010c0102fd
             'file'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               118           0 RESUME                   0
+               117           0 RESUME                   0
                
-               120           2 LOAD_CONST               0 (None)
+               119           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('bundle', 'file')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       '_per_file_analyzer'
-               firstlineno 118
+               firstlineno 117
                lnotab 0x0202
             'results'
             code
                argcount  : 2
                nlocals   : 7
                stacksize : 6
                flags     : 3
@@ -980,211 +989,221 @@
                   000000000000007404000000000000000000006a030000000000000000a6
                   010000ab0100000000000000007d027c0280027c01530067007d037c0144
                   005d447d0464017d057c0244005d257d067409000000000000000000006a
                   0500000000000000007c066a0600000000000000007c046a070000000000
                   000000a6020000ab020000000000000000810464027d0501006e018c267c
                   0573018c2f7c03a00800000000000000000000000000000000000000007c
                   04a6010000ab01000000000000000001008c457c035300
-               122           0 RESUME                   0
+               121           0 RESUME                   0
                
-               123           2 LOAD_FAST                0 (self)
+               122           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (rulesets)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_GLOBAL              4 (FalseFindingsBuilder)
                             48 LOAD_ATTR                3 (ruleset_name)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               2 (false_finding_rules)
                
-               124          74 LOAD_FAST                2 (false_finding_rules)
+               123          74 LOAD_FAST                2 (false_finding_rules)
                             76 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 82)
                
-               125          78 LOAD_FAST                1 (results)
+               124          78 LOAD_FAST                1 (results)
                             80 RETURN_VALUE
                
-               128     >>   82 BUILD_LIST               0
+               127     >>   82 BUILD_LIST               0
                             84 STORE_FAST               3 (final)
                
-               129          86 LOAD_FAST                1 (results)
+               128          86 LOAD_FAST                1 (results)
                             88 GET_ITER
                        >>   90 FOR_ITER                68 (to 228)
                             92 STORE_FAST               4 (result)
                
-               130          94 LOAD_CONST               1 (True)
+               129          94 LOAD_CONST               1 (True)
                             96 STORE_FAST               5 (good_result)
                
-               131          98 LOAD_FAST                2 (false_finding_rules)
+               130          98 LOAD_FAST                2 (false_finding_rules)
                            100 GET_ITER
                        >>  102 FOR_ITER                37 (to 178)
                            104 STORE_FAST               6 (false_pattern)
                
-               132         106 LOAD_GLOBAL              9 (NULL + re)
+               131         106 LOAD_GLOBAL              9 (NULL + re)
                            118 LOAD_ATTR                5 (match)
                            128 LOAD_FAST                6 (false_pattern)
                            130 LOAD_ATTR                6 (pattern)
                            140 LOAD_FAST                4 (result)
                            142 LOAD_ATTR                7 (detection)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 POP_JUMP_FORWARD_IF_NONE     4 (to 176)
                
-               133         168 LOAD_CONST               2 (False)
+               132         168 LOAD_CONST               2 (False)
                            170 STORE_FAST               5 (good_result)
                
-               134         172 POP_TOP
+               133         172 POP_TOP
                            174 JUMP_FORWARD             1 (to 178)
                
-               132     >>  176 JUMP_BACKWARD           38 (to 102)
+               131     >>  176 JUMP_BACKWARD           38 (to 102)
                
-               135     >>  178 LOAD_FAST                5 (good_result)
+               134     >>  178 LOAD_FAST                5 (good_result)
                            180 POP_JUMP_FORWARD_IF_TRUE     1 (to 184)
                
-               136         182 JUMP_BACKWARD           47 (to 90)
+               135         182 JUMP_BACKWARD           47 (to 90)
                
-               138     >>  184 LOAD_FAST                3 (final)
+               137     >>  184 LOAD_FAST                3 (final)
                            186 LOAD_METHOD              8 (append)
                            208 LOAD_FAST                4 (result)
                            210 PRECALL                  1
                            214 CALL                     1
                            224 POP_TOP
                            226 JUMP_BACKWARD           69 (to 90)
                
-               140     >>  228 LOAD_FAST                3 (final)
+               139     >>  228 LOAD_FAST                3 (final)
                            230 RETURN_VALUE
                consts
                   None
                   True
                   False
                names      ('rulesets', 'get', 'FalseFindingsBuilder', 'ruleset_name', 're', 'match', 'pattern', 'detection', 'append')
                varnames   ('self', 'results', 'false_finding_rules', 'final', 'result', 'good_result', 'false_pattern')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/modes/iscan_mode.py'
                name       'filter_false_positives'
-               firstlineno 122
+               firstlineno 121
                lnotab
                   0x020148010401040304010801040108013e01040104fe0203040102022c
                   02
             (None,)
             ('return', None)
          names      ('__name__', '__module__', '__qualname__', 'Config', '__annotations__', 'List', 'str', 'path_exclusion_rules', 'ExcludePathRule', 'FileAnalyzer', 'Type', 'Optional', 'Any', '__init__', 'int', '_get_process_count_for_runner', 'Finding', 'run', '_get_files_list', 'bool', '_path_included', 'abstractmethod', 'prepare_for_scan', 'DotWiz', 'analyzer_bundle', 'abstractstaticmethod', '_per_file_analyzer', 'filter_false_positives')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/modes/iscan_mode.py'
          name       'ScanMode'
-         firstlineno 22
+         firstlineno 23
          lnotab
-            0x0c010a0116011a010a010a02220d0c07181e18141008020106ff0e0102
+            0x0c010a0116011a010a010a02220d0c08181b18141008020106ff0e0102
             030c0702011aff0e010203
       'ScanMode'
       'bundle'
       'runner'
       'file'
       'return'
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 10
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d0302007c017c007c02a6020000ab020000000000
-            0000007d047405000000000000000000006a03000000000000000064017c
-            029b0064027401000000000000000000006a010000000000000000a60000
-            00ab0000000000000000007c037a0a0000a0040000000000000000000000
-            000000000000000000a6000000ab0000000000000000009b006403740b00
-            0000000000000000007c04a6010000ab0100000000000000009b0064049d
-            07a6010000ab01000000000000000001007405000000000000000000006a
-            06000000000000000064017c029b006405740b000000000000000000007c
-            04a6010000ab0100000000000000009b0064049d05a6010000ab01000000
-            000000000001007c045300
-         143           0 RESUME                   0
+            0000007d047404000000000000000000006a030000000000000000740800
+            0000000000000000006a0500000000000000006b02000000007252740500
+            0000000000000000006a06000000000000000064017c029b006402740100
+            0000000000000000006a010000000000000000a6000000ab000000000000
+            0000007c037a0a0000a00700000000000000000000000000000000000000
+            00a6000000ab0000000000000000009b0064037411000000000000000000
+            007c04a6010000ab0100000000000000009b0064049d07a6010000ab0100
+            0000000000000001006e287405000000000000000000006a090000000000
+            00000064017c029b0064057411000000000000000000007c04a6010000ab
+            0100000000000000009b0064049d05a6010000ab01000000000000000001
+            007c045300
+         142           0 RESUME                   0
          
-         144           2 LOAD_GLOBAL              1 (NULL + datetime)
+         143           2 LOAD_GLOBAL              1 (NULL + datetime)
                       14 LOAD_ATTR                1 (now)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               3 (start_ts)
          
-         145          40 PUSH_NULL
+         144          40 PUSH_NULL
                       42 LOAD_FAST                1 (runner)
                       44 LOAD_FAST                0 (bundle)
                       46 LOAD_FAST                2 (file)
                       48 PRECALL                  2
                       52 CALL                     2
                       62 STORE_FAST               4 (result)
          
-         146          64 LOAD_GLOBAL              5 (NULL + logger)
-                      76 LOAD_ATTR                3 (debug)
-         
-         147          86 LOAD_CONST               1 (' ✓ [')
-                      88 LOAD_FAST                2 (file)
-                      90 FORMAT_VALUE             0
-                      92 LOAD_CONST               2 ('] ')
-                      94 LOAD_GLOBAL              1 (NULL + datetime)
-                     106 LOAD_ATTR                1 (now)
-                     116 PRECALL                  0
-                     120 CALL                     0
-                     130 LOAD_FAST                3 (start_ts)
-                     132 BINARY_OP               10 (-)
-                     136 LOAD_METHOD              4 (total_seconds)
-                     158 PRECALL                  0
-                     162 CALL                     0
-                     172 FORMAT_VALUE             0
-                     174 LOAD_CONST               3 ('s elapsed \t ')
-                     176 LOAD_GLOBAL             11 (NULL + len)
-                     188 LOAD_FAST                4 (result)
-                     190 PRECALL                  1
-                     194 CALL                     1
-                     204 FORMAT_VALUE             0
-                     206 LOAD_CONST               4 (' potential findings')
-                     208 BUILD_STRING             7
-         
-         146         210 PRECALL                  1
-                     214 CALL                     1
-                     224 POP_TOP
-         
-         149         226 LOAD_GLOBAL              5 (NULL + logger)
-                     238 LOAD_ATTR                6 (info)
-                     248 LOAD_CONST               1 (' ✓ [')
-                     250 LOAD_FAST                2 (file)
-                     252 FORMAT_VALUE             0
-                     254 LOAD_CONST               5 ('] \t ')
-                     256 LOAD_GLOBAL             11 (NULL + len)
-                     268 LOAD_FAST                4 (result)
-                     270 PRECALL                  1
-                     274 CALL                     1
-                     284 FORMAT_VALUE             0
-                     286 LOAD_CONST               4 (' potential findings')
-                     288 BUILD_STRING             5
-                     290 PRECALL                  1
-                     294 CALL                     1
-                     304 POP_TOP
+         145          64 LOAD_GLOBAL              4 (logger)
+                      76 LOAD_ATTR                3 (level)
+                      86 LOAD_GLOBAL              8 (logging)
+                      98 LOAD_ATTR                5 (DEBUG)
+                     108 COMPARE_OP               2 (==)
+                     114 POP_JUMP_FORWARD_IF_FALSE    82 (to 280)
+         
+         146         116 LOAD_GLOBAL              5 (NULL + logger)
+                     128 LOAD_ATTR                6 (debug)
+         
+         147         138 LOAD_CONST               1 (' ✓ [')
+                     140 LOAD_FAST                2 (file)
+                     142 FORMAT_VALUE             0
+                     144 LOAD_CONST               2 ('] ')
+                     146 LOAD_GLOBAL              1 (NULL + datetime)
+                     158 LOAD_ATTR                1 (now)
+                     168 PRECALL                  0
+                     172 CALL                     0
+                     182 LOAD_FAST                3 (start_ts)
+                     184 BINARY_OP               10 (-)
+                     188 LOAD_METHOD              7 (total_seconds)
+                     210 PRECALL                  0
+                     214 CALL                     0
+                     224 FORMAT_VALUE             0
+                     226 LOAD_CONST               3 ('s elapsed \t ')
+                     228 LOAD_GLOBAL             17 (NULL + len)
+                     240 LOAD_FAST                4 (result)
+                     242 PRECALL                  1
+                     246 CALL                     1
+                     256 FORMAT_VALUE             0
+                     258 LOAD_CONST               4 (' potential findings')
+                     260 BUILD_STRING             7
+         
+         146         262 PRECALL                  1
+                     266 CALL                     1
+                     276 POP_TOP
+                     278 JUMP_FORWARD            40 (to 360)
+         
+         150     >>  280 LOAD_GLOBAL              5 (NULL + logger)
+                     292 LOAD_ATTR                9 (info)
+                     302 LOAD_CONST               1 (' ✓ [')
+                     304 LOAD_FAST                2 (file)
+                     306 FORMAT_VALUE             0
+                     308 LOAD_CONST               5 ('] \t ')
+                     310 LOAD_GLOBAL             17 (NULL + len)
+                     322 LOAD_FAST                4 (result)
+                     324 PRECALL                  1
+                     328 CALL                     1
+                     338 FORMAT_VALUE             0
+                     340 LOAD_CONST               4 (' potential findings')
+                     342 BUILD_STRING             5
+                     344 PRECALL                  1
+                     348 CALL                     1
+                     358 POP_TOP
          
-         150         306 LOAD_FAST                4 (result)
-                     308 RETURN_VALUE
+         151     >>  360 LOAD_FAST                4 (result)
+                     362 RETURN_VALUE
          consts
             None
             ' ✓ ['
             '] '
             's elapsed \t '
             ' potential findings'
             '] \t '
-         names      ('datetime', 'now', 'logger', 'debug', 'total_seconds', 'len', 'info')
+         names      ('datetime', 'now', 'logger', 'level', 'logging', 'DEBUG', 'debug', 'total_seconds', 'len', 'info')
          varnames   ('bundle', 'runner', 'file', 'start_ts', 'result')
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/modes/iscan_mode.py'
          name       'pool_wrapper'
-         firstlineno 143
-         lnotab 0x02012601180116017cff10035001
-   names      ('multiprocessing', 'get_context', 'os', 'abc', 'abstractmethod', 'abstractstaticmethod', 'datetime', 'functools', 'partial', 'multiprocessing.pool', 'Pool', 'typing', 'Any', 'Callable', 'List', 'Optional', 'Type', 'regex', 're', 'dotwiz', 'DotWiz', 'deepsecrets', 'PLATFORM', 'PROFILER_ON', 'logger', 'deepsecrets.config', 'Config', 'deepsecrets.core.model.finding', 'Finding', 'FindingMerger', 'deepsecrets.core.model.rules.exlcuded_path', 'ExcludePathRule', 'deepsecrets.core.rulesets.excluded_paths', 'ExcludedPathsBuilder', 'deepsecrets.core.rulesets.false_findings', 'FalseFindingsBuilder', 'deepsecrets.core.utils.file_analyzer', 'FileAnalyzer', 'deepsecrets.core.utils.fs', 'get_abspath', 'ScanMode', 'str', 'pool_wrapper')
+         firstlineno 142
+         lnotab 0x020126011801340116017cff12045001
+   names      ('logging', 'multiprocessing', 'get_context', 'os', 'abc', 'abstractmethod', 'abstractstaticmethod', 'datetime', 'functools', 'partial', 'multiprocessing.pool', 'Pool', 'typing', 'Any', 'Callable', 'List', 'Optional', 'Type', 'regex', 're', 'dotwiz', 'DotWiz', 'deepsecrets', 'PLATFORM', 'PROFILER_ON', 'logger', 'deepsecrets.config', 'Config', 'deepsecrets.core.model.finding', 'Finding', 'FindingMerger', 'deepsecrets.core.model.rules.exlcuded_path', 'ExcludePathRule', 'deepsecrets.core.rulesets.excluded_paths', 'ExcludedPathsBuilder', 'deepsecrets.core.rulesets.false_findings', 'FalseFindingsBuilder', 'deepsecrets.core.utils.file_analyzer', 'FileAnalyzer', 'deepsecrets.core.utils.fs', 'get_abspath', 'ScanMode', 'str', 'pool_wrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/modes/iscan_mode.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c01080110010c010c010c011c0108020c0214010c0110010c
-      010c010c010c010c031a79
+      0x00ff020108010c01080110010c010c010c011c0108020c0214010c0110
+      010c010c010c010c010c031a77
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.1.0/deepsecrets/core/modes/iscan_mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from multiprocessing import get_context
 import os
 from abc import abstractmethod, abstractstaticmethod
 from datetime import datetime
 from functools import partial
 from multiprocessing.pool import Pool
 from typing import Any, Callable, List, Optional, Type
@@ -36,41 +37,39 @@
             self.pool_engine = pool_engine
 
         self.config = config
         self.filepaths = self._get_files_list()
         self.prepare_for_scan()
 
     def _get_process_count_for_runner(self) -> int:
-        base = 15
+        limit = self.config.process_count
+
         file_count = len(self.filepaths)
         if file_count == 0:
             return 0
-        return base if file_count >= base else file_count
+        return limit if file_count >= limit else file_count
 
     def run(self) -> List[Finding]:
         final: List[Finding] = []
 
         bundle = self.analyzer_bundle()
         proc_count = self._get_process_count_for_runner()
         if proc_count == 0:
             return final
 
         if PROFILER_ON:
             for file in self.filepaths:
-                final.extend(self._per_file_analyzer(file=file))
+                final.extend(self._per_file_analyzer(file=file, bundle=bundle))
         else:
             with self.pool_engine(processes=proc_count) as pool:
                 per_file_findings: List[List[Finding]] = pool.map(
                     partial(pool_wrapper, bundle, self._per_file_analyzer),
                     self.filepaths,
                 )  # type: ignore
                 
-                # pool.close()
-                # pool.join()  # not calling because of suprusingly big delays
-
             for file_findings in list(per_file_findings):
                 if not file_findings:
                     continue
                 final.extend(file_findings)
 
         fin = FindingMerger(final).merge()
         fin = self.filter_false_positives(fin)
@@ -108,15 +107,15 @@
     def prepare_for_scan(self) -> None:
         pass
 
     def analyzer_bundle(self) -> DotWiz:
         return DotWiz(
             workdir=self.config.workdir_path,
             path_exclusion_rules=self.path_exclusion_rules,
-            engines={},
+            engines={}
         )
 
     @abstractstaticmethod
     def _per_file_analyzer(bundle, file: Any) -> List[Finding]:  # type: ignore
         pass
 
     def filter_false_positives(self, results: List[Finding]) -> List[Finding]:
@@ -139,12 +138,14 @@
 
         return final
 
 
 def pool_wrapper(bundle: DotWiz, runner: Callable, file: str) -> List[Finding]:  # pragma: nocover
     start_ts = datetime.now()
     result = runner(bundle, file)
-    logger.debug(
-        f' ✓ [{file}] {(datetime.now() - start_ts).total_seconds()}s elapsed \t {len(result)} potential findings'
-    )
-    logger.info(f' ✓ [{file}] \t {len(result)} potential findings')
+    if logger.level == logging.DEBUG:
+        logger.debug(
+            f' ✓ [{file}] {(datetime.now() - start_ts).total_seconds()}s elapsed \t {len(result)} potential findings'
+        )
+    else:
+        logger.info(f' ✓ [{file}] \t {len(result)} potential findings')
     return result
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.1.0/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,192 +1,196 @@
 magic:    0xa70d0d0a
-moddate:  0xaa959964 (Mon Jun 26 13:42:02 2023 UTC)
-files sz: 6481
+moddate:  0x080aa464 (Tue Jul  4 12:01:12 2023 UTC)
+files sz: 6862
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
-      00640064026c066d075a070100640064036c086d095a090100640064046c
-      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f6d
-      105a100100640064076c116d125a130100640064086c146d155a15010064
-      0064096c166d175a1701006400640a6c186d195a1901006400640b6c1a6d
-      1b5a1b6d1c5a1c6d125a1201006400640c6c1d6d1e5a1e01006400640d6c
-      1f6d205a2001006400640e6c216d225a2201006400640f6c236d245a246d
-      255a256d265a260100640064106c276d285a28010067006411a2015a2902
-      0047006412840064136528a6030000ab0300000000000000005a2a641453
-      00
+      0x9700640064016c006d015a016d025a026d035a036d045a046d055a056d
+      065a060100640064026c076d085a080100640064036c096d0a5a0a010064
+      0064046c0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
+      105a106d115a110100640064076c126d135a140100640064086c156d165a
+      160100640064096c176d185a1801006400640a6c196d1a5a1a6d1b5a1b6d
+      135a1301006400640b6c1c6d1d5a1d01006400640c6c1e6d1f5a1f6d205a
+      2001006400640d6c216d225a2201006400640e6c236d245a246d255a256d
+      265a2601006400640f6c276d285a280100640064106c296d2a5a2a010067
+      006411a2015a2b020047006412840064136528a6030000ab030000000000
+      0000005a2c64145300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('List', 'Sequence', 'Set', 'Type', 'Union'))
+                 4 LOAD_CONST               1 (('List', 'Optional', 'Sequence', 'Set', 'Type', 'Union'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
-                12 IMPORT_FROM              2 (Sequence)
-                14 STORE_NAME               2 (Sequence)
-                16 IMPORT_FROM              3 (Set)
-                18 STORE_NAME               3 (Set)
-                20 IMPORT_FROM              4 (Type)
-                22 STORE_NAME               4 (Type)
-                24 IMPORT_FROM              5 (Union)
-                26 STORE_NAME               5 (Union)
-                28 POP_TOP
+                12 IMPORT_FROM              2 (Optional)
+                14 STORE_NAME               2 (Optional)
+                16 IMPORT_FROM              3 (Sequence)
+                18 STORE_NAME               3 (Sequence)
+                20 IMPORT_FROM              4 (Set)
+                22 STORE_NAME               4 (Set)
+                24 IMPORT_FROM              5 (Type)
+                26 STORE_NAME               5 (Type)
+                28 IMPORT_FROM              6 (Union)
+                30 STORE_NAME               6 (Union)
+                32 POP_TOP
    
-     3          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               2 (('OrderedSet',))
-                34 IMPORT_NAME              6 (ordered_set)
-                36 IMPORT_FROM              7 (OrderedSet)
-                38 STORE_NAME               7 (OrderedSet)
-                40 POP_TOP
+     3          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               2 (('logger',))
+                38 IMPORT_NAME              7 (deepsecrets)
+                40 IMPORT_FROM              8 (logger)
+                42 STORE_NAME               8 (logger)
+                44 POP_TOP
    
-     4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('highlight',))
-                46 IMPORT_NAME              8 (pygments)
-                48 IMPORT_FROM              9 (highlight)
-                50 STORE_NAME               9 (highlight)
-                52 POP_TOP
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               3 (('OrderedSet',))
+                50 IMPORT_NAME              9 (ordered_set)
+                52 IMPORT_FROM             10 (OrderedSet)
+                54 STORE_NAME              10 (OrderedSet)
+                56 POP_TOP
    
-     5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('RawTokenFormatter',))
-                58 IMPORT_NAME             10 (pygments.formatters)
-                60 IMPORT_FROM             11 (RawTokenFormatter)
-                62 STORE_NAME              11 (RawTokenFormatter)
-                64 POP_TOP
+     6          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               4 (('highlight',))
+                62 IMPORT_NAME             11 (pygments)
+                64 IMPORT_FROM             12 (highlight)
+                66 STORE_NAME              12 (highlight)
+                68 POP_TOP
    
-     6          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('get_lexer_for_filename',))
-                70 IMPORT_NAME             12 (pygments.lexers)
-                72 IMPORT_FROM             13 (get_lexer_for_filename)
-                74 STORE_NAME              13 (get_lexer_for_filename)
-                76 POP_TOP
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('RawTokenFormatter',))
+                74 IMPORT_NAME             13 (pygments.formatters)
+                76 IMPORT_FROM             14 (RawTokenFormatter)
+                78 STORE_NAME              14 (RawTokenFormatter)
+                80 POP_TOP
    
-     7          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
-                82 IMPORT_NAME             14 (pygments.lexers.special)
-                84 IMPORT_FROM             15 (Lexer)
-                86 STORE_NAME              15 (Lexer)
-                88 IMPORT_FROM             16 (RawTokenLexer)
-                90 STORE_NAME              16 (RawTokenLexer)
-                92 POP_TOP
+     8          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
+                86 IMPORT_NAME             15 (pygments.lexers.special)
+                88 IMPORT_FROM             16 (Lexer)
+                90 STORE_NAME              16 (Lexer)
+                92 IMPORT_FROM             17 (RawTokenLexer)
+                94 STORE_NAME              17 (RawTokenLexer)
+                96 POP_TOP
    
-     8          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               7 (('Token',))
-                98 IMPORT_NAME             17 (pygments.token)
-               100 IMPORT_FROM             18 (Token)
-               102 STORE_NAME              19 (PygmentsToken)
-               104 POP_TOP
+     9          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               7 (('Token',))
+               102 IMPORT_NAME             18 (pygments.token)
+               104 IMPORT_FROM             19 (Token)
+               106 STORE_NAME              20 (PygmentsToken)
+               108 POP_TOP
    
-     9         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('ClassNotFound',))
-               110 IMPORT_NAME             20 (pygments.util)
-               112 IMPORT_FROM             21 (ClassNotFound)
-               114 STORE_NAME              21 (ClassNotFound)
-               116 POP_TOP
+    11         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               8 (('File',))
+               114 IMPORT_NAME             21 (deepsecrets.core.model.file)
+               116 IMPORT_FROM             22 (File)
+               118 STORE_NAME              22 (File)
+               120 POP_TOP
    
-    11         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               9 (('File',))
-               122 IMPORT_NAME             22 (deepsecrets.core.model.file)
-               124 IMPORT_FROM             23 (File)
-               126 STORE_NAME              23 (File)
-               128 POP_TOP
+    12         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST               9 (('Variable',))
+               126 IMPORT_NAME             23 (deepsecrets.core.model.semantic)
+               128 IMPORT_FROM             24 (Variable)
+               130 STORE_NAME              24 (Variable)
+               132 POP_TOP
    
-    12         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (('Variable',))
-               134 IMPORT_NAME             24 (deepsecrets.core.model.semantic)
-               136 IMPORT_FROM             25 (Variable)
-               138 STORE_NAME              25 (Variable)
-               140 POP_TOP
+    13         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST              10 (('Semantic', 'SemanticType', 'Token'))
+               138 IMPORT_NAME             25 (deepsecrets.core.model.token)
+               140 IMPORT_FROM             26 (Semantic)
+               142 STORE_NAME              26 (Semantic)
+               144 IMPORT_FROM             27 (SemanticType)
+               146 STORE_NAME              27 (SemanticType)
+               148 IMPORT_FROM             19 (Token)
+               150 STORE_NAME              19 (Token)
+               152 POP_TOP
    
-    13         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              11 (('Semantic', 'SemanticType', 'Token'))
-               146 IMPORT_NAME             26 (deepsecrets.core.model.token)
-               148 IMPORT_FROM             27 (Semantic)
-               150 STORE_NAME              27 (Semantic)
-               152 IMPORT_FROM             28 (SemanticType)
-               154 STORE_NAME              28 (SemanticType)
-               156 IMPORT_FROM             18 (Token)
-               158 STORE_NAME              18 (Token)
-               160 POP_TOP
+    14         154 LOAD_CONST               0 (0)
+               156 LOAD_CONST              11 (('Language',))
+               158 IMPORT_NAME             28 (deepsecrets.core.tokenizers.helpers.semantic.language)
+               160 IMPORT_FROM             29 (Language)
+               162 STORE_NAME              29 (Language)
+               164 POP_TOP
    
-    14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              12 (('Language',))
-               166 IMPORT_NAME             29 (deepsecrets.core.tokenizers.helpers.semantic.language)
-               168 IMPORT_FROM             30 (Language)
-               170 STORE_NAME              30 (Language)
-               172 POP_TOP
+    15         166 LOAD_CONST               0 (0)
+               168 LOAD_CONST              12 (('VariableDetectionRules', 'VariableSuppressionRules'))
+               170 IMPORT_NAME             30 (deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules)
+               172 IMPORT_FROM             31 (VariableDetectionRules)
+               174 STORE_NAME              31 (VariableDetectionRules)
+               176 IMPORT_FROM             32 (VariableSuppressionRules)
+               178 STORE_NAME              32 (VariableSuppressionRules)
+               180 POP_TOP
    
-    15         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              13 (('VariableDetectionRules',))
-               178 IMPORT_NAME             31 (deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules)
-               180 IMPORT_FROM             32 (VariableDetectionRules)
-               182 STORE_NAME              32 (VariableDetectionRules)
-               184 POP_TOP
+    16         182 LOAD_CONST               0 (0)
+               184 LOAD_CONST              13 (('SpotImprovements',))
+               186 IMPORT_NAME             33 (deepsecrets.core.tokenizers.helpers.spot_improvements)
+               188 IMPORT_FROM             34 (SpotImprovements)
+               190 STORE_NAME              34 (SpotImprovements)
+               192 POP_TOP
    
-    16         186 LOAD_CONST               0 (0)
-               188 LOAD_CONST              14 (('SpotImprovements',))
-               190 IMPORT_NAME             33 (deepsecrets.core.tokenizers.helpers.spot_improvements)
-               192 IMPORT_FROM             34 (SpotImprovements)
-               194 STORE_NAME              34 (SpotImprovements)
-               196 POP_TOP
+    17         194 LOAD_CONST               0 (0)
+               196 LOAD_CONST              14 (('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before'))
+               198 IMPORT_NAME             35 (deepsecrets.core.tokenizers.helpers.type_stream)
+               200 IMPORT_FROM             36 (token_to_typestream_item)
+               202 STORE_NAME              36 (token_to_typestream_item)
+               204 IMPORT_FROM             37 (types_to_filter_after)
+               206 STORE_NAME              37 (types_to_filter_after)
+               208 IMPORT_FROM             38 (types_to_filter_before)
+               210 STORE_NAME              38 (types_to_filter_before)
+               212 POP_TOP
    
-    17         198 LOAD_CONST               0 (0)
-               200 LOAD_CONST              15 (('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before'))
-               202 IMPORT_NAME             35 (deepsecrets.core.tokenizers.helpers.type_stream)
-               204 IMPORT_FROM             36 (token_to_typestream_item)
-               206 STORE_NAME              36 (token_to_typestream_item)
-               208 IMPORT_FROM             37 (types_to_filter_after)
-               210 STORE_NAME              37 (types_to_filter_after)
-               212 IMPORT_FROM             38 (types_to_filter_before)
-               214 STORE_NAME              38 (types_to_filter_before)
-               216 POP_TOP
+    22         214 LOAD_CONST               0 (0)
+               216 LOAD_CONST              15 (('Tokenizer',))
+               218 IMPORT_NAME             39 (deepsecrets.core.tokenizers.itokenizer)
+               220 IMPORT_FROM             40 (Tokenizer)
+               222 STORE_NAME              40 (Tokenizer)
+               224 POP_TOP
    
-    22         218 LOAD_CONST               0 (0)
-               220 LOAD_CONST              16 (('Tokenizer',))
-               222 IMPORT_NAME             39 (deepsecrets.core.tokenizers.itokenizer)
-               224 IMPORT_FROM             40 (Tokenizer)
-               226 STORE_NAME              40 (Tokenizer)
-               228 POP_TOP
+    23         226 LOAD_CONST               0 (0)
+               228 LOAD_CONST              16 (('LexerFinder',))
+               230 IMPORT_NAME             41 (deepsecrets.core.utils.lexer_finder)
+               232 IMPORT_FROM             42 (LexerFinder)
+               234 STORE_NAME              42 (LexerFinder)
+               236 POP_TOP
    
-    24         230 BUILD_LIST               0
-               232 LOAD_CONST              17 (('\n', '\t', "'", "''", '"', '""'))
-               234 LIST_EXTEND              1
-               236 STORE_NAME              41 (empty_tokens)
+    25         238 BUILD_LIST               0
+               240 LOAD_CONST              17 (('\n', '\t', "'", "''", '"', '""'))
+               242 LIST_EXTEND              1
+               244 STORE_NAME              43 (empty_tokens)
    
-    27         238 PUSH_NULL
-               240 LOAD_BUILD_CLASS
-               242 LOAD_CONST              18 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer.py", line 27>)
-               244 MAKE_FUNCTION            0
-               246 LOAD_CONST              19 ('LexerTokenizer')
-               248 LOAD_NAME               40 (Tokenizer)
-               250 PRECALL                  3
-               254 CALL                     3
-               264 STORE_NAME              42 (LexerTokenizer)
-               266 LOAD_CONST              20 (None)
-               268 RETURN_VALUE
+    28         246 PUSH_NULL
+               248 LOAD_BUILD_CLASS
+               250 LOAD_CONST              18 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer.py", line 28>)
+               252 MAKE_FUNCTION            0
+               254 LOAD_CONST              19 ('LexerTokenizer')
+               256 LOAD_NAME               40 (Tokenizer)
+               258 PRECALL                  3
+               262 CALL                     3
+               272 STORE_NAME              44 (LexerTokenizer)
+               274 LOAD_CONST              20 (None)
+               276 RETURN_VALUE
    consts
       0
-      ('List', 'Sequence', 'Set', 'Type', 'Union')
+      ('List', 'Optional', 'Sequence', 'Set', 'Type', 'Union')
+      ('logger',)
       ('OrderedSet',)
       ('highlight',)
       ('RawTokenFormatter',)
-      ('get_lexer_for_filename',)
       ('Lexer', 'RawTokenLexer')
       ('Token',)
-      ('ClassNotFound',)
       ('File',)
       ('Variable',)
       ('Semantic', 'SemanticType', 'Token')
       ('Language',)
-      ('VariableDetectionRules',)
+      ('VariableDetectionRules', 'VariableSuppressionRules')
       ('SpotImprovements',)
       ('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before')
       ('Tokenizer',)
+      ('LexerFinder',)
       ('\n', '\t', "'", "''", '"', '""')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
@@ -194,133 +198,141 @@
             0000006506650464033c0000006404650764056508650919000000000000
             0000006604640684045a0a640765036405650b6503650c66021900000000
             00000000006604640884045a0d6409650e6602640a84045a0f6416640965
             0e640565086510190000000000000000006604640c84055a11640d650865
             10190000000000000000006405640e6604640f84045a1264106513651019
             000000000000000000641165136510190000000000000000006405650865
             10190000000000000000006606641284045a146405651565101900000000
-            00000000006602641384045a166405650865101900000000000000000066
-            02641484045a176417641584045a18640e5300
-          27           0 RESUME                   0
+            00000000006602641384045a166417640d65176508651019000000000000
+            000000190000000000000000006405650865101900000000000000000066
+            04641484055a186418641584045a19640e5300
+          28           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LexerTokenizer')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          28          12 LOAD_NAME                3 (str)
+          29          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('token_stream')
                       18 STORE_SUBSCR
          
-          29          22 LOAD_NAME                5 (Lexer)
+          30          22 LOAD_NAME                5 (Lexer)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('lexer')
                       28 STORE_SUBSCR
          
-          30          32 LOAD_NAME                6 (Language)
+          31          32 LOAD_NAME                6 (Language)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('language')
                       38 STORE_SUBSCR
          
-          32          42 LOAD_CONST               4 ('token')
+          33          42 LOAD_CONST               4 ('token')
                       44 LOAD_NAME                7 (PygmentsToken)
                       46 LOAD_CONST               5 ('return')
                       48 LOAD_NAME                8 (List)
                       50 LOAD_NAME                9 (Type)
                       52 BINARY_SUBSCR
                       62 BUILD_TUPLE              4
-                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer.py", line 32>)
+                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer.py", line 33>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME              10 (_get_types_for_token)
          
-          42          70 LOAD_CONST               7 ('content')
+          43          70 LOAD_CONST               7 ('content')
                       72 LOAD_NAME                3 (str)
                       74 LOAD_CONST               5 ('return')
                       76 LOAD_NAME               11 (Union)
                       78 LOAD_NAME                3 (str)
                       80 LOAD_NAME               12 (bool)
                       82 BUILD_TUPLE              2
                       84 BINARY_SUBSCR
                       94 BUILD_TUPLE              4
-                      96 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 42>)
+                      96 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 43>)
                       98 MAKE_FUNCTION            4 (annotations)
                      100 STORE_NAME              13 (sanitize)
          
-          63         102 LOAD_CONST               9 ('file')
+          64         102 LOAD_CONST               9 ('file')
                      104 LOAD_NAME               14 (File)
                      106 BUILD_TUPLE              2
-                     108 LOAD_CONST              10 (<code object _find_lexer_for_file, file "/app/deepsecrets/core/tokenizers/lexer.py", line 63>)
+                     108 LOAD_CONST              10 (<code object _find_lexer_for_file, file "/app/deepsecrets/core/tokenizers/lexer.py", line 64>)
                      110 MAKE_FUNCTION            4 (annotations)
                      112 STORE_NAME              15 (_find_lexer_for_file)
          
-          83         114 LOAD_CONST              22 ((True,))
+          71         114 LOAD_CONST              22 ((True,))
                      116 LOAD_CONST               9 ('file')
                      118 LOAD_NAME               14 (File)
                      120 LOAD_CONST               5 ('return')
                      122 LOAD_NAME                8 (List)
                      124 LOAD_NAME               16 (Token)
                      126 BINARY_SUBSCR
                      136 BUILD_TUPLE              4
-                     138 LOAD_CONST              12 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 83>)
+                     138 LOAD_CONST              12 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 71>)
                      140 MAKE_FUNCTION            5 (defaults, annotations)
                      142 STORE_NAME              17 (tokenize)
          
-         131         144 LOAD_CONST              13 ('tokens')
+         121         144 LOAD_CONST              13 ('tokens')
                      146 LOAD_NAME                8 (List)
                      148 LOAD_NAME               16 (Token)
                      150 BINARY_SUBSCR
                      160 LOAD_CONST               5 ('return')
                      162 LOAD_CONST              14 (None)
                      164 BUILD_TUPLE              4
-                     166 LOAD_CONST              15 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 131>)
+                     166 LOAD_CONST              15 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 121>)
                      168 MAKE_FUNCTION            4 (annotations)
                      170 STORE_NAME              18 (add_to_token_stream)
          
-         135         172 LOAD_CONST              16 ('tokens_all')
+         125         172 LOAD_CONST              16 ('tokens_all')
                      174 LOAD_NAME               19 (Sequence)
                      176 LOAD_NAME               16 (Token)
                      178 BINARY_SUBSCR
                      188 LOAD_CONST              17 ('tokens_to_be_excluded')
                      190 LOAD_NAME               19 (Sequence)
                      192 LOAD_NAME               16 (Token)
                      194 BINARY_SUBSCR
                      204 LOAD_CONST               5 ('return')
                      206 LOAD_NAME                8 (List)
                      208 LOAD_NAME               16 (Token)
                      210 BINARY_SUBSCR
                      220 BUILD_TUPLE              6
-                     222 LOAD_CONST              18 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer.py", line 135>)
+                     222 LOAD_CONST              18 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer.py", line 125>)
                      224 MAKE_FUNCTION            4 (annotations)
                      226 STORE_NAME              20 (final_cleanup)
          
-         155         228 LOAD_CONST               5 ('return')
+         145         228 LOAD_CONST               5 ('return')
                      230 LOAD_NAME               21 (Set)
                      232 LOAD_NAME               16 (Token)
                      234 BINARY_SUBSCR
                      244 BUILD_TUPLE              2
-                     246 LOAD_CONST              19 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer.py", line 155>)
+                     246 LOAD_CONST              19 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer.py", line 145>)
                      248 MAKE_FUNCTION            4 (annotations)
                      250 STORE_NAME              22 (deep_analyze)
          
-         177         252 LOAD_CONST               5 ('return')
-                     254 LOAD_NAME                8 (List)
-                     256 LOAD_NAME               16 (Token)
-                     258 BINARY_SUBSCR
-                     268 BUILD_TUPLE              2
-                     270 LOAD_CONST              20 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer.py", line 177>)
-                     272 MAKE_FUNCTION            4 (annotations)
-                     274 STORE_NAME              23 (get_variables)
+         180         252 LOAD_CONST              23 ((None,))
+                     254 LOAD_CONST              13 ('tokens')
+                     256 LOAD_NAME               23 (Optional)
+                     258 LOAD_NAME                8 (List)
+                     260 LOAD_NAME               16 (Token)
+                     262 BINARY_SUBSCR
+                     272 BINARY_SUBSCR
+                     282 LOAD_CONST               5 ('return')
+                     284 LOAD_NAME                8 (List)
+                     286 LOAD_NAME               16 (Token)
+                     288 BINARY_SUBSCR
+                     298 BUILD_TUPLE              4
+                     300 LOAD_CONST              20 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer.py", line 180>)
+                     302 MAKE_FUNCTION            5 (defaults, annotations)
+                     304 STORE_NAME              24 (get_variables)
          
-         193         276 LOAD_CONST              23 (('return', None))
-                     278 LOAD_CONST              21 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 193>)
-                     280 MAKE_FUNCTION            4 (annotations)
-                     282 STORE_NAME              24 (print_token_type_stream)
-                     284 LOAD_CONST              14 (None)
-                     286 RETURN_VALUE
+         197         306 LOAD_CONST              24 (('return', None))
+                     308 LOAD_CONST              21 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 197>)
+                     310 MAKE_FUNCTION            4 (annotations)
+                     312 STORE_NAME              25 (print_token_type_stream)
+                     314 LOAD_CONST              14 (None)
+                     316 RETURN_VALUE
          consts
             'LexerTokenizer'
             'token_stream'
             'lexer'
             'language'
             'token'
             'return'
@@ -333,65 +345,65 @@
                   0x970067007d027c02a00000000000000000000000000000000000000000
                   007c01a6010000ab01000000000000000001007c016a0100000000000000
                   0081417c016a0100000000000000007404000000000000000000006b0200
                   00000072027c0253007c00a0030000000000000000000000000000000000
                   0000007c016a010000000000000000a6010000ab0100000000000000007d
                   037c02a00400000000000000000000000000000000000000007c03a60100
                   00ab01000000000000000001007c025300
-                32           0 RESUME                   0
+                33           0 RESUME                   0
                
-                33           2 BUILD_LIST               0
+                34           2 BUILD_LIST               0
                              4 STORE_FAST               2 (types)
                
-                34           6 LOAD_FAST                2 (types)
+                35           6 LOAD_FAST                2 (types)
                              8 LOAD_METHOD              0 (append)
                             30 LOAD_FAST                1 (token)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 POP_TOP
                
-                35          48 LOAD_FAST                1 (token)
+                36          48 LOAD_FAST                1 (token)
                             50 LOAD_ATTR                1 (parent)
                             60 POP_JUMP_FORWARD_IF_NONE    65 (to 192)
                
-                36          62 LOAD_FAST                1 (token)
+                37          62 LOAD_FAST                1 (token)
                             64 LOAD_ATTR                1 (parent)
                             74 LOAD_GLOBAL              4 (PygmentsToken)
                             86 COMPARE_OP               2 (==)
                             92 POP_JUMP_FORWARD_IF_FALSE     2 (to 98)
                
-                37          94 LOAD_FAST                2 (types)
+                38          94 LOAD_FAST                2 (types)
                             96 RETURN_VALUE
                
-                38     >>   98 LOAD_FAST                0 (self)
+                39     >>   98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              3 (_get_types_for_token)
                            122 LOAD_FAST                1 (token)
                            124 LOAD_ATTR                1 (parent)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               3 (deep)
                
-                39         150 LOAD_FAST                2 (types)
+                40         150 LOAD_FAST                2 (types)
                            152 LOAD_METHOD              4 (extend)
                            174 LOAD_FAST                3 (deep)
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
-                40     >>  192 LOAD_FAST                2 (types)
+                41     >>  192 LOAD_FAST                2 (types)
                            194 RETURN_VALUE
                consts
                   None
                names      ('append', 'parent', 'PygmentsToken', '_get_types_for_token', 'extend')
                varnames   ('self', 'token', 'types', 'deep')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       '_get_types_for_token'
-               firstlineno 32
+               firstlineno 33
                lnotab 0x020104012a010e012001040134012a01
             'content'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -402,30 +414,30 @@
                   0100000000720664046b020000000072056e0201006e0264055300740300
                   0000000000000000007c01a6010000ab01000000000000000064066b0400
                   00000072167c0164071900000000000000000064086b0200000000720a7c
                   01640064078502190000000000000000007d017c01640419000000000000
                   0000007c016407190000000000000000006b020000000072147c01640419
                   0000000000000000007c027600720a7c0164066407850219000000000000
                   0000007d017c017c0276007202640553007c015300
-                42           0 RESUME                   0
+                43           0 RESUME                   0
                
-                43           2 BUILD_LIST               0
+                44           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (("'", "''", '"', '""'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               2 (quotes)
                
-                45          10 LOAD_FAST                1 (content)
+                46          10 LOAD_FAST                1 (content)
                             12 LOAD_METHOD              0 (replace)
                             34 LOAD_CONST               2 (' ')
                             36 LOAD_CONST               3 ('')
                             38 PRECALL                  2
                             42 CALL                     2
                             52 STORE_FAST               3 (whitespace_cleaned)
                
-                46          54 LOAD_CONST               4 (0)
+                47          54 LOAD_CONST               4 (0)
                             56 LOAD_GLOBAL              3 (NULL + len)
                             68 LOAD_FAST                3 (whitespace_cleaned)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 SWAP                     2
                             86 COPY                     2
                             88 COMPARE_OP               1 (<=)
@@ -433,70 +445,70 @@
                             96 LOAD_CONST               4 (0)
                             98 COMPARE_OP               2 (==)
                            104 POP_JUMP_FORWARD_IF_FALSE     5 (to 116)
                            106 JUMP_FORWARD             2 (to 112)
                        >>  108 POP_TOP
                            110 JUMP_FORWARD             2 (to 116)
                
-                47     >>  112 LOAD_CONST               5 (False)
+                48     >>  112 LOAD_CONST               5 (False)
                            114 RETURN_VALUE
                
-                51     >>  116 LOAD_GLOBAL              3 (NULL + len)
+                52     >>  116 LOAD_GLOBAL              3 (NULL + len)
                            128 LOAD_FAST                1 (content)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               6 (1)
                            146 COMPARE_OP               4 (>)
                            152 POP_JUMP_FORWARD_IF_FALSE    22 (to 198)
                            154 LOAD_FAST                1 (content)
                            156 LOAD_CONST               7 (-1)
                            158 BINARY_SUBSCR
                            168 LOAD_CONST               8 ('\n')
                            170 COMPARE_OP               2 (==)
                            176 POP_JUMP_FORWARD_IF_FALSE    10 (to 198)
                
-                52         178 LOAD_FAST                1 (content)
+                53         178 LOAD_FAST                1 (content)
                            180 LOAD_CONST               0 (None)
                            182 LOAD_CONST               7 (-1)
                            184 BUILD_SLICE              2
                            186 BINARY_SUBSCR
                            196 STORE_FAST               1 (content)
                
-                54     >>  198 LOAD_FAST                1 (content)
+                55     >>  198 LOAD_FAST                1 (content)
                            200 LOAD_CONST               4 (0)
                            202 BINARY_SUBSCR
                            212 LOAD_FAST                1 (content)
                            214 LOAD_CONST               7 (-1)
                            216 BINARY_SUBSCR
                            226 COMPARE_OP               2 (==)
                            232 POP_JUMP_FORWARD_IF_FALSE    20 (to 274)
                
-                55         234 LOAD_FAST                1 (content)
+                56         234 LOAD_FAST                1 (content)
                            236 LOAD_CONST               4 (0)
                            238 BINARY_SUBSCR
                            248 LOAD_FAST                2 (quotes)
                            250 CONTAINS_OP              0
                            252 POP_JUMP_FORWARD_IF_FALSE    10 (to 274)
                
-                56         254 LOAD_FAST                1 (content)
+                57         254 LOAD_FAST                1 (content)
                            256 LOAD_CONST               6 (1)
                            258 LOAD_CONST               7 (-1)
                            260 BUILD_SLICE              2
                            262 BINARY_SUBSCR
                            272 STORE_FAST               1 (content)
                
-                58     >>  274 LOAD_FAST                1 (content)
+                59     >>  274 LOAD_FAST                1 (content)
                            276 LOAD_FAST                2 (quotes)
                            278 CONTAINS_OP              0
                            280 POP_JUMP_FORWARD_IF_FALSE     2 (to 286)
                
-                59         282 LOAD_CONST               5 (False)
+                60         282 LOAD_CONST               5 (False)
                            284 RETURN_VALUE
                
-                61     >>  286 LOAD_FAST                1 (content)
+                62     >>  286 LOAD_FAST                1 (content)
                            288 RETURN_VALUE
                consts
                   None
                   ("'", "''", '"', '""')
                   ' '
                   ''
                   0
@@ -506,620 +518,594 @@
                   '\n'
                names      ('replace', 'len')
                varnames   ('self', 'content', 'quotes', 'whitespace_cleaned')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'sanitize'
-               firstlineno 42
+               firstlineno 43
                lnotab 0x020108022c013a0104043e01140224011401140208010402
             'file'
             code
                argcount  : 2
                nlocals   : 3
-               stacksize : 5
+               stacksize : 3
                flags     : 3
                code
-                  0x970064007d027c016a0000000000000000008127090074030000000000
-                  00000000007c016a020000000000000000a6010000ab0100000000000000
-                  007d027c025300230074060000000000000000000024007203010059006e
-                  0477007803590077017c016a040000000000000000813109007403000000
-                  000000000000007c016a0200000000000000009b0064017c016a04000000
-                  00000000009b009d03a6010000ab0100000000000000007d027c02530023
-                  0074060000000000000000000024007203010059006e0477007803590077
-                  017c025300
-                63           0 RESUME                   0
-               
-                64           2 LOAD_CONST               0 (None)
-                             4 STORE_FAST               2 (lexer)
-               
-                65           6 LOAD_FAST                1 (file)
-                             8 LOAD_ATTR                0 (extension)
-                            18 POP_JUMP_FORWARD_IF_NONE    39 (to 98)
-               
-                66          20 NOP
-               
-                67          22 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
-                            34 LOAD_FAST                1 (file)
-                            36 LOAD_ATTR                2 (path)
-                            46 PRECALL                  1
-                            50 CALL                     1
-                            60 STORE_FAST               2 (lexer)
-               
-                68          62 LOAD_FAST                2 (lexer)
-                            64 RETURN_VALUE
-                       >>   66 PUSH_EXC_INFO
-               
-                69          68 LOAD_GLOBAL              6 (ClassNotFound)
-                            80 CHECK_EXC_MATCH
-                            82 POP_JUMP_FORWARD_IF_FALSE     3 (to 90)
-                            84 POP_TOP
-               
-                70          86 POP_EXCEPT
-                            88 JUMP_FORWARD             4 (to 98)
-               
-                69     >>   90 RERAISE                  0
-                       >>   92 COPY                     3
-                            94 POP_EXCEPT
-                            96 RERAISE                  1
-               
-                72     >>   98 LOAD_FAST                1 (file)
-                           100 LOAD_ATTR                4 (guessed_extension)
-                           110 POP_JUMP_FORWARD_IF_NONE    49 (to 210)
-               
-                73         112 NOP
-               
-                74         114 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
-                           126 LOAD_FAST                1 (file)
-                           128 LOAD_ATTR                2 (path)
-                           138 FORMAT_VALUE             0
-                           140 LOAD_CONST               1 ('.')
-                           142 LOAD_FAST                1 (file)
-                           144 LOAD_ATTR                4 (guessed_extension)
-                           154 FORMAT_VALUE             0
-                           156 BUILD_STRING             3
-                           158 PRECALL                  1
-                           162 CALL                     1
-                           172 STORE_FAST               2 (lexer)
-               
-                75         174 LOAD_FAST                2 (lexer)
-                           176 RETURN_VALUE
-                       >>  178 PUSH_EXC_INFO
-               
-                76         180 LOAD_GLOBAL              6 (ClassNotFound)
-                           192 CHECK_EXC_MATCH
-                           194 POP_JUMP_FORWARD_IF_FALSE     3 (to 202)
-                           196 POP_TOP
-               
-                77         198 POP_EXCEPT
-                           200 JUMP_FORWARD             4 (to 210)
-               
-                76     >>  202 RERAISE                  0
-                       >>  204 COPY                     3
-                           206 POP_EXCEPT
-                           208 RERAISE                  1
+                  0x9700740100000000000000000000a6000000ab000000000000000000a0
+                  0100000000000000000000000000000000000000007c01ac01a6010000ab
+                  0100000000000000007d027c02810d7c026a02000000000000000064026b
+                  02000000007202640053007c025300
+                64           0 RESUME                   0
+               
+                65           2 LOAD_GLOBAL              1 (NULL + LexerFinder)
+                            14 PRECALL                  0
+                            18 CALL                     0
+                            28 LOAD_METHOD              1 (find)
+                            50 LOAD_FAST                1 (file)
+                            52 KW_NAMES                 1
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 STORE_FAST               2 (lexer)
+               
+                66          70 LOAD_FAST                2 (lexer)
+                            72 POP_JUMP_FORWARD_IF_NONE    13 (to 100)
+                            74 LOAD_FAST                2 (lexer)
+                            76 LOAD_ATTR                2 (name)
+                            86 LOAD_CONST               2 ('Text only')
+                            88 COMPARE_OP               2 (==)
+                            94 POP_JUMP_FORWARD_IF_FALSE     2 (to 100)
                
-                79     >>  210 LOAD_FAST                2 (lexer)
-                           212 RETURN_VALUE
-               ExceptionTable:
-                 22 to 62 -> 66 [0]
-                 66 to 84 -> 92 [1] lasti
-                 90 to 90 -> 92 [1] lasti
-                 114 to 174 -> 178 [0]
-                 178 to 196 -> 204 [1] lasti
-                 202 to 202 -> 204 [1] lasti
+                67          96 LOAD_CONST               0 (None)
+                            98 RETURN_VALUE
+               
+                68     >>  100 LOAD_FAST                2 (lexer)
+                           102 RETURN_VALUE
                consts
                   None
-                  '.'
-               names      ('extension', 'get_lexer_for_filename', 'path', 'ClassNotFound', 'guessed_extension')
+                  ('file',)
+                  'Text only'
+               names      ('LexerFinder', 'find', 'name')
                varnames   ('self', 'file', 'lexer')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       '_find_lexer_for_file'
-               firstlineno 63
-               lnotab
-                  0x020104010e01020128010601120104ff08030e0102013c010601120104
-                  ff0803
+               firstlineno 64
+               lnotab 0x020144011a010401
             True
             code
                argcount  : 3
                nlocals   : 18
                stacksize : 7
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c00a001000000000000000000
                   00000000000000000000007c01a6010000ab0100000000000000007c005f
                   0200000000000000007c006a02000000000000000073077c006a03000000
                   0000000000530009007409000000000000000000006a0500000000000000
                   007c006a0200000000000000006a06000000000000000064021900000000
                   0000000000a6010000ab0100000000000000007c005f0700000000000000
-                  006e2e230074100000000000000000000024007221010074090000000000
-                  00000000006a0500000000000000007c016a090000000000000000a60100
-                  00ab0100000000000000007c005f07000000000000000059006e04770078
-                  03590077017415000000000000000000007c016a0b00000000000000007c
-                  006a020000000000000000741900000000000000000000a6000000ab0000
-                  00000000000000a6030000ab0300000000000000007d03741b0000000000
-                  0000000000741d00000000000000000000a6000000ab0000000000000000
-                  00a00f00000000000000000000000000000000000000007c03a6010000ab
-                  010000000000000000a6010000ab0100000000000000007d047421000000
+                  006e5b230074100000000000000000000074120000000000000000000066
+                  022400722101007409000000000000000000006a0500000000000000007c
+                  016a0a0000000000000000a6010000ab0100000000000000007c005f0700
+                  0000000000000059006e2a7416000000000000000000002400721e7d0374
+                  19000000000000000000006a0d00000000000000007c03a6010000ab0100
+                  000000000000000100590064007d037e036e0864007d037e037701770078
+                  0359007701741d000000000000000000007c016a0f00000000000000007c
+                  006a020000000000000000742100000000000000000000a6000000ab0000
+                  00000000000000a6030000ab0300000000000000007d0474230000000000
+                  0000000000742500000000000000000000a6000000ab0000000000000000
+                  00a01300000000000000000000000000000000000000007c04a6010000ab
+                  010000000000000000a6010000ab0100000000000000007d057429000000
                   000000000000007c006a070000000000000000ac03a6010000ab01000000
-                  00000000007d0564027d067423000000000000000000007c04a6010000ab
-                  010000000000000000440090015d145c0200007d077d087c086404190000
-                  000000000000007d097c00a0120000000000000000000000000000000000
-                  0000007c08640219000000000000000000a6010000ab0100000000000000
-                  007d0a7c067d0b7c0b7427000000000000000000007c09a6010000ab0100
-                  000000000000007a0000007d0c7c0c7d0609007c00a01400000000000000
-                  000000000000000000000000007c09a6010000ab0100000000000000007d
-                  097c0973018c587c01a01500000000000000000000000000000000000000
-                  007c097c0b64047a0a00007c0c64047a0000006702ac05a6020000ab0200
-                  000000000000007d0d742d000000000000000000007c017c097c0dac06a6
-                  030000ab0300000000000000007d0e7c0ea0170000000000000000000000
-                  0000000000000000007c0aa6010000ab01000000000000000001007c05a0
-                  1800000000000000000000000000000000000000007c006a030000000000
-                  0000007c006a0000000000000000007c0ea6030000ab0300000000000000
-                  007d0f7c006a030000000000000000a01900000000000000000000000000
-                  000000000000007c0fa6010000ab01000000000000000001007c00a01a00
-                  000000000000000000000000000000000000007c0fa6010000ab01000000
-                  000000000001008cef23007436000000000000000000002400721a7d1074
-                  39000000000000000000007c10a6010000ab010000000000000000010059
-                  0064007d107e1090018c0e64007d107e107701770078035900770167007d
-                  117c006a1d00000000000000006a1e00000000000000006407750072147c
-                  00a01f0000000000000000000000000000000000000000a6000000ab0000
-                  000000000000007d117c02721b7c00a02000000000000000000000000000
+                  00000000007d0664027d07742b000000000000000000007c05a6010000ab
+                  010000000000000000440090015d145c0200007d087d097c096404190000
+                  000000000000007d0a7c00a0160000000000000000000000000000000000
+                  0000007c09640219000000000000000000a6010000ab0100000000000000
+                  007d0b7c077d0c7c0c742f000000000000000000007c0aa6010000ab0100
+                  000000000000007a0000007d0d7c0d7d0709007c00a01800000000000000
+                  000000000000000000000000007c0aa6010000ab0100000000000000007d
+                  0a7c0a73018c587c01a01900000000000000000000000000000000000000
+                  007c0a7c0c64047a0a00007c0d64047a0000006702ac05a6020000ab0200
+                  000000000000007d0e7435000000000000000000007c017c0a7c0eac06a6
+                  030000ab0300000000000000007d0f7c0fa01b0000000000000000000000
+                  0000000000000000007c0ba6010000ab01000000000000000001007c06a0
+                  1c00000000000000000000000000000000000000007c006a030000000000
+                  0000007c006a0000000000000000007c0fa6030000ab0300000000000000
+                  007d107c006a030000000000000000a01d00000000000000000000000000
+                  000000000000007c10a6010000ab01000000000000000001007c00a01e00
+                  000000000000000000000000000000000000007c10a6010000ab01000000
+                  000000000001008cef23007416000000000000000000002400721a7d0374
+                  3f000000000000000000007c03a6010000ab010000000000000000010059
+                  0064007d037e0390018c0e64007d037e037701770078035900770167007d
+                  117c006a2000000000000000006a2100000000000000006407750072147c
+                  00a0220000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d117c02721b7c00a02300000000000000000000000000
                   000000000000007c006a0300000000000000007c11a6020000ab02000000
-                  00000000006e13741b000000000000000000007c006a0300000000000000
+                  00000000006e137423000000000000000000007c006a0300000000000000
                   00a6010000ab0100000000000000005300
-                83           0 RESUME                   0
+                71           0 RESUME                   0
                
-                84           2 LOAD_CONST               1 ('')
+                72           2 LOAD_CONST               1 ('')
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (token_stream)
                
-                87          16 LOAD_FAST                0 (self)
+                75          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (_find_lexer_for_file)
                             40 LOAD_FAST                1 (file)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_FAST                0 (self)
                             58 STORE_ATTR               2 (lexer)
                
-                88          68 LOAD_FAST                0 (self)
+                76          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (lexer)
                             80 POP_JUMP_FORWARD_IF_TRUE     7 (to 96)
                
-                89          82 LOAD_FAST                0 (self)
+                77          82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (tokens)
                             94 RETURN_VALUE
                
-                91     >>   96 NOP
+                79     >>   96 NOP
                
-                92          98 LOAD_GLOBAL              9 (NULL + Language)
+                80          98 LOAD_GLOBAL              9 (NULL + Language)
                            110 LOAD_ATTR                5 (from_text)
                            120 LOAD_FAST                0 (self)
                            122 LOAD_ATTR                2 (lexer)
                            132 LOAD_ATTR                6 (filenames)
                            142 LOAD_CONST               2 (0)
                            144 BINARY_SUBSCR
                            154 PRECALL                  1
                            158 CALL                     1
                            168 LOAD_FAST                0 (self)
                            170 STORE_ATTR               7 (language)
-                           180 JUMP_FORWARD            46 (to 274)
+                           180 JUMP_FORWARD            91 (to 364)
                        >>  182 PUSH_EXC_INFO
                
-                93         184 LOAD_GLOBAL             16 (ValueError)
-                           196 CHECK_EXC_MATCH
-                           198 POP_JUMP_FORWARD_IF_FALSE    33 (to 266)
-                           200 POP_TOP
-               
-                94         202 LOAD_GLOBAL              9 (NULL + Language)
-                           214 LOAD_ATTR                5 (from_text)
-                           224 LOAD_FAST                1 (file)
-                           226 LOAD_ATTR                9 (extension)
-                           236 PRECALL                  1
-                           240 CALL                     1
-                           250 LOAD_FAST                0 (self)
-                           252 STORE_ATTR               7 (language)
-                           262 POP_EXCEPT
-                           264 JUMP_FORWARD             4 (to 274)
-               
-                93     >>  266 RERAISE                  0
-                       >>  268 COPY                     3
-                           270 POP_EXCEPT
-                           272 RERAISE                  1
-               
-                96     >>  274 LOAD_GLOBAL             21 (NULL + highlight)
-                           286 LOAD_FAST                1 (file)
-                           288 LOAD_ATTR               11 (content)
-                           298 LOAD_FAST                0 (self)
-                           300 LOAD_ATTR                2 (lexer)
-                           310 LOAD_GLOBAL             25 (NULL + RawTokenFormatter)
-                           322 PRECALL                  0
-                           326 CALL                     0
-                           336 PRECALL                  3
-                           340 CALL                     3
-                           350 STORE_FAST               3 (result)
-               
-                97         352 LOAD_GLOBAL             27 (NULL + list)
-                           364 LOAD_GLOBAL             29 (NULL + RawTokenLexer)
-                           376 PRECALL                  0
-                           380 CALL                     0
-                           390 LOAD_METHOD             15 (get_tokens)
-                           412 LOAD_FAST                3 (result)
-                           414 PRECALL                  1
-                           418 CALL                     1
-                           428 PRECALL                  1
-                           432 CALL                     1
-                           442 STORE_FAST               4 (raw_tokens)
-               
-                98         444 LOAD_GLOBAL             33 (NULL + SpotImprovements)
-                           456 LOAD_FAST                0 (self)
-                           458 LOAD_ATTR                7 (language)
-                           468 KW_NAMES                 3
-                           470 PRECALL                  1
-                           474 CALL                     1
-                           484 STORE_FAST               5 (token_improver)
-               
-               100         486 LOAD_CONST               2 (0)
-                           488 STORE_FAST               6 (current_position)
-               
-               102         490 LOAD_GLOBAL             35 (NULL + enumerate)
-                           502 LOAD_FAST                4 (raw_tokens)
+                81         184 LOAD_GLOBAL             16 (ValueError)
+                           196 LOAD_GLOBAL             18 (IndexError)
+                           208 BUILD_TUPLE              2
+                           210 CHECK_EXC_MATCH
+                           212 POP_JUMP_FORWARD_IF_FALSE    33 (to 280)
+                           214 POP_TOP
+               
+                82         216 LOAD_GLOBAL              9 (NULL + Language)
+                           228 LOAD_ATTR                5 (from_text)
+                           238 LOAD_FAST                1 (file)
+                           240 LOAD_ATTR               10 (extension)
+                           250 PRECALL                  1
+                           254 CALL                     1
+                           264 LOAD_FAST                0 (self)
+                           266 STORE_ATTR               7 (language)
+                           276 POP_EXCEPT
+                           278 JUMP_FORWARD            42 (to 364)
+               
+                83     >>  280 LOAD_GLOBAL             22 (Exception)
+                           292 CHECK_EXC_MATCH
+                           294 POP_JUMP_FORWARD_IF_FALSE    30 (to 356)
+                           296 STORE_FAST               3 (e)
+               
+                84         298 LOAD_GLOBAL             25 (NULL + logger)
+                           310 LOAD_ATTR               13 (exception)
+                           320 LOAD_FAST                3 (e)
+                           322 PRECALL                  1
+                           326 CALL                     1
+                           336 POP_TOP
+                           338 POP_EXCEPT
+                           340 LOAD_CONST               0 (None)
+                           342 STORE_FAST               3 (e)
+                           344 DELETE_FAST              3 (e)
+                           346 JUMP_FORWARD             8 (to 364)
+                       >>  348 LOAD_CONST               0 (None)
+                           350 STORE_FAST               3 (e)
+                           352 DELETE_FAST              3 (e)
+                           354 RERAISE                  1
+               
+                83     >>  356 RERAISE                  0
+                       >>  358 COPY                     3
+                           360 POP_EXCEPT
+                           362 RERAISE                  1
+               
+                86     >>  364 LOAD_GLOBAL             29 (NULL + highlight)
+                           376 LOAD_FAST                1 (file)
+                           378 LOAD_ATTR               15 (content)
+                           388 LOAD_FAST                0 (self)
+                           390 LOAD_ATTR                2 (lexer)
+                           400 LOAD_GLOBAL             33 (NULL + RawTokenFormatter)
+                           412 PRECALL                  0
+                           416 CALL                     0
+                           426 PRECALL                  3
+                           430 CALL                     3
+                           440 STORE_FAST               4 (result)
+               
+                87         442 LOAD_GLOBAL             35 (NULL + list)
+                           454 LOAD_GLOBAL             37 (NULL + RawTokenLexer)
+                           466 PRECALL                  0
+                           470 CALL                     0
+                           480 LOAD_METHOD             19 (get_tokens)
+                           502 LOAD_FAST                4 (result)
                            504 PRECALL                  1
                            508 CALL                     1
-                           518 GET_ITER
-                       >>  520 EXTENDED_ARG             1
-                           522 FOR_ITER               276 (to 1076)
-                           524 UNPACK_SEQUENCE          2
-                           528 STORE_FAST               7 (i)
-                           530 STORE_FAST               8 (raw_token)
-               
-               103         532 LOAD_FAST                8 (raw_token)
-                           534 LOAD_CONST               4 (1)
-                           536 BINARY_SUBSCR
-                           546 STORE_FAST               9 (content)
-               
-               104         548 LOAD_FAST                0 (self)
-                           550 LOAD_METHOD             18 (_get_types_for_token)
-                           572 LOAD_FAST                8 (raw_token)
-                           574 LOAD_CONST               2 (0)
-                           576 BINARY_SUBSCR
-                           586 PRECALL                  1
-                           590 CALL                     1
-                           600 STORE_FAST              10 (types)
-               
-               105         602 LOAD_FAST                6 (current_position)
-                           604 STORE_FAST              11 (start)
-               
-               106         606 LOAD_FAST               11 (start)
-                           608 LOAD_GLOBAL             39 (NULL + len)
-                           620 LOAD_FAST                9 (content)
-                           622 PRECALL                  1
-                           626 CALL                     1
-                           636 BINARY_OP                0 (+)
-                           640 STORE_FAST              12 (end)
-               
-               107         642 LOAD_FAST               12 (end)
-                           644 STORE_FAST               6 (current_position)
-               
-               109         646 NOP
-               
-               110         648 LOAD_FAST                0 (self)
-                           650 LOAD_METHOD             20 (sanitize)
-                           672 LOAD_FAST                9 (content)
-                           674 PRECALL                  1
-                           678 CALL                     1
-                           688 STORE_FAST               9 (content)
-               
-               111         690 LOAD_FAST                9 (content)
-                           692 POP_JUMP_FORWARD_IF_TRUE     1 (to 696)
-               
-               112         694 JUMP_BACKWARD           88 (to 520)
-               
-               114     >>  696 LOAD_FAST                1 (file)
-                           698 LOAD_METHOD             21 (get_span_for_string)
-                           720 LOAD_FAST                9 (content)
-                           722 LOAD_FAST               11 (start)
-                           724 LOAD_CONST               4 (1)
-                           726 BINARY_OP               10 (-)
-                           730 LOAD_FAST               12 (end)
-                           732 LOAD_CONST               4 (1)
-                           734 BINARY_OP                0 (+)
-                           738 BUILD_LIST               2
-                           740 KW_NAMES                 5
-                           742 PRECALL                  2
-                           746 CALL                     2
-                           756 STORE_FAST              13 (span)
-               
-               115         758 LOAD_GLOBAL             45 (NULL + Token)
-                           770 LOAD_FAST                1 (file)
-                           772 LOAD_FAST                9 (content)
-                           774 LOAD_FAST               13 (span)
-                           776 KW_NAMES                 6
-                           778 PRECALL                  3
-                           782 CALL                     3
-                           792 STORE_FAST              14 (token)
-               
-               116         794 LOAD_FAST               14 (token)
-                           796 LOAD_METHOD             23 (set_type)
-                           818 LOAD_FAST               10 (types)
-                           820 PRECALL                  1
-                           824 CALL                     1
-                           834 POP_TOP
-               
-               118         836 LOAD_FAST                5 (token_improver)
-                           838 LOAD_METHOD             24 (improve_token)
-                           860 LOAD_FAST                0 (self)
-                           862 LOAD_ATTR                3 (tokens)
-                           872 LOAD_FAST                0 (self)
-                           874 LOAD_ATTR                0 (token_stream)
-                           884 LOAD_FAST               14 (token)
-                           886 PRECALL                  3
-                           890 CALL                     3
-                           900 STORE_FAST              15 (improved_tokens)
-               
-               120         902 LOAD_FAST                0 (self)
-                           904 LOAD_ATTR                3 (tokens)
-                           914 LOAD_METHOD             25 (extend)
-                           936 LOAD_FAST               15 (improved_tokens)
-                           938 PRECALL                  1
-                           942 CALL                     1
-                           952 POP_TOP
-               
-               121         954 LOAD_FAST                0 (self)
-                           956 LOAD_METHOD             26 (add_to_token_stream)
-                           978 LOAD_FAST               15 (improved_tokens)
-                           980 PRECALL                  1
-                           984 CALL                     1
-                           994 POP_TOP
-                           996 JUMP_BACKWARD          239 (to 520)
-                       >>  998 PUSH_EXC_INFO
-               
-               122        1000 LOAD_GLOBAL             54 (Exception)
-                          1012 CHECK_EXC_MATCH
-                          1014 POP_JUMP_FORWARD_IF_FALSE    26 (to 1068)
-                          1016 STORE_FAST              16 (e)
-               
-               123        1018 LOAD_GLOBAL             57 (NULL + str)
-                          1030 LOAD_FAST               16 (e)
-                          1032 PRECALL                  1
-                          1036 CALL                     1
-                          1046 POP_TOP
-                          1048 POP_EXCEPT
-                          1050 LOAD_CONST               0 (None)
-                          1052 STORE_FAST              16 (e)
-                          1054 DELETE_FAST             16 (e)
-                          1056 EXTENDED_ARG             1
-                          1058 JUMP_BACKWARD          270 (to 520)
-                       >> 1060 LOAD_CONST               0 (None)
-                          1062 STORE_FAST              16 (e)
-                          1064 DELETE_FAST             16 (e)
-                          1066 RERAISE                  1
-               
-               122     >> 1068 RERAISE                  0
-                       >> 1070 COPY                     3
-                          1072 POP_EXCEPT
-                          1074 RERAISE                  1
-               
-               125     >> 1076 BUILD_LIST               0
-                          1078 STORE_FAST              17 (tokens_to_be_excluded)
-               
-               126        1080 LOAD_FAST                0 (self)
-                          1082 LOAD_ATTR               29 (settings)
-                          1092 LOAD_ATTR               30 (deep_token_inspection)
-                          1102 LOAD_CONST               7 (True)
-                          1104 IS_OP                    0
-                          1106 POP_JUMP_FORWARD_IF_FALSE    20 (to 1148)
-               
-               127        1108 LOAD_FAST                0 (self)
-                          1110 LOAD_METHOD             31 (deep_analyze)
-                          1132 PRECALL                  0
-                          1136 CALL                     0
-                          1146 STORE_FAST              17 (tokens_to_be_excluded)
-               
-               129     >> 1148 LOAD_FAST                2 (post_filter)
-                          1150 POP_JUMP_FORWARD_IF_FALSE    27 (to 1206)
-                          1152 LOAD_FAST                0 (self)
-                          1154 LOAD_METHOD             32 (final_cleanup)
-                          1176 LOAD_FAST                0 (self)
-                          1178 LOAD_ATTR                3 (tokens)
-                          1188 LOAD_FAST               17 (tokens_to_be_excluded)
-                          1190 PRECALL                  2
-                          1194 CALL                     2
-                          1204 JUMP_FORWARD            19 (to 1244)
-                       >> 1206 LOAD_GLOBAL             27 (NULL + list)
-                          1218 LOAD_FAST                0 (self)
-                          1220 LOAD_ATTR                3 (tokens)
-                          1230 PRECALL                  1
-                          1234 CALL                     1
-                       >> 1244 RETURN_VALUE
+                           518 PRECALL                  1
+                           522 CALL                     1
+                           532 STORE_FAST               5 (raw_tokens)
+               
+                88         534 LOAD_GLOBAL             41 (NULL + SpotImprovements)
+                           546 LOAD_FAST                0 (self)
+                           548 LOAD_ATTR                7 (language)
+                           558 KW_NAMES                 3
+                           560 PRECALL                  1
+                           564 CALL                     1
+                           574 STORE_FAST               6 (token_improver)
+               
+                90         576 LOAD_CONST               2 (0)
+                           578 STORE_FAST               7 (current_position)
+               
+                92         580 LOAD_GLOBAL             43 (NULL + enumerate)
+                           592 LOAD_FAST                5 (raw_tokens)
+                           594 PRECALL                  1
+                           598 CALL                     1
+                           608 GET_ITER
+                       >>  610 EXTENDED_ARG             1
+                           612 FOR_ITER               276 (to 1166)
+                           614 UNPACK_SEQUENCE          2
+                           618 STORE_FAST               8 (i)
+                           620 STORE_FAST               9 (raw_token)
+               
+                93         622 LOAD_FAST                9 (raw_token)
+                           624 LOAD_CONST               4 (1)
+                           626 BINARY_SUBSCR
+                           636 STORE_FAST              10 (content)
+               
+                94         638 LOAD_FAST                0 (self)
+                           640 LOAD_METHOD             22 (_get_types_for_token)
+                           662 LOAD_FAST                9 (raw_token)
+                           664 LOAD_CONST               2 (0)
+                           666 BINARY_SUBSCR
+                           676 PRECALL                  1
+                           680 CALL                     1
+                           690 STORE_FAST              11 (types)
+               
+                95         692 LOAD_FAST                7 (current_position)
+                           694 STORE_FAST              12 (start)
+               
+                96         696 LOAD_FAST               12 (start)
+                           698 LOAD_GLOBAL             47 (NULL + len)
+                           710 LOAD_FAST               10 (content)
+                           712 PRECALL                  1
+                           716 CALL                     1
+                           726 BINARY_OP                0 (+)
+                           730 STORE_FAST              13 (end)
+               
+                97         732 LOAD_FAST               13 (end)
+                           734 STORE_FAST               7 (current_position)
+               
+                99         736 NOP
+               
+               100         738 LOAD_FAST                0 (self)
+                           740 LOAD_METHOD             24 (sanitize)
+                           762 LOAD_FAST               10 (content)
+                           764 PRECALL                  1
+                           768 CALL                     1
+                           778 STORE_FAST              10 (content)
+               
+               101         780 LOAD_FAST               10 (content)
+                           782 POP_JUMP_FORWARD_IF_TRUE     1 (to 786)
+               
+               102         784 JUMP_BACKWARD           88 (to 610)
+               
+               104     >>  786 LOAD_FAST                1 (file)
+                           788 LOAD_METHOD             25 (get_span_for_string)
+                           810 LOAD_FAST               10 (content)
+                           812 LOAD_FAST               12 (start)
+                           814 LOAD_CONST               4 (1)
+                           816 BINARY_OP               10 (-)
+                           820 LOAD_FAST               13 (end)
+                           822 LOAD_CONST               4 (1)
+                           824 BINARY_OP                0 (+)
+                           828 BUILD_LIST               2
+                           830 KW_NAMES                 5
+                           832 PRECALL                  2
+                           836 CALL                     2
+                           846 STORE_FAST              14 (span)
+               
+               105         848 LOAD_GLOBAL             53 (NULL + Token)
+                           860 LOAD_FAST                1 (file)
+                           862 LOAD_FAST               10 (content)
+                           864 LOAD_FAST               14 (span)
+                           866 KW_NAMES                 6
+                           868 PRECALL                  3
+                           872 CALL                     3
+                           882 STORE_FAST              15 (token)
+               
+               106         884 LOAD_FAST               15 (token)
+                           886 LOAD_METHOD             27 (set_type)
+                           908 LOAD_FAST               11 (types)
+                           910 PRECALL                  1
+                           914 CALL                     1
+                           924 POP_TOP
+               
+               108         926 LOAD_FAST                6 (token_improver)
+                           928 LOAD_METHOD             28 (improve_token)
+                           950 LOAD_FAST                0 (self)
+                           952 LOAD_ATTR                3 (tokens)
+                           962 LOAD_FAST                0 (self)
+                           964 LOAD_ATTR                0 (token_stream)
+                           974 LOAD_FAST               15 (token)
+                           976 PRECALL                  3
+                           980 CALL                     3
+                           990 STORE_FAST              16 (improved_tokens)
+               
+               110         992 LOAD_FAST                0 (self)
+                           994 LOAD_ATTR                3 (tokens)
+                          1004 LOAD_METHOD             29 (extend)
+                          1026 LOAD_FAST               16 (improved_tokens)
+                          1028 PRECALL                  1
+                          1032 CALL                     1
+                          1042 POP_TOP
+               
+               111        1044 LOAD_FAST                0 (self)
+                          1046 LOAD_METHOD             30 (add_to_token_stream)
+                          1068 LOAD_FAST               16 (improved_tokens)
+                          1070 PRECALL                  1
+                          1074 CALL                     1
+                          1084 POP_TOP
+                          1086 JUMP_BACKWARD          239 (to 610)
+                       >> 1088 PUSH_EXC_INFO
+               
+               112        1090 LOAD_GLOBAL             22 (Exception)
+                          1102 CHECK_EXC_MATCH
+                          1104 POP_JUMP_FORWARD_IF_FALSE    26 (to 1158)
+                          1106 STORE_FAST               3 (e)
+               
+               113        1108 LOAD_GLOBAL             63 (NULL + str)
+                          1120 LOAD_FAST                3 (e)
+                          1122 PRECALL                  1
+                          1126 CALL                     1
+                          1136 POP_TOP
+                          1138 POP_EXCEPT
+                          1140 LOAD_CONST               0 (None)
+                          1142 STORE_FAST               3 (e)
+                          1144 DELETE_FAST              3 (e)
+                          1146 EXTENDED_ARG             1
+                          1148 JUMP_BACKWARD          270 (to 610)
+                       >> 1150 LOAD_CONST               0 (None)
+                          1152 STORE_FAST               3 (e)
+                          1154 DELETE_FAST              3 (e)
+                          1156 RERAISE                  1
+               
+               112     >> 1158 RERAISE                  0
+                       >> 1160 COPY                     3
+                          1162 POP_EXCEPT
+                          1164 RERAISE                  1
+               
+               115     >> 1166 BUILD_LIST               0
+                          1168 STORE_FAST              17 (tokens_to_be_excluded)
+               
+               116        1170 LOAD_FAST                0 (self)
+                          1172 LOAD_ATTR               32 (settings)
+                          1182 LOAD_ATTR               33 (deep_token_inspection)
+                          1192 LOAD_CONST               7 (True)
+                          1194 IS_OP                    0
+                          1196 POP_JUMP_FORWARD_IF_FALSE    20 (to 1238)
+               
+               117        1198 LOAD_FAST                0 (self)
+                          1200 LOAD_METHOD             34 (deep_analyze)
+                          1222 PRECALL                  0
+                          1226 CALL                     0
+                          1236 STORE_FAST              17 (tokens_to_be_excluded)
+               
+               119     >> 1238 LOAD_FAST                2 (post_filter)
+                          1240 POP_JUMP_FORWARD_IF_FALSE    27 (to 1296)
+                          1242 LOAD_FAST                0 (self)
+                          1244 LOAD_METHOD             35 (final_cleanup)
+                          1266 LOAD_FAST                0 (self)
+                          1268 LOAD_ATTR                3 (tokens)
+                          1278 LOAD_FAST               17 (tokens_to_be_excluded)
+                          1280 PRECALL                  2
+                          1284 CALL                     2
+                          1294 JUMP_FORWARD            19 (to 1334)
+                       >> 1296 LOAD_GLOBAL             35 (NULL + list)
+                          1308 LOAD_FAST                0 (self)
+                          1310 LOAD_ATTR                3 (tokens)
+                          1320 PRECALL                  1
+                          1324 CALL                     1
+                       >> 1334 RETURN_VALUE
                ExceptionTable:
                  98 to 178 -> 182 [0]
-                 182 to 260 -> 268 [1] lasti
-                 266 to 266 -> 268 [1] lasti
-                 648 to 692 -> 998 [1]
-                 696 to 994 -> 998 [1]
-                 998 to 1016 -> 1070 [2] lasti
-                 1018 to 1046 -> 1060 [2] lasti
-                 1060 to 1068 -> 1070 [2] lasti
+                 182 to 274 -> 358 [1] lasti
+                 280 to 296 -> 358 [1] lasti
+                 298 to 336 -> 348 [1] lasti
+                 348 to 356 -> 358 [1] lasti
+                 738 to 782 -> 1088 [1]
+                 786 to 1084 -> 1088 [1]
+                 1088 to 1106 -> 1160 [2] lasti
+                 1108 to 1136 -> 1150 [2] lasti
+                 1150 to 1158 -> 1160 [2] lasti
                consts
                   None
                   ''
                   0
                   ('lang',)
                   1
                   ('between',)
                   ('file', 'content', 'span')
                   True
-               names      ('token_stream', '_find_lexer_for_file', 'lexer', 'tokens', 'Language', 'from_text', 'filenames', 'language', 'ValueError', 'extension', 'highlight', 'content', 'RawTokenFormatter', 'list', 'RawTokenLexer', 'get_tokens', 'SpotImprovements', 'enumerate', '_get_types_for_token', 'len', 'sanitize', 'get_span_for_string', 'Token', 'set_type', 'improve_token', 'extend', 'add_to_token_stream', 'Exception', 'str', 'settings', 'deep_token_inspection', 'deep_analyze', 'final_cleanup')
-               varnames   ('self', 'file', 'post_filter', 'result', 'raw_tokens', 'token_improver', 'current_position', 'i', 'raw_token', 'content', 'types', 'start', 'end', 'span', 'token', 'improved_tokens', 'e', 'tokens_to_be_excluded')
+               names      ('token_stream', '_find_lexer_for_file', 'lexer', 'tokens', 'Language', 'from_text', 'filenames', 'language', 'ValueError', 'IndexError', 'extension', 'Exception', 'logger', 'exception', 'highlight', 'content', 'RawTokenFormatter', 'list', 'RawTokenLexer', 'get_tokens', 'SpotImprovements', 'enumerate', '_get_types_for_token', 'len', 'sanitize', 'get_span_for_string', 'Token', 'set_type', 'improve_token', 'extend', 'add_to_token_stream', 'str', 'settings', 'deep_token_inspection', 'deep_analyze', 'final_cleanup')
+               varnames   ('self', 'file', 'post_filter', 'e', 'result', 'raw_tokens', 'token_improver', 'current_position', 'i', 'raw_token', 'content', 'types', 'start', 'end', 'span', 'token', 'improved_tokens', 'tokens_to_be_excluded')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'tokenize'
-               firstlineno 83
+               firstlineno 71
                lnotab
-                  0x02010e0334010e010e0202015601120140ff08034e015c012a0204022a
-                  011001360104012401040202012a01040102023e0124012a02420234012e
-                  01120132ff080304011c012802
+                  0x02010e0334010e010e02020156012001400112013aff08034e015c012a
+                  0204022a011001360104012401040202012a01040102023e0124012a0242
+                  0234012e01120132ff080304011c012802
             'tokens'
             None
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c0144005d207d027c0078016a0000000000000000007403000000
                   000000000000007c02ac01a6010000ab0100000000000000007a0d000063
                   025f0000000000000000008c2164005300
-               131           0 RESUME                   0
+               121           0 RESUME                   0
                
-               132           2 LOAD_FAST                1 (tokens)
+               122           2 LOAD_FAST                1 (tokens)
                              4 GET_ITER
                        >>    6 FOR_ITER                32 (to 72)
                              8 STORE_FAST               2 (token)
                
-               133          10 LOAD_FAST                0 (self)
+               123          10 LOAD_FAST                0 (self)
                             12 COPY                     1
                             14 LOAD_ATTR                0 (token_stream)
                             24 LOAD_GLOBAL              3 (NULL + token_to_typestream_item)
                             36 LOAD_FAST                2 (token)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 BINARY_OP               13 (+=)
                             58 SWAP                     2
                             60 STORE_ATTR               0 (token_stream)
                             70 JUMP_BACKWARD           33 (to 6)
                
-               132     >>   72 LOAD_CONST               0 (None)
+               122     >>   72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   ('token',)
                names      ('token_stream', 'token_to_typestream_item')
                varnames   ('self', 'tokens', 'token')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'add_to_token_stream'
-               firstlineno 131
+               firstlineno 121
                lnotab 0x020108013eff
             'tokens_all'
             'tokens_to_be_excluded'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x870497007401000000000000000000007c017402000000000000000000
                   00a6020000ab020000000000000000730f7403000000000000000000007c
                   01a6010000ab0100000000000000007d017c017c027a0a00007d0167007d
-                  037c0144005d688a04740500000000000000000000880466016401840874
+                  037c0144005d7c8a04740500000000000000000000880466016401840874
                   06000000000000000000004400a6000000ab000000000000000000a60100
                   00ab01000000000000000072018c23740500000000000000000000880466
                   01640284087408000000000000000000004400a6000000ab000000000000
                   000000a6010000ab01000000000000000072018c4489046a050000000000
-                  000000740c00000000000000000000760072018c537c03a0070000000000
-                  0000000000000000000000000000008904a6010000ab0100000000000000
-                  0001008c697c035300
+                  000000a006000000000000000000000000000000000000000064036404a6
+                  020000ab020000000000000000740e00000000000000000000760072018c
+                  677c03a00800000000000000000000000000000000000000008904a60100
+                  00ab01000000000000000001008c7d7c035300
                              0 MAKE_CELL                4 (token)
                
-               135           2 RESUME                   0
+               125           2 RESUME                   0
                
-               136           4 LOAD_GLOBAL              1 (NULL + isinstance)
+               126           4 LOAD_GLOBAL              1 (NULL + isinstance)
                             16 LOAD_FAST                1 (tokens_all)
                             18 LOAD_GLOBAL              2 (OrderedSet)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_TRUE    15 (to 76)
                
-               137          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
+               127          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
                             58 LOAD_FAST                1 (tokens_all)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 STORE_FAST               1 (tokens_all)
                
-               139     >>   76 LOAD_FAST                1 (tokens_all)
+               129     >>   76 LOAD_FAST                1 (tokens_all)
                             78 LOAD_FAST                2 (tokens_to_be_excluded)
                             80 BINARY_OP               10 (-)
                             84 STORE_FAST               1 (tokens_all)
                
-               140          86 BUILD_LIST               0
+               130          86 BUILD_LIST               0
                             88 STORE_FAST               3 (final)
                
-               141          90 LOAD_FAST                1 (tokens_all)
+               131          90 LOAD_FAST                1 (tokens_all)
                             92 GET_ITER
-                       >>   94 FOR_ITER               104 (to 304)
+                       >>   94 FOR_ITER               124 (to 344)
                             96 STORE_DEREF              4 (token)
                
-               142          98 LOAD_GLOBAL              5 (NULL + any)
+               132          98 LOAD_GLOBAL              5 (NULL + any)
                            110 LOAD_CLOSURE             4 (token)
                            112 BUILD_TUPLE              1
-                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 142>)
+                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 132>)
                            116 MAKE_FUNCTION            8 (closure)
                            118 LOAD_GLOBAL              6 (types_to_filter_before)
                            130 GET_ITER
                            132 PRECALL                  0
                            136 CALL                     0
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_JUMP_FORWARD_IF_FALSE     1 (to 164)
                
-               143         162 JUMP_BACKWARD           35 (to 94)
+               133         162 JUMP_BACKWARD           35 (to 94)
                
-               145     >>  164 LOAD_GLOBAL              5 (NULL + any)
+               135     >>  164 LOAD_GLOBAL              5 (NULL + any)
                            176 LOAD_CLOSURE             4 (token)
                            178 BUILD_TUPLE              1
-                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 145>)
+                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 135>)
                            182 MAKE_FUNCTION            8 (closure)
                            184 LOAD_GLOBAL              8 (types_to_filter_after)
                            196 GET_ITER
                            198 PRECALL                  0
                            202 CALL                     0
                            212 PRECALL                  1
                            216 CALL                     1
                            226 POP_JUMP_FORWARD_IF_FALSE     1 (to 230)
                
-               146         228 JUMP_BACKWARD           68 (to 94)
+               136         228 JUMP_BACKWARD           68 (to 94)
                
-               148     >>  230 LOAD_DEREF               4 (token)
+               138     >>  230 LOAD_DEREF               4 (token)
                            232 LOAD_ATTR                5 (content)
-                           242 LOAD_GLOBAL             12 (empty_tokens)
-                           254 CONTAINS_OP              0
-                           256 POP_JUMP_FORWARD_IF_FALSE     1 (to 260)
-               
-               149         258 JUMP_BACKWARD           83 (to 94)
-               
-               151     >>  260 LOAD_FAST                3 (final)
-                           262 LOAD_METHOD              7 (append)
-                           284 LOAD_DEREF               4 (token)
-                           286 PRECALL                  1
-                           290 CALL                     1
-                           300 POP_TOP
-                           302 JUMP_BACKWARD          105 (to 94)
+                           242 LOAD_METHOD              6 (replace)
+                           264 LOAD_CONST               3 (' ')
+                           266 LOAD_CONST               4 ('')
+                           268 PRECALL                  2
+                           272 CALL                     2
+                           282 LOAD_GLOBAL             14 (empty_tokens)
+                           294 CONTAINS_OP              0
+                           296 POP_JUMP_FORWARD_IF_FALSE     1 (to 300)
+               
+               139         298 JUMP_BACKWARD          103 (to 94)
+               
+               141     >>  300 LOAD_FAST                3 (final)
+                           302 LOAD_METHOD              8 (append)
+                           324 LOAD_DEREF               4 (token)
+                           326 PRECALL                  1
+                           330 CALL                     1
+                           340 POP_TOP
+                           342 JUMP_BACKWARD          125 (to 94)
                
-               153     >>  304 LOAD_FAST                3 (final)
-                           306 RETURN_VALUE
+               143     >>  344 LOAD_FAST                3 (final)
+                           346 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     142           2 RETURN_GENERATOR
+                     132           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1135,27 +1121,27 @@
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
                      filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 142
+                     firstlineno 132
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     145           2 RETURN_GENERATOR
+                     135           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1171,230 +1157,320 @@
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
                      filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 145
+                     firstlineno 135
                      lnotab 0x
-               names      ('isinstance', 'OrderedSet', 'any', 'types_to_filter_before', 'types_to_filter_after', 'content', 'empty_tokens', 'append')
+                  ' '
+                  ''
+               names      ('isinstance', 'OrderedSet', 'any', 'types_to_filter_before', 'types_to_filter_after', 'content', 'replace', 'empty_tokens', 'append')
                varnames   ('self', 'tokens_all', 'tokens_to_be_excluded', 'final')
                freevars   ()
                cellvars   ('token',)
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'final_cleanup'
-               firstlineno 135
-               lnotab 0x04012a011e020a010401080140010202400102021c0102022c02
+               firstlineno 125
+               lnotab 0x04012a011e020a01040108014001020240010202440102022c02
             code
                argcount  : 1
-               nlocals   : 7
+               nlocals   : 10
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000007d017c006a02000000000000000080027c0153
                   00740700000000000000000000a6000000ab0000000000000000007d0267
-                  007d037409000000000000000000006a0500000000000000007c006a0200
-                  00000000000000a6010000ab0100000000000000007d047c0444005d357d
-                  057c03a00600000000000000000000000000000000000000007c05a00700
-                  000000000000000000000000000000000000007c006a0100000000000000
-                  007c006a080000000000000000a6020000ab020000000000000000a60100
-                  00ab01000000000000000001008c367c0344005d567d0674130000000000
-                  00000000007414000000000000000000006a0b00000000000000007c066a
-                  0c00000000000000006a0d00000000000000007c066a0e00000000000000
-                  006a0f0000000000000000ac01a6030000ab0300000000000000007c066a
-                  1000000000000000005f1100000000000000007c02a01200000000000000
-                  000000000000000000000000007c066a0c0000000000000000a6010000ab
-                  01000000000000000001008c577c025300
-               155           0 RESUME                   0
+                  007d0367007d047409000000000000000000006a0500000000000000007c
+                  006a020000000000000000a6010000ab0100000000000000007d05740d00
+                  0000000000000000006a0500000000000000007c006a0200000000000000
+                  00a6010000ab0100000000000000007d067c0544005d357d077c03a00700
+                  000000000000000000000000000000000000007c07a00800000000000000
+                  000000000000000000000000007c006a0100000000000000007c006a0900
+                  00000000000000a6020000ab020000000000000000a6010000ab01000000
+                  000000000001008c367c0644005d357d077c04a007000000000000000000
+                  00000000000000000000007c07a008000000000000000000000000000000
+                  00000000007c006a0100000000000000007c006a090000000000000000a6
+                  020000ab020000000000000000a6010000ab01000000000000000001008c
+                  367c0344005dab7d087c0444005d527d097c086a0a000000000000000064
+                  01190000000000000000007c096401190000000000000000006b05000000
+                  0072397c086a0a00000000000000006402190000000000000000007c0964
+                  02190000000000000000006b010000000072227c02a00b00000000000000
+                  000000000000000000000000007c086a0c00000000000000007c086a0d00
+                  000000000000006702a6010000ab01000000000000000001008c528c5374
+                  1d00000000000000000000741e000000000000000000006a100000000000
+                  0000007c086a0c00000000000000006a1100000000000000007c086a1200
+                  000000000000006a130000000000000000ac03a6030000ab030000000000
+                  0000007c086a0d00000000000000005f1400000000000000007c02a01500
+                  000000000000000000000000000000000000007c086a0c00000000000000
+                  00a6010000ab01000000000000000001008cac7c025300
+               145           0 RESUME                   0
                
-               156           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
+               146           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (tokens)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (tokens_all)
                
-               157          42 LOAD_FAST                0 (self)
+               147          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                2 (language)
                             54 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 60)
                
-               158          56 LOAD_FAST                1 (tokens_all)
+               148          56 LOAD_FAST                1 (tokens_all)
                             58 RETURN_VALUE
                
-               160     >>   60 LOAD_GLOBAL              7 (NULL + set)
+               150     >>   60 LOAD_GLOBAL              7 (NULL + set)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               2 (exclude_after)
                
-               162          88 BUILD_LIST               0
+               152          88 BUILD_LIST               0
                             90 STORE_FAST               3 (true_detections)
                
-               163          92 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
-                           104 LOAD_ATTR                5 (for_language)
-                           114 LOAD_FAST                0 (self)
-                           116 LOAD_ATTR                2 (language)
-                           126 PRECALL                  1
-                           130 CALL                     1
-                           140 STORE_FAST               4 (rules)
-               
-               164         142 LOAD_FAST                4 (rules)
-                           144 GET_ITER
-                       >>  146 FOR_ITER                53 (to 254)
-                           148 STORE_FAST               5 (rule)
-               
-               165         150 LOAD_FAST                3 (true_detections)
-                           152 LOAD_METHOD              6 (extend)
-                           174 LOAD_FAST                5 (rule)
-                           176 LOAD_METHOD              7 (match)
-                           198 LOAD_FAST                0 (self)
-                           200 LOAD_ATTR                1 (tokens)
-                           210 LOAD_FAST                0 (self)
-                           212 LOAD_ATTR                8 (token_stream)
-                           222 PRECALL                  2
-                           226 CALL                     2
-                           236 PRECALL                  1
-                           240 CALL                     1
-                           250 POP_TOP
-                           252 JUMP_BACKWARD           54 (to 146)
-               
-               167     >>  254 LOAD_FAST                3 (true_detections)
-                           256 GET_ITER
-                       >>  258 FOR_ITER                86 (to 432)
-                           260 STORE_FAST               6 (var)
-               
-               168         262 LOAD_GLOBAL             19 (NULL + Semantic)
-               
-               169         274 LOAD_GLOBAL             20 (SemanticType)
-                           286 LOAD_ATTR               11 (VAR)
-               
-               170         296 LOAD_FAST                6 (var)
-                           298 LOAD_ATTR               12 (name)
-                           308 LOAD_ATTR               13 (content)
-               
-               171         318 LOAD_FAST                6 (var)
-                           320 LOAD_ATTR               14 (found_by)
-                           330 LOAD_ATTR               15 (creds_probability)
-               
-               168         340 KW_NAMES                 1
-                           342 PRECALL                  3
-                           346 CALL                     3
-                           356 LOAD_FAST                6 (var)
-                           358 LOAD_ATTR               16 (value)
-                           368 STORE_ATTR              17 (semantic)
-               
-               173         378 LOAD_FAST                2 (exclude_after)
-                           380 LOAD_METHOD             18 (add)
-                           402 LOAD_FAST                6 (var)
-                           404 LOAD_ATTR               12 (name)
-                           414 PRECALL                  1
-                           418 CALL                     1
-                           428 POP_TOP
-                           430 JUMP_BACKWARD           87 (to 258)
+               153          92 BUILD_LIST               0
+                            94 STORE_FAST               4 (suppression_regions)
+               
+               155          96 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
+                           108 LOAD_ATTR                5 (for_language)
+                           118 LOAD_FAST                0 (self)
+                           120 LOAD_ATTR                2 (language)
+                           130 PRECALL                  1
+                           134 CALL                     1
+                           144 STORE_FAST               5 (detection_rules)
                
-               175     >>  432 LOAD_FAST                2 (exclude_after)
-                           434 RETURN_VALUE
+               156         146 LOAD_GLOBAL             13 (NULL + VariableSuppressionRules)
+                           158 LOAD_ATTR                5 (for_language)
+                           168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                2 (language)
+                           180 PRECALL                  1
+                           184 CALL                     1
+                           194 STORE_FAST               6 (suppression_rules)
+               
+               158         196 LOAD_FAST                5 (detection_rules)
+                           198 GET_ITER
+                       >>  200 FOR_ITER                53 (to 308)
+                           202 STORE_FAST               7 (rule)
+               
+               159         204 LOAD_FAST                3 (true_detections)
+                           206 LOAD_METHOD              7 (extend)
+                           228 LOAD_FAST                7 (rule)
+                           230 LOAD_METHOD              8 (match)
+                           252 LOAD_FAST                0 (self)
+                           254 LOAD_ATTR                1 (tokens)
+                           264 LOAD_FAST                0 (self)
+                           266 LOAD_ATTR                9 (token_stream)
+                           276 PRECALL                  2
+                           280 CALL                     2
+                           290 PRECALL                  1
+                           294 CALL                     1
+                           304 POP_TOP
+                           306 JUMP_BACKWARD           54 (to 200)
+               
+               161     >>  308 LOAD_FAST                6 (suppression_rules)
+                           310 GET_ITER
+                       >>  312 FOR_ITER                53 (to 420)
+                           314 STORE_FAST               7 (rule)
+               
+               162         316 LOAD_FAST                4 (suppression_regions)
+                           318 LOAD_METHOD              7 (extend)
+                           340 LOAD_FAST                7 (rule)
+                           342 LOAD_METHOD              8 (match)
+                           364 LOAD_FAST                0 (self)
+                           366 LOAD_ATTR                1 (tokens)
+                           376 LOAD_FAST                0 (self)
+                           378 LOAD_ATTR                9 (token_stream)
+                           388 PRECALL                  2
+                           392 CALL                     2
+                           402 PRECALL                  1
+                           406 CALL                     1
+                           416 POP_TOP
+                           418 JUMP_BACKWARD           54 (to 312)
+               
+               165     >>  420 LOAD_FAST                3 (true_detections)
+                           422 GET_ITER
+                       >>  424 FOR_ITER               171 (to 768)
+                           426 STORE_FAST               8 (var)
+               
+               166         428 LOAD_FAST                4 (suppression_regions)
+                           430 GET_ITER
+                       >>  432 FOR_ITER                82 (to 598)
+                           434 STORE_FAST               9 (reg)
+               
+               167         436 LOAD_FAST                8 (var)
+                           438 LOAD_ATTR               10 (span)
+                           448 LOAD_CONST               1 (0)
+                           450 BINARY_SUBSCR
+                           460 LOAD_FAST                9 (reg)
+                           462 LOAD_CONST               1 (0)
+                           464 BINARY_SUBSCR
+                           474 COMPARE_OP               5 (>=)
+                           480 POP_JUMP_FORWARD_IF_FALSE    57 (to 596)
+                           482 LOAD_FAST                8 (var)
+                           484 LOAD_ATTR               10 (span)
+                           494 LOAD_CONST               2 (1)
+                           496 BINARY_SUBSCR
+                           506 LOAD_FAST                9 (reg)
+                           508 LOAD_CONST               2 (1)
+                           510 BINARY_SUBSCR
+                           520 COMPARE_OP               1 (<=)
+                           526 POP_JUMP_FORWARD_IF_FALSE    34 (to 596)
+               
+               168         528 LOAD_FAST                2 (exclude_after)
+                           530 LOAD_METHOD             11 (update)
+                           552 LOAD_FAST                8 (var)
+                           554 LOAD_ATTR               12 (name)
+                           564 LOAD_FAST                8 (var)
+                           566 LOAD_ATTR               13 (value)
+                           576 BUILD_LIST               2
+                           578 PRECALL                  1
+                           582 CALL                     1
+                           592 POP_TOP
+               
+               169         594 JUMP_BACKWARD           82 (to 432)
+                       >>  596 JUMP_BACKWARD           83 (to 432)
+               
+               171     >>  598 LOAD_GLOBAL             29 (NULL + Semantic)
+               
+               172         610 LOAD_GLOBAL             30 (SemanticType)
+                           622 LOAD_ATTR               16 (VAR)
+               
+               173         632 LOAD_FAST                8 (var)
+                           634 LOAD_ATTR               12 (name)
+                           644 LOAD_ATTR               17 (content)
+               
+               174         654 LOAD_FAST                8 (var)
+                           656 LOAD_ATTR               18 (found_by)
+                           666 LOAD_ATTR               19 (creds_probability)
+               
+               171         676 KW_NAMES                 3
+                           678 PRECALL                  3
+                           682 CALL                     3
+                           692 LOAD_FAST                8 (var)
+                           694 LOAD_ATTR               13 (value)
+                           704 STORE_ATTR              20 (semantic)
+               
+               176         714 LOAD_FAST                2 (exclude_after)
+                           716 LOAD_METHOD             21 (add)
+                           738 LOAD_FAST                8 (var)
+                           740 LOAD_ATTR               12 (name)
+                           750 PRECALL                  1
+                           754 CALL                     1
+                           764 POP_TOP
+                           766 JUMP_BACKWARD          172 (to 424)
+               
+               178     >>  768 LOAD_FAST                2 (exclude_after)
+                           770 RETURN_VALUE
                consts
                   None
+                  0
+                  1
                   ('type', 'name', 'creds_probability')
-               names      ('OrderedSet', 'tokens', 'language', 'set', 'VariableDetectionRules', 'for_language', 'extend', 'match', 'token_stream', 'Semantic', 'SemanticType', 'VAR', 'name', 'content', 'found_by', 'creds_probability', 'value', 'semantic', 'add')
-               varnames   ('self', 'tokens_all', 'exclude_after', 'true_detections', 'rules', 'rule', 'var')
+               names      ('OrderedSet', 'tokens', 'language', 'set', 'VariableDetectionRules', 'for_language', 'VariableSuppressionRules', 'extend', 'match', 'token_stream', 'span', 'update', 'name', 'value', 'Semantic', 'SemanticType', 'VAR', 'content', 'found_by', 'creds_probability', 'semantic', 'add')
+               varnames   ('self', 'tokens_all', 'exclude_after', 'true_detections', 'suppression_regions', 'detection_rules', 'suppression_rules', 'rule', 'var', 'reg')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'deep_analyze'
-               firstlineno 155
+               firstlineno 145
                lnotab
-                  0x020128010e0104021c02040132010801680208010c011601160116fd26
-                  053602
+                  0x020128010e0104021c0204010402320132020801680208016803080108
+                  015c01420104020c011601160116fd26053602
             code
-               argcount  : 1
-               nlocals   : 3
+               argcount  : 2
+               nlocals   : 4
                stacksize : 4
                flags     : 3
                code
-                  0x970067007d017401000000000000000000007c006a0100000000000000
-                  00a6010000ab01000000000000000064016b02000000007202670053007c
-                  006a01000000000000000044005d3a7d027c026a02000000000000000080
-                  018c0a7c026a0200000000000000006a0300000000000000007408000000
-                  000000000000006a0500000000000000006b030000000072018c257c01a0
-                  0600000000000000000000000000000000000000007c02a6010000ab0100
-                  0000000000000001008c3b7c015300
-               177           0 RESUME                   0
-               
-               178           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (vars)
-               
-               179           6 LOAD_GLOBAL              1 (NULL + len)
-                            18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (tokens)
-                            30 PRECALL                  1
-                            34 CALL                     1
-                            44 LOAD_CONST               1 (0)
-                            46 COMPARE_OP               2 (==)
-                            52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
-               
-               180          54 BUILD_LIST               0
-                            56 RETURN_VALUE
-               
-               182     >>   58 LOAD_FAST                0 (self)
-                            60 LOAD_ATTR                1 (tokens)
-                            70 GET_ITER
-                       >>   72 FOR_ITER                58 (to 190)
-                            74 STORE_FAST               2 (token)
-               
-               183          76 LOAD_FAST                2 (token)
-                            78 LOAD_ATTR                2 (semantic)
-                            88 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 92)
-               
-               184          90 JUMP_BACKWARD           10 (to 72)
-               
-               186     >>   92 LOAD_FAST                2 (token)
-                            94 LOAD_ATTR                2 (semantic)
-                           104 LOAD_ATTR                3 (type)
-                           114 LOAD_GLOBAL              8 (SemanticType)
-                           126 LOAD_ATTR                5 (VAR)
-                           136 COMPARE_OP               3 (!=)
-                           142 POP_JUMP_FORWARD_IF_FALSE     1 (to 146)
-               
-               187         144 JUMP_BACKWARD           37 (to 72)
-               
-               189     >>  146 LOAD_FAST                1 (vars)
-                           148 LOAD_METHOD              6 (append)
-                           170 LOAD_FAST                2 (token)
-                           172 PRECALL                  1
-                           176 CALL                     1
-                           186 POP_TOP
-                           188 JUMP_BACKWARD           59 (to 72)
+                  0x97007c0181027c016e067c006a0000000000000000007d0167007d0274
+                  03000000000000000000007c01a6010000ab01000000000000000064016b
+                  02000000007202670053007c0144005d3a7d037c036a0200000000000000
+                  0080018c0a7c036a0200000000000000006a030000000000000000740800
+                  0000000000000000006a0500000000000000006b030000000072018c257c
+                  02a00600000000000000000000000000000000000000007c03a6010000ab
+                  01000000000000000001008c3b7c025300
+               180           0 RESUME                   0
+               
+               181           2 LOAD_FAST                1 (tokens)
+                             4 POP_JUMP_FORWARD_IF_NONE     2 (to 10)
+                             6 LOAD_FAST                1 (tokens)
+                             8 JUMP_FORWARD             6 (to 22)
+                       >>   10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (tokens)
+                       >>   22 STORE_FAST               1 (tokens)
+               
+               182          24 BUILD_LIST               0
+                            26 STORE_FAST               2 (vars)
+               
+               183          28 LOAD_GLOBAL              3 (NULL + len)
+                            40 LOAD_FAST                1 (tokens)
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 LOAD_CONST               1 (0)
+                            58 COMPARE_OP               2 (==)
+                            64 POP_JUMP_FORWARD_IF_FALSE     2 (to 70)
+               
+               184          66 BUILD_LIST               0
+                            68 RETURN_VALUE
+               
+               186     >>   70 LOAD_FAST                1 (tokens)
+                            72 GET_ITER
+                       >>   74 FOR_ITER                58 (to 192)
+                            76 STORE_FAST               3 (token)
+               
+               187          78 LOAD_FAST                3 (token)
+                            80 LOAD_ATTR                2 (semantic)
+                            90 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 94)
+               
+               188          92 JUMP_BACKWARD           10 (to 74)
+               
+               190     >>   94 LOAD_FAST                3 (token)
+                            96 LOAD_ATTR                2 (semantic)
+                           106 LOAD_ATTR                3 (type)
+                           116 LOAD_GLOBAL              8 (SemanticType)
+                           128 LOAD_ATTR                5 (VAR)
+                           138 COMPARE_OP               3 (!=)
+                           144 POP_JUMP_FORWARD_IF_FALSE     1 (to 148)
+               
+               191         146 JUMP_BACKWARD           37 (to 74)
+               
+               193     >>  148 LOAD_FAST                2 (vars)
+                           150 LOAD_METHOD              6 (append)
+                           172 LOAD_FAST                3 (token)
+                           174 PRECALL                  1
+                           178 CALL                     1
+                           188 POP_TOP
+                           190 JUMP_BACKWARD           59 (to 74)
                
-               191     >>  190 LOAD_FAST                1 (vars)
-                           192 RETURN_VALUE
+               195     >>  192 LOAD_FAST                2 (vars)
+                           194 RETURN_VALUE
                consts
                   None
                   0
-               names      ('len', 'tokens', 'semantic', 'type', 'SemanticType', 'VAR', 'append')
-               varnames   ('self', 'vars', 'token')
+               names      ('tokens', 'len', 'semantic', 'type', 'SemanticType', 'VAR', 'append')
+               varnames   ('self', 'tokens', 'vars', 'token')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'get_variables'
-               firstlineno 177
-               lnotab 0x020104013001040212010e010202340102022c02
+               firstlineno 180
+               lnotab 0x0201160104012601040208010e010202340102022c02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab010000000000000000010064005300
-               193           0 RESUME                   0
+               197           0 RESUME                   0
                
-               194           2 LOAD_GLOBAL              1 (NULL + print)
+               198           2 LOAD_GLOBAL              1 (NULL + print)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (token_stream)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
@@ -1402,31 +1478,32 @@
                   None
                names      ('print', 'token_stream')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'print_token_type_stream'
-               firstlineno 193
+               firstlineno 197
                lnotab 0x0201
             (True,)
+            (None,)
             ('return', None)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'Union', 'bool', 'sanitize', 'File', '_find_lexer_for_file', 'Token', 'tokenize', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'Set', 'deep_analyze', 'get_variables', 'print_token_type_stream')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'Union', 'bool', 'sanitize', 'File', '_find_lexer_for_file', 'Token', 'tokenize', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'Set', 'deep_analyze', 'Optional', 'get_variables', 'print_token_type_stream')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/lexer.py'
          name       'LexerTokenizer'
-         firstlineno 27
-         lnotab 0x0c010a010a010a021c0a20150c141e301c04381418161810
+         firstlineno 28
+         lnotab 0x0c010a010a010a021c0a20150c071e321c04381418233611
       'LexerTokenizer'
       None
-   names      ('typing', 'List', 'Sequence', 'Set', 'Type', 'Union', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers', 'get_lexer_for_filename', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'pygments.util', 'ClassNotFound', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules', 'VariableDetectionRules', 'deepsecrets.core.tokenizers.helpers.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.helpers.type_stream', 'token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'empty_tokens', 'LexerTokenizer')
+   names      ('typing', 'List', 'Optional', 'Sequence', 'Set', 'Type', 'Union', 'deepsecrets', 'logger', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules', 'VariableDetectionRules', 'VariableSuppressionRules', 'deepsecrets.core.tokenizers.helpers.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.helpers.type_stream', 'token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'deepsecrets.core.utils.lexer_finder', 'LexerFinder', 'empty_tokens', 'LexerTokenizer')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/lexer.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02011c020c010c010c010c0110010c010c020c010c0114010c010c
-      010c0114050c020803
+      0x00ff020120020c020c010c010c0110010c020c010c0114010c0110010c
+      0114050c010c020803
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x65a04264 (Fri Apr 21 14:40:37 2023 UTC)
+moddate:  0x116e9c64 (Wed Jun 28 17:29:53 2023 UTC)
 files sz: 1801
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,41 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0xc4f83764 (Thu Apr 13 12:42:44 2023 UTC)
-files sz: 529
+moddate:  0x7f789c64 (Wed Jun 28 18:14:23 2023 UTC)
+files sz: 556
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
       00ab0300000000000000005a0264045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Enum',))
-                 6 IMPORT_NAME              0 (enum)
-                 8 IMPORT_FROM              1 (Enum)
-                10 STORE_NAME               1 (Enum)
+                 4 LOAD_CONST               1 (('MultiValueEnum',))
+                 6 IMPORT_NAME              0 (aenum)
+                 8 IMPORT_FROM              1 (MultiValueEnum)
+                10 STORE_NAME               1 (MultiValueEnum)
                 12 POP_TOP
    
      4          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
                 18 LOAD_CONST               2 (<code object Language, file "/app/deepsecrets/core/tokenizers/helpers/semantic/language.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('Language')
-                24 LOAD_NAME                1 (Enum)
+                24 LOAD_NAME                1 (MultiValueEnum)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (Language)
                 42 LOAD_CONST               4 (None)
                 44 RETURN_VALUE
    consts
       0
-      ('Enum',)
+      ('MultiValueEnum',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
@@ -54,15 +54,15 @@
          
            6          14 LOAD_CONST               2 ('go')
                       16 STORE_NAME               4 (GOLANG)
          
            7          18 LOAD_CONST               3 ('php')
                       20 STORE_NAME               5 (PHP)
          
-           8          22 LOAD_CONST               4 ('js')
+           8          22 LOAD_CONST               4 (('js', 'jsx'))
                       24 STORE_NAME               6 (JS)
          
            9          26 LOAD_CONST               5 ('toml')
                       28 STORE_NAME               7 (TOML)
          
           10          30 LOAD_CONST               6 ('json')
                       32 STORE_NAME               8 (JSON)
@@ -126,15 +126,15 @@
                      134 LOAD_CONST              21 (None)
                      136 RETURN_VALUE
          consts
             'Language'
             'py'
             'go'
             'php'
-            'js'
+            ('js', 'jsx')
             'toml'
             'json'
             'yaml'
             'ini'
             'pp'
             'sh'
             'cs'
@@ -213,15 +213,15 @@
          name       'Language'
          firstlineno 4
          lnotab
             0x0a01040104010401040104010401040104010401040104010401040204
             01040202010eff0e01020402010eff0e01
       'Language'
       None
-   names      ('enum', 'Enum', 'Language')
+   names      ('aenum', 'MultiValueEnum', 'Language')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/language.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c03
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,792 +1,796 @@
 magic:    0xa70d0d0a
-moddate:  0x534e3964 (Fri Apr 14 13:00:03 2023 UTC)
-files sz: 2711
+moddate:  0xe0eca364 (Tue Jul  4 09:56:48 2023 UTC)
+files sz: 3022
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a01640064026c026d035a036d045a046d055a0501
-      00640064036c066d075a076d085a086d095a090100640064046c0a6d0b5a
-      0b0100640064056c0c6d0d5a0d0100020047006406840064076507a60300
-      00ab0300000000000000005a0e020047006408840064096507a6030000ab
-      0300000000000000005a0f6400640a6c106d115a11010064015300
+      0x9700640064016c006d015a010100640064026c026d035a030100640064
+      036c046d055a056d065a066d075a076d085a080100640064046c096d0a5a
+      0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064
+      076c0f6d105a100100640064086c116d125a120100640064096c136d145a
+      1401006400640a6c156d165a16010002004700640b8400640c650aa60300
+      00ab0300000000000000005a1702004700640d8400640ea6020000ab0200
+      000000000000005a18640f5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (regex)
-                 8 STORE_NAME               1 (re)
-   
-     2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Dict', 'List', 'Optional'))
-                14 IMPORT_NAME              2 (typing)
-                16 IMPORT_FROM              3 (Dict)
-                18 STORE_NAME               3 (Dict)
-                20 IMPORT_FROM              4 (List)
-                22 STORE_NAME               4 (List)
-                24 IMPORT_FROM              5 (Optional)
-                26 STORE_NAME               5 (Optional)
-                28 POP_TOP
-   
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('BaseModel', 'Field', 'validator'))
-                34 IMPORT_NAME              6 (pydantic)
-                36 IMPORT_FROM              7 (BaseModel)
-                38 STORE_NAME               7 (BaseModel)
-                40 IMPORT_FROM              8 (Field)
-                42 STORE_NAME               8 (Field)
-                44 IMPORT_FROM              9 (validator)
-                46 STORE_NAME               9 (validator)
+                 4 LOAD_CONST               1 (('RLock',))
+                 6 IMPORT_NAME              0 (multiprocessing)
+                 8 IMPORT_FROM              1 (RLock)
+                10 STORE_NAME               1 (RLock)
+                12 POP_TOP
+   
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('Pool',))
+                18 IMPORT_NAME              2 (multiprocessing.pool)
+                20 IMPORT_FROM              3 (Pool)
+                22 STORE_NAME               3 (Pool)
+                24 POP_TOP
+   
+     3          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('Dict', 'List', 'Optional', 'Type'))
+                30 IMPORT_NAME              4 (typing)
+                32 IMPORT_FROM              5 (Dict)
+                34 STORE_NAME               5 (Dict)
+                36 IMPORT_FROM              6 (List)
+                38 STORE_NAME               6 (List)
+                40 IMPORT_FROM              7 (Optional)
+                42 STORE_NAME               7 (Optional)
+                44 IMPORT_FROM              8 (Type)
+                46 STORE_NAME               8 (Type)
                 48 POP_TOP
    
-     6          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('Token',))
-                54 IMPORT_NAME             10 (deepsecrets.core.model.token)
-                56 IMPORT_FROM             11 (Token)
-                58 STORE_NAME              11 (Token)
+     5          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               4 (('BaseModel',))
+                54 IMPORT_NAME              9 (pydantic)
+                56 IMPORT_FROM             10 (BaseModel)
+                58 STORE_NAME              10 (BaseModel)
                 60 POP_TOP
    
      7          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('Language',))
-                66 IMPORT_NAME             12 (deepsecrets.core.tokenizers.helpers.semantic.language)
-                68 IMPORT_FROM             13 (Language)
-                70 STORE_NAME              13 (Language)
+                64 LOAD_CONST               5 (('logger',))
+                66 IMPORT_NAME             11 (deepsecrets)
+                68 IMPORT_FROM             12 (logger)
+                70 STORE_NAME              12 (logger)
                 72 POP_TOP
    
-    10          74 PUSH_NULL
-                76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               6 (<code object Match, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 10>)
-                80 MAKE_FUNCTION            0
-                82 LOAD_CONST               7 ('Match')
-                84 LOAD_NAME                7 (BaseModel)
-                86 PRECALL                  3
-                90 CALL                     3
-               100 STORE_NAME              14 (Match)
-   
-    53         102 PUSH_NULL
-               104 LOAD_BUILD_CLASS
-               106 LOAD_CONST               8 (<code object VaribleDetector, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 53>)
-               108 MAKE_FUNCTION            0
-               110 LOAD_CONST               9 ('VaribleDetector')
-               112 LOAD_NAME                7 (BaseModel)
-               114 PRECALL                  3
-               118 CALL                     3
-               128 STORE_NAME              15 (VaribleDetector)
-   
-    90         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (('Variable',))
-               134 IMPORT_NAME             16 (deepsecrets.core.model.semantic)
-               136 IMPORT_FROM             17 (Variable)
-               138 STORE_NAME              17 (Variable)
-               140 POP_TOP
-               142 LOAD_CONST               1 (None)
-               144 RETURN_VALUE
+     8          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               6 (('IEngine',))
+                78 IMPORT_NAME             13 (deepsecrets.core.engines.iengine)
+                80 IMPORT_FROM             14 (IEngine)
+                82 STORE_NAME              14 (IEngine)
+                84 POP_TOP
+   
+     9          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               7 (('File',))
+                90 IMPORT_NAME             15 (deepsecrets.core.model.file)
+                92 IMPORT_FROM             16 (File)
+                94 STORE_NAME              16 (File)
+                96 POP_TOP
+   
+    10          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               8 (('Finding',))
+               102 IMPORT_NAME             17 (deepsecrets.core.model.finding)
+               104 IMPORT_FROM             18 (Finding)
+               106 STORE_NAME              18 (Finding)
+               108 POP_TOP
+   
+    11         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               9 (('Token',))
+               114 IMPORT_NAME             19 (deepsecrets.core.model.token)
+               116 IMPORT_FROM             20 (Token)
+               118 STORE_NAME              20 (Token)
+               120 POP_TOP
+   
+    12         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST              10 (('Tokenizer',))
+               126 IMPORT_NAME             21 (deepsecrets.core.tokenizers.itokenizer)
+               128 IMPORT_FROM             22 (Tokenizer)
+               130 STORE_NAME              22 (Tokenizer)
+               132 POP_TOP
+   
+    15         134 PUSH_NULL
+               136 LOAD_BUILD_CLASS
+               138 LOAD_CONST              11 (<code object EngineWithTokenizer, file "/app/deepsecrets/core/utils/file_analyzer.py", line 15>)
+               140 MAKE_FUNCTION            0
+               142 LOAD_CONST              12 ('EngineWithTokenizer')
+               144 LOAD_NAME               10 (BaseModel)
+               146 PRECALL                  3
+               150 CALL                     3
+               160 STORE_NAME              23 (EngineWithTokenizer)
+   
+    23         162 PUSH_NULL
+               164 LOAD_BUILD_CLASS
+               166 LOAD_CONST              13 (<code object FileAnalyzer, file "/app/deepsecrets/core/utils/file_analyzer.py", line 23>)
+               168 MAKE_FUNCTION            0
+               170 LOAD_CONST              14 ('FileAnalyzer')
+               172 PRECALL                  2
+               176 CALL                     2
+               186 STORE_NAME              24 (FileAnalyzer)
+               188 LOAD_CONST              15 (None)
+               190 RETURN_VALUE
    consts
       0
-      None
-      ('Dict', 'List', 'Optional')
-      ('BaseModel', 'Field', 'validator')
+      ('RLock',)
+      ('Pool',)
+      ('Dict', 'List', 'Optional', 'Type')
+      ('BaseModel',)
+      ('logger',)
+      ('IEngine',)
+      ('File',)
+      ('Finding',)
       ('Token',)
-      ('Language',)
+      ('Tokenizer',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 6
+         stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a025500020065036504ac01a6010000ab01000000
-            00000000005a05650665076a080000000000000000190000000000000000
-            00650964023c000000020065036504ac01a6010000ab0100000000000000
-            005a0a650665076a08000000000000000019000000000000000000650964
-            033c00000064046506650b190000000000000000006405650c6604640684
-            045a0d0200650e640264036407ac08a6030000ab03000000000000000064
-            02650f6405650665076a0800000000000000001900000000000000000066
-            0464098404a6000000ab0000000000000000005a1002004700640a840064
-            0ba6020000ab0200000000000000005a11640c5300
-          10           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c0000006505650464023c
+            00000002004700640384006404a6020000ab0200000000000000005a0664
+            055300
+          15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('Match')
+                       6 LOAD_CONST               0 ('EngineWithTokenizer')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          11          12 PUSH_NULL
-                      14 LOAD_NAME                3 (Field)
-                      16 LOAD_NAME                4 (list)
-                      18 KW_NAMES                 1
-                      20 PRECALL                  1
-                      24 CALL                     1
-                      34 STORE_NAME               5 (values)
-                      36 LOAD_NAME                6 (List)
-                      38 LOAD_NAME                7 (re)
-                      40 LOAD_ATTR                8 (Pattern)
-                      50 BINARY_SUBSCR
-                      60 LOAD_NAME                9 (__annotations__)
-                      62 LOAD_CONST               2 ('values')
-                      64 STORE_SUBSCR
-         
-          12          68 PUSH_NULL
-                      70 LOAD_NAME                3 (Field)
-                      72 LOAD_NAME                4 (list)
-                      74 KW_NAMES                 1
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 STORE_NAME              10 (not_values)
-                      92 LOAD_NAME                6 (List)
-                      94 LOAD_NAME                7 (re)
-                      96 LOAD_ATTR                8 (Pattern)
-                     106 BINARY_SUBSCR
-                     116 LOAD_NAME                9 (__annotations__)
-                     118 LOAD_CONST               3 ('not_values')
-                     120 STORE_SUBSCR
-         
-          14         124 LOAD_CONST               4 ('tokens')
-                     126 LOAD_NAME                6 (List)
-                     128 LOAD_NAME               11 (Token)
-                     130 BINARY_SUBSCR
-                     140 LOAD_CONST               5 ('return')
-                     142 LOAD_NAME               12 (bool)
-                     144 BUILD_TUPLE              4
-                     146 LOAD_CONST               6 (<code object check, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 14>)
-                     148 MAKE_FUNCTION            4 (annotations)
-                     150 STORE_NAME              13 (check)
-         
-          31         152 PUSH_NULL
-                     154 LOAD_NAME               14 (validator)
-                     156 LOAD_CONST               2 ('values')
-                     158 LOAD_CONST               3 ('not_values')
-                     160 LOAD_CONST               7 (True)
-                     162 KW_NAMES                 8
-                     164 PRECALL                  3
-                     168 CALL                     3
-         
-          32         178 LOAD_CONST               2 ('values')
-                     180 LOAD_NAME               15 (Dict)
-                     182 LOAD_CONST               5 ('return')
-                     184 LOAD_NAME                6 (List)
-                     186 LOAD_NAME                7 (re)
-                     188 LOAD_ATTR                8 (Pattern)
-                     198 BINARY_SUBSCR
-                     208 BUILD_TUPLE              4
-                     210 LOAD_CONST               9 (<code object regexify_values, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 31>)
-                     212 MAKE_FUNCTION            4 (annotations)
-         
-          31         214 PRECALL                  0
-                     218 CALL                     0
-         
-          32         228 STORE_NAME              16 (regexify_values)
-         
-          49         230 PUSH_NULL
-                     232 LOAD_BUILD_CLASS
-                     234 LOAD_CONST              10 (<code object Config, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 49>)
-                     236 MAKE_FUNCTION            0
-                     238 LOAD_CONST              11 ('Config')
-                     240 PRECALL                  2
-                     244 CALL                     2
-                     254 STORE_NAME              17 (Config)
-                     256 LOAD_CONST              12 (None)
-                     258 RETURN_VALUE
+          16          12 LOAD_NAME                3 (IEngine)
+                      14 LOAD_NAME                4 (__annotations__)
+                      16 LOAD_CONST               1 ('engine')
+                      18 STORE_SUBSCR
+         
+          17          22 LOAD_NAME                5 (Tokenizer)
+                      24 LOAD_NAME                4 (__annotations__)
+                      26 LOAD_CONST               2 ('tokenizer')
+                      28 STORE_SUBSCR
+         
+          19          32 PUSH_NULL
+                      34 LOAD_BUILD_CLASS
+                      36 LOAD_CONST               3 (<code object Config, file "/app/deepsecrets/core/utils/file_analyzer.py", line 19>)
+                      38 MAKE_FUNCTION            0
+                      40 LOAD_CONST               4 ('Config')
+                      42 PRECALL                  2
+                      46 CALL                     2
+                      56 STORE_NAME               6 (Config)
+                      58 LOAD_CONST               5 (None)
+                      60 RETURN_VALUE
          consts
-            'Match'
-            ('default_factory',)
-            'values'
-            'not_values'
-            'tokens'
-            'return'
-            code
-               argcount  : 2
-               nlocals   : 5
-               stacksize : 6
-               flags     : 3
-               code
-                  0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab01000000000000000064016b0400000000723164027d027c0144005d
-                  287d037c006a01000000000000000044005d1e7d04740500000000000000
-                  0000006a0300000000000000007c047c036a040000000000000000a60200
-                  00ab020000000000000000810264037d028c1f8c297c0273026402530074
-                  01000000000000000000007c006a050000000000000000a6010000ab0100
-                  0000000000000064016b0400000000722d7c0144005d2a7d037c006a0500
-                  0000000000000044005d207d047405000000000000000000006a03000000
-                  00000000007c047c036a040000000000000000a6020000ab020000000000
-                  000000810401000100640253008c218c2b64035300
-                14           0 RESUME                   0
-               
-                15           2 LOAD_GLOBAL              1 (NULL + len)
-                            14 LOAD_FAST                0 (self)
-                            16 LOAD_ATTR                1 (values)
-                            26 PRECALL                  1
-                            30 CALL                     1
-                            40 LOAD_CONST               1 (0)
-                            42 COMPARE_OP               4 (>)
-                            48 POP_JUMP_FORWARD_IF_FALSE    49 (to 148)
-               
-                16          50 LOAD_CONST               2 (False)
-                            52 STORE_FAST               2 (matched)
-               
-                17          54 LOAD_FAST                1 (tokens)
-                            56 GET_ITER
-                       >>   58 FOR_ITER                40 (to 140)
-                            60 STORE_FAST               3 (token)
-               
-                18          62 LOAD_FAST                0 (self)
-                            64 LOAD_ATTR                1 (values)
-                            74 GET_ITER
-                       >>   76 FOR_ITER                30 (to 138)
-                            78 STORE_FAST               4 (pattern)
-               
-                19          80 LOAD_GLOBAL              5 (NULL + re)
-                            92 LOAD_ATTR                3 (match)
-                           102 LOAD_FAST                4 (pattern)
-                           104 LOAD_FAST                3 (token)
-                           106 LOAD_ATTR                4 (content)
-                           116 PRECALL                  2
-                           120 CALL                     2
-                           130 POP_JUMP_FORWARD_IF_NONE     2 (to 136)
-               
-                20         132 LOAD_CONST               3 (True)
-                           134 STORE_FAST               2 (matched)
-                       >>  136 JUMP_BACKWARD           31 (to 76)
-               
-                18     >>  138 JUMP_BACKWARD           41 (to 58)
-               
-                21     >>  140 LOAD_FAST                2 (matched)
-                           142 POP_JUMP_FORWARD_IF_TRUE     2 (to 148)
-               
-                22         144 LOAD_CONST               2 (False)
-                           146 RETURN_VALUE
-               
-                24     >>  148 LOAD_GLOBAL              1 (NULL + len)
-                           160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                5 (not_values)
-                           172 PRECALL                  1
-                           176 CALL                     1
-                           186 LOAD_CONST               1 (0)
-                           188 COMPARE_OP               4 (>)
-                           194 POP_JUMP_FORWARD_IF_FALSE    45 (to 286)
-               
-                25         196 LOAD_FAST                1 (tokens)
-                           198 GET_ITER
-                       >>  200 FOR_ITER                42 (to 286)
-                           202 STORE_FAST               3 (token)
-               
-                26         204 LOAD_FAST                0 (self)
-                           206 LOAD_ATTR                5 (not_values)
-                           216 GET_ITER
-                       >>  218 FOR_ITER                32 (to 284)
-                           220 STORE_FAST               4 (pattern)
-               
-                27         222 LOAD_GLOBAL              5 (NULL + re)
-                           234 LOAD_ATTR                3 (match)
-                           244 LOAD_FAST                4 (pattern)
-                           246 LOAD_FAST                3 (token)
-                           248 LOAD_ATTR                4 (content)
-                           258 PRECALL                  2
-                           262 CALL                     2
-                           272 POP_JUMP_FORWARD_IF_NONE     4 (to 282)
-               
-                28         274 POP_TOP
-                           276 POP_TOP
-                           278 LOAD_CONST               2 (False)
-                           280 RETURN_VALUE
-               
-                27     >>  282 JUMP_BACKWARD           33 (to 218)
-               
-                26     >>  284 JUMP_BACKWARD           43 (to 200)
-               
-                29     >>  286 LOAD_CONST               3 (True)
-                           288 RETURN_VALUE
-               consts
-                  None
-                  0
-                  False
-                  True
-               names      ('len', 'values', 're', 'match', 'content', 'not_values')
-               varnames   ('self', 'tokens', 'matched', 'token', 'pattern')
-               freevars   ()
-               cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-               name       'check'
-               firstlineno 14
-               lnotab
-                  0x02013001040108011201340106fe020304010402300108011201340108
-                  ff02ff0203
-            True
-            ('pre',)
-            code
-               argcount  : 2
-               nlocals   : 4
-               stacksize : 8
-               flags     : 3
-               code
-                  0x97007c0180027c0153007401000000000000000000007c017402000000
-                  00000000000000a6020000ab020000000000000000730f74050000000000
-                  00000000006401a6010000ab010000000000000000820167007d027c0144
-                  005d767d037401000000000000000000007c037406000000000000000000
-                  006a040000000000000000a6020000ab02000000000000000072167c02a0
-                  0500000000000000000000000000000000000000007c03a6010000ab0100
-                  0000000000000001008c327c02a005000000000000000000000000000000
-                  00000000007407000000000000000000006a060000000000000000740700
-                  0000000000000000006a0700000000000000007c03a6010000ab01000000
-                  00000000007406000000000000000000006a080000000000000000a60200
-                  00ab020000000000000000a6010000ab01000000000000000001008c777c
-                  025300
-                31           0 RESUME                   0
-               
-                33           2 LOAD_FAST                1 (values)
-                             4 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 10)
-               
-                34           6 LOAD_FAST                1 (values)
-                             8 RETURN_VALUE
-               
-                36     >>   10 LOAD_GLOBAL              1 (NULL + isinstance)
-                            22 LOAD_FAST                1 (values)
-                            24 LOAD_GLOBAL              2 (list)
-                            36 PRECALL                  2
-                            40 CALL                     2
-                            50 POP_JUMP_FORWARD_IF_TRUE    15 (to 82)
-               
-                37          52 LOAD_GLOBAL              5 (NULL + Exception)
-                            64 LOAD_CONST               1 ('value must be an array')
-                            66 PRECALL                  1
-                            70 CALL                     1
-                            80 RAISE_VARARGS            1
-               
-                39     >>   82 BUILD_LIST               0
-                            84 STORE_FAST               2 (patterns)
-               
-                40          86 LOAD_FAST                1 (values)
-                            88 GET_ITER
-                       >>   90 FOR_ITER               118 (to 328)
-                            92 STORE_FAST               3 (val)
-               
-                41          94 LOAD_GLOBAL              1 (NULL + isinstance)
-                           106 LOAD_FAST                3 (val)
-                           108 LOAD_GLOBAL              6 (re)
-                           120 LOAD_ATTR                4 (Pattern)
-                           130 PRECALL                  2
-                           134 CALL                     2
-                           144 POP_JUMP_FORWARD_IF_FALSE    22 (to 190)
-               
-                42         146 LOAD_FAST                2 (patterns)
-                           148 LOAD_METHOD              5 (append)
-                           170 LOAD_FAST                3 (val)
-                           172 PRECALL                  1
-                           176 CALL                     1
-                           186 POP_TOP
-               
-                43         188 JUMP_BACKWARD           50 (to 90)
-               
-                45     >>  190 LOAD_FAST                2 (patterns)
-                           192 LOAD_METHOD              5 (append)
-                           214 LOAD_GLOBAL              7 (NULL + re)
-                           226 LOAD_ATTR                6 (compile)
-                           236 LOAD_GLOBAL              7 (NULL + re)
-                           248 LOAD_ATTR                7 (escape)
-                           258 LOAD_FAST                3 (val)
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 LOAD_GLOBAL              6 (re)
-                           286 LOAD_ATTR                8 (IGNORECASE)
-                           296 PRECALL                  2
-                           300 CALL                     2
-                           310 PRECALL                  1
-                           314 CALL                     1
-                           324 POP_TOP
-                           326 JUMP_BACKWARD          119 (to 90)
-               
-                47     >>  328 LOAD_FAST                2 (patterns)
-                           330 RETURN_VALUE
-               consts
-                  None
-                  'value must be an array'
-               names      ('isinstance', 'list', 'Exception', 're', 'Pattern', 'append', 'compile', 'escape', 'IGNORECASE')
-               varnames   ('cls', 'values', 'patterns', 'val')
-               freevars   ()
-               cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-               name       'regexify_values'
-               firstlineno 31
-               lnotab 0x0202040104022a011e020401080134012a0102028a02
+            'EngineWithTokenizer'
+            'engine'
+            'tokenizer'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-                49           0 RESUME                   0
+                19           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('Match.Config')
+                             6 LOAD_CONST               0 ('EngineWithTokenizer.Config')
                              8 STORE_NAME               2 (__qualname__)
                
-                50          10 LOAD_CONST               1 (True)
+                20          10 LOAD_CONST               1 (True)
                             12 STORE_NAME               3 (arbitrary_types_allowed)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
-                  'Match.Config'
+                  'EngineWithTokenizer.Config'
                   True
                   None
                names      ('__name__', '__module__', '__qualname__', 'arbitrary_types_allowed')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
+               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
                name       'Config'
-               firstlineno 49
+               firstlineno 19
                lnotab 0x0a01
             'Config'
             None
-         names      ('__name__', '__module__', '__qualname__', 'Field', 'list', 'values', 'List', 're', 'Pattern', '__annotations__', 'not_values', 'Token', 'bool', 'check', 'validator', 'Dict', 'regexify_values', 'Config')
+         names      ('__name__', '__module__', '__qualname__', 'IEngine', '__annotations__', 'Tokenizer', 'Config')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-         name       'Match'
-         firstlineno 10
-         lnotab 0x0c01380138021c111a0124ff0e010211
-      'Match'
+         filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+         name       'EngineWithTokenizer'
+         firstlineno 15
+         lnotab 0x0c010a010a02
+      'EngineWithTokenizer'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 7
+         stacksize : 6
          flags     : 0
          code
-            0x970065005a0164005a02550064015a0365046505190000000000000000
-            00650664023c00000065076a080000000000000000650664033c00000065
-            09650a650b660219000000000000000000650664043c0000006509650a65
-            0c660219000000000000000000650664053c00000064065a0d650a650664
-            073c00000002004700640884006409a6020000ab0200000000000000005a
-            0e640a650f651019000000000000000000640b650c640c650f640d190000
-            000000000000006606640e84045a11640f65076a0b000000000000000064
-            0a650f651019000000000000000000640c65126606641084045a13640153
-            00
-          53           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c00000065056506190000
+            00000000000000650464023c000000650765086505650919000000000000
+            000000660219000000000000000000650464033c0000006508650464043c
+            0000006410640165036404650a6508190000000000000000006604640684
+            055a0b6407650c64086505650d1900000000000000000064096405660664
+            0a84045a0e6411640c650f64096505651019000000000000000000660464
+            0d84055a11640e6506640965056510190000000000000000006604640f84
+            045a1264055300
+          23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('VaribleDetector')
+                       6 LOAD_CONST               0 ('FileAnalyzer')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          54          12 LOAD_CONST               1 (None)
-                      14 STORE_NAME               3 (language)
-                      16 LOAD_NAME                4 (Optional)
-                      18 LOAD_NAME                5 (Language)
-                      20 BINARY_SUBSCR
-                      30 LOAD_NAME                6 (__annotations__)
-                      32 LOAD_CONST               2 ('language')
-                      34 STORE_SUBSCR
-         
-          55          38 LOAD_NAME                7 (re)
-                      40 LOAD_ATTR                8 (Pattern)
-                      50 LOAD_NAME                6 (__annotations__)
-                      52 LOAD_CONST               3 ('stream_pattern')
-                      54 STORE_SUBSCR
-         
-          56          58 LOAD_NAME                9 (Dict)
-                      60 LOAD_NAME               10 (int)
-                      62 LOAD_NAME               11 (Match)
-                      64 BUILD_TUPLE              2
-                      66 BINARY_SUBSCR
-                      76 LOAD_NAME                6 (__annotations__)
-                      78 LOAD_CONST               4 ('match_rules')
-                      80 STORE_SUBSCR
-         
-          57          84 LOAD_NAME                9 (Dict)
-                      86 LOAD_NAME               10 (int)
-                      88 LOAD_NAME               12 (str)
-                      90 BUILD_TUPLE              2
-                      92 BINARY_SUBSCR
-                     102 LOAD_NAME                6 (__annotations__)
-                     104 LOAD_CONST               5 ('match_semantics')
-                     106 STORE_SUBSCR
-         
-          58         110 LOAD_CONST               6 (0)
-                     112 STORE_NAME              13 (creds_probability)
-                     114 LOAD_NAME               10 (int)
-                     116 LOAD_NAME                6 (__annotations__)
-                     118 LOAD_CONST               7 ('creds_probability')
-                     120 STORE_SUBSCR
-         
-          60         124 PUSH_NULL
-                     126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               8 (<code object Config, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 60>)
-                     130 MAKE_FUNCTION            0
-                     132 LOAD_CONST               9 ('Config')
-                     134 PRECALL                  2
-                     138 CALL                     2
-                     148 STORE_NAME              14 (Config)
-         
-          63         150 LOAD_CONST              10 ('tokens')
-                     152 LOAD_NAME               15 (List)
-                     154 LOAD_NAME               16 (Token)
-                     156 BINARY_SUBSCR
-                     166 LOAD_CONST              11 ('token_stream')
-                     168 LOAD_NAME               12 (str)
-                     170 LOAD_CONST              12 ('return')
-                     172 LOAD_NAME               15 (List)
-                     174 LOAD_CONST              13 ('Variable')
-                     176 BINARY_SUBSCR
-                     186 BUILD_TUPLE              6
-                     188 LOAD_CONST              14 (<code object match, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 63>)
-                     190 MAKE_FUNCTION            4 (annotations)
-                     192 STORE_NAME              17 (match)
-         
-          79         194 LOAD_CONST              15 ('match')
-                     196 LOAD_NAME                7 (re)
-                     198 LOAD_ATTR               11 (Match)
-                     208 LOAD_CONST              10 ('tokens')
-                     210 LOAD_NAME               15 (List)
-                     212 LOAD_NAME               16 (Token)
-                     214 BINARY_SUBSCR
-                     224 LOAD_CONST              12 ('return')
-                     226 LOAD_NAME               18 (bool)
-                     228 BUILD_TUPLE              6
-                     230 LOAD_CONST              16 (<code object _verify, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py", line 79>)
-                     232 MAKE_FUNCTION            4 (annotations)
-                     234 STORE_NAME              19 (_verify)
-                     236 LOAD_CONST               1 (None)
-                     238 RETURN_VALUE
+          24          12 LOAD_NAME                3 (File)
+                      14 LOAD_NAME                4 (__annotations__)
+                      16 LOAD_CONST               1 ('file')
+                      18 STORE_SUBSCR
+         
+          25          22 LOAD_NAME                5 (List)
+                      24 LOAD_NAME                6 (EngineWithTokenizer)
+                      26 BINARY_SUBSCR
+                      36 LOAD_NAME                4 (__annotations__)
+                      38 LOAD_CONST               2 ('engine_tokenizers')
+                      40 STORE_SUBSCR
+         
+          26          44 LOAD_NAME                7 (Dict)
+                      46 LOAD_NAME                8 (Type)
+                      48 LOAD_NAME                5 (List)
+                      50 LOAD_NAME                9 (Token)
+                      52 BINARY_SUBSCR
+                      62 BUILD_TUPLE              2
+                      64 BINARY_SUBSCR
+                      74 LOAD_NAME                4 (__annotations__)
+                      76 LOAD_CONST               3 ('tokens')
+                      78 STORE_SUBSCR
+         
+          27          82 LOAD_NAME                8 (Type)
+                      84 LOAD_NAME                4 (__annotations__)
+                      86 LOAD_CONST               4 ('pool_class')
+                      88 STORE_SUBSCR
+         
+          29          92 LOAD_CONST              16 ((None,))
+                      94 LOAD_CONST               1 ('file')
+                      96 LOAD_NAME                3 (File)
+                      98 LOAD_CONST               4 ('pool_class')
+                     100 LOAD_NAME               10 (Optional)
+                     102 LOAD_NAME                8 (Type)
+                     104 BINARY_SUBSCR
+                     114 BUILD_TUPLE              4
+                     116 LOAD_CONST               6 (<code object __init__, file "/app/deepsecrets/core/utils/file_analyzer.py", line 29>)
+                     118 MAKE_FUNCTION            5 (defaults, annotations)
+                     120 STORE_NAME              11 (__init__)
+         
+          40         122 LOAD_CONST               7 ('engine')
+                     124 LOAD_NAME               12 (IEngine)
+                     126 LOAD_CONST               8 ('tokenizers')
+                     128 LOAD_NAME                5 (List)
+                     130 LOAD_NAME               13 (Tokenizer)
+                     132 BINARY_SUBSCR
+                     142 LOAD_CONST               9 ('return')
+                     144 LOAD_CONST               5 (None)
+                     146 BUILD_TUPLE              6
+                     148 LOAD_CONST              10 (<code object add_engine, file "/app/deepsecrets/core/utils/file_analyzer.py", line 40>)
+                     150 MAKE_FUNCTION            4 (annotations)
+                     152 STORE_NAME              14 (add_engine)
+         
+          44         154 LOAD_CONST              17 ((False,))
+                     156 LOAD_CONST              12 ('threaded')
+                     158 LOAD_NAME               15 (bool)
+                     160 LOAD_CONST               9 ('return')
+                     162 LOAD_NAME                5 (List)
+                     164 LOAD_NAME               16 (Finding)
+                     166 BINARY_SUBSCR
+                     176 BUILD_TUPLE              4
+                     178 LOAD_CONST              13 (<code object process, file "/app/deepsecrets/core/utils/file_analyzer.py", line 44>)
+                     180 MAKE_FUNCTION            5 (defaults, annotations)
+                     182 STORE_NAME              17 (process)
+         
+          67         184 LOAD_CONST              14 ('et')
+                     186 LOAD_NAME                6 (EngineWithTokenizer)
+                     188 LOAD_CONST               9 ('return')
+                     190 LOAD_NAME                5 (List)
+                     192 LOAD_NAME               16 (Finding)
+                     194 BINARY_SUBSCR
+                     204 BUILD_TUPLE              4
+                     206 LOAD_CONST              15 (<code object _run_engine, file "/app/deepsecrets/core/utils/file_analyzer.py", line 67>)
+                     208 MAKE_FUNCTION            4 (annotations)
+                     210 STORE_NAME              18 (_run_engine)
+                     212 LOAD_CONST               5 (None)
+                     214 RETURN_VALUE
          consts
-            'VaribleDetector'
+            'FileAnalyzer'
+            'file'
+            'engine_tokenizers'
+            'tokens'
+            'pool_class'
             None
-            'language'
-            'stream_pattern'
-            'match_rules'
-            'match_semantics'
-            0
-            'creds_probability'
             code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 1
-               flags     : 0
-               code 0x970065005a0164005a0264015a0364025300
-                60           0 RESUME                   0
-                             2 LOAD_NAME                0 (__name__)
-                             4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('VaribleDetector.Config')
-                             8 STORE_NAME               2 (__qualname__)
-               
-                61          10 LOAD_CONST               1 (True)
-                            12 STORE_NAME               3 (arbitrary_types_allowed)
-                            14 LOAD_CONST               2 (None)
-                            16 RETURN_VALUE
+               argcount  : 3
+               nlocals   : 3
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c02810d7400000000000000000000007c005f0100000000000000
+                  006e077c027c005f01000000000000000067007c005f0200000000000000
+                  007c017c005f03000000000000000069007c005f04000000000000000074
+                  0b00000000000000000000a6000000ab0000000000000000007c005f0600
+                  0000000000000064005300
+                29           0 RESUME                   0
+               
+                30           2 LOAD_FAST                2 (pool_class)
+                             4 POP_JUMP_FORWARD_IF_NONE    13 (to 32)
+               
+                31           6 LOAD_GLOBAL              0 (Pool)
+                            18 LOAD_FAST                0 (self)
+                            20 STORE_ATTR               1 (pool_class)
+                            30 JUMP_FORWARD             7 (to 46)
+               
+                33     >>   32 LOAD_FAST                2 (pool_class)
+                            34 LOAD_FAST                0 (self)
+                            36 STORE_ATTR               1 (pool_class)
+               
+                35     >>   46 BUILD_LIST               0
+                            48 LOAD_FAST                0 (self)
+                            50 STORE_ATTR               2 (engine_tokenizers)
+               
+                36          60 LOAD_FAST                1 (file)
+                            62 LOAD_FAST                0 (self)
+                            64 STORE_ATTR               3 (file)
+               
+                37          74 BUILD_MAP                0
+                            76 LOAD_FAST                0 (self)
+                            78 STORE_ATTR               4 (tokens)
+               
+                38          88 LOAD_GLOBAL             11 (NULL + RLock)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 LOAD_FAST                0 (self)
+                           116 STORE_ATTR               6 (tokenizers_lock)
+                           126 LOAD_CONST               0 (None)
+                           128 RETURN_VALUE
                consts
-                  'VaribleDetector.Config'
-                  True
                   None
-               names      ('__name__', '__module__', '__qualname__', 'arbitrary_types_allowed')
-               varnames   ()
+               names      ('Pool', 'pool_class', 'engine_tokenizers', 'file', 'tokens', 'RLock', 'tokenizers_lock')
+               varnames   ('self', 'file', 'pool_class')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-               name       'Config'
-               firstlineno 60
-               lnotab 0x0a01
-            'Config'
-            'tokens'
-            'token_stream'
+               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+               name       '__init__'
+               firstlineno 29
+               lnotab 0x020104011a020e020e010e010e01
+            'engine'
+            'tokenizers'
             'return'
-            'Variable'
             code
                argcount  : 3
-               nlocals   : 8
-               stacksize : 10
+               nlocals   : 4
+               stacksize : 7
                flags     : 3
                code
-                  0x970067007d037401000000000000000000006a0100000000000000007c
-                  006a0200000000000000007c026401ac02a6030000ab0300000000000000
-                  0044005d927d047c00a00300000000000000000000000000000000000000
-                  007c047c01a6020000ab02000000000000000073018c1974090000000000
-                  0000000000a6000000ab0000000000000000007d057c006a050000000000
-                  000000a0060000000000000000000000000000000000000000a6000000ab
-                  00000000000000000044005d355c0200007d067d07740f00000000000000
-                  0000007c057c077c017c04a0080000000000000000000000000000000000
-                  0000007c06a6010000ab0100000000000000006403190000000000000000
-                  0019000000000000000000a6030000ab03000000000000000001008c367c
-                  007c055f0900000000000000007c03a00a00000000000000000000000000
-                  000000000000007c05a6010000ab01000000000000000001008c937c0353
-                  00
-                63           0 RESUME                   0
-               
-                64           2 BUILD_LIST               0
-                             4 STORE_FAST               3 (true_detections)
-               
-                66           6 LOAD_GLOBAL              1 (NULL + re)
-                            18 LOAD_ATTR                1 (finditer)
-                            28 LOAD_FAST                0 (self)
-                            30 LOAD_ATTR                2 (stream_pattern)
-                            40 LOAD_FAST                2 (token_stream)
-                            42 LOAD_CONST               1 (True)
-                            44 KW_NAMES                 2
-                            46 PRECALL                  3
-                            50 CALL                     3
-                            60 GET_ITER
-                       >>   62 FOR_ITER               146 (to 356)
-                            64 STORE_FAST               4 (match)
-               
-                67          66 LOAD_FAST                0 (self)
-                            68 LOAD_METHOD              3 (_verify)
-                            90 LOAD_FAST                4 (match)
-                            92 LOAD_FAST                1 (tokens)
-                            94 PRECALL                  2
-                            98 CALL                     2
-                           108 POP_JUMP_FORWARD_IF_TRUE     1 (to 112)
-               
-                68         110 JUMP_BACKWARD           25 (to 62)
-               
-                70     >>  112 LOAD_GLOBAL              9 (NULL + Variable)
-                           124 PRECALL                  0
-                           128 CALL                     0
-                           138 STORE_FAST               5 (var)
-               
-                71         140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                5 (match_semantics)
-                           152 LOAD_METHOD              6 (items)
-                           174 PRECALL                  0
-                           178 CALL                     0
-                           188 GET_ITER
-                       >>  190 FOR_ITER                53 (to 298)
-                           192 UNPACK_SEQUENCE          2
-                           196 STORE_FAST               6 (i)
-                           198 STORE_FAST               7 (name)
-               
-                72         200 LOAD_GLOBAL             15 (NULL + setattr)
-                           212 LOAD_FAST                5 (var)
-                           214 LOAD_FAST                7 (name)
-                           216 LOAD_FAST                1 (tokens)
-                           218 LOAD_FAST                4 (match)
-                           220 LOAD_METHOD              8 (span)
-                           242 LOAD_FAST                6 (i)
-                           244 PRECALL                  1
-                           248 CALL                     1
-                           258 LOAD_CONST               3 (0)
-                           260 BINARY_SUBSCR
-                           270 BINARY_SUBSCR
-                           280 PRECALL                  3
-                           284 CALL                     3
-                           294 POP_TOP
-                           296 JUMP_BACKWARD           54 (to 190)
-               
-                73     >>  298 LOAD_FAST                0 (self)
-                           300 LOAD_FAST                5 (var)
-                           302 STORE_ATTR               9 (found_by)
-               
-                75         312 LOAD_FAST                3 (true_detections)
-                           314 LOAD_METHOD             10 (append)
-                           336 LOAD_FAST                5 (var)
-                           338 PRECALL                  1
-                           342 CALL                     1
-                           352 POP_TOP
-                           354 JUMP_BACKWARD          147 (to 62)
+                  0x97007c0244005d2b7d037c006a000000000000000000a0010000000000
+                  0000000000000000000000000000007405000000000000000000007c017c
+                  03ac01a6020000ab020000000000000000a6010000ab0100000000000000
+                  0001008c2c64005300
+                40           0 RESUME                   0
+               
+                41           2 LOAD_FAST                2 (tokenizers)
+                             4 GET_ITER
+                       >>    6 FOR_ITER                43 (to 94)
+                             8 STORE_FAST               3 (tokenizer)
+               
+                42          10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (engine_tokenizers)
+                            22 LOAD_METHOD              1 (append)
+                            44 LOAD_GLOBAL              5 (NULL + EngineWithTokenizer)
+                            56 LOAD_FAST                1 (engine)
+                            58 LOAD_FAST                3 (tokenizer)
+                            60 KW_NAMES                 1
+                            62 PRECALL                  2
+                            66 CALL                     2
+                            76 PRECALL                  1
+                            80 CALL                     1
+                            90 POP_TOP
+                            92 JUMP_BACKWARD           44 (to 6)
                
-                77     >>  356 LOAD_FAST                3 (true_detections)
-                           358 RETURN_VALUE
+                41     >>   94 LOAD_CONST               0 (None)
+                            96 RETURN_VALUE
                consts
                   None
-                  True
-                  ('overlapped',)
-                  0
-               names      ('re', 'finditer', 'stream_pattern', '_verify', 'Variable', 'match_semantics', 'items', 'setattr', 'span', 'found_by', 'append')
-               varnames   ('self', 'tokens', 'token_stream', 'true_detections', 'match', 'var', 'i', 'name')
+                  ('engine', 'tokenizer')
+               names      ('engine_tokenizers', 'append', 'EngineWithTokenizer')
+               varnames   ('self', 'engine', 'tokenizers', 'tokenizer')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-               name       'match'
-               firstlineno 63
-               lnotab 0x020104023c012c0102021c013c0162010e022c02
-            'match'
+               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+               name       'add_engine'
+               firstlineno 40
+               lnotab 0x0201080154ff
+            False
+            'threaded'
             code
-               argcount  : 3
+               argcount  : 2
                nlocals   : 7
-               stacksize : 5
+               stacksize : 6
                flags     : 3
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
-                  00000000000000a6000000ab00000000000000000044005d485c0200007d
-                  037d047c01a00200000000000000000000000000000000000000007c03a6
-                  010000ab0100000000000000007d057c027c056401190000000000000000
-                  007c056402190000000000000000008502190000000000000000007d067c
-                  04a00300000000000000000000000000000000000000007c06a6010000ab
-                  01000000000000000073030100640353008c4964045300
-                79           0 RESUME                   0
-               
-                80           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (match_rules)
-                            14 LOAD_METHOD              1 (items)
-                            36 PRECALL                  0
-                            40 CALL                     0
-                            50 GET_ITER
-                       >>   52 FOR_ITER                72 (to 198)
-                            54 UNPACK_SEQUENCE          2
-                            58 STORE_FAST               3 (group_i)
-                            60 STORE_FAST               4 (match_rule)
-               
-                81          62 LOAD_FAST                1 (match)
-                            64 LOAD_METHOD              2 (span)
-                            86 LOAD_FAST                3 (group_i)
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 STORE_FAST               5 (span)
-               
-                82         104 LOAD_FAST                2 (tokens)
-                           106 LOAD_FAST                5 (span)
-                           108 LOAD_CONST               1 (0)
-                           110 BINARY_SUBSCR
-                           120 LOAD_FAST                5 (span)
-                           122 LOAD_CONST               2 (1)
-                           124 BINARY_SUBSCR
-                           134 BUILD_SLICE              2
-                           136 BINARY_SUBSCR
-                           146 STORE_FAST               6 (window)
-               
-                84         148 LOAD_FAST                4 (match_rule)
-                           150 LOAD_METHOD              3 (check)
-                           172 LOAD_FAST                6 (window)
-                           174 PRECALL                  1
-                           178 CALL                     1
-                           188 POP_JUMP_FORWARD_IF_TRUE     3 (to 196)
-               
-                85         190 POP_TOP
-                           192 LOAD_CONST               3 (False)
-                           194 RETURN_VALUE
+                  0x970067007d027c0172977c00a000000000000000000000000000000000
+                  00000000006401a6010000ab01000000000000000035007d037c03a00100
+                  000000000000000000000000000000000000007c006a0200000000000000
+                  007c006a030000000000000000a6020000ab0200000000000000007d047c
+                  03a0040000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001007c03a0050000000000000000000000000000000000
+                  000000a6000000ab0000000000000000000100640064006400a6020000ab
+                  02000000000000000001006e0b2300310073047702780359007701010059
+                  00010001007c0480027c0253007c0444005d1a7d057c0573018c057c02a0
+                  0600000000000000000000000000000000000000007c05a6010000ab0100
+                  0000000000000001008c1b6e327c006a03000000000000000044005d2a7d
+                  067c02a00600000000000000000000000000000000000000007c00a00200
+                  000000000000000000000000000000000000007c06a6010000ab01000000
+                  0000000000a6010000ab01000000000000000001008c2b7c025300
+                44           0 RESUME                   0
+               
+                45           2 BUILD_LIST               0
+                             4 STORE_FAST               2 (results)
+               
+                47           6 LOAD_FAST                1 (threaded)
+                             8 POP_JUMP_FORWARD_IF_FALSE   151 (to 312)
+               
+                48          10 LOAD_FAST                0 (self)
+                            12 LOAD_METHOD              0 (pool_class)
+                            34 LOAD_CONST               1 (2)
+                            36 PRECALL                  1
+                            40 CALL                     1
+                            50 BEFORE_WITH
+                            52 STORE_FAST               3 (pool)
+               
+                49          54 LOAD_FAST                3 (pool)
+                            56 LOAD_METHOD              1 (imap)
+                            78 LOAD_FAST                0 (self)
+                            80 LOAD_ATTR                2 (_run_engine)
+                            90 LOAD_FAST                0 (self)
+                            92 LOAD_ATTR                3 (engine_tokenizers)
+                           102 PRECALL                  2
+                           106 CALL                     2
+                           116 STORE_FAST               4 (engine_results)
+               
+                50         118 LOAD_FAST                3 (pool)
+                           120 LOAD_METHOD              4 (close)
+                           142 PRECALL                  0
+                           146 CALL                     0
+                           156 POP_TOP
+               
+                51         158 LOAD_FAST                3 (pool)
+                           160 LOAD_METHOD              5 (join)
+                           182 PRECALL                  0
+                           186 CALL                     0
+                           196 POP_TOP
+               
+                48         198 LOAD_CONST               0 (None)
+                           200 LOAD_CONST               0 (None)
+                           202 LOAD_CONST               0 (None)
+                           204 PRECALL                  2
+                           208 CALL                     2
+                           218 POP_TOP
+                           220 JUMP_FORWARD            11 (to 244)
+                       >>  222 PUSH_EXC_INFO
+                           224 WITH_EXCEPT_START
+                           226 POP_JUMP_FORWARD_IF_TRUE     4 (to 236)
+                           228 RERAISE                  2
+                       >>  230 COPY                     3
+                           232 POP_EXCEPT
+                           234 RERAISE                  1
+                       >>  236 POP_TOP
+                           238 POP_EXCEPT
+                           240 POP_TOP
+                           242 POP_TOP
+               
+                53     >>  244 LOAD_FAST                4 (engine_results)
+                           246 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 252)
+               
+                54         248 LOAD_FAST                2 (results)
+                           250 RETURN_VALUE
+               
+                56     >>  252 LOAD_FAST                4 (engine_results)
+                           254 GET_ITER
+                       >>  256 FOR_ITER                26 (to 310)
+                           258 STORE_FAST               5 (er)
+               
+                57         260 LOAD_FAST                5 (er)
+                           262 POP_JUMP_FORWARD_IF_TRUE     1 (to 266)
+               
+                58         264 JUMP_BACKWARD            5 (to 256)
+               
+                59     >>  266 LOAD_FAST                2 (results)
+                           268 LOAD_METHOD              6 (extend)
+                           290 LOAD_FAST                5 (er)
+                           292 PRECALL                  1
+                           296 CALL                     1
+                           306 POP_TOP
+                           308 JUMP_BACKWARD           27 (to 256)
+               
+                56     >>  310 JUMP_FORWARD            50 (to 412)
+               
+                62     >>  312 LOAD_FAST                0 (self)
+                           314 LOAD_ATTR                3 (engine_tokenizers)
+                           324 GET_ITER
+                       >>  326 FOR_ITER                42 (to 412)
+                           328 STORE_FAST               6 (et)
+               
+                63         330 LOAD_FAST                2 (results)
+                           332 LOAD_METHOD              6 (extend)
+                           354 LOAD_FAST                0 (self)
+                           356 LOAD_METHOD              2 (_run_engine)
+                           378 LOAD_FAST                6 (et)
+                           380 PRECALL                  1
+                           384 CALL                     1
+                           394 PRECALL                  1
+                           398 CALL                     1
+                           408 POP_TOP
+                           410 JUMP_BACKWARD           43 (to 326)
+               
+                65     >>  412 LOAD_FAST                2 (results)
+                           414 RETURN_VALUE
+               ExceptionTable:
+                 52 to 196 -> 222 [1] lasti
+                 222 to 228 -> 230 [3] lasti
+                 236 to 236 -> 230 [3] lasti
+               consts
+                  None
+                  2
+               names      ('pool_class', 'imap', '_run_engine', 'engine_tokenizers', 'close', 'join', 'extend')
+               varnames   ('self', 'threaded', 'results', 'pool', 'engine_results', 'er', 'et')
+               freevars   ()
+               cellvars   ()
+               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+               name       'process'
+               firstlineno 44
+               lnotab
+                  0x0201040204012c014001280128fd2e05040104020801040102012cfd02
+                  0612015202
+            'et'
+            code
+               argcount  : 2
+               nlocals   : 10
+               stacksize : 7
+               flags     : 3
+               code
+                  0x970067007d0269007d037c006a000000000000000000350001007c016a
+                  0100000000000000007c006a0200000000000000007601722c7c016a0100
+                  00000000000000a00300000000000000000000000000000000000000007c
+                  006a040000000000000000a6010000ab0100000000000000007c006a0200
+                  000000000000007c016a0100000000000000003c000000640064006400a6
+                  020000ab02000000000000000001006e0b23003100730477027803590077
+                  0101005900010001007c006a0200000000000000007c016a010000000000
+                  000000190000000000000000007d047c0444005de57d057c03a005000000
+                  00000000000000000000000000000000007c05a006000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a6010000ab
+                  0100000000000000007d067c0681057c066401750072018c3064017c037c
+                  05a0060000000000000000000000000000000000000000a6000000ab0000
+                  000000000000003c00000009007c016a070000000000000000a008000000
+                  00000000000000000000000000000000007c05a6010000ab010000000000
+                  0000007d077c0744005d557d087c08a00900000000000000000000000000
+                  000000000000007c006a0400000000000000007c056a0a00000000000000
+                  00640219000000000000000000ac03a6020000ab02000000000000000001
+                  007c02a00b00000000000000000000000000000000000000007c08a60100
+                  00ab010000000000000000010064047c037c05a006000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000003c0000008c
+                  568cbb23007418000000000000000000002400721e7d09741b0000000000
+                  00000000006a0e00000000000000006405a6010000ab0100000000000000
+                  000100590064007d097e098cde64007d097e09770177007803590077017c
+                  025300
+                67           0 RESUME                   0
+               
+                68           2 BUILD_LIST               0
+                             4 STORE_FAST               2 (results)
                
-                84     >>  196 JUMP_BACKWARD           73 (to 52)
+                69           6 BUILD_MAP                0
+                             8 STORE_FAST               3 (processed_values)
                
-                87     >>  198 LOAD_CONST               4 (True)
-                           200 RETURN_VALUE
+                71          10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (tokenizers_lock)
+                            22 BEFORE_WITH
+                            24 POP_TOP
+               
+                72          26 LOAD_FAST                1 (et)
+                            28 LOAD_ATTR                1 (tokenizer)
+                            38 LOAD_FAST                0 (self)
+                            40 LOAD_ATTR                2 (tokens)
+                            50 CONTAINS_OP              1
+                            52 POP_JUMP_FORWARD_IF_FALSE    44 (to 142)
+               
+                73          54 LOAD_FAST                1 (et)
+                            56 LOAD_ATTR                1 (tokenizer)
+                            66 LOAD_METHOD              3 (tokenize)
+                            88 LOAD_FAST                0 (self)
+                            90 LOAD_ATTR                4 (file)
+                           100 PRECALL                  1
+                           104 CALL                     1
+                           114 LOAD_FAST                0 (self)
+                           116 LOAD_ATTR                2 (tokens)
+                           126 LOAD_FAST                1 (et)
+                           128 LOAD_ATTR                1 (tokenizer)
+                           138 STORE_SUBSCR
+               
+                71     >>  142 LOAD_CONST               0 (None)
+                           144 LOAD_CONST               0 (None)
+                           146 LOAD_CONST               0 (None)
+                           148 PRECALL                  2
+                           152 CALL                     2
+                           162 POP_TOP
+                           164 JUMP_FORWARD            11 (to 188)
+                       >>  166 PUSH_EXC_INFO
+                           168 WITH_EXCEPT_START
+                           170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                           172 RERAISE                  2
+                       >>  174 COPY                     3
+                           176 POP_EXCEPT
+                           178 RERAISE                  1
+                       >>  180 POP_TOP
+                           182 POP_EXCEPT
+                           184 POP_TOP
+                           186 POP_TOP
+               
+                75     >>  188 LOAD_FAST                0 (self)
+                           190 LOAD_ATTR                2 (tokens)
+                           200 LOAD_FAST                1 (et)
+                           202 LOAD_ATTR                1 (tokenizer)
+                           212 BINARY_SUBSCR
+                           222 STORE_FAST               4 (tokens)
+               
+                77         224 LOAD_FAST                4 (tokens)
+                           226 GET_ITER
+                       >>  228 FOR_ITER               229 (to 688)
+                           230 STORE_FAST               5 (token)
+               
+                78         232 LOAD_FAST                3 (processed_values)
+                           234 LOAD_METHOD              5 (get)
+                           256 LOAD_FAST                5 (token)
+                           258 LOAD_METHOD              6 (val_hash)
+                           280 PRECALL                  0
+                           284 CALL                     0
+                           294 PRECALL                  1
+                           298 CALL                     1
+                           308 STORE_FAST               6 (is_known_content)
+               
+                79         310 LOAD_FAST                6 (is_known_content)
+                           312 POP_JUMP_FORWARD_IF_NONE     5 (to 324)
+                           314 LOAD_FAST                6 (is_known_content)
+                           316 LOAD_CONST               1 (False)
+                           318 IS_OP                    0
+                           320 POP_JUMP_FORWARD_IF_FALSE     1 (to 324)
+               
+                80         322 JUMP_BACKWARD           48 (to 228)
+               
+                82     >>  324 LOAD_CONST               1 (False)
+                           326 LOAD_FAST                3 (processed_values)
+                           328 LOAD_FAST                5 (token)
+                           330 LOAD_METHOD              6 (val_hash)
+                           352 PRECALL                  0
+                           356 CALL                     0
+                           366 STORE_SUBSCR
+               
+                84         370 NOP
+               
+                85         372 LOAD_FAST                1 (et)
+                           374 LOAD_ATTR                7 (engine)
+                           384 LOAD_METHOD              8 (search)
+                           406 LOAD_FAST                5 (token)
+                           408 PRECALL                  1
+                           412 CALL                     1
+                           422 STORE_FAST               7 (findings)
+               
+                86         424 LOAD_FAST                7 (findings)
+                           426 GET_ITER
+                       >>  428 FOR_ITER                85 (to 600)
+                           430 STORE_FAST               8 (finding)
+               
+                87         432 LOAD_FAST                8 (finding)
+                           434 LOAD_METHOD              9 (map_on_file)
+                           456 LOAD_FAST                0 (self)
+                           458 LOAD_ATTR                4 (file)
+                           468 LOAD_FAST                5 (token)
+                           470 LOAD_ATTR               10 (span)
+                           480 LOAD_CONST               2 (0)
+                           482 BINARY_SUBSCR
+                           492 KW_NAMES                 3
+                           494 PRECALL                  2
+                           498 CALL                     2
+                           508 POP_TOP
+               
+                88         510 LOAD_FAST                2 (results)
+                           512 LOAD_METHOD             11 (append)
+                           534 LOAD_FAST                8 (finding)
+                           536 PRECALL                  1
+                           540 CALL                     1
+                           550 POP_TOP
+               
+                89         552 LOAD_CONST               4 (True)
+                           554 LOAD_FAST                3 (processed_values)
+                           556 LOAD_FAST                5 (token)
+                           558 LOAD_METHOD              6 (val_hash)
+                           580 PRECALL                  0
+                           584 CALL                     0
+                           594 STORE_SUBSCR
+                           598 JUMP_BACKWARD           86 (to 428)
+               
+                86     >>  600 JUMP_BACKWARD          187 (to 228)
+                       >>  602 PUSH_EXC_INFO
+               
+                91         604 LOAD_GLOBAL             24 (Exception)
+                           616 CHECK_EXC_MATCH
+                           618 POP_JUMP_FORWARD_IF_FALSE    30 (to 680)
+                           620 STORE_FAST               9 (e)
+               
+                92         622 LOAD_GLOBAL             27 (NULL + logger)
+                           634 LOAD_ATTR               14 (exception)
+                           644 LOAD_CONST               5 ('Unable to process token')
+                           646 PRECALL                  1
+                           650 CALL                     1
+                           660 POP_TOP
+               
+                93         662 POP_EXCEPT
+                           664 LOAD_CONST               0 (None)
+                           666 STORE_FAST               9 (e)
+                           668 DELETE_FAST              9 (e)
+                           670 JUMP_BACKWARD          222 (to 228)
+                       >>  672 LOAD_CONST               0 (None)
+                           674 STORE_FAST               9 (e)
+                           676 DELETE_FAST              9 (e)
+                           678 RERAISE                  1
+               
+                91     >>  680 RERAISE                  0
+                       >>  682 COPY                     3
+                           684 POP_EXCEPT
+                           686 RERAISE                  1
+               
+                95     >>  688 LOAD_FAST                2 (results)
+                           690 RETURN_VALUE
+               ExceptionTable:
+                 24 to 140 -> 166 [1] lasti
+                 166 to 172 -> 174 [3] lasti
+                 180 to 180 -> 174 [3] lasti
+                 372 to 598 -> 602 [1]
+                 602 to 620 -> 682 [2] lasti
+                 622 to 660 -> 672 [2] lasti
+                 672 to 680 -> 682 [2] lasti
                consts
                   None
-                  0
-                  1
                   False
+                  0
+                  ('file', 'relative_start')
                   True
-               names      ('match_rules', 'items', 'span', 'check')
-               varnames   ('self', 'match', 'tokens', 'group_i', 'match_rule', 'span', 'window')
+                  'Unable to process token'
+               names      ('tokenizers_lock', 'tokenizer', 'tokens', 'tokenize', 'file', 'get', 'val_hash', 'engine', 'search', 'map_on_file', 'span', 'append', 'Exception', 'logger', 'exception')
+               varnames   ('self', 'et', 'results', 'processed_values', 'tokens', 'token', 'is_known_content', 'findings', 'finding', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-               name       '_verify'
-               firstlineno 79
-               lnotab 0x02013c012a012c022a0106ff0203
-         names      ('__name__', '__module__', '__qualname__', 'language', 'Optional', 'Language', '__annotations__', 're', 'Pattern', 'Dict', 'int', 'Match', 'str', 'creds_probability', 'Config', 'List', 'Token', 'match', 'bool', '_verify')
+               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+               name       '_run_engine'
+               firstlineno 67
+               lnotab
+                  0x02010401040210011c0158fe2e04240208014e010c0102022e02020134
+                  0108014e012a0130fd04051201280112fe0804
+            (None,)
+            (False,)
+         names      ('__name__', '__module__', '__qualname__', 'File', '__annotations__', 'List', 'EngineWithTokenizer', 'Dict', 'Type', 'Token', 'Optional', '__init__', 'IEngine', 'Tokenizer', 'add_engine', 'bool', 'Finding', 'process', '_run_engine')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
-         name       'VaribleDetector'
-         firstlineno 53
-         lnotab 0x0c011a0114011a011a010e021a032c10
-      'VaribleDetector'
-      ('Variable',)
-   names      ('regex', 're', 'typing', 'Dict', 'List', 'Optional', 'pydantic', 'BaseModel', 'Field', 'validator', 'deepsecrets.core.model.token', 'Token', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'Match', 'VaribleDetector', 'deepsecrets.core.model.semantic', 'Variable')
+         filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+         name       'FileAnalyzer'
+         firstlineno 23
+         lnotab 0x0c010a01160126010a021e0b20041e17
+      'FileAnalyzer'
+      None
+   names      ('multiprocessing', 'RLock', 'multiprocessing.pool', 'Pool', 'typing', 'Dict', 'List', 'Optional', 'Type', 'pydantic', 'BaseModel', 'deepsecrets', 'logger', 'deepsecrets.core.engines.iengine', 'IEngine', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.finding', 'Finding', 'deepsecrets.core.model.token', 'Token', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'EngineWithTokenizer', 'FileAnalyzer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py'
+   filename   '/app/deepsecrets/core/utils/file_analyzer.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801140214020c010c031c2b1c25
+   lnotab 0x00ff02010c010c0118020c020c010c010c010c010c010c031c08
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xd5ef9a64 (Tue Jun 27 14:19:01 2023 UTC)
-files sz: 5885
+moddate:  0xf920a464 (Tue Jul  4 13:39:05 2023 UTC)
+files sz: 6529
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 4
+   stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
-      055a050100640064046c066d075a076d085a080100020047006405840064
-      06a6020000ab0200000000000000005a0964015300
+      055a050100640064046c066d075a076d085a086d095a090100640064056c
+      0a6d0b5a0c010002004700640684006407a6020000ab0200000000000000
+      005a0d02004700640884006409650da6030000ab0300000000000000005a
+      0e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (regex)
                  8 STORE_NAME               1 (re)
    
@@ -28,38 +30,58 @@
                 24 LOAD_CONST               3 (('Language',))
                 26 IMPORT_NAME              4 (deepsecrets.core.tokenizers.helpers.semantic.language)
                 28 IMPORT_FROM              5 (Language)
                 30 STORE_NAME               5 (Language)
                 32 POP_TOP
    
      5          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('Match', 'VaribleDetector'))
+                36 LOAD_CONST               4 (('Match', 'VaribleDetector', 'VaribleSuppressor'))
                 38 IMPORT_NAME              6 (deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector)
                 40 IMPORT_FROM              7 (Match)
                 42 STORE_NAME               7 (Match)
                 44 IMPORT_FROM              8 (VaribleDetector)
                 46 STORE_NAME               8 (VaribleDetector)
-                48 POP_TOP
+                48 IMPORT_FROM              9 (VaribleSuppressor)
+                50 STORE_NAME               9 (VaribleSuppressor)
+                52 POP_TOP
    
-     8          50 PUSH_NULL
-                52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               5 (<code object VariableDetectionRules, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 8>)
-                56 MAKE_FUNCTION            0
-                58 LOAD_CONST               6 ('VariableDetectionRules')
-                60 PRECALL                  2
-                64 CALL                     2
-                74 STORE_NAME               9 (VariableDetectionRules)
-                76 LOAD_CONST               1 (None)
-                78 RETURN_VALUE
+     6          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('Token',))
+                58 IMPORT_NAME             10 (pygments.token)
+                60 IMPORT_FROM             11 (Token)
+                62 STORE_NAME              12 (PygmentsToken)
+                64 POP_TOP
+   
+     9          66 PUSH_NULL
+                68 LOAD_BUILD_CLASS
+                70 LOAD_CONST               6 (<code object VariableDetectionRules, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 9>)
+                72 MAKE_FUNCTION            0
+                74 LOAD_CONST               7 ('VariableDetectionRules')
+                76 PRECALL                  2
+                80 CALL                     2
+                90 STORE_NAME              13 (VariableDetectionRules)
+   
+   166          92 PUSH_NULL
+                94 LOAD_BUILD_CLASS
+                96 LOAD_CONST               8 (<code object VariableSuppressionRules, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 166>)
+                98 MAKE_FUNCTION            0
+               100 LOAD_CONST               9 ('VariableSuppressionRules')
+               102 LOAD_NAME               13 (VariableDetectionRules)
+               104 PRECALL                  3
+               108 CALL                     3
+               118 STORE_NAME              14 (VariableSuppressionRules)
+               120 LOAD_CONST               1 (None)
+               122 RETURN_VALUE
    consts
       0
       None
       ('List',)
       ('Language',)
-      ('Match', 'VaribleDetector')
+      ('Match', 'VaribleDetector', 'VaribleSuppressor')
+      ('Token',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 28
          flags     : 0
          code
             0x970065005a0164005a020200650365046a050000000000000000020065
@@ -74,167 +96,168 @@
             0100000000000000000200650864036701ac05a6010000ab010000000000
             000000640d9c0264066407640e9c02ac09a6040000ab0400000000000000
             000200650365046a090000000000000000020065066a0700000000000000
             00640fa6010000ab010000000000000000640202006508640464036702ac
             05a6010000ab01000000000000000069016406640764089c02ac09a60400
             00ab0400000000000000000200650365046a090000000000000000020065
             066a0700000000000000006410a6010000ab010000000000000000020065
-            0864116701ac05a6010000ab0100000000000000000200650864126701ac
-            05a6010000ab0100000000000000000200650864136701ac05a6010000ab
-            01000000000000000064149c036406640764159c02ac09a6040000ab0400
-            000000000000000200650365046a090000000000000000020065066a0700
-            000000000000006416a6010000ab01000000000000000002006508641767
-            01ac05a6010000ab01000000000000000002006508641864116702ac19a6
-            010000ab010000000000000000640d9c0264066407640e9c02ac09a60400
-            00ab0400000000000000000200650365046a090000000000000000020065
-            066a070000000000000000641aa6010000ab010000000000000000640202
-            006508641b641c6702ac05a6010000ab0100000000000000006901640664
-            0764089c02ac09a6040000ab0400000000000000000200650365046a0a00
-            00000000000000020065066a070000000000000000641da6010000ab0100
-            000000000000006402020065086403641e6702ac05a6010000ab01000000
-            000000000069016406640764089c02ac09a6040000ab0400000000000000
-            000200650365046a0a0000000000000000020065066a0700000000000000
-            00641fa6010000ab01000000000000000002006508641e6701ac05a60100
-            00ab0100000000000000000200650864206701ac05a6010000ab01000000
-            00000000000200650864126701ac05a6010000ab01000000000000000064
-            219c036406640764229c02ac09a6040000ab040000000000000000020065
-            0365046a0b0000000000000000020065066a0700000000000000006423a6
-            010000ab01000000000000000064020200650864036701ac05a6010000ab
-            01000000000000000069016406640764089c02ac09a6040000ab04000000
-            00000000000200650365046a0c0000000000000000020065066a07000000
-            00000000006424a6010000ab010000000000000000640202006508640467
-            01ac05a6010000ab01000000000000000069016406640764089c02ac09a6
-            040000ab0400000000000000000200650365046a0d000000000000000002
-            0065066a0700000000000000006425a6010000ab01000000000000000064
-            020200650864036701ac05a6010000ab0100000000000000006901640664
-            0764089c02ac09a6040000ab0400000000000000000200650365046a0e00
-            00000000000000020065066a0700000000000000006426a6010000ab0100
-            00000000000000640202006508641e64036702ac05a6010000ab01000000
-            000000000069016406640764089c02ac09a6040000ab0400000000000000
-            000200650365046a0f0000000000000000020065066a0700000000000000
-            006427a6010000ab010000000000000000640202006508020065066a0700
-            000000000000006428a6010000ab010000000000000000020065066a0700
-            000000000000006429a6010000ab0100000000000000006702ac05a60100
+            08641164126702ac05a6010000ab01000000000000000002006508641367
+            01ac05a6010000ab0100000000000000000200650864146701ac05a60100
+            00ab01000000000000000064159c036406640764169c02ac09a6040000ab
+            0400000000000000000200650365046a090000000000000000020065066a
+            0700000000000000006417a6010000ab0100000000000000000200650864
+            186701ac05a6010000ab01000000000000000002006508641264116702ac
+            19a6010000ab010000000000000000640d9c0264066407641a9c02ac09a6
+            040000ab0400000000000000000200650365046a09000000000000000002
+            0065066a070000000000000000641ba6010000ab01000000000000000064
+            0202006508641c641d6702ac05a6010000ab010000000000000000690164
+            06640764089c02ac09a6040000ab0400000000000000000200650365046a
+            0a0000000000000000020065066a070000000000000000641ea6010000ab
+            0100000000000000006402020065086403641f6702ac05a6010000ab0100
+            0000000000000069016406640764089c02ac09a6040000ab040000000000
+            0000000200650365046a0a0000000000000000020065066a070000000000
+            0000006420a6010000ab01000000000000000002006508641f6701ac05a6
+            010000ab0100000000000000000200650864216701ac05a6010000ab0100
+            000000000000000200650864136701ac05a6010000ab0100000000000000
+            0064229c0364066407641a9c02ac09a6040000ab04000000000000000002
+            00650365046a0b0000000000000000020065066a07000000000000000064
+            23a6010000ab01000000000000000064020200650864036701ac05a60100
             00ab01000000000000000069016406640764089c02ac09a6040000ab0400
-            000000000000000200650365046a100000000000000000020065066a0700
-            00000000000000642aa6010000ab01000000000000000002006508020065
-            066a070000000000000000642ba6010000ab0100000000000000006701ac
-            05a6010000ab01000000000000000002006508020065066a070000000000
-            000000642ca6010000ab0100000000000000006701ac05a6010000ab0100
-            0000000000000002006508020065066a070000000000000000642da60100
-            00ab0100000000000000006701ac19a6010000ab01000000000000000064
-            2e9c036406640764159c02642fac30a6050000ab05000000000000000002
+            000000000000000200650365046a0c0000000000000000020065066a0700
+            000000000000006424a6010000ab01000000000000000064020200650864
+            046701ac05a6010000ab01000000000000000069016406640764089c02ac
+            09a6040000ab0400000000000000000200650365046a0d00000000000000
+            00020065066a0700000000000000006425a6010000ab0100000000000000
+            0064020200650864036701ac05a6010000ab010000000000000000690164
+            06640764089c02ac09a6040000ab0400000000000000000200650365046a
+            0e0000000000000000020065066a0700000000000000006426a6010000ab
+            010000000000000000640202006508641f64036702ac05a6010000ab0100
+            0000000000000069016406640764089c02ac09a6040000ab040000000000
+            0000000200650365046a0f0000000000000000020065066a070000000000
+            0000006427a6010000ab010000000000000000640202006508020065066a
+            0700000000000000006428a6010000ab010000000000000000020065066a
+            0700000000000000006429a6010000ab0100000000000000006702ac05a6
+            010000ab01000000000000000069016406640764089c02ac09a6040000ab
+            0400000000000000000200650365046a100000000000000000020065066a
+            070000000000000000642aa6010000ab0100000000000000000200650802
+            0065066a070000000000000000642ba6010000ab01000000000000000067
+            01ac05a6010000ab01000000000000000002006508020065066a07000000
+            0000000000642ca6010000ab0100000000000000006701ac05a6010000ab
+            01000000000000000002006508020065066a070000000000000000642da6
+            010000ab0100000000000000006701ac19a6010000ab0100000000000000
+            00642e9c036406640764169c02642fac30a6050000ab0500000000000000
+            000200650365046a110000000000000000020065066a0700000000000000
+            006431a6010000ab01000000000000000002006508020065066a07000000
+            00000000006432a6010000ab0100000000000000006701ac05a6010000ab
+            01000000000000000002006508020065066a0700000000000000006433a6
+            010000ab0100000000000000006701ac19a6010000ab0100000000000000
+            00640e9c0264066407640d9c02ac09a6040000ab04000000000000000002
             00650365046a110000000000000000020065066a07000000000000000064
-            31a6010000ab01000000000000000002006508020065066a070000000000
-            0000006432a6010000ab0100000000000000006701ac05a6010000ab0100
-            0000000000000002006508020065066a0700000000000000006433a60100
-            00ab0100000000000000006701ac19a6010000ab01000000000000000064
-            0e9c0264066407640d9c02ac09a6040000ab040000000000000000020065
-            0365046a110000000000000000020065066a0700000000000000006434a6
-            010000ab01000000000000000002006508020065066a0700000000000000
-            006435a6010000ab0100000000000000006701ac05a6010000ab01000000
-            000000000002006508020065066a0700000000000000006436a6010000ab
+            34a6010000ab01000000000000000002006508020065066a070000000000
+            0000006435a6010000ab0100000000000000006701ac05a6010000ab0100
+            0000000000000002006508020065066a0700000000000000006436a60100
+            00ab0100000000000000006701ac05a6010000ab01000000000000000002
+            006508020065066a0700000000000000006433a6010000ab010000000000
+            0000006701ac05a6010000ab01000000000000000064379c036406640764
+            389c02ac09a6040000ab0400000000000000000200650365046a12000000
+            0000000000020065066a0700000000000000006439a6010000ab01000000
+            000000000002006508020065066a070000000000000000643aa6010000ab
             0100000000000000006701ac05a6010000ab010000000000000000020065
-            08020065066a0700000000000000006433a6010000ab0100000000000000
-            006701ac05a6010000ab01000000000000000064379c036406640764389c
-            02ac09a6040000ab0400000000000000000200650365046a120000000000
-            000000020065066a0700000000000000006439a6010000ab010000000000
-            00000002006508020065066a070000000000000000643aa6010000ab0100
-            000000000000006701ac05a6010000ab0100000000000000000200650802
-            0065066a070000000000000000643ba6010000ab01000000000000000067
-            01ac05a6010000ab01000000000000000002006508020065066a07000000
-            00000000006436a6010000ab0100000000000000006701ac05a6010000ab
-            010000000000000000642e9c0364066407643c9c02ac09a6040000ab0400
-            0000000000000067125a136514643d6504643e6515650319000000000000
-            0000006604643f8404a6000000ab0000000000000000005a1664405300
-           8           0 RESUME                   0
+            08020065066a070000000000000000643ba6010000ab0100000000000000
+            006701ac05a6010000ab01000000000000000002006508020065066a0700
+            000000000000006436a6010000ab0100000000000000006701ac05a60100
+            00ab010000000000000000642e9c0364066407643c9c02ac09a6040000ab
+            04000000000000000067125a136514643d6504643e651565031900000000
+            00000000006604643f8404a6000000ab0000000000000000005a16644053
+            00
+           9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('VariableDetectionRules')
                        8 STORE_NAME               2 (__qualname__)
          
-          10          10 PUSH_NULL
+          11          10 PUSH_NULL
                       12 LOAD_NAME                3 (VaribleDetector)
          
-          11          14 LOAD_NAME                4 (Language)
+          12          14 LOAD_NAME                4 (Language)
                       16 LOAD_ATTR                5 (PYTHON)
          
-          12          26 PUSH_NULL
+          13          26 PUSH_NULL
                       28 LOAD_NAME                6 (re)
                       30 LOAD_ATTR                7 (compile)
                       40 LOAD_CONST               1 ('(n)(o|p)(?:\n?)(L)(?:\n|p|\\?)')
                       42 PRECALL                  1
                       46 CALL                     1
          
-          13          56 LOAD_CONST               2 (2)
+          14          56 LOAD_CONST               2 (2)
                       58 PUSH_NULL
                       60 LOAD_NAME                8 (Match)
                       62 LOAD_CONST               3 ('=')
                       64 LOAD_CONST               4 (':')
                       66 BUILD_LIST               2
                       68 KW_NAMES                 5
                       70 PRECALL                  1
                       74 CALL                     1
                       84 BUILD_MAP                1
          
-          14          86 LOAD_CONST               6 ('name')
+          15          86 LOAD_CONST               6 ('name')
                       88 LOAD_CONST               7 ('value')
                       90 LOAD_CONST               8 ((1, 3))
                       92 BUILD_CONST_KEY_MAP      2
          
-          10          94 KW_NAMES                 9
+          11          94 KW_NAMES                 9
                       96 PRECALL                  4
                      100 CALL                     4
          
-          16         110 PUSH_NULL
+          17         110 PUSH_NULL
                      112 LOAD_NAME                3 (VaribleDetector)
          
-          17         114 LOAD_NAME                4 (Language)
+          18         114 LOAD_NAME                4 (Language)
                      116 LOAD_ATTR                5 (PYTHON)
          
-          18         126 PUSH_NULL
+          19         126 PUSH_NULL
                      128 LOAD_NAME                6 (re)
                      130 LOAD_ATTR                7 (compile)
                      140 LOAD_CONST              10 ('(L)(p)(L)(?:p|\n)')
                      142 PRECALL                  1
                      146 CALL                     1
          
-          19         156 LOAD_CONST               2 (2)
+          20         156 LOAD_CONST               2 (2)
                      158 PUSH_NULL
                      160 LOAD_NAME                8 (Match)
                      162 LOAD_CONST               4 (':')
                      164 BUILD_LIST               1
                      166 KW_NAMES                 5
                      168 PRECALL                  1
                      172 CALL                     1
                      182 BUILD_MAP                1
          
-          20         184 LOAD_CONST               6 ('name')
+          21         184 LOAD_CONST               6 ('name')
                      186 LOAD_CONST               7 ('value')
                      188 LOAD_CONST               8 ((1, 3))
                      190 BUILD_CONST_KEY_MAP      2
          
-          16         192 KW_NAMES                 9
+          17         192 KW_NAMES                 9
                      194 PRECALL                  4
                      198 CALL                     4
          
-          22         208 PUSH_NULL
+          23         208 PUSH_NULL
                      210 LOAD_NAME                3 (VaribleDetector)
          
-          23         212 LOAD_NAME                4 (Language)
+          24         212 LOAD_NAME                4 (Language)
                      214 LOAD_ATTR                5 (PYTHON)
          
-          24         224 PUSH_NULL
+          25         224 PUSH_NULL
                      226 LOAD_NAME                6 (re)
                      228 LOAD_ATTR                7 (compile)
                      238 LOAD_CONST              11 ('(L)(p)(o)(L)')
                      240 PRECALL                  1
                      244 CALL                     1
          
-          25         254 PUSH_NULL
+          26         254 PUSH_NULL
                      256 LOAD_NAME                8 (Match)
                      258 LOAD_CONST              12 (']')
                      260 BUILD_LIST               1
                      262 KW_NAMES                 5
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PUSH_NULL
@@ -243,704 +266,705 @@
                      284 BUILD_LIST               1
                      286 KW_NAMES                 5
                      288 PRECALL                  1
                      292 CALL                     1
                      302 LOAD_CONST              13 ((2, 3))
                      304 BUILD_CONST_KEY_MAP      2
          
-          26         306 LOAD_CONST               6 ('name')
+          27         306 LOAD_CONST               6 ('name')
                      308 LOAD_CONST               7 ('value')
                      310 LOAD_CONST              14 ((1, 4))
                      312 BUILD_CONST_KEY_MAP      2
          
-          22         314 KW_NAMES                 9
+          23         314 KW_NAMES                 9
                      316 PRECALL                  4
                      320 CALL                     4
          
-          29         330 PUSH_NULL
+          30         330 PUSH_NULL
                      332 LOAD_NAME                3 (VaribleDetector)
          
-          30         334 LOAD_NAME                4 (Language)
+          31         334 LOAD_NAME                4 (Language)
                      336 LOAD_ATTR                9 (GOLANG)
          
-          31         346 PUSH_NULL
+          32         346 PUSH_NULL
                      348 LOAD_NAME                6 (re)
                      350 LOAD_ATTR                7 (compile)
                      360 LOAD_CONST              15 ('(n)(p)(L)(?:p|\n)?')
                      362 PRECALL                  1
                      366 CALL                     1
          
-          32         376 LOAD_CONST               2 (2)
+          33         376 LOAD_CONST               2 (2)
                      378 PUSH_NULL
                      380 LOAD_NAME                8 (Match)
                      382 LOAD_CONST               4 (':')
                      384 LOAD_CONST               3 ('=')
                      386 BUILD_LIST               2
                      388 KW_NAMES                 5
                      390 PRECALL                  1
                      394 CALL                     1
                      404 BUILD_MAP                1
          
-          33         406 LOAD_CONST               6 ('name')
+          34         406 LOAD_CONST               6 ('name')
                      408 LOAD_CONST               7 ('value')
                      410 LOAD_CONST               8 ((1, 3))
                      412 BUILD_CONST_KEY_MAP      2
          
-          29         414 KW_NAMES                 9
+          30         414 KW_NAMES                 9
                      416 PRECALL                  4
                      420 CALL                     4
          
-          35         430 PUSH_NULL
+          36         430 PUSH_NULL
                      432 LOAD_NAME                3 (VaribleDetector)
          
-          36         434 LOAD_NAME                4 (Language)
+          37         434 LOAD_NAME                4 (Language)
                      436 LOAD_ATTR                9 (GOLANG)
          
-          37         446 PUSH_NULL
+          38         446 PUSH_NULL
                      448 LOAD_NAME                6 (re)
                      450 LOAD_ATTR                7 (compile)
                      460 LOAD_CONST              16 ('(n)(p)(L)(?:p|\n)?(L)(p)')
                      462 PRECALL                  1
                      466 CALL                     1
          
-          39         476 PUSH_NULL
+          40         476 PUSH_NULL
                      478 LOAD_NAME                8 (Match)
                      480 LOAD_CONST              17 ('Setenv')
-                     482 BUILD_LIST               1
-                     484 KW_NAMES                 5
-                     486 PRECALL                  1
-                     490 CALL                     1
-         
-          40         500 PUSH_NULL
-                     502 LOAD_NAME                8 (Match)
-                     504 LOAD_CONST              18 ('(')
-                     506 BUILD_LIST               1
-                     508 KW_NAMES                 5
-                     510 PRECALL                  1
-                     514 CALL                     1
-         
-          41         524 PUSH_NULL
-                     526 LOAD_NAME                8 (Match)
-                     528 LOAD_CONST              19 (')')
-                     530 BUILD_LIST               1
-                     532 KW_NAMES                 5
-                     534 PRECALL                  1
-                     538 CALL                     1
-         
-          38         548 LOAD_CONST              20 ((1, 2, 5))
-                     550 BUILD_CONST_KEY_MAP      3
-         
-          43         552 LOAD_CONST               6 ('name')
-                     554 LOAD_CONST               7 ('value')
-                     556 LOAD_CONST              21 ((3, 4))
-                     558 BUILD_CONST_KEY_MAP      2
-         
-          35         560 KW_NAMES                 9
-                     562 PRECALL                  4
-                     566 CALL                     4
-         
-          45         576 PUSH_NULL
-                     578 LOAD_NAME                3 (VaribleDetector)
-         
-          46         580 LOAD_NAME                4 (Language)
-                     582 LOAD_ATTR                9 (GOLANG)
-         
-          47         592 PUSH_NULL
-                     594 LOAD_NAME                6 (re)
-                     596 LOAD_ATTR                7 (compile)
-                     606 LOAD_CONST              22 ('(n)(?:p|n|u)?(o)(n|p){0,5}(L)')
-                     608 PRECALL                  1
-                     612 CALL                     1
-         
-          49         622 PUSH_NULL
-                     624 LOAD_NAME                8 (Match)
-                     626 LOAD_CONST              23 (':=')
-                     628 BUILD_LIST               1
-                     630 KW_NAMES                 5
-                     632 PRECALL                  1
-                     636 CALL                     1
-         
-          50         646 PUSH_NULL
-                     648 LOAD_NAME                8 (Match)
-                     650 LOAD_CONST              24 ('Getenv')
-                     652 LOAD_CONST              17 ('Setenv')
-                     654 BUILD_LIST               2
-                     656 KW_NAMES                25
-                     658 PRECALL                  1
-                     662 CALL                     1
-         
-          48         672 LOAD_CONST              13 ((2, 3))
-                     674 BUILD_CONST_KEY_MAP      2
-         
-          52         676 LOAD_CONST               6 ('name')
-                     678 LOAD_CONST               7 ('value')
-                     680 LOAD_CONST              14 ((1, 4))
-                     682 BUILD_CONST_KEY_MAP      2
-         
-          45         684 KW_NAMES                 9
-                     686 PRECALL                  4
-                     690 CALL                     4
-         
-          54         700 PUSH_NULL
-                     702 LOAD_NAME                3 (VaribleDetector)
-         
-          55         704 LOAD_NAME                4 (Language)
-                     706 LOAD_ATTR                9 (GOLANG)
-         
-          56         716 PUSH_NULL
-                     718 LOAD_NAME                6 (re)
-                     720 LOAD_ATTR                7 (compile)
-                     730 LOAD_CONST              26 ('(n)(?:o|p){1,3}(\\?|u)p(L)p')
-                     732 PRECALL                  1
-                     736 CALL                     1
-         
-          57         746 LOAD_CONST               2 (2)
-                     748 PUSH_NULL
-                     750 LOAD_NAME                8 (Match)
-                     752 LOAD_CONST              27 ('byte')
-                     754 LOAD_CONST              28 ('string')
-                     756 BUILD_LIST               2
-                     758 KW_NAMES                 5
-                     760 PRECALL                  1
-                     764 CALL                     1
-                     774 BUILD_MAP                1
-         
-          58         776 LOAD_CONST               6 ('name')
-                     778 LOAD_CONST               7 ('value')
-                     780 LOAD_CONST               8 ((1, 3))
-                     782 BUILD_CONST_KEY_MAP      2
-         
-          54         784 KW_NAMES                 9
-                     786 PRECALL                  4
-                     790 CALL                     4
-         
-          61         800 PUSH_NULL
-                     802 LOAD_NAME                3 (VaribleDetector)
-         
-          62         804 LOAD_NAME                4 (Language)
-                     806 LOAD_ATTR               10 (PHP)
-         
-          63         816 PUSH_NULL
-                     818 LOAD_NAME                6 (re)
-                     820 LOAD_ATTR                7 (compile)
-                     830 LOAD_CONST              29 ('(n|v|L)(o)(L)')
-                     832 PRECALL                  1
-                     836 CALL                     1
-         
-          64         846 LOAD_CONST               2 (2)
-                     848 PUSH_NULL
-                     850 LOAD_NAME                8 (Match)
-                     852 LOAD_CONST               3 ('=')
-                     854 LOAD_CONST              30 ('=>')
-                     856 BUILD_LIST               2
-                     858 KW_NAMES                 5
-                     860 PRECALL                  1
-                     864 CALL                     1
-                     874 BUILD_MAP                1
-         
-          65         876 LOAD_CONST               6 ('name')
-                     878 LOAD_CONST               7 ('value')
-                     880 LOAD_CONST               8 ((1, 3))
-                     882 BUILD_CONST_KEY_MAP      2
-         
-          61         884 KW_NAMES                 9
-                     886 PRECALL                  4
-                     890 CALL                     4
-         
-          67         900 PUSH_NULL
-                     902 LOAD_NAME                3 (VaribleDetector)
-         
-          68         904 LOAD_NAME                4 (Language)
-                     906 LOAD_ATTR               10 (PHP)
-         
-          69         916 PUSH_NULL
-                     918 LOAD_NAME                6 (re)
-                     920 LOAD_ATTR                7 (compile)
-                     930 LOAD_CONST              31 ('(L)(o)(n)(p)Lp(L)p')
-                     932 PRECALL                  1
-                     936 CALL                     1
-         
-          71         946 PUSH_NULL
-                     948 LOAD_NAME                8 (Match)
-                     950 LOAD_CONST              30 ('=>')
-                     952 BUILD_LIST               1
-                     954 KW_NAMES                 5
-                     956 PRECALL                  1
-                     960 CALL                     1
-         
-          72         970 PUSH_NULL
-                     972 LOAD_NAME                8 (Match)
-                     974 LOAD_CONST              32 ('env')
-                     976 BUILD_LIST               1
-                     978 KW_NAMES                 5
-                     980 PRECALL                  1
-                     984 CALL                     1
-         
-          73         994 PUSH_NULL
-                     996 LOAD_NAME                8 (Match)
-                     998 LOAD_CONST              18 ('(')
-                    1000 BUILD_LIST               1
-                    1002 KW_NAMES                 5
-                    1004 PRECALL                  1
-                    1008 CALL                     1
-         
-          70        1018 LOAD_CONST              33 ((2, 3, 4))
-                    1020 BUILD_CONST_KEY_MAP      3
-         
-          75        1022 LOAD_CONST               6 ('name')
-                    1024 LOAD_CONST               7 ('value')
-                    1026 LOAD_CONST              34 ((1, 5))
-                    1028 BUILD_CONST_KEY_MAP      2
-         
-          67        1030 KW_NAMES                 9
-                    1032 PRECALL                  4
-                    1036 CALL                     4
-         
-          78        1046 PUSH_NULL
-                    1048 LOAD_NAME                3 (VaribleDetector)
-         
-          79        1050 LOAD_NAME                4 (Language)
-                    1052 LOAD_ATTR               11 (TOML)
-         
-          80        1062 PUSH_NULL
-                    1064 LOAD_NAME                6 (re)
-                    1066 LOAD_ATTR                7 (compile)
-                    1076 LOAD_CONST              35 ('(n)(o)(L)\n')
-                    1078 PRECALL                  1
-                    1082 CALL                     1
-         
-          81        1092 LOAD_CONST               2 (2)
-                    1094 PUSH_NULL
-                    1096 LOAD_NAME                8 (Match)
-                    1098 LOAD_CONST               3 ('=')
-                    1100 BUILD_LIST               1
-                    1102 KW_NAMES                 5
-                    1104 PRECALL                  1
-                    1108 CALL                     1
-                    1118 BUILD_MAP                1
-         
-          82        1120 LOAD_CONST               6 ('name')
-                    1122 LOAD_CONST               7 ('value')
-                    1124 LOAD_CONST               8 ((1, 3))
-                    1126 BUILD_CONST_KEY_MAP      2
-         
-          78        1128 KW_NAMES                 9
-                    1130 PRECALL                  4
-                    1134 CALL                     4
-         
-          84        1144 PUSH_NULL
-                    1146 LOAD_NAME                3 (VaribleDetector)
-         
-          85        1148 LOAD_NAME                4 (Language)
-                    1150 LOAD_ATTR               12 (YAML)
-         
-          86        1160 PUSH_NULL
-                    1162 LOAD_NAME                6 (re)
-                    1164 LOAD_ATTR                7 (compile)
-                    1174 LOAD_CONST              36 ('(L)(p)(L)')
-                    1176 PRECALL                  1
-                    1180 CALL                     1
-         
-          87        1190 LOAD_CONST               2 (2)
-                    1192 PUSH_NULL
-                    1194 LOAD_NAME                8 (Match)
-                    1196 LOAD_CONST               4 (':')
-                    1198 BUILD_LIST               1
-                    1200 KW_NAMES                 5
-                    1202 PRECALL                  1
-                    1206 CALL                     1
-                    1216 BUILD_MAP                1
-         
-          88        1218 LOAD_CONST               6 ('name')
-                    1220 LOAD_CONST               7 ('value')
-                    1222 LOAD_CONST               8 ((1, 3))
-                    1224 BUILD_CONST_KEY_MAP      2
-         
-          84        1226 KW_NAMES                 9
-                    1228 PRECALL                  4
-                    1232 CALL                     4
-         
-          90        1242 PUSH_NULL
-                    1244 LOAD_NAME                3 (VaribleDetector)
-         
-          91        1246 LOAD_NAME                4 (Language)
-                    1248 LOAD_ATTR               13 (INI)
-         
-          92        1258 PUSH_NULL
-                    1260 LOAD_NAME                6 (re)
-                    1262 LOAD_ATTR                7 (compile)
-                    1272 LOAD_CONST              37 ('(n)(o)(L)')
-                    1274 PRECALL                  1
-                    1278 CALL                     1
-         
-          93        1288 LOAD_CONST               2 (2)
-                    1290 PUSH_NULL
-                    1292 LOAD_NAME                8 (Match)
-                    1294 LOAD_CONST               3 ('=')
-                    1296 BUILD_LIST               1
-                    1298 KW_NAMES                 5
-                    1300 PRECALL                  1
-                    1304 CALL                     1
-                    1314 BUILD_MAP                1
-         
-          94        1316 LOAD_CONST               6 ('name')
-                    1318 LOAD_CONST               7 ('value')
-                    1320 LOAD_CONST               8 ((1, 3))
-                    1322 BUILD_CONST_KEY_MAP      2
-         
-          90        1324 KW_NAMES                 9
-                    1326 PRECALL                  4
-                    1330 CALL                     4
-         
-          96        1340 PUSH_NULL
-                    1342 LOAD_NAME                3 (VaribleDetector)
-         
-          97        1344 LOAD_NAME                4 (Language)
-                    1346 LOAD_ATTR               14 (PUPPET)
-         
-          98        1356 PUSH_NULL
-                    1358 LOAD_NAME                6 (re)
-                    1360 LOAD_ATTR                7 (compile)
-                    1370 LOAD_CONST              38 ('(v|n)(o)(L)')
-                    1372 PRECALL                  1
-                    1376 CALL                     1
-         
-          99        1386 LOAD_CONST               2 (2)
-                    1388 PUSH_NULL
-                    1390 LOAD_NAME                8 (Match)
-                    1392 LOAD_CONST              30 ('=>')
-                    1394 LOAD_CONST               3 ('=')
-                    1396 BUILD_LIST               2
-                    1398 KW_NAMES                 5
-                    1400 PRECALL                  1
-                    1404 CALL                     1
-                    1414 BUILD_MAP                1
-         
-         100        1416 LOAD_CONST               6 ('name')
-                    1418 LOAD_CONST               7 ('value')
-                    1420 LOAD_CONST               8 ((1, 3))
-                    1422 BUILD_CONST_KEY_MAP      2
-         
-          96        1424 KW_NAMES                 9
-                    1426 PRECALL                  4
-                    1430 CALL                     4
-         
-         102        1440 PUSH_NULL
-                    1442 LOAD_NAME                3 (VaribleDetector)
-         
-         103        1444 LOAD_NAME                4 (Language)
-                    1446 LOAD_ATTR               15 (ANY)
-         
-         104        1456 PUSH_NULL
-                    1458 LOAD_NAME                6 (re)
-                    1460 LOAD_ATTR                7 (compile)
-                    1470 LOAD_CONST              39 ('(v|n)(p|o)(L)')
-                    1472 PRECALL                  1
-                    1476 CALL                     1
-         
-         106        1486 LOAD_CONST               2 (2)
-                    1488 PUSH_NULL
-                    1490 LOAD_NAME                8 (Match)
-         
-         107        1492 PUSH_NULL
-                    1494 LOAD_NAME                6 (re)
-                    1496 LOAD_ATTR                7 (compile)
-                    1506 LOAD_CONST              40 ('^:$')
-                    1508 PRECALL                  1
-                    1512 CALL                     1
-         
-         108        1522 PUSH_NULL
-                    1524 LOAD_NAME                6 (re)
-                    1526 LOAD_ATTR                7 (compile)
-                    1536 LOAD_CONST              41 ('^=$')
-                    1538 PRECALL                  1
-                    1542 CALL                     1
-         
-         106        1552 BUILD_LIST               2
-                    1554 KW_NAMES                 5
-                    1556 PRECALL                  1
-                    1560 CALL                     1
-         
-         105        1570 BUILD_MAP                1
-         
-         110        1572 LOAD_CONST               6 ('name')
-                    1574 LOAD_CONST               7 ('value')
-                    1576 LOAD_CONST               8 ((1, 3))
-                    1578 BUILD_CONST_KEY_MAP      2
-         
-         102        1580 KW_NAMES                 9
-                    1582 PRECALL                  4
-                    1586 CALL                     4
-         
-         112        1596 PUSH_NULL
-                    1598 LOAD_NAME                3 (VaribleDetector)
-         
-         113        1600 LOAD_NAME                4 (Language)
-                    1602 LOAD_ATTR               16 (SHELL)
-         
-         114        1612 PUSH_NULL
-                    1614 LOAD_NAME                6 (re)
-                    1616 LOAD_ATTR                7 (compile)
-                    1626 LOAD_CONST              42 ('(L)(L)(L)(L)')
-                    1628 PRECALL                  1
-                    1632 CALL                     1
-         
-         116        1642 PUSH_NULL
-                    1644 LOAD_NAME                8 (Match)
-                    1646 PUSH_NULL
-                    1648 LOAD_NAME                6 (re)
-                    1650 LOAD_ATTR                7 (compile)
-                    1660 LOAD_CONST              43 ('^curl$')
-                    1662 PRECALL                  1
-                    1666 CALL                     1
-                    1676 BUILD_LIST               1
-                    1678 KW_NAMES                 5
-                    1680 PRECALL                  1
-                    1684 CALL                     1
-         
-         117        1694 PUSH_NULL
-                    1696 LOAD_NAME                8 (Match)
-                    1698 PUSH_NULL
-                    1700 LOAD_NAME                6 (re)
-                    1702 LOAD_ATTR                7 (compile)
-                    1712 LOAD_CONST              44 ('^-u$')
-                    1714 PRECALL                  1
-                    1718 CALL                     1
-                    1728 BUILD_LIST               1
-                    1730 KW_NAMES                 5
-                    1732 PRECALL                  1
-                    1736 CALL                     1
-         
-         118        1746 PUSH_NULL
-                    1748 LOAD_NAME                8 (Match)
-                    1750 PUSH_NULL
-                    1752 LOAD_NAME                6 (re)
-                    1754 LOAD_ATTR                7 (compile)
-                    1764 LOAD_CONST              45 ('^\\$')
-                    1766 PRECALL                  1
-                    1770 CALL                     1
-                    1780 BUILD_LIST               1
-                    1782 KW_NAMES                25
-                    1784 PRECALL                  1
-                    1788 CALL                     1
-         
-         115        1798 LOAD_CONST              46 ((1, 2, 4))
-                    1800 BUILD_CONST_KEY_MAP      3
-         
-         120        1802 LOAD_CONST               6 ('name')
-                    1804 LOAD_CONST               7 ('value')
-                    1806 LOAD_CONST              21 ((3, 4))
-                    1808 BUILD_CONST_KEY_MAP      2
-         
-         121        1810 LOAD_CONST              47 (9)
-         
-         112        1812 KW_NAMES                48
-                    1814 PRECALL                  5
-                    1818 CALL                     5
-         
-         124        1828 PUSH_NULL
-                    1830 LOAD_NAME                3 (VaribleDetector)
-         
-         125        1832 LOAD_NAME                4 (Language)
-                    1834 LOAD_ATTR               17 (CSHARP)
-         
-         126        1844 PUSH_NULL
-                    1846 LOAD_NAME                6 (re)
-                    1848 LOAD_ATTR                7 (compile)
-                    1858 LOAD_CONST              49 ('(n).{0,6}(u|L)p(L)(p)')
-                    1860 PRECALL                  1
-                    1864 CALL                     1
-         
-         128        1874 PUSH_NULL
-                    1876 LOAD_NAME                8 (Match)
-                    1878 PUSH_NULL
-                    1880 LOAD_NAME                6 (re)
-                    1882 LOAD_ATTR                7 (compile)
-                    1892 LOAD_CONST              50 ('^KeyValuePair$')
-                    1894 PRECALL                  1
-                    1898 CALL                     1
-                    1908 BUILD_LIST               1
-                    1910 KW_NAMES                 5
-                    1912 PRECALL                  1
-                    1916 CALL                     1
-         
-         129        1926 PUSH_NULL
-                    1928 LOAD_NAME                8 (Match)
-                    1930 PUSH_NULL
-                    1932 LOAD_NAME                6 (re)
-                    1934 LOAD_ATTR                7 (compile)
-                    1944 LOAD_CONST              51 ('^}$')
-                    1946 PRECALL                  1
-                    1950 CALL                     1
-                    1960 BUILD_LIST               1
-                    1962 KW_NAMES                25
-                    1964 PRECALL                  1
-                    1968 CALL                     1
-         
-         127        1978 LOAD_CONST              14 ((1, 4))
-                    1980 BUILD_CONST_KEY_MAP      2
-         
-         131        1982 LOAD_CONST               6 ('name')
-                    1984 LOAD_CONST               7 ('value')
-                    1986 LOAD_CONST              13 ((2, 3))
-                    1988 BUILD_CONST_KEY_MAP      2
-         
-         124        1990 KW_NAMES                 9
-                    1992 PRECALL                  4
-                    1996 CALL                     4
-         
-         134        2006 PUSH_NULL
-                    2008 LOAD_NAME                3 (VaribleDetector)
-         
-         135        2010 LOAD_NAME                4 (Language)
-                    2012 LOAD_ATTR               17 (CSHARP)
-         
-         136        2022 PUSH_NULL
-                    2024 LOAD_NAME                6 (re)
-                    2026 LOAD_ATTR                7 (compile)
-                    2036 LOAD_CONST              52 ('(p)(.)(p)(L)(p)')
-                    2038 PRECALL                  1
-                    2042 CALL                     1
-         
-         138        2052 PUSH_NULL
-                    2054 LOAD_NAME                8 (Match)
-                    2056 PUSH_NULL
-                    2058 LOAD_NAME                6 (re)
-                    2060 LOAD_ATTR                7 (compile)
-                    2070 LOAD_CONST              53 ('^{$')
-                    2072 PRECALL                  1
-                    2076 CALL                     1
-                    2086 BUILD_LIST               1
-                    2088 KW_NAMES                 5
-                    2090 PRECALL                  1
-                    2094 CALL                     1
-         
-         139        2104 PUSH_NULL
-                    2106 LOAD_NAME                8 (Match)
-                    2108 PUSH_NULL
-                    2110 LOAD_NAME                6 (re)
-                    2112 LOAD_ATTR                7 (compile)
-                    2122 LOAD_CONST              54 ('^,$')
-                    2124 PRECALL                  1
-                    2128 CALL                     1
-                    2138 BUILD_LIST               1
-                    2140 KW_NAMES                 5
-                    2142 PRECALL                  1
-                    2146 CALL                     1
-         
-         140        2156 PUSH_NULL
-                    2158 LOAD_NAME                8 (Match)
-                    2160 PUSH_NULL
-                    2162 LOAD_NAME                6 (re)
-                    2164 LOAD_ATTR                7 (compile)
-                    2174 LOAD_CONST              51 ('^}$')
-                    2176 PRECALL                  1
-                    2180 CALL                     1
-                    2190 BUILD_LIST               1
-                    2192 KW_NAMES                 5
-                    2194 PRECALL                  1
-                    2198 CALL                     1
-         
-         137        2208 LOAD_CONST              55 ((1, 3, 5))
-                    2210 BUILD_CONST_KEY_MAP      3
-         
-         142        2212 LOAD_CONST               6 ('name')
-                    2214 LOAD_CONST               7 ('value')
-                    2216 LOAD_CONST              56 ((2, 4))
-                    2218 BUILD_CONST_KEY_MAP      2
-         
-         134        2220 KW_NAMES                 9
-                    2222 PRECALL                  4
-                    2226 CALL                     4
-         
-         145        2236 PUSH_NULL
-                    2238 LOAD_NAME                3 (VaribleDetector)
-         
-         146        2240 LOAD_NAME                4 (Language)
-                    2242 LOAD_ATTR               18 (JAVA)
-         
-         147        2252 PUSH_NULL
-                    2254 LOAD_NAME                6 (re)
-                    2256 LOAD_ATTR                7 (compile)
-                    2266 LOAD_CONST              57 ('(n)(p)(.)(p)(L)')
-                    2268 PRECALL                  1
-                    2272 CALL                     1
-         
-         149        2282 PUSH_NULL
-                    2284 LOAD_NAME                8 (Match)
-                    2286 PUSH_NULL
-                    2288 LOAD_NAME                6 (re)
-                    2290 LOAD_ATTR                7 (compile)
-                    2300 LOAD_CONST              58 ('^put$')
-                    2302 PRECALL                  1
-                    2306 CALL                     1
-                    2316 BUILD_LIST               1
-                    2318 KW_NAMES                 5
-                    2320 PRECALL                  1
-                    2324 CALL                     1
-         
-         150        2334 PUSH_NULL
-                    2336 LOAD_NAME                8 (Match)
-                    2338 PUSH_NULL
-                    2340 LOAD_NAME                6 (re)
-                    2342 LOAD_ATTR                7 (compile)
-                    2352 LOAD_CONST              59 ('^\\($')
-                    2354 PRECALL                  1
-                    2358 CALL                     1
-                    2368 BUILD_LIST               1
-                    2370 KW_NAMES                 5
-                    2372 PRECALL                  1
-                    2376 CALL                     1
-         
-         151        2386 PUSH_NULL
-                    2388 LOAD_NAME                8 (Match)
-                    2390 PUSH_NULL
-                    2392 LOAD_NAME                6 (re)
-                    2394 LOAD_ATTR                7 (compile)
-                    2404 LOAD_CONST              54 ('^,$')
-                    2406 PRECALL                  1
-                    2410 CALL                     1
-                    2420 BUILD_LIST               1
-                    2422 KW_NAMES                 5
-                    2424 PRECALL                  1
-                    2428 CALL                     1
-         
-         148        2438 LOAD_CONST              46 ((1, 2, 4))
-                    2440 BUILD_CONST_KEY_MAP      3
-         
-         153        2442 LOAD_CONST               6 ('name')
-                    2444 LOAD_CONST               7 ('value')
-                    2446 LOAD_CONST              60 ((3, 5))
-                    2448 BUILD_CONST_KEY_MAP      2
-         
-         145        2450 KW_NAMES                 9
-                    2452 PRECALL                  4
-                    2456 CALL                     4
-         
-           9        2466 BUILD_LIST              18
-                    2468 STORE_NAME              19 (rules)
-         
-         158        2470 LOAD_NAME               20 (classmethod)
-         
-         159        2472 LOAD_CONST              61 ('language')
-                    2474 LOAD_NAME                4 (Language)
-                    2476 LOAD_CONST              62 ('return')
-                    2478 LOAD_NAME               21 (List)
-                    2480 LOAD_NAME                3 (VaribleDetector)
-                    2482 BINARY_SUBSCR
-                    2492 BUILD_TUPLE              4
-                    2494 LOAD_CONST              63 (<code object for_language, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 158>)
-                    2496 MAKE_FUNCTION            4 (annotations)
-         
-         158        2498 PRECALL                  0
-                    2502 CALL                     0
-         
-         159        2512 STORE_NAME              22 (for_language)
-                    2514 LOAD_CONST              64 (None)
-                    2516 RETURN_VALUE
+                     482 LOAD_CONST              18 ('Getenv')
+                     484 BUILD_LIST               2
+                     486 KW_NAMES                 5
+                     488 PRECALL                  1
+                     492 CALL                     1
+         
+          41         502 PUSH_NULL
+                     504 LOAD_NAME                8 (Match)
+                     506 LOAD_CONST              19 ('(')
+                     508 BUILD_LIST               1
+                     510 KW_NAMES                 5
+                     512 PRECALL                  1
+                     516 CALL                     1
+         
+          42         526 PUSH_NULL
+                     528 LOAD_NAME                8 (Match)
+                     530 LOAD_CONST              20 (')')
+                     532 BUILD_LIST               1
+                     534 KW_NAMES                 5
+                     536 PRECALL                  1
+                     540 CALL                     1
+         
+          39         550 LOAD_CONST              21 ((1, 2, 5))
+                     552 BUILD_CONST_KEY_MAP      3
+         
+          44         554 LOAD_CONST               6 ('name')
+                     556 LOAD_CONST               7 ('value')
+                     558 LOAD_CONST              22 ((3, 4))
+                     560 BUILD_CONST_KEY_MAP      2
+         
+          36         562 KW_NAMES                 9
+                     564 PRECALL                  4
+                     568 CALL                     4
+         
+          47         578 PUSH_NULL
+                     580 LOAD_NAME                3 (VaribleDetector)
+         
+          48         582 LOAD_NAME                4 (Language)
+                     584 LOAD_ATTR                9 (GOLANG)
+         
+          49         594 PUSH_NULL
+                     596 LOAD_NAME                6 (re)
+                     598 LOAD_ATTR                7 (compile)
+                     608 LOAD_CONST              23 ('(n)(?:p|n|u){0,3}?(o).*(n)(p)(L)')
+                     610 PRECALL                  1
+                     614 CALL                     1
+         
+          51         624 PUSH_NULL
+                     626 LOAD_NAME                8 (Match)
+                     628 LOAD_CONST              24 (':=')
+                     630 BUILD_LIST               1
+                     632 KW_NAMES                 5
+                     634 PRECALL                  1
+                     638 CALL                     1
+         
+          52         648 PUSH_NULL
+                     650 LOAD_NAME                8 (Match)
+                     652 LOAD_CONST              18 ('Getenv')
+                     654 LOAD_CONST              17 ('Setenv')
+                     656 BUILD_LIST               2
+                     658 KW_NAMES                25
+                     660 PRECALL                  1
+                     664 CALL                     1
+         
+          50         674 LOAD_CONST              13 ((2, 3))
+                     676 BUILD_CONST_KEY_MAP      2
+         
+          54         678 LOAD_CONST               6 ('name')
+                     680 LOAD_CONST               7 ('value')
+                     682 LOAD_CONST              26 ((1, 5))
+                     684 BUILD_CONST_KEY_MAP      2
+         
+          47         686 KW_NAMES                 9
+                     688 PRECALL                  4
+                     692 CALL                     4
+         
+          57         702 PUSH_NULL
+                     704 LOAD_NAME                3 (VaribleDetector)
+         
+          58         706 LOAD_NAME                4 (Language)
+                     708 LOAD_ATTR                9 (GOLANG)
+         
+          59         718 PUSH_NULL
+                     720 LOAD_NAME                6 (re)
+                     722 LOAD_ATTR                7 (compile)
+                     732 LOAD_CONST              27 ('(n)(?:o|p){1,3}(\\?|u)p(L)p')
+                     734 PRECALL                  1
+                     738 CALL                     1
+         
+          60         748 LOAD_CONST               2 (2)
+                     750 PUSH_NULL
+                     752 LOAD_NAME                8 (Match)
+                     754 LOAD_CONST              28 ('byte')
+                     756 LOAD_CONST              29 ('string')
+                     758 BUILD_LIST               2
+                     760 KW_NAMES                 5
+                     762 PRECALL                  1
+                     766 CALL                     1
+                     776 BUILD_MAP                1
+         
+          61         778 LOAD_CONST               6 ('name')
+                     780 LOAD_CONST               7 ('value')
+                     782 LOAD_CONST               8 ((1, 3))
+                     784 BUILD_CONST_KEY_MAP      2
+         
+          57         786 KW_NAMES                 9
+                     788 PRECALL                  4
+                     792 CALL                     4
+         
+          64         802 PUSH_NULL
+                     804 LOAD_NAME                3 (VaribleDetector)
+         
+          65         806 LOAD_NAME                4 (Language)
+                     808 LOAD_ATTR               10 (PHP)
+         
+          66         818 PUSH_NULL
+                     820 LOAD_NAME                6 (re)
+                     822 LOAD_ATTR                7 (compile)
+                     832 LOAD_CONST              30 ('(n|v|L)(o)(L)')
+                     834 PRECALL                  1
+                     838 CALL                     1
+         
+          67         848 LOAD_CONST               2 (2)
+                     850 PUSH_NULL
+                     852 LOAD_NAME                8 (Match)
+                     854 LOAD_CONST               3 ('=')
+                     856 LOAD_CONST              31 ('=>')
+                     858 BUILD_LIST               2
+                     860 KW_NAMES                 5
+                     862 PRECALL                  1
+                     866 CALL                     1
+                     876 BUILD_MAP                1
+         
+          68         878 LOAD_CONST               6 ('name')
+                     880 LOAD_CONST               7 ('value')
+                     882 LOAD_CONST               8 ((1, 3))
+                     884 BUILD_CONST_KEY_MAP      2
+         
+          64         886 KW_NAMES                 9
+                     888 PRECALL                  4
+                     892 CALL                     4
+         
+          70         902 PUSH_NULL
+                     904 LOAD_NAME                3 (VaribleDetector)
+         
+          71         906 LOAD_NAME                4 (Language)
+                     908 LOAD_ATTR               10 (PHP)
+         
+          72         918 PUSH_NULL
+                     920 LOAD_NAME                6 (re)
+                     922 LOAD_ATTR                7 (compile)
+                     932 LOAD_CONST              32 ('(L)(o)(n)(p)Lp(L)p')
+                     934 PRECALL                  1
+                     938 CALL                     1
+         
+          74         948 PUSH_NULL
+                     950 LOAD_NAME                8 (Match)
+                     952 LOAD_CONST              31 ('=>')
+                     954 BUILD_LIST               1
+                     956 KW_NAMES                 5
+                     958 PRECALL                  1
+                     962 CALL                     1
+         
+          75         972 PUSH_NULL
+                     974 LOAD_NAME                8 (Match)
+                     976 LOAD_CONST              33 ('env')
+                     978 BUILD_LIST               1
+                     980 KW_NAMES                 5
+                     982 PRECALL                  1
+                     986 CALL                     1
+         
+          76         996 PUSH_NULL
+                     998 LOAD_NAME                8 (Match)
+                    1000 LOAD_CONST              19 ('(')
+                    1002 BUILD_LIST               1
+                    1004 KW_NAMES                 5
+                    1006 PRECALL                  1
+                    1010 CALL                     1
+         
+          73        1020 LOAD_CONST              34 ((2, 3, 4))
+                    1022 BUILD_CONST_KEY_MAP      3
+         
+          78        1024 LOAD_CONST               6 ('name')
+                    1026 LOAD_CONST               7 ('value')
+                    1028 LOAD_CONST              26 ((1, 5))
+                    1030 BUILD_CONST_KEY_MAP      2
+         
+          70        1032 KW_NAMES                 9
+                    1034 PRECALL                  4
+                    1038 CALL                     4
+         
+          81        1048 PUSH_NULL
+                    1050 LOAD_NAME                3 (VaribleDetector)
+         
+          82        1052 LOAD_NAME                4 (Language)
+                    1054 LOAD_ATTR               11 (TOML)
+         
+          83        1064 PUSH_NULL
+                    1066 LOAD_NAME                6 (re)
+                    1068 LOAD_ATTR                7 (compile)
+                    1078 LOAD_CONST              35 ('(n)(o)(L)\n')
+                    1080 PRECALL                  1
+                    1084 CALL                     1
+         
+          84        1094 LOAD_CONST               2 (2)
+                    1096 PUSH_NULL
+                    1098 LOAD_NAME                8 (Match)
+                    1100 LOAD_CONST               3 ('=')
+                    1102 BUILD_LIST               1
+                    1104 KW_NAMES                 5
+                    1106 PRECALL                  1
+                    1110 CALL                     1
+                    1120 BUILD_MAP                1
+         
+          85        1122 LOAD_CONST               6 ('name')
+                    1124 LOAD_CONST               7 ('value')
+                    1126 LOAD_CONST               8 ((1, 3))
+                    1128 BUILD_CONST_KEY_MAP      2
+         
+          81        1130 KW_NAMES                 9
+                    1132 PRECALL                  4
+                    1136 CALL                     4
+         
+          87        1146 PUSH_NULL
+                    1148 LOAD_NAME                3 (VaribleDetector)
+         
+          88        1150 LOAD_NAME                4 (Language)
+                    1152 LOAD_ATTR               12 (YAML)
+         
+          89        1162 PUSH_NULL
+                    1164 LOAD_NAME                6 (re)
+                    1166 LOAD_ATTR                7 (compile)
+                    1176 LOAD_CONST              36 ('(L)(p)(L)')
+                    1178 PRECALL                  1
+                    1182 CALL                     1
+         
+          90        1192 LOAD_CONST               2 (2)
+                    1194 PUSH_NULL
+                    1196 LOAD_NAME                8 (Match)
+                    1198 LOAD_CONST               4 (':')
+                    1200 BUILD_LIST               1
+                    1202 KW_NAMES                 5
+                    1204 PRECALL                  1
+                    1208 CALL                     1
+                    1218 BUILD_MAP                1
+         
+          91        1220 LOAD_CONST               6 ('name')
+                    1222 LOAD_CONST               7 ('value')
+                    1224 LOAD_CONST               8 ((1, 3))
+                    1226 BUILD_CONST_KEY_MAP      2
+         
+          87        1228 KW_NAMES                 9
+                    1230 PRECALL                  4
+                    1234 CALL                     4
+         
+          93        1244 PUSH_NULL
+                    1246 LOAD_NAME                3 (VaribleDetector)
+         
+          94        1248 LOAD_NAME                4 (Language)
+                    1250 LOAD_ATTR               13 (INI)
+         
+          95        1260 PUSH_NULL
+                    1262 LOAD_NAME                6 (re)
+                    1264 LOAD_ATTR                7 (compile)
+                    1274 LOAD_CONST              37 ('(n)(o)(L)')
+                    1276 PRECALL                  1
+                    1280 CALL                     1
+         
+          96        1290 LOAD_CONST               2 (2)
+                    1292 PUSH_NULL
+                    1294 LOAD_NAME                8 (Match)
+                    1296 LOAD_CONST               3 ('=')
+                    1298 BUILD_LIST               1
+                    1300 KW_NAMES                 5
+                    1302 PRECALL                  1
+                    1306 CALL                     1
+                    1316 BUILD_MAP                1
+         
+          97        1318 LOAD_CONST               6 ('name')
+                    1320 LOAD_CONST               7 ('value')
+                    1322 LOAD_CONST               8 ((1, 3))
+                    1324 BUILD_CONST_KEY_MAP      2
+         
+          93        1326 KW_NAMES                 9
+                    1328 PRECALL                  4
+                    1332 CALL                     4
+         
+          99        1342 PUSH_NULL
+                    1344 LOAD_NAME                3 (VaribleDetector)
+         
+         100        1346 LOAD_NAME                4 (Language)
+                    1348 LOAD_ATTR               14 (PUPPET)
+         
+         101        1358 PUSH_NULL
+                    1360 LOAD_NAME                6 (re)
+                    1362 LOAD_ATTR                7 (compile)
+                    1372 LOAD_CONST              38 ('(v|n)(o)(L)')
+                    1374 PRECALL                  1
+                    1378 CALL                     1
+         
+         102        1388 LOAD_CONST               2 (2)
+                    1390 PUSH_NULL
+                    1392 LOAD_NAME                8 (Match)
+                    1394 LOAD_CONST              31 ('=>')
+                    1396 LOAD_CONST               3 ('=')
+                    1398 BUILD_LIST               2
+                    1400 KW_NAMES                 5
+                    1402 PRECALL                  1
+                    1406 CALL                     1
+                    1416 BUILD_MAP                1
+         
+         103        1418 LOAD_CONST               6 ('name')
+                    1420 LOAD_CONST               7 ('value')
+                    1422 LOAD_CONST               8 ((1, 3))
+                    1424 BUILD_CONST_KEY_MAP      2
+         
+          99        1426 KW_NAMES                 9
+                    1428 PRECALL                  4
+                    1432 CALL                     4
+         
+         105        1442 PUSH_NULL
+                    1444 LOAD_NAME                3 (VaribleDetector)
+         
+         106        1446 LOAD_NAME                4 (Language)
+                    1448 LOAD_ATTR               15 (ANY)
+         
+         107        1458 PUSH_NULL
+                    1460 LOAD_NAME                6 (re)
+                    1462 LOAD_ATTR                7 (compile)
+                    1472 LOAD_CONST              39 ('(v|n)(p|o)(L)')
+                    1474 PRECALL                  1
+                    1478 CALL                     1
+         
+         109        1488 LOAD_CONST               2 (2)
+                    1490 PUSH_NULL
+                    1492 LOAD_NAME                8 (Match)
+         
+         110        1494 PUSH_NULL
+                    1496 LOAD_NAME                6 (re)
+                    1498 LOAD_ATTR                7 (compile)
+                    1508 LOAD_CONST              40 ('^:$')
+                    1510 PRECALL                  1
+                    1514 CALL                     1
+         
+         111        1524 PUSH_NULL
+                    1526 LOAD_NAME                6 (re)
+                    1528 LOAD_ATTR                7 (compile)
+                    1538 LOAD_CONST              41 ('^=$')
+                    1540 PRECALL                  1
+                    1544 CALL                     1
+         
+         109        1554 BUILD_LIST               2
+                    1556 KW_NAMES                 5
+                    1558 PRECALL                  1
+                    1562 CALL                     1
+         
+         108        1572 BUILD_MAP                1
+         
+         113        1574 LOAD_CONST               6 ('name')
+                    1576 LOAD_CONST               7 ('value')
+                    1578 LOAD_CONST               8 ((1, 3))
+                    1580 BUILD_CONST_KEY_MAP      2
+         
+         105        1582 KW_NAMES                 9
+                    1584 PRECALL                  4
+                    1588 CALL                     4
+         
+         115        1598 PUSH_NULL
+                    1600 LOAD_NAME                3 (VaribleDetector)
+         
+         116        1602 LOAD_NAME                4 (Language)
+                    1604 LOAD_ATTR               16 (SHELL)
+         
+         117        1614 PUSH_NULL
+                    1616 LOAD_NAME                6 (re)
+                    1618 LOAD_ATTR                7 (compile)
+                    1628 LOAD_CONST              42 ('(L)(L)(L)(L)')
+                    1630 PRECALL                  1
+                    1634 CALL                     1
+         
+         119        1644 PUSH_NULL
+                    1646 LOAD_NAME                8 (Match)
+                    1648 PUSH_NULL
+                    1650 LOAD_NAME                6 (re)
+                    1652 LOAD_ATTR                7 (compile)
+                    1662 LOAD_CONST              43 ('^curl$')
+                    1664 PRECALL                  1
+                    1668 CALL                     1
+                    1678 BUILD_LIST               1
+                    1680 KW_NAMES                 5
+                    1682 PRECALL                  1
+                    1686 CALL                     1
+         
+         120        1696 PUSH_NULL
+                    1698 LOAD_NAME                8 (Match)
+                    1700 PUSH_NULL
+                    1702 LOAD_NAME                6 (re)
+                    1704 LOAD_ATTR                7 (compile)
+                    1714 LOAD_CONST              44 ('^-u$')
+                    1716 PRECALL                  1
+                    1720 CALL                     1
+                    1730 BUILD_LIST               1
+                    1732 KW_NAMES                 5
+                    1734 PRECALL                  1
+                    1738 CALL                     1
+         
+         121        1748 PUSH_NULL
+                    1750 LOAD_NAME                8 (Match)
+                    1752 PUSH_NULL
+                    1754 LOAD_NAME                6 (re)
+                    1756 LOAD_ATTR                7 (compile)
+                    1766 LOAD_CONST              45 ('^\\$')
+                    1768 PRECALL                  1
+                    1772 CALL                     1
+                    1782 BUILD_LIST               1
+                    1784 KW_NAMES                25
+                    1786 PRECALL                  1
+                    1790 CALL                     1
+         
+         118        1800 LOAD_CONST              46 ((1, 2, 4))
+                    1802 BUILD_CONST_KEY_MAP      3
+         
+         123        1804 LOAD_CONST               6 ('name')
+                    1806 LOAD_CONST               7 ('value')
+                    1808 LOAD_CONST              22 ((3, 4))
+                    1810 BUILD_CONST_KEY_MAP      2
+         
+         124        1812 LOAD_CONST              47 (9)
+         
+         115        1814 KW_NAMES                48
+                    1816 PRECALL                  5
+                    1820 CALL                     5
+         
+         127        1830 PUSH_NULL
+                    1832 LOAD_NAME                3 (VaribleDetector)
+         
+         128        1834 LOAD_NAME                4 (Language)
+                    1836 LOAD_ATTR               17 (CSHARP)
+         
+         129        1846 PUSH_NULL
+                    1848 LOAD_NAME                6 (re)
+                    1850 LOAD_ATTR                7 (compile)
+                    1860 LOAD_CONST              49 ('(n).{0,6}(u|L)p(L)(p)')
+                    1862 PRECALL                  1
+                    1866 CALL                     1
+         
+         131        1876 PUSH_NULL
+                    1878 LOAD_NAME                8 (Match)
+                    1880 PUSH_NULL
+                    1882 LOAD_NAME                6 (re)
+                    1884 LOAD_ATTR                7 (compile)
+                    1894 LOAD_CONST              50 ('^KeyValuePair$')
+                    1896 PRECALL                  1
+                    1900 CALL                     1
+                    1910 BUILD_LIST               1
+                    1912 KW_NAMES                 5
+                    1914 PRECALL                  1
+                    1918 CALL                     1
+         
+         132        1928 PUSH_NULL
+                    1930 LOAD_NAME                8 (Match)
+                    1932 PUSH_NULL
+                    1934 LOAD_NAME                6 (re)
+                    1936 LOAD_ATTR                7 (compile)
+                    1946 LOAD_CONST              51 ('^}$')
+                    1948 PRECALL                  1
+                    1952 CALL                     1
+                    1962 BUILD_LIST               1
+                    1964 KW_NAMES                25
+                    1966 PRECALL                  1
+                    1970 CALL                     1
+         
+         130        1980 LOAD_CONST              14 ((1, 4))
+                    1982 BUILD_CONST_KEY_MAP      2
+         
+         134        1984 LOAD_CONST               6 ('name')
+                    1986 LOAD_CONST               7 ('value')
+                    1988 LOAD_CONST              13 ((2, 3))
+                    1990 BUILD_CONST_KEY_MAP      2
+         
+         127        1992 KW_NAMES                 9
+                    1994 PRECALL                  4
+                    1998 CALL                     4
+         
+         137        2008 PUSH_NULL
+                    2010 LOAD_NAME                3 (VaribleDetector)
+         
+         138        2012 LOAD_NAME                4 (Language)
+                    2014 LOAD_ATTR               17 (CSHARP)
+         
+         139        2024 PUSH_NULL
+                    2026 LOAD_NAME                6 (re)
+                    2028 LOAD_ATTR                7 (compile)
+                    2038 LOAD_CONST              52 ('(p)(.)(p)(L)(p)')
+                    2040 PRECALL                  1
+                    2044 CALL                     1
+         
+         141        2054 PUSH_NULL
+                    2056 LOAD_NAME                8 (Match)
+                    2058 PUSH_NULL
+                    2060 LOAD_NAME                6 (re)
+                    2062 LOAD_ATTR                7 (compile)
+                    2072 LOAD_CONST              53 ('^{$')
+                    2074 PRECALL                  1
+                    2078 CALL                     1
+                    2088 BUILD_LIST               1
+                    2090 KW_NAMES                 5
+                    2092 PRECALL                  1
+                    2096 CALL                     1
+         
+         142        2106 PUSH_NULL
+                    2108 LOAD_NAME                8 (Match)
+                    2110 PUSH_NULL
+                    2112 LOAD_NAME                6 (re)
+                    2114 LOAD_ATTR                7 (compile)
+                    2124 LOAD_CONST              54 ('^,$')
+                    2126 PRECALL                  1
+                    2130 CALL                     1
+                    2140 BUILD_LIST               1
+                    2142 KW_NAMES                 5
+                    2144 PRECALL                  1
+                    2148 CALL                     1
+         
+         143        2158 PUSH_NULL
+                    2160 LOAD_NAME                8 (Match)
+                    2162 PUSH_NULL
+                    2164 LOAD_NAME                6 (re)
+                    2166 LOAD_ATTR                7 (compile)
+                    2176 LOAD_CONST              51 ('^}$')
+                    2178 PRECALL                  1
+                    2182 CALL                     1
+                    2192 BUILD_LIST               1
+                    2194 KW_NAMES                 5
+                    2196 PRECALL                  1
+                    2200 CALL                     1
+         
+         140        2210 LOAD_CONST              55 ((1, 3, 5))
+                    2212 BUILD_CONST_KEY_MAP      3
+         
+         145        2214 LOAD_CONST               6 ('name')
+                    2216 LOAD_CONST               7 ('value')
+                    2218 LOAD_CONST              56 ((2, 4))
+                    2220 BUILD_CONST_KEY_MAP      2
+         
+         137        2222 KW_NAMES                 9
+                    2224 PRECALL                  4
+                    2228 CALL                     4
+         
+         148        2238 PUSH_NULL
+                    2240 LOAD_NAME                3 (VaribleDetector)
+         
+         149        2242 LOAD_NAME                4 (Language)
+                    2244 LOAD_ATTR               18 (JAVA)
+         
+         150        2254 PUSH_NULL
+                    2256 LOAD_NAME                6 (re)
+                    2258 LOAD_ATTR                7 (compile)
+                    2268 LOAD_CONST              57 ('(n)(p)(.)(p)(L)')
+                    2270 PRECALL                  1
+                    2274 CALL                     1
+         
+         152        2284 PUSH_NULL
+                    2286 LOAD_NAME                8 (Match)
+                    2288 PUSH_NULL
+                    2290 LOAD_NAME                6 (re)
+                    2292 LOAD_ATTR                7 (compile)
+                    2302 LOAD_CONST              58 ('^put$')
+                    2304 PRECALL                  1
+                    2308 CALL                     1
+                    2318 BUILD_LIST               1
+                    2320 KW_NAMES                 5
+                    2322 PRECALL                  1
+                    2326 CALL                     1
+         
+         153        2336 PUSH_NULL
+                    2338 LOAD_NAME                8 (Match)
+                    2340 PUSH_NULL
+                    2342 LOAD_NAME                6 (re)
+                    2344 LOAD_ATTR                7 (compile)
+                    2354 LOAD_CONST              59 ('^\\($')
+                    2356 PRECALL                  1
+                    2360 CALL                     1
+                    2370 BUILD_LIST               1
+                    2372 KW_NAMES                 5
+                    2374 PRECALL                  1
+                    2378 CALL                     1
+         
+         154        2388 PUSH_NULL
+                    2390 LOAD_NAME                8 (Match)
+                    2392 PUSH_NULL
+                    2394 LOAD_NAME                6 (re)
+                    2396 LOAD_ATTR                7 (compile)
+                    2406 LOAD_CONST              54 ('^,$')
+                    2408 PRECALL                  1
+                    2412 CALL                     1
+                    2422 BUILD_LIST               1
+                    2424 KW_NAMES                 5
+                    2426 PRECALL                  1
+                    2430 CALL                     1
+         
+         151        2440 LOAD_CONST              46 ((1, 2, 4))
+                    2442 BUILD_CONST_KEY_MAP      3
+         
+         156        2444 LOAD_CONST               6 ('name')
+                    2446 LOAD_CONST               7 ('value')
+                    2448 LOAD_CONST              60 ((3, 5))
+                    2450 BUILD_CONST_KEY_MAP      2
+         
+         148        2452 KW_NAMES                 9
+                    2454 PRECALL                  4
+                    2458 CALL                     4
+         
+          10        2468 BUILD_LIST              18
+                    2470 STORE_NAME              19 (rules)
+         
+         161        2472 LOAD_NAME               20 (classmethod)
+         
+         162        2474 LOAD_CONST              61 ('language')
+                    2476 LOAD_NAME                4 (Language)
+                    2478 LOAD_CONST              62 ('return')
+                    2480 LOAD_NAME               21 (List)
+                    2482 LOAD_NAME                3 (VaribleDetector)
+                    2484 BINARY_SUBSCR
+                    2494 BUILD_TUPLE              4
+                    2496 LOAD_CONST              63 (<code object for_language, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 161>)
+                    2498 MAKE_FUNCTION            4 (annotations)
+         
+         161        2500 PRECALL                  0
+                    2504 CALL                     0
+         
+         162        2514 STORE_NAME              22 (for_language)
+                    2516 LOAD_CONST              64 (None)
+                    2518 RETURN_VALUE
          consts
             'VariableDetectionRules'
             '(n)(o|p)(?:\n?)(L)(?:\n|p|\\?)'
             2
             '='
             ':'
             ('values',)
@@ -952,31 +976,31 @@
             '(L)(p)(o)(L)'
             ']'
             (2, 3)
             (1, 4)
             '(n)(p)(L)(?:p|\n)?'
             '(n)(p)(L)(?:p|\n)?(L)(p)'
             'Setenv'
+            'Getenv'
             '('
             ')'
             (1, 2, 5)
             (3, 4)
-            '(n)(?:p|n|u)?(o)(n|p){0,5}(L)'
+            '(n)(?:p|n|u){0,3}?(o).*(n)(p)(L)'
             ':='
-            'Getenv'
             ('not_values',)
+            (1, 5)
             '(n)(?:o|p){1,3}(\\?|u)p(L)p'
             'byte'
             'string'
             '(n|v|L)(o)(L)'
             '=>'
             '(L)(o)(n)(p)Lp(L)p'
             'env'
             (2, 3, 4)
-            (1, 5)
             '(n)(o)(L)\n'
             '(L)(p)(L)'
             '(n)(o)(L)'
             '(v|n)(o)(L)'
             '(v|n)(p|o)(L)'
             '^:$'
             '^=$'
@@ -1008,21 +1032,21 @@
                flags     : 3
                code
                   0x8701970074010000000000000000000074030000000000000000000088
                   016601640184087c006a020000000000000000a6020000ab020000000000
                   000000a6010000ab0100000000000000005300
                              0 MAKE_CELL                1 (language)
                
-               158           2 RESUME                   0
+               161           2 RESUME                   0
                
-               160           4 LOAD_GLOBAL              1 (NULL + list)
+               163           4 LOAD_GLOBAL              1 (NULL + list)
                             16 LOAD_GLOBAL              3 (NULL + filter)
                             28 LOAD_CLOSURE             1 (language)
                             30 BUILD_TUPLE              1
-                            32 LOAD_CONST               1 (<code object <lambda>, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 160>)
+                            32 LOAD_CONST               1 (<code object <lambda>, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 163>)
                             34 MAKE_FUNCTION            8 (closure)
                             36 LOAD_FAST                0 (cls)
                             38 LOAD_ATTR                2 (rules)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 PRECALL                  1
                             66 CALL                     1
@@ -1035,15 +1059,15 @@
                      stacksize : 3
                      flags     : 19
                      code
                         0x950197007c006a00000000000000000089017402000000000000000000
                         006a020000000000000000660276005300
                                    0 COPY_FREE_VARS           1
                      
-                     160           2 RESUME                   0
+                     163           2 RESUME                   0
                                    4 LOAD_FAST                0 (x)
                                    6 LOAD_ATTR                0 (language)
                                   16 LOAD_DEREF               1 (language)
                                   18 LOAD_GLOBAL              2 (Language)
                                   30 LOAD_ATTR                2 (ANY)
                                   40 BUILD_TUPLE              2
                                   42 CONTAINS_OP              0
@@ -1052,45 +1076,154 @@
                         None
                      names      ('language', 'Language', 'ANY')
                      varnames   ('x',)
                      freevars   ('language',)
                      cellvars   ()
                      filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
                      name       '<lambda>'
-                     firstlineno 160
+                     firstlineno 163
                      lnotab 0x
                names      ('list', 'filter', 'rules')
                varnames   ('cls', 'language')
                freevars   ()
                cellvars   ('language',)
                filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
                name       'for_language'
-               firstlineno 158
+               firstlineno 161
                lnotab 0x0402
             None
          names      ('__name__', '__module__', '__qualname__', 'VaribleDetector', 'Language', 'PYTHON', 're', 'compile', 'Match', 'GOLANG', 'PHP', 'TOML', 'YAML', 'INI', 'PUPPET', 'ANY', 'SHELL', 'CSHARP', 'JAVA', 'rules', 'classmethod', 'List', 'for_language')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
          name       'VariableDetectionRules'
-         firstlineno 8
+         firstlineno 9
          lnotab
             0x0a0204010c011e011e0108fc100604010c011e011c0108fc100604010c
-            011e01340108fc100704010c011e011e0108fc100604010c011e02180118
-            0118fd040508f8100a04010c011e0218011afe040408f9100904010c011e
+            011e01340108fc100704010c011e011e0108fc100604010c011e021a0118
+            0118fd040508f8100b04010c011e0218011afe040408f9100a04010c011e
             011e0108fc100704010c011e011e0108fc100604010c011e021801180118
             fd040508f8100b04010c011e011c0108fc100604010c011e011c0108fc10
             0604010c011e011c0108fc100604010c011e011e0108fc100604010c011e
             0206011e011efe12ff020508f8100a04010c011e023401340134fd040508
             0102f7100c04010c011e02340134fe040408f9100a04010c011e02340134
-            0134fd040508f8100b04010c011e023401340134fd040508f8108000f804
-            7f001602011aff0e01
+            0134fd040508f8100b04010c011e023401340134fd040508f8108000f604
+            7f001802011aff0e01
       'VariableDetectionRules'
-   names      ('regex', 're', 'typing', 'List', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector', 'Match', 'VaribleDetector', 'VariableDetectionRules')
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 11
+         flags     : 0
+         code
+            0x970065005a0164005a020200650365046a050000000000000000020065
+            066a0700000000000000006401a6010000ab010000000000000000020065
+            08020065066a0700000000000000006402a6010000ab0100000000000000
+            006701ac03a6010000ab0100000000000000000200650865096a0a000000
+            00000000006a0b00000000000000006701ac04a6010000ab010000000000
+            00000002006508020065066a0700000000000000006405a6010000ab0100
+            000000000000006701ac03a6010000ab01000000000000000064069c0369
+            00ac07a6040000ab04000000000000000067015a0c64085300
+         166           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('VariableSuppressionRules')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         168          10 PUSH_NULL
+                      12 LOAD_NAME                3 (VaribleSuppressor)
+         
+         169          14 LOAD_NAME                4 (Language)
+                      16 LOAD_ATTR                5 (JS)
+         
+         170          26 PUSH_NULL
+                      28 LOAD_NAME                6 (re)
+                      30 LOAD_ATTR                7 (compile)
+                      40 LOAD_CONST               1 ('(p)(n).*?p(p)')
+                      42 PRECALL                  1
+                      46 CALL                     1
+         
+         172          56 PUSH_NULL
+                      58 LOAD_NAME                8 (Match)
+         
+         173          60 PUSH_NULL
+                      62 LOAD_NAME                6 (re)
+                      64 LOAD_ATTR                7 (compile)
+                      74 LOAD_CONST               2 ('^<$')
+                      76 PRECALL                  1
+                      80 CALL                     1
+         
+         172          90 BUILD_LIST               1
+                      92 KW_NAMES                 3
+                      94 PRECALL                  1
+                      98 CALL                     1
+         
+         175         108 PUSH_NULL
+                     110 LOAD_NAME                8 (Match)
+         
+         176         112 LOAD_NAME                9 (PygmentsToken)
+                     114 LOAD_ATTR               10 (Name)
+                     124 LOAD_ATTR               11 (Tag)
+                     134 BUILD_LIST               1
+         
+         175         136 KW_NAMES                 4
+                     138 PRECALL                  1
+                     142 CALL                     1
+         
+         178         152 PUSH_NULL
+                     154 LOAD_NAME                8 (Match)
+         
+         179         156 PUSH_NULL
+                     158 LOAD_NAME                6 (re)
+                     160 LOAD_ATTR                7 (compile)
+                     170 LOAD_CONST               5 ('^>$')
+                     172 PRECALL                  1
+                     176 CALL                     1
+         
+         178         186 BUILD_LIST               1
+                     188 KW_NAMES                 3
+                     190 PRECALL                  1
+                     194 CALL                     1
+         
+         171         204 LOAD_CONST               6 ((1, 2, 3))
+                     206 BUILD_CONST_KEY_MAP      3
+         
+         182         208 BUILD_MAP                0
+         
+         168         210 KW_NAMES                 7
+                     212 PRECALL                  4
+                     216 CALL                     4
+         
+         167         226 BUILD_LIST               1
+                     228 STORE_NAME              12 (rules)
+                     230 LOAD_CONST               8 (None)
+                     232 RETURN_VALUE
+         consts
+            'VariableSuppressionRules'
+            '(p)(n).*?p(p)'
+            '^<$'
+            ('values',)
+            ('types',)
+            '^>$'
+            (1, 2, 3)
+            ('language', 'stream_pattern', 'match_rules', 'match_semantics')
+            None
+         names      ('__name__', '__module__', '__qualname__', 'VaribleSuppressor', 'Language', 'JS', 're', 'compile', 'Match', 'PygmentsToken', 'Name', 'Tag', 'rules')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
+         name       'VariableSuppressionRules'
+         firstlineno 166
+         lnotab
+            0x0a0204010c011e0204011eff1203040118ff100304011eff12f9040b02
+            f210ff
+      'VariableSuppressionRules'
+   names      ('regex', 're', 'typing', 'List', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector', 'Match', 'VaribleDetector', 'VaribleSuppressor', 'pygments.token', 'Token', 'PygmentsToken', 'VariableDetectionRules', 'VariableSuppressionRules')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c020c011003
+   lnotab 0x00ff020108010c020c0114010c031a7f001e
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,75 @@
 import regex as re
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field, validator
 
 from deepsecrets.core.model.token import Token
 from deepsecrets.core.tokenizers.helpers.semantic.language import Language
 
 
 class Match(BaseModel):
+    types: List[Any] = Field(default_factory=list)
     values: List[re.Pattern] = Field(default_factory=list)
     not_values: List[re.Pattern] = Field(default_factory=list)
 
     def check(self, tokens: List[Token]) -> bool:
-        if len(self.values) > 0:
-            matched = False
-            for token in tokens:
-                for pattern in self.values:
-                    if re.match(pattern, token.content) is not None:
-                        matched = True
-            if not matched:
-                return False
+        
+        types_match = self._check_types(tokens)
+        values_match = self._check_values(tokens)
+        not_values_match = self._check_not_values(tokens)
+
+        if not types_match:
+            return False
+        
+        if not values_match:
+            return False 
+        
+        if not_values_match:
+            return False
 
-        if len(self.not_values) > 0:
-            for token in tokens:
-                for pattern in self.not_values:
-                    if re.match(pattern, token.content) is not None:
-                        return False
         return True
 
+    
+
+    def _check_types(self, tokens):
+        if len(self.types) == 0:
+            return True # should match any type
+        
+        for token in tokens:
+            if token.type[0] in self.types:
+                return True
+
+
+    def _check_values(self, tokens):
+        if len(self.values) == 0:
+            return True # should match any value
+        
+        for token in tokens:
+            for pattern in self.values:
+                if re.match(pattern, token.content) is not None:
+                    return True
+        return False
+    
+
+    def _check_not_values(self, tokens):
+        if len(self.not_values) == 0:
+            return False
+        
+        for token in tokens:
+            for pattern in self.not_values:
+                if re.match(pattern, token.content) is not None:
+                    return True
+        return False     
+            
+
+
+
+
+
     @validator('values', 'not_values', pre=True)
     def regexify_values(cls, values: Dict) -> List[re.Pattern]:
         if values is None:
             return values
 
         if not isinstance(values, list):
             raise Exception('value must be an array')
@@ -67,14 +105,15 @@
             if not self._verify(match, tokens):
                 continue
 
             var = Variable()
             for i, name in self.match_semantics.items():
                 setattr(var, name, tokens[match.span(i)[0]])
             var.found_by = self
+            var.span = [match.span(0)[0], match.span(0)[1]]
 
             true_detections.append(var)
 
         return true_detections
 
     def _verify(self, match: re.Match, tokens: List[Token]) -> bool:
         for group_i, match_rule in self.match_rules.items():
@@ -83,8 +122,20 @@
 
             if not match_rule.check(window):
                 return False
 
         return True
 
 
+class VaribleSuppressor(VaribleDetector):
+
+    def match(self, tokens: List[Token], token_stream: str) -> List['Variable']:
+        detections = super().match(tokens, token_stream)
+        spans = []
+        for detection in detections:
+            spans.append(detection.span)
+        
+        return spans
+    
+
+
 from deepsecrets.core.model.semantic import Variable
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import regex as re
 from typing import List
 
 from deepsecrets.core.tokenizers.helpers.semantic.language import Language
-from deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector import Match, VaribleDetector
+from deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector import Match, VaribleDetector, VaribleSuppressor
+from pygments.token import Token as PygmentsToken
 
 
 class VariableDetectionRules:
     rules = [
         VaribleDetector(
             language=Language.PYTHON,
             stream_pattern=re.compile('(n)(o|p)(?:\n?)(L)(?:\n|p|\?)'),  # noqa
@@ -32,29 +33,31 @@
             match_rules={2: Match(values=[':', '='])},
             match_semantics={1: 'name', 3: 'value'},
         ),
         VaribleDetector(
             language=Language.GOLANG,
             stream_pattern=re.compile('(n)(p)(L)(?:p|\n)?(L)(p)'),
             match_rules={
-                1: Match(values=['Setenv']),
+                1: Match(values=['Setenv', 'Getenv']),
                 2: Match(values=['(']),
                 5: Match(values=[')']),
             },
             match_semantics={3: 'name', 4: 'value'},
         ),
-        VaribleDetector(
+        
+       VaribleDetector(
             language=Language.GOLANG,
-            stream_pattern=re.compile('(n)(?:p|n|u)?(o)(n|p){0,5}(L)'),
+            stream_pattern=re.compile('(n)(?:p|n|u){0,3}?(o).*(n)(p)(L)'),
             match_rules={
-                2: Match(values=[':=']),
-                3: Match(not_values=['Getenv', 'Setenv']),
-            },
-            match_semantics={1: 'name', 4: 'value'},
+               2: Match(values=[':=']),
+               3: Match(not_values=['Getenv', 'Setenv']),
+           },
+            match_semantics={1: 'name', 5: 'value'},
         ),
+
         VaribleDetector(
             language=Language.GOLANG,
             stream_pattern=re.compile('(n)(?:o|p){1,3}(\?|u)p(L)p'),  # noqa
             match_rules={2: Match(values=['byte', 'string'])},
             match_semantics={1: 'name', 3: 'value'},
         ),
         # PHP
@@ -154,7 +157,28 @@
         ),
 
     ]
 
     @classmethod
     def for_language(cls, language: Language) -> List[VaribleDetector]:
         return list(filter(lambda x: x.language in [language, Language.ANY], cls.rules))
+
+
+class VariableSuppressionRules(VariableDetectionRules):
+    rules=[
+        VaribleSuppressor(
+            language=Language.JS,
+            stream_pattern=re.compile('(p)(n).*?p(p)'),
+            match_rules={
+                1: Match(values=[
+                    re.compile('^<$'),
+                ]),
+                2: Match(
+                    types=[PygmentsToken.Name.Tag]
+                ),
+                3: Match(values=[
+                    re.compile('^>$'),
+                ]),
+            },
+            match_semantics={}
+        )
+    ]
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/lexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from typing import List, Sequence, Set, Type, Union
+from typing import List, Optional, Sequence, Set, Type, Union
+
+from deepsecrets import logger
 
 from ordered_set import OrderedSet
 from pygments import highlight
 from pygments.formatters import RawTokenFormatter
-from pygments.lexers import get_lexer_for_filename
 from pygments.lexers.special import Lexer, RawTokenLexer
 from pygments.token import Token as PygmentsToken
-from pygments.util import ClassNotFound
 
 from deepsecrets.core.model.file import File
 from deepsecrets.core.model.semantic import Variable
 from deepsecrets.core.model.token import Semantic, SemanticType, Token
 from deepsecrets.core.tokenizers.helpers.semantic.language import Language
-from deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules import VariableDetectionRules
+from deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules import VariableDetectionRules, VariableSuppressionRules
 from deepsecrets.core.tokenizers.helpers.spot_improvements import SpotImprovements
 from deepsecrets.core.tokenizers.helpers.type_stream import (
     token_to_typestream_item,
     types_to_filter_after,
     types_to_filter_before,
 )
 from deepsecrets.core.tokenizers.itokenizer import Tokenizer
+from deepsecrets.core.utils.lexer_finder import LexerFinder
 
 empty_tokens = ['\n', '\t', "'", "''", '"', '""']
 
 
 class LexerTokenizer(Tokenizer):
     token_stream: str
     lexer: Lexer
@@ -57,45 +58,34 @@
 
         if content in quotes:
             return False
 
         return content
 
     def _find_lexer_for_file(self, file: File):
-        lexer = None
-        if file.extension is not None:
-            try:
-                lexer = get_lexer_for_filename(file.path)
-                return lexer
-            except ClassNotFound:
-                pass
-        
-        if file.guessed_extension is not None:
-            try:
-                lexer = get_lexer_for_filename(f'{file.path}.{file.guessed_extension}')
-                return lexer
-            except ClassNotFound:
-                pass
-        
+        lexer = LexerFinder().find(file=file)
+        if lexer is not None and lexer.name == 'Text only':
+            return None
         return lexer
 
 
-
     def tokenize(self, file: File, post_filter=True) -> List[Token]:
         self.token_stream = ''
         # TODO: don't trust the extension, use 'file' utility ?
 
         self.lexer = self._find_lexer_for_file(file)
         if not self.lexer:
             return self.tokens
 
         try:
             self.language: Language = Language.from_text(self.lexer.filenames[0])
-        except ValueError:
+        except (ValueError, IndexError):
             self.language: Language = Language.from_text(file.extension)
+        except Exception as e:
+            logger.exception(e)
 
         result = highlight(file.content, self.lexer, RawTokenFormatter())
         raw_tokens = list(RawTokenLexer().get_tokens(result))
         token_improver = SpotImprovements(lang=self.language)
 
         current_position = 0
 
@@ -141,49 +131,63 @@
         for token in tokens_all:
             if any(type in token.type for type in types_to_filter_before):  # type: ignore
                 continue
 
             if any(type in token.type for type in types_to_filter_after):  # type: ignore
                 continue
 
-            if token.content in empty_tokens:
+            if token.content.replace(' ', '') in empty_tokens:
                 continue
 
             final.append(token)
 
         return final
 
     def deep_analyze(self) -> Set[Token]:
         tokens_all = OrderedSet(self.tokens)
         if self.language is None:
             return tokens_all
 
         exclude_after = set()
 
         true_detections: List[Variable] = []
-        rules = VariableDetectionRules.for_language(self.language)
-        for rule in rules:
+        suppression_regions: List[List[int]] = []
+        
+        detection_rules = VariableDetectionRules.for_language(self.language)
+        suppression_rules = VariableSuppressionRules.for_language(self.language)
+    
+        for rule in detection_rules:
             true_detections.extend(rule.match(self.tokens, self.token_stream))
+        
+        for rule in suppression_rules:
+            suppression_regions.extend(rule.match(self.tokens, self.token_stream))
+
 
         for var in true_detections:
+            for reg in suppression_regions:
+                if var.span[0] >= reg[0] and var.span[1] <= reg[1]:
+                    exclude_after.update([var.name, var.value])
+                    continue
+
             var.value.semantic = Semantic(
                 type=SemanticType.VAR,
                 name=var.name.content,
                 creds_probability=var.found_by.creds_probability,
             )
             exclude_after.add(var.name)
 
         return exclude_after
 
-    def get_variables(self) -> List[Token]:
+    def get_variables(self, tokens: Optional[List[Token]] = None) -> List[Token]:
+        tokens = tokens if tokens is not None else self.tokens
         vars = []
-        if len(self.tokens) == 0:
+        if len(tokens) == 0:
             return []
 
-        for token in self.tokens:
+        for token in tokens:
             if token.semantic is None:
                 continue
 
             if token.semantic.type != SemanticType.VAR:
                 continue
 
             vars.append(token)
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.1.0/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,796 +1,743 @@
 magic:    0xa70d0d0a
-moddate:  0x2cfb2164 (Mon Mar 27 20:23:08 2023 UTC)
-files sz: 3018
+moddate:  0x1e09a464 (Tue Jul  4 11:57:18 2023 UTC)
+files sz: 3333
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a056d065a066d075a076d085a080100640064046c096d0a5a
-      0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064
-      076c0f6d105a100100640064086c116d125a120100640064096c136d145a
-      1401006400640a6c156d165a16010002004700640b8400640c650aa60300
-      00ab0300000000000000005a1702004700640d8400640ea6020000ab0200
-      000000000000005a18640f5300
+      0x9700640064016c005a00640064016c015a01640064026c026d035a036d
+      045a046d055a056d065a060100640064036c076d085a080100640064046c
+      096d0a5a0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d
+      0f5a0f0100640064076c106d115a110100640064086c126d135a13010064
+      0064096c146d155a1501006400640a6c166d175a1701006400640b6c186d
+      195a1901006400640c6c1a6d1b5a1b01006400640d6c1c6d1d5a1d010064
+      00640e6c1e6d1f5a1f01006400640f6c206d215a21010002004700641084
+      0064116517a6030000ab0300000000000000005a2264015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('RLock',))
-                 6 IMPORT_NAME              0 (multiprocessing)
-                 8 IMPORT_FROM              1 (RLock)
-                10 STORE_NAME               1 (RLock)
-                12 POP_TOP
-   
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('Pool',))
-                18 IMPORT_NAME              2 (multiprocessing.pool)
-                20 IMPORT_FROM              3 (Pool)
-                22 STORE_NAME               3 (Pool)
-                24 POP_TOP
-   
-     3          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('Dict', 'List', 'Optional', 'Type'))
-                30 IMPORT_NAME              4 (typing)
-                32 IMPORT_FROM              5 (Dict)
-                34 STORE_NAME               5 (Dict)
-                36 IMPORT_FROM              6 (List)
-                38 STORE_NAME               6 (List)
-                40 IMPORT_FROM              7 (Optional)
-                42 STORE_NAME               7 (Optional)
-                44 IMPORT_FROM              8 (Type)
-                46 STORE_NAME               8 (Type)
-                48 POP_TOP
-   
-     5          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('BaseModel',))
-                54 IMPORT_NAME              9 (pydantic)
-                56 IMPORT_FROM             10 (BaseModel)
-                58 STORE_NAME              10 (BaseModel)
-                60 POP_TOP
-   
-     7          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('logger',))
-                66 IMPORT_NAME             11 (deepsecrets)
-                68 IMPORT_FROM             12 (logger)
-                70 STORE_NAME              12 (logger)
-                72 POP_TOP
-   
-     8          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               6 (('IEngine',))
-                78 IMPORT_NAME             13 (deepsecrets.core.engines.iengine)
-                80 IMPORT_FROM             14 (IEngine)
-                82 STORE_NAME              14 (IEngine)
-                84 POP_TOP
-   
-     9          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('File',))
-                90 IMPORT_NAME             15 (deepsecrets.core.model.file)
-                92 IMPORT_FROM             16 (File)
-                94 STORE_NAME              16 (File)
-                96 POP_TOP
-   
-    10          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('Finding',))
-               102 IMPORT_NAME             17 (deepsecrets.core.model.finding)
-               104 IMPORT_FROM             18 (Finding)
-               106 STORE_NAME              18 (Finding)
-               108 POP_TOP
-   
-    11         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('Token',))
-               114 IMPORT_NAME             19 (deepsecrets.core.model.token)
-               116 IMPORT_FROM             20 (Token)
-               118 STORE_NAME              20 (Token)
-               120 POP_TOP
-   
-    12         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST              10 (('Tokenizer',))
-               126 IMPORT_NAME             21 (deepsecrets.core.tokenizers.itokenizer)
-               128 IMPORT_FROM             22 (Tokenizer)
-               130 STORE_NAME              22 (Tokenizer)
-               132 POP_TOP
-   
-    15         134 PUSH_NULL
-               136 LOAD_BUILD_CLASS
-               138 LOAD_CONST              11 (<code object EngineWithTokenizer, file "/app/deepsecrets/core/utils/file_analyzer.py", line 15>)
-               140 MAKE_FUNCTION            0
-               142 LOAD_CONST              12 ('EngineWithTokenizer')
-               144 LOAD_NAME               10 (BaseModel)
-               146 PRECALL                  3
-               150 CALL                     3
-               160 STORE_NAME              23 (EngineWithTokenizer)
-   
-    23         162 PUSH_NULL
-               164 LOAD_BUILD_CLASS
-               166 LOAD_CONST              13 (<code object FileAnalyzer, file "/app/deepsecrets/core/utils/file_analyzer.py", line 23>)
-               168 MAKE_FUNCTION            0
-               170 LOAD_CONST              14 ('FileAnalyzer')
-               172 PRECALL                  2
-               176 CALL                     2
-               186 STORE_NAME              24 (FileAnalyzer)
-               188 LOAD_CONST              15 (None)
-               190 RETURN_VALUE
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (logging)
+                 8 STORE_NAME               0 (logging)
+   
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               1 (None)
+                14 IMPORT_NAME              1 (os)
+                16 STORE_NAME               1 (os)
+   
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('Any', 'Dict', 'List', 'Type'))
+                22 IMPORT_NAME              2 (typing)
+                24 IMPORT_FROM              3 (Any)
+                26 STORE_NAME               3 (Any)
+                28 IMPORT_FROM              4 (Dict)
+                30 STORE_NAME               4 (Dict)
+                32 IMPORT_FROM              5 (List)
+                34 STORE_NAME               5 (List)
+                36 IMPORT_FROM              6 (Type)
+                38 STORE_NAME               6 (Type)
+                40 POP_TOP
+   
+     5          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               3 (('DotWiz',))
+                46 IMPORT_NAME              7 (dotwiz)
+                48 IMPORT_FROM              8 (DotWiz)
+                50 STORE_NAME               8 (DotWiz)
+                52 POP_TOP
+   
+     7          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               4 (('PROFILER_ON', 'logger'))
+                58 IMPORT_NAME              9 (deepsecrets)
+                60 IMPORT_FROM             10 (PROFILER_ON)
+                62 STORE_NAME              10 (PROFILER_ON)
+                64 IMPORT_FROM             11 (logger)
+                66 STORE_NAME              11 (logger)
+                68 POP_TOP
+   
+     8          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('HashedSecretEngine',))
+                74 IMPORT_NAME             12 (deepsecrets.core.engines.hashed_secret)
+                76 IMPORT_FROM             13 (HashedSecretEngine)
+                78 STORE_NAME              13 (HashedSecretEngine)
+                80 POP_TOP
+   
+     9          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('RegexEngine',))
+                86 IMPORT_NAME             14 (deepsecrets.core.engines.regex)
+                88 IMPORT_FROM             15 (RegexEngine)
+                90 STORE_NAME              15 (RegexEngine)
+                92 POP_TOP
+   
+    10          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               7 (('SemanticEngine',))
+                98 IMPORT_NAME             16 (deepsecrets.core.engines.semantic)
+               100 IMPORT_FROM             17 (SemanticEngine)
+               102 STORE_NAME              17 (SemanticEngine)
+               104 POP_TOP
+   
+    11         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               8 (('File',))
+               110 IMPORT_NAME             18 (deepsecrets.core.model.file)
+               112 IMPORT_FROM             19 (File)
+               114 STORE_NAME              19 (File)
+               116 POP_TOP
+   
+    12         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('Finding',))
+               122 IMPORT_NAME             20 (deepsecrets.core.model.finding)
+               124 IMPORT_FROM             21 (Finding)
+               126 STORE_NAME              21 (Finding)
+               128 POP_TOP
+   
+    13         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              10 (('ScanMode',))
+               134 IMPORT_NAME             22 (deepsecrets.core.modes.iscan_mode)
+               136 IMPORT_FROM             23 (ScanMode)
+               138 STORE_NAME              23 (ScanMode)
+               140 POP_TOP
+   
+    14         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              11 (('HashedSecretsRulesetBuilder',))
+               146 IMPORT_NAME             24 (deepsecrets.core.rulesets.hashed_secrets)
+               148 IMPORT_FROM             25 (HashedSecretsRulesetBuilder)
+               150 STORE_NAME              25 (HashedSecretsRulesetBuilder)
+               152 POP_TOP
+   
+    15         154 LOAD_CONST               0 (0)
+               156 LOAD_CONST              12 (('RegexRulesetBuilder',))
+               158 IMPORT_NAME             26 (deepsecrets.core.rulesets.regex)
+               160 IMPORT_FROM             27 (RegexRulesetBuilder)
+               162 STORE_NAME              27 (RegexRulesetBuilder)
+               164 POP_TOP
+   
+    16         166 LOAD_CONST               0 (0)
+               168 LOAD_CONST              13 (('FullContentTokenizer',))
+               170 IMPORT_NAME             28 (deepsecrets.core.tokenizers.full_content)
+               172 IMPORT_FROM             29 (FullContentTokenizer)
+               174 STORE_NAME              29 (FullContentTokenizer)
+               176 POP_TOP
+   
+    17         178 LOAD_CONST               0 (0)
+               180 LOAD_CONST              14 (('LexerTokenizer',))
+               182 IMPORT_NAME             30 (deepsecrets.core.tokenizers.lexer)
+               184 IMPORT_FROM             31 (LexerTokenizer)
+               186 STORE_NAME              31 (LexerTokenizer)
+               188 POP_TOP
+   
+    18         190 LOAD_CONST               0 (0)
+               192 LOAD_CONST              15 (('FileAnalyzer',))
+               194 IMPORT_NAME             32 (deepsecrets.core.utils.file_analyzer)
+               196 IMPORT_FROM             33 (FileAnalyzer)
+               198 STORE_NAME              33 (FileAnalyzer)
+               200 POP_TOP
+   
+    21         202 PUSH_NULL
+               204 LOAD_BUILD_CLASS
+               206 LOAD_CONST              16 (<code object CliScanMode, file "/app/deepsecrets/scan_modes/cli.py", line 21>)
+               208 MAKE_FUNCTION            0
+               210 LOAD_CONST              17 ('CliScanMode')
+               212 LOAD_NAME               23 (ScanMode)
+               214 PRECALL                  3
+               218 CALL                     3
+               228 STORE_NAME              34 (CliScanMode)
+               230 LOAD_CONST               1 (None)
+               232 RETURN_VALUE
    consts
       0
-      ('RLock',)
-      ('Pool',)
-      ('Dict', 'List', 'Optional', 'Type')
-      ('BaseModel',)
-      ('logger',)
-      ('IEngine',)
+      None
+      ('Any', 'Dict', 'List', 'Type')
+      ('DotWiz',)
+      ('PROFILER_ON', 'logger')
+      ('HashedSecretEngine',)
+      ('RegexEngine',)
+      ('SemanticEngine',)
       ('File',)
       ('Finding',)
-      ('Token',)
-      ('Tokenizer',)
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 4
-         flags     : 0
-         code
-            0x970065005a0164005a0255006503650464013c0000006505650464023c
-            00000002004700640384006404a6020000ab0200000000000000005a0664
-            055300
-          15           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('EngineWithTokenizer')
-                       8 STORE_NAME               2 (__qualname__)
-                      10 SETUP_ANNOTATIONS
-         
-          16          12 LOAD_NAME                3 (IEngine)
-                      14 LOAD_NAME                4 (__annotations__)
-                      16 LOAD_CONST               1 ('engine')
-                      18 STORE_SUBSCR
-         
-          17          22 LOAD_NAME                5 (Tokenizer)
-                      24 LOAD_NAME                4 (__annotations__)
-                      26 LOAD_CONST               2 ('tokenizer')
-                      28 STORE_SUBSCR
-         
-          19          32 PUSH_NULL
-                      34 LOAD_BUILD_CLASS
-                      36 LOAD_CONST               3 (<code object Config, file "/app/deepsecrets/core/utils/file_analyzer.py", line 19>)
-                      38 MAKE_FUNCTION            0
-                      40 LOAD_CONST               4 ('Config')
-                      42 PRECALL                  2
-                      46 CALL                     2
-                      56 STORE_NAME               6 (Config)
-                      58 LOAD_CONST               5 (None)
-                      60 RETURN_VALUE
-         consts
-            'EngineWithTokenizer'
-            'engine'
-            'tokenizer'
-            code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 1
-               flags     : 0
-               code 0x970065005a0164005a0264015a0364025300
-                19           0 RESUME                   0
-                             2 LOAD_NAME                0 (__name__)
-                             4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('EngineWithTokenizer.Config')
-                             8 STORE_NAME               2 (__qualname__)
-               
-                20          10 LOAD_CONST               1 (True)
-                            12 STORE_NAME               3 (arbitrary_types_allowed)
-                            14 LOAD_CONST               2 (None)
-                            16 RETURN_VALUE
-               consts
-                  'EngineWithTokenizer.Config'
-                  True
-                  None
-               names      ('__name__', '__module__', '__qualname__', 'arbitrary_types_allowed')
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-               name       'Config'
-               firstlineno 19
-               lnotab 0x0a01
-            'Config'
-            None
-         names      ('__name__', '__module__', '__qualname__', 'IEngine', '__annotations__', 'Tokenizer', 'Config')
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-         name       'EngineWithTokenizer'
-         firstlineno 15
-         lnotab 0x0c010a010a02
-      'EngineWithTokenizer'
+      ('ScanMode',)
+      ('HashedSecretsRulesetBuilder',)
+      ('RegexRulesetBuilder',)
+      ('FullContentTokenizer',)
+      ('LexerTokenizer',)
+      ('FileAnalyzer',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c00000065056506190000
-            00000000000000650464023c000000650765086505650919000000000000
-            000000660219000000000000000000650464033c0000006508650464043c
-            0000006410640165036404650a6508190000000000000000006604640684
-            055a0b6407650c64086505650d1900000000000000000064096405660664
-            0a84045a0e6411640c650f64096505651019000000000000000000660464
-            0d84055a11640e6506640965056510190000000000000000006604640f84
-            045a1264055300
-          23           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('FileAnalyzer')
-                       8 STORE_NAME               2 (__qualname__)
-                      10 SETUP_ANNOTATIONS
-         
-          24          12 LOAD_NAME                3 (File)
-                      14 LOAD_NAME                4 (__annotations__)
-                      16 LOAD_CONST               1 ('file')
-                      18 STORE_SUBSCR
-         
-          25          22 LOAD_NAME                5 (List)
-                      24 LOAD_NAME                6 (EngineWithTokenizer)
+            0x8700970065005a0164005a02550069005a036504650565066602190000
+            00000000000000650764013c00000069005a0865046509650a6602190000
+            00000000000000650764023c0000006409640584045a0b6403650c660288
+            0066016406840c5a0d650e6407650f6403650a6510190000000000000000
+            00660464088404a6000000ab0000000000000000005a11880078015a1253
+            00
+                       0 MAKE_CELL                0 (__class__)
+         
+          21           2 RESUME                   0
+                       4 LOAD_NAME                0 (__name__)
+                       6 STORE_NAME               1 (__module__)
+                       8 LOAD_CONST               0 ('CliScanMode')
+                      10 STORE_NAME               2 (__qualname__)
+                      12 SETUP_ANNOTATIONS
+         
+          22          14 BUILD_MAP                0
+                      16 STORE_NAME               3 (engines_enabled)
+                      18 LOAD_NAME                4 (Dict)
+                      20 LOAD_NAME                5 (Type)
+                      22 LOAD_NAME                6 (bool)
+                      24 BUILD_TUPLE              2
                       26 BINARY_SUBSCR
-                      36 LOAD_NAME                4 (__annotations__)
-                      38 LOAD_CONST               2 ('engine_tokenizers')
+                      36 LOAD_NAME                7 (__annotations__)
+                      38 LOAD_CONST               1 ('engines_enabled')
                       40 STORE_SUBSCR
          
-          26          44 LOAD_NAME                7 (Dict)
-                      46 LOAD_NAME                8 (Type)
-                      48 LOAD_NAME                5 (List)
-                      50 LOAD_NAME                9 (Token)
-                      52 BINARY_SUBSCR
-                      62 BUILD_TUPLE              2
-                      64 BINARY_SUBSCR
-                      74 LOAD_NAME                4 (__annotations__)
-                      76 LOAD_CONST               3 ('tokens')
-                      78 STORE_SUBSCR
-         
-          27          82 LOAD_NAME                8 (Type)
-                      84 LOAD_NAME                4 (__annotations__)
-                      86 LOAD_CONST               4 ('pool_class')
-                      88 STORE_SUBSCR
-         
-          29          92 LOAD_CONST              16 ((None,))
-                      94 LOAD_CONST               1 ('file')
-                      96 LOAD_NAME                3 (File)
-                      98 LOAD_CONST               4 ('pool_class')
-                     100 LOAD_NAME               10 (Optional)
-                     102 LOAD_NAME                8 (Type)
-                     104 BINARY_SUBSCR
-                     114 BUILD_TUPLE              4
-                     116 LOAD_CONST               6 (<code object __init__, file "/app/deepsecrets/core/utils/file_analyzer.py", line 29>)
-                     118 MAKE_FUNCTION            5 (defaults, annotations)
-                     120 STORE_NAME              11 (__init__)
-         
-          40         122 LOAD_CONST               7 ('engine')
-                     124 LOAD_NAME               12 (IEngine)
-                     126 LOAD_CONST               8 ('tokenizers')
-                     128 LOAD_NAME                5 (List)
-                     130 LOAD_NAME               13 (Tokenizer)
-                     132 BINARY_SUBSCR
-                     142 LOAD_CONST               9 ('return')
-                     144 LOAD_CONST               5 (None)
-                     146 BUILD_TUPLE              6
-                     148 LOAD_CONST              10 (<code object add_engine, file "/app/deepsecrets/core/utils/file_analyzer.py", line 40>)
-                     150 MAKE_FUNCTION            4 (annotations)
-                     152 STORE_NAME              14 (add_engine)
-         
-          44         154 LOAD_CONST              17 ((False,))
-                     156 LOAD_CONST              12 ('threaded')
-                     158 LOAD_NAME               15 (bool)
-                     160 LOAD_CONST               9 ('return')
-                     162 LOAD_NAME                5 (List)
-                     164 LOAD_NAME               16 (Finding)
-                     166 BINARY_SUBSCR
-                     176 BUILD_TUPLE              4
-                     178 LOAD_CONST              13 (<code object process, file "/app/deepsecrets/core/utils/file_analyzer.py", line 44>)
-                     180 MAKE_FUNCTION            5 (defaults, annotations)
-                     182 STORE_NAME              17 (process)
-         
-          67         184 LOAD_CONST              14 ('et')
-                     186 LOAD_NAME                6 (EngineWithTokenizer)
-                     188 LOAD_CONST               9 ('return')
-                     190 LOAD_NAME                5 (List)
-                     192 LOAD_NAME               16 (Finding)
-                     194 BINARY_SUBSCR
-                     204 BUILD_TUPLE              4
-                     206 LOAD_CONST              15 (<code object _run_engine, file "/app/deepsecrets/core/utils/file_analyzer.py", line 67>)
-                     208 MAKE_FUNCTION            4 (annotations)
-                     210 STORE_NAME              18 (_run_engine)
-                     212 LOAD_CONST               5 (None)
-                     214 RETURN_VALUE
+          23          44 BUILD_MAP                0
+                      46 STORE_NAME               8 (rulesets)
+                      48 LOAD_NAME                4 (Dict)
+                      50 LOAD_NAME                9 (str)
+                      52 LOAD_NAME               10 (List)
+                      54 BUILD_TUPLE              2
+                      56 BINARY_SUBSCR
+                      66 LOAD_NAME                7 (__annotations__)
+                      68 LOAD_CONST               2 ('rulesets')
+                      70 STORE_SUBSCR
+         
+          25          74 LOAD_CONST               9 (('return', None))
+                      76 LOAD_CONST               5 (<code object prepare_for_scan, file "/app/deepsecrets/scan_modes/cli.py", line 25>)
+                      78 MAKE_FUNCTION            4 (annotations)
+                      80 STORE_NAME              11 (prepare_for_scan)
+         
+          40          82 LOAD_CONST               3 ('return')
+                      84 LOAD_NAME               12 (DotWiz)
+                      86 BUILD_TUPLE              2
+                      88 LOAD_CLOSURE             0 (__class__)
+                      90 BUILD_TUPLE              1
+                      92 LOAD_CONST               6 (<code object analyzer_bundle, file "/app/deepsecrets/scan_modes/cli.py", line 40>)
+                      94 MAKE_FUNCTION           12 (annotations, closure)
+                      96 STORE_NAME              13 (analyzer_bundle)
+         
+          50          98 LOAD_NAME               14 (staticmethod)
+         
+          51         100 LOAD_CONST               7 ('file')
+                     102 LOAD_NAME               15 (Any)
+                     104 LOAD_CONST               3 ('return')
+                     106 LOAD_NAME               10 (List)
+                     108 LOAD_NAME               16 (Finding)
+                     110 BINARY_SUBSCR
+                     120 BUILD_TUPLE              4
+                     122 LOAD_CONST               8 (<code object _per_file_analyzer, file "/app/deepsecrets/scan_modes/cli.py", line 50>)
+                     124 MAKE_FUNCTION            4 (annotations)
+         
+          50         126 PRECALL                  0
+                     130 CALL                     0
+         
+          51         140 STORE_NAME              17 (_per_file_analyzer)
+                     142 LOAD_CLOSURE             0 (__class__)
+                     144 COPY                     1
+                     146 STORE_NAME              18 (__classcell__)
+                     148 RETURN_VALUE
          consts
-            'FileAnalyzer'
-            'file'
-            'engine_tokenizers'
-            'tokens'
-            'pool_class'
-            None
-            code
-               argcount  : 3
-               nlocals   : 3
-               stacksize : 2
-               flags     : 3
-               code
-                  0x97007c02810d7400000000000000000000007c005f0100000000000000
-                  006e077c027c005f01000000000000000067007c005f0200000000000000
-                  007c017c005f03000000000000000069007c005f04000000000000000074
-                  0b00000000000000000000a6000000ab0000000000000000007c005f0600
-                  0000000000000064005300
-                29           0 RESUME                   0
-               
-                30           2 LOAD_FAST                2 (pool_class)
-                             4 POP_JUMP_FORWARD_IF_NONE    13 (to 32)
-               
-                31           6 LOAD_GLOBAL              0 (Pool)
-                            18 LOAD_FAST                0 (self)
-                            20 STORE_ATTR               1 (pool_class)
-                            30 JUMP_FORWARD             7 (to 46)
-               
-                33     >>   32 LOAD_FAST                2 (pool_class)
-                            34 LOAD_FAST                0 (self)
-                            36 STORE_ATTR               1 (pool_class)
-               
-                35     >>   46 BUILD_LIST               0
-                            48 LOAD_FAST                0 (self)
-                            50 STORE_ATTR               2 (engine_tokenizers)
-               
-                36          60 LOAD_FAST                1 (file)
-                            62 LOAD_FAST                0 (self)
-                            64 STORE_ATTR               3 (file)
-               
-                37          74 BUILD_MAP                0
-                            76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               4 (tokens)
-               
-                38          88 LOAD_GLOBAL             11 (NULL + RLock)
-                           100 PRECALL                  0
-                           104 CALL                     0
-                           114 LOAD_FAST                0 (self)
-                           116 STORE_ATTR               6 (tokenizers_lock)
-                           126 LOAD_CONST               0 (None)
-                           128 RETURN_VALUE
-               consts
-                  None
-               names      ('Pool', 'pool_class', 'engine_tokenizers', 'file', 'tokens', 'RLock', 'tokenizers_lock')
-               varnames   ('self', 'file', 'pool_class')
-               freevars   ()
-               cellvars   ()
-               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-               name       '__init__'
-               firstlineno 29
-               lnotab 0x020104011a020e020e010e010e01
-            'engine'
-            'tokenizers'
+            'CliScanMode'
+            'engines_enabled'
+            'rulesets'
             'return'
+            None
             code
-               argcount  : 3
-               nlocals   : 4
+               argcount  : 1
+               nlocals   : 6
                stacksize : 7
                flags     : 3
                code
-                  0x97007c0244005d2b7d037c006a000000000000000000a0010000000000
-                  0000000000000000000000000000007405000000000000000000007c017c
-                  03ac01a6020000ab020000000000000000a6010000ab0100000000000000
-                  0001008c2c64005300
-                40           0 RESUME                   0
-               
-                41           2 LOAD_FAST                2 (tokenizers)
-                             4 GET_ITER
-                       >>    6 FOR_ITER                43 (to 94)
-                             8 STORE_FAST               3 (tokenizer)
-               
-                42          10 LOAD_FAST                0 (self)
-                            12 LOAD_ATTR                0 (engine_tokenizers)
-                            22 LOAD_METHOD              1 (append)
-                            44 LOAD_GLOBAL              5 (NULL + EngineWithTokenizer)
-                            56 LOAD_FAST                1 (engine)
-                            58 LOAD_FAST                3 (tokenizer)
-                            60 KW_NAMES                 1
-                            62 PRECALL                  2
-                            66 CALL                     2
-                            76 PRECALL                  1
-                            80 CALL                     1
-                            90 POP_TOP
-                            92 JUMP_BACKWARD           44 (to 6)
+                  0x97007401000000000000000000006a0100000000000000006401740500
+                  0000000000000000007c006a030000000000000000a6010000ab01000000
+                  00000000009b0064029d03a6010000ab0100000000000000000100740500
+                  0000000000000000007c006a030000000000000000a6010000ab01000000
+                  000000000064036b02000000007202640053007c006a0400000000000000
+                  006a05000000000000000044005d117d0164047c006a0600000000000000
+                  007c016a0700000000000000003c0000008c127c006a0400000000000000
+                  006a080000000000000000a0090000000000000000000000000000000000
+                  000000a6000000ab00000000000000000044005d5a5c0200007d027d0302
+                  007c02a6000000ab0000000000000000007d047c0344005d347d057c04a0
+                  0a0000000000000000000000000000000000000000741600000000000000
+                  0000006a0c0000000000000000a00d000000000000000000000000000000
+                  00000000007c05a6010000ab010000000000000000a6010000ab01000000
+                  000000000001008c357c046a0e00000000000000007c006a080000000000
+                  0000007c046a0f00000000000000003c0000008c5b64005300
+                25           0 RESUME                   0
+               
+                26           2 LOAD_GLOBAL              1 (NULL + logger)
+                            14 LOAD_ATTR                1 (info)
+                            24 LOAD_CONST               1 ('Found ')
+                            26 LOAD_GLOBAL              5 (NULL + len)
+                            38 LOAD_FAST                0 (self)
+                            40 LOAD_ATTR                3 (filepaths)
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 FORMAT_VALUE             0
+                            66 LOAD_CONST               2 (' applicable files for the scan')
+                            68 BUILD_STRING             3
+                            70 PRECALL                  1
+                            74 CALL                     1
+                            84 POP_TOP
+               
+                27          86 LOAD_GLOBAL              5 (NULL + len)
+                            98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                3 (filepaths)
+                           110 PRECALL                  1
+                           114 CALL                     1
+                           124 LOAD_CONST               3 (0)
+                           126 COMPARE_OP               2 (==)
+                           132 POP_JUMP_FORWARD_IF_FALSE     2 (to 138)
+               
+                28         134 LOAD_CONST               0 (None)
+                           136 RETURN_VALUE
+               
+                30     >>  138 LOAD_FAST                0 (self)
+                           140 LOAD_ATTR                4 (config)
+                           150 LOAD_ATTR                5 (engines)
+                           160 GET_ITER
+                       >>  162 FOR_ITER                17 (to 198)
+                           164 STORE_FAST               1 (engine)
+               
+                31         166 LOAD_CONST               4 (True)
+                           168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                6 (engines_enabled)
+                           180 LOAD_FAST                1 (engine)
+                           182 LOAD_ATTR                7 (name)
+                           192 STORE_SUBSCR
+                           196 JUMP_BACKWARD           18 (to 162)
+               
+                33     >>  198 LOAD_FAST                0 (self)
+                           200 LOAD_ATTR                4 (config)
+                           210 LOAD_ATTR                8 (rulesets)
+                           220 LOAD_METHOD              9 (items)
+                           242 PRECALL                  0
+                           246 CALL                     0
+                           256 GET_ITER
+                       >>  258 FOR_ITER                90 (to 440)
+                           260 UNPACK_SEQUENCE          2
+                           264 STORE_FAST               2 (ruleset_builder)
+                           266 STORE_FAST               3 (paths)
+               
+                34         268 PUSH_NULL
+                           270 LOAD_FAST                2 (ruleset_builder)
+                           272 PRECALL                  0
+                           276 CALL                     0
+                           286 STORE_FAST               4 (builder)
+               
+                35         288 LOAD_FAST                3 (paths)
+                           290 GET_ITER
+                       >>  292 FOR_ITER                52 (to 398)
+                           294 STORE_FAST               5 (path)
+               
+                36         296 LOAD_FAST                4 (builder)
+                           298 LOAD_METHOD             10 (with_rules_from_file)
+                           320 LOAD_GLOBAL             22 (os)
+                           332 LOAD_ATTR               12 (path)
+                           342 LOAD_METHOD             13 (abspath)
+                           364 LOAD_FAST                5 (path)
+                           366 PRECALL                  1
+                           370 CALL                     1
+                           380 PRECALL                  1
+                           384 CALL                     1
+                           394 POP_TOP
+                           396 JUMP_BACKWARD           53 (to 292)
                
-                41     >>   94 LOAD_CONST               0 (None)
-                            96 RETURN_VALUE
+                37     >>  398 LOAD_FAST                4 (builder)
+                           400 LOAD_ATTR               14 (rules)
+                           410 LOAD_FAST                0 (self)
+                           412 LOAD_ATTR                8 (rulesets)
+                           422 LOAD_FAST                4 (builder)
+                           424 LOAD_ATTR               15 (ruleset_name)
+                           434 STORE_SUBSCR
+                           438 JUMP_BACKWARD           91 (to 258)
+               
+                33     >>  440 LOAD_CONST               0 (None)
+                           442 RETURN_VALUE
                consts
                   None
-                  ('engine', 'tokenizer')
-               names      ('engine_tokenizers', 'append', 'EngineWithTokenizer')
-               varnames   ('self', 'engine', 'tokenizers', 'tokenizer')
+                  'Found '
+                  ' applicable files for the scan'
+                  0
+                  True
+               names      ('logger', 'info', 'len', 'filepaths', 'config', 'engines', 'engines_enabled', 'name', 'rulesets', 'items', 'with_rules_from_file', 'os', 'path', 'abspath', 'rules', 'ruleset_name')
+               varnames   ('self', 'engine', 'ruleset_builder', 'paths', 'builder', 'path')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-               name       'add_engine'
-               firstlineno 40
-               lnotab 0x0201080154ff
-            False
-            'threaded'
+               filename   '/app/deepsecrets/scan_modes/cli.py'
+               name       'prepare_for_scan'
+               firstlineno 25
+               lnotab 0x02015401300104021c01200246011401080166012afc
             code
-               argcount  : 2
-               nlocals   : 7
-               stacksize : 6
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
                flags     : 3
                code
-                  0x970067007d027c0172977c00a000000000000000000000000000000000
-                  00000000006401a6010000ab01000000000000000035007d037c03a00100
-                  000000000000000000000000000000000000007c006a0200000000000000
-                  007c006a030000000000000000a6020000ab0200000000000000007d047c
-                  03a0040000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001007c03a0050000000000000000000000000000000000
-                  000000a6000000ab0000000000000000000100640064006400a6020000ab
-                  02000000000000000001006e0b2300310073047702780359007701010059
-                  00010001007c0480027c0253007c0444005d1a7d057c0573018c057c02a0
-                  0600000000000000000000000000000000000000007c05a6010000ab0100
-                  0000000000000001008c1b6e327c006a03000000000000000044005d2a7d
-                  067c02a00600000000000000000000000000000000000000007c00a00200
-                  000000000000000000000000000000000000007c06a6010000ab01000000
-                  0000000000a6010000ab01000000000000000001008c2b7c025300
-                44           0 RESUME                   0
-               
-                45           2 BUILD_LIST               0
-                             4 STORE_FAST               2 (results)
-               
-                47           6 LOAD_FAST                1 (threaded)
-                             8 POP_JUMP_FORWARD_IF_FALSE   151 (to 312)
-               
-                48          10 LOAD_FAST                0 (self)
-                            12 LOAD_METHOD              0 (pool_class)
-                            34 LOAD_CONST               1 (2)
-                            36 PRECALL                  1
-                            40 CALL                     1
-                            50 BEFORE_WITH
-                            52 STORE_FAST               3 (pool)
-               
-                49          54 LOAD_FAST                3 (pool)
-                            56 LOAD_METHOD              1 (imap)
-                            78 LOAD_FAST                0 (self)
-                            80 LOAD_ATTR                2 (_run_engine)
-                            90 LOAD_FAST                0 (self)
-                            92 LOAD_ATTR                3 (engine_tokenizers)
-                           102 PRECALL                  2
-                           106 CALL                     2
-                           116 STORE_FAST               4 (engine_results)
-               
-                50         118 LOAD_FAST                3 (pool)
-                           120 LOAD_METHOD              4 (close)
-                           142 PRECALL                  0
-                           146 CALL                     0
-                           156 POP_TOP
-               
-                51         158 LOAD_FAST                3 (pool)
-                           160 LOAD_METHOD              5 (join)
-                           182 PRECALL                  0
-                           186 CALL                     0
-                           196 POP_TOP
-               
-                48         198 LOAD_CONST               0 (None)
-                           200 LOAD_CONST               0 (None)
-                           202 LOAD_CONST               0 (None)
-                           204 PRECALL                  2
-                           208 CALL                     2
-                           218 POP_TOP
-                           220 JUMP_FORWARD            11 (to 244)
-                       >>  222 PUSH_EXC_INFO
-                           224 WITH_EXCEPT_START
-                           226 POP_JUMP_FORWARD_IF_TRUE     4 (to 236)
-                           228 RERAISE                  2
-                       >>  230 COPY                     3
-                           232 POP_EXCEPT
-                           234 RERAISE                  1
-                       >>  236 POP_TOP
-                           238 POP_EXCEPT
-                           240 POP_TOP
-                           242 POP_TOP
-               
-                53     >>  244 LOAD_FAST                4 (engine_results)
-                           246 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 252)
-               
-                54         248 LOAD_FAST                2 (results)
-                           250 RETURN_VALUE
-               
-                56     >>  252 LOAD_FAST                4 (engine_results)
-                           254 GET_ITER
-                       >>  256 FOR_ITER                26 (to 310)
-                           258 STORE_FAST               5 (er)
-               
-                57         260 LOAD_FAST                5 (er)
-                           262 POP_JUMP_FORWARD_IF_TRUE     1 (to 266)
-               
-                58         264 JUMP_BACKWARD            5 (to 256)
-               
-                59     >>  266 LOAD_FAST                2 (results)
-                           268 LOAD_METHOD              6 (extend)
-                           290 LOAD_FAST                5 (er)
-                           292 PRECALL                  1
-                           296 CALL                     1
-                           306 POP_TOP
-                           308 JUMP_BACKWARD           27 (to 256)
-               
-                56     >>  310 JUMP_FORWARD            50 (to 412)
-               
-                62     >>  312 LOAD_FAST                0 (self)
-                           314 LOAD_ATTR                3 (engine_tokenizers)
-                           324 GET_ITER
-                       >>  326 FOR_ITER                42 (to 412)
-                           328 STORE_FAST               6 (et)
-               
-                63         330 LOAD_FAST                2 (results)
-                           332 LOAD_METHOD              6 (extend)
-                           354 LOAD_FAST                0 (self)
-                           356 LOAD_METHOD              2 (_run_engine)
-                           378 LOAD_FAST                6 (et)
-                           380 PRECALL                  1
-                           384 CALL                     1
-                           394 PRECALL                  1
-                           398 CALL                     1
-                           408 POP_TOP
-                           410 JUMP_BACKWARD           43 (to 326)
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a0010000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d017c01a0020000000000000000000000000000000000
+                  0000007c006a0300000000000000006a0400000000000000007c006a0500
+                  000000000000007c006a060000000000000000ac01a6030000ab03000000
+                  000000000001007c015300
+                             0 COPY_FREE_VARS           1
+               
+                40           2 RESUME                   0
+               
+                41           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (analyzer_bundle)
+                            52 PRECALL                  0
+                            56 CALL                     0
+                            66 STORE_FAST               1 (bundle)
+               
+                42          68 LOAD_FAST                1 (bundle)
+                            70 LOAD_METHOD              2 (update)
+               
+                43          92 LOAD_FAST                0 (self)
+                            94 LOAD_ATTR                3 (config)
+                           104 LOAD_ATTR                4 (workdir_path)
+               
+                44         114 LOAD_FAST                0 (self)
+                           116 LOAD_ATTR                5 (engines_enabled)
+               
+                45         126 LOAD_FAST                0 (self)
+                           128 LOAD_ATTR                6 (rulesets)
+               
+                42         138 KW_NAMES                 1
+                           140 PRECALL                  3
+                           144 CALL                     3
+                           154 POP_TOP
                
-                65     >>  412 LOAD_FAST                2 (results)
-                           414 RETURN_VALUE
-               ExceptionTable:
-                 52 to 196 -> 222 [1] lasti
-                 222 to 228 -> 230 [3] lasti
-                 236 to 236 -> 230 [3] lasti
+                47         156 LOAD_FAST                1 (bundle)
+                           158 RETURN_VALUE
                consts
                   None
-                  2
-               names      ('pool_class', 'imap', '_run_engine', 'engine_tokenizers', 'close', 'join', 'extend')
-               varnames   ('self', 'threaded', 'results', 'pool', 'engine_results', 'er', 'et')
-               freevars   ()
+                  ('workdir', 'engines', 'rulesets')
+               names      ('super', 'analyzer_bundle', 'update', 'config', 'workdir_path', 'engines_enabled', 'rulesets')
+               varnames   ('self', 'bundle')
+               freevars   ('__class__',)
                cellvars   ()
-               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-               name       'process'
-               firstlineno 44
-               lnotab
-                  0x0201040204012c014001280128fd2e05040104020801040102012cfd02
-                  0612015202
-            'et'
+               filename   '/app/deepsecrets/scan_modes/cli.py'
+               name       'analyzer_bundle'
+               firstlineno 40
+               lnotab 0x04014001180116010c010cfd1205
+            'file'
             code
                argcount  : 2
-               nlocals   : 10
+               nlocals   : 12
                stacksize : 7
                flags     : 3
                code
-                  0x970067007d0269007d037c006a000000000000000000350001007c016a
-                  0100000000000000007c006a0200000000000000007601722c7c016a0100
-                  00000000000000a00300000000000000000000000000000000000000007c
-                  006a040000000000000000a6010000ab0100000000000000007c006a0200
-                  000000000000007c016a0100000000000000003c000000640064006400a6
-                  020000ab02000000000000000001006e0b23003100730477027803590077
-                  0101005900010001007c006a0200000000000000007c016a010000000000
-                  000000190000000000000000007d047c0444005de57d057c03a005000000
-                  00000000000000000000000000000000007c05a006000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a6010000ab
-                  0100000000000000007d067c0681057c066401750072018c3064017c037c
-                  05a0060000000000000000000000000000000000000000a6000000ab0000
-                  000000000000003c00000009007c016a070000000000000000a008000000
-                  00000000000000000000000000000000007c05a6010000ab010000000000
-                  0000007d077c0744005d557d087c08a00900000000000000000000000000
-                  000000000000007c006a0400000000000000007c056a0a00000000000000
-                  00640219000000000000000000ac03a6020000ab02000000000000000001
-                  007c02a00b00000000000000000000000000000000000000007c08a60100
-                  00ab010000000000000000010064047c037c05a006000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000003c0000008c
-                  568cbb23007418000000000000000000002400721e7d09741b0000000000
-                  00000000006a0e00000000000000006405a6010000ab0100000000000000
-                  000100590064007d097e098cde64007d097e09770177007803590077017c
-                  025300
-                67           0 RESUME                   0
-               
-                68           2 BUILD_LIST               0
-                             4 STORE_FAST               2 (results)
-               
-                69           6 BUILD_MAP                0
-                             8 STORE_FAST               3 (processed_values)
-               
-                71          10 LOAD_FAST                0 (self)
-                            12 LOAD_ATTR                0 (tokenizers_lock)
-                            22 BEFORE_WITH
-                            24 POP_TOP
+                  0x97007400000000000000000000006a0100000000000000007404000000
+                  000000000000006a0300000000000000006b020000000072177401000000
+                  000000000000006a04000000000000000064017c019b009d02a6010000ab
+                  010000000000000000010067007d02740b000000000000000000007c0174
+                  0c00000000000000000000a6020000ab020000000000000000730f740f00
+                  0000000000000000006402a6010000ab0100000000000000008201741100
+                  0000000000000000007c017c01a009000000000000000000000000000000
+                  00000000007c006a0a00000000000000009b0064039d026404a6020000ab
+                  020000000000000000ac05a6020000ab0200000000000000007d017c016a
+                  0b000000000000000064066b020000000072027c02530074190000000000
+                  00000000007c01a6010000ab0100000000000000007d03741b0000000000
+                  0000000000a6000000ab0000000000000000007d04741d00000000000000
+                  0000006407ac08a6010000ab0100000000000000007d05741f0000000000
+                  00000000007c006a100000000000000000a0110000000000000000000000
+                  0000000000000000007424000000000000000000006a1300000000000000
+                  006700a6020000ab020000000000000000ac09a6010000ab010000000000
+                  0000007d067c006a140000000000000000a0150000000000000000000000
+                  000000000000000000a6000000ab00000000000000000044005dbf5c0200
+                  007d077d087c0873018c087c07741e000000000000000000006a16000000
+                  00000000006b020000000072177c03a01700000000000000000000000000
+                  000000000000007c067c046701a6020000ab02000000000000000001007c
+                  077430000000000000000000006a1600000000000000006b020000000072
+                  4a7431000000000000000000007c006a190000000000000000a011000000
+                  00000000000000000000000000000000007434000000000000000000006a
+                  1300000000000000006700a6020000ab020000000000000000ac09a60100
+                  00ab0100000000000000007d097c03a01700000000000000000000000000
+                  000000000000007c097c056701a6020000ab02000000000000000001007c
+                  077436000000000000000000006a1600000000000000006b020000000072
+                  267437000000000000000000007c06a6010000ab0100000000000000007d
+                  0a7c03a01700000000000000000000000000000000000000007c0a7c0567
+                  01a6020000ab02000000000000000001008cc009007c03a01c0000000000
+                  000000000000000000000000000000640aac0ba6010000ab010000000000
+                  0000007d026e2b2300740e000000000000000000002400721e7d0b740100
+                  0000000000000000006a1d00000000000000007c0ba6010000ab01000000
+                  00000000000100590064007d0b7e0b6e0864007d0b7e0b77017700780359
+                  007701743c00000000000000000000720109007c025300
+                50           0 RESUME                   0
+               
+                52           2 LOAD_GLOBAL              0 (logger)
+                            14 LOAD_ATTR                1 (level)
+                            24 LOAD_GLOBAL              4 (logging)
+                            36 LOAD_ATTR                3 (DEBUG)
+                            46 COMPARE_OP               2 (==)
+                            52 POP_JUMP_FORWARD_IF_FALSE    23 (to 100)
+               
+                53          54 LOAD_GLOBAL              1 (NULL + logger)
+                            66 LOAD_ATTR                4 (debug)
+                            76 LOAD_CONST               1 ('Starting analysis for ')
+                            78 LOAD_FAST                1 (file)
+                            80 FORMAT_VALUE             0
+                            82 BUILD_STRING             2
+                            84 PRECALL                  1
+                            88 CALL                     1
+                            98 POP_TOP
+               
+                55     >>  100 BUILD_LIST               0
+                           102 STORE_FAST               2 (results)
+               
+                57         104 LOAD_GLOBAL             11 (NULL + isinstance)
+                           116 LOAD_FAST                1 (file)
+                           118 LOAD_GLOBAL             12 (str)
+                           130 PRECALL                  2
+                           134 CALL                     2
+                           144 POP_JUMP_FORWARD_IF_TRUE    15 (to 176)
+               
+                58         146 LOAD_GLOBAL             15 (NULL + Exception)
+                           158 LOAD_CONST               2 ('Filepath as str expected')
+                           160 PRECALL                  1
+                           164 CALL                     1
+                           174 RAISE_VARARGS            1
+               
+                60     >>  176 LOAD_GLOBAL             17 (NULL + File)
+                           188 LOAD_FAST                1 (file)
+                           190 LOAD_FAST                1 (file)
+                           192 LOAD_METHOD              9 (replace)
+                           214 LOAD_FAST                0 (bundle)
+                           216 LOAD_ATTR               10 (workdir)
+                           226 FORMAT_VALUE             0
+                           228 LOAD_CONST               3 ('/')
+                           230 BUILD_STRING             2
+                           232 LOAD_CONST               4 ('')
+                           234 PRECALL                  2
+                           238 CALL                     2
+                           248 KW_NAMES                 5
+                           250 PRECALL                  2
+                           254 CALL                     2
+                           264 STORE_FAST               1 (file)
+               
+                61         266 LOAD_FAST                1 (file)
+                           268 LOAD_ATTR               11 (length)
+                           278 LOAD_CONST               6 (0)
+                           280 COMPARE_OP               2 (==)
+                           286 POP_JUMP_FORWARD_IF_FALSE     2 (to 292)
+               
+                62         288 LOAD_FAST                2 (results)
+                           290 RETURN_VALUE
+               
+                64     >>  292 LOAD_GLOBAL             25 (NULL + FileAnalyzer)
+                           304 LOAD_FAST                1 (file)
+                           306 PRECALL                  1
+                           310 CALL                     1
+                           320 STORE_FAST               3 (file_analyzer)
+               
+                65         322 LOAD_GLOBAL             27 (NULL + FullContentTokenizer)
+                           334 PRECALL                  0
+                           338 CALL                     0
+                           348 STORE_FAST               4 (fct)
+               
+                66         350 LOAD_GLOBAL             29 (NULL + LexerTokenizer)
+                           362 LOAD_CONST               7 (True)
+                           364 KW_NAMES                 8
+                           366 PRECALL                  1
+                           370 CALL                     1
+                           380 STORE_FAST               5 (lex)
+               
+                68         382 LOAD_GLOBAL             31 (NULL + RegexEngine)
+               
+                69         394 LOAD_FAST                0 (bundle)
+                           396 LOAD_ATTR               16 (rulesets)
+                           406 LOAD_METHOD             17 (get)
+                           428 LOAD_GLOBAL             36 (RegexRulesetBuilder)
+                           440 LOAD_ATTR               19 (ruleset_name)
+                           450 BUILD_LIST               0
+                           452 PRECALL                  2
+                           456 CALL                     2
+               
+                68         466 KW_NAMES                 9
+                           468 PRECALL                  1
+                           472 CALL                     1
+                           482 STORE_FAST               6 (regex_engine)
+               
+                72         484 LOAD_FAST                0 (bundle)
+                           486 LOAD_ATTR               20 (engines)
+                           496 LOAD_METHOD             21 (items)
+                           518 PRECALL                  0
+                           522 CALL                     0
+                           532 GET_ITER
+                       >>  534 FOR_ITER               191 (to 918)
+                           536 UNPACK_SEQUENCE          2
+                           540 STORE_FAST               7 (eng)
+                           542 STORE_FAST               8 (enabled)
+               
+                73         544 LOAD_FAST                8 (enabled)
+                           546 POP_JUMP_FORWARD_IF_TRUE     1 (to 550)
+               
+                74         548 JUMP_BACKWARD            8 (to 534)
+               
+                76     >>  550 LOAD_FAST                7 (eng)
+                           552 LOAD_GLOBAL             30 (RegexEngine)
+                           564 LOAD_ATTR               22 (name)
+                           574 COMPARE_OP               2 (==)
+                           580 POP_JUMP_FORWARD_IF_FALSE    23 (to 628)
+               
+                77         582 LOAD_FAST                3 (file_analyzer)
+                           584 LOAD_METHOD             23 (add_engine)
+                           606 LOAD_FAST                6 (regex_engine)
+                           608 LOAD_FAST                4 (fct)
+                           610 BUILD_LIST               1
+                           612 PRECALL                  2
+                           616 CALL                     2
+                           626 POP_TOP
+               
+                79     >>  628 LOAD_FAST                7 (eng)
+                           630 LOAD_GLOBAL             48 (HashedSecretEngine)
+                           642 LOAD_ATTR               22 (name)
+                           652 COMPARE_OP               2 (==)
+                           658 POP_JUMP_FORWARD_IF_FALSE    74 (to 808)
+               
+                80         660 LOAD_GLOBAL             49 (NULL + HashedSecretEngine)
+               
+                81         672 LOAD_FAST                0 (bundle)
+                           674 LOAD_ATTR               25 (ruleset)
+                           684 LOAD_METHOD             17 (get)
+                           706 LOAD_GLOBAL             52 (HashedSecretsRulesetBuilder)
+                           718 LOAD_ATTR               19 (ruleset_name)
+                           728 BUILD_LIST               0
+                           730 PRECALL                  2
+                           734 CALL                     2
+               
+                80         744 KW_NAMES                 9
+                           746 PRECALL                  1
+                           750 CALL                     1
+                           760 STORE_FAST               9 (hashed_secret_engine)
+               
+                83         762 LOAD_FAST                3 (file_analyzer)
+                           764 LOAD_METHOD             23 (add_engine)
+                           786 LOAD_FAST                9 (hashed_secret_engine)
+                           788 LOAD_FAST                5 (lex)
+                           790 BUILD_LIST               1
+                           792 PRECALL                  2
+                           796 CALL                     2
+                           806 POP_TOP
+               
+                85     >>  808 LOAD_FAST                7 (eng)
+                           810 LOAD_GLOBAL             54 (SemanticEngine)
+                           822 LOAD_ATTR               22 (name)
+                           832 COMPARE_OP               2 (==)
+                           838 POP_JUMP_FORWARD_IF_FALSE    38 (to 916)
+               
+                86         840 LOAD_GLOBAL             55 (NULL + SemanticEngine)
+                           852 LOAD_FAST                6 (regex_engine)
+                           854 PRECALL                  1
+                           858 CALL                     1
+                           868 STORE_FAST              10 (semantic_engine)
+               
+                87         870 LOAD_FAST                3 (file_analyzer)
+                           872 LOAD_METHOD             23 (add_engine)
+                           894 LOAD_FAST               10 (semantic_engine)
+                           896 LOAD_FAST                5 (lex)
+                           898 BUILD_LIST               1
+                           900 PRECALL                  2
+                           904 CALL                     2
+                           914 POP_TOP
+                       >>  916 JUMP_BACKWARD          192 (to 534)
+               
+                89     >>  918 NOP
+               
+                90         920 LOAD_FAST                3 (file_analyzer)
+                           922 LOAD_METHOD             28 (process)
+                           944 LOAD_CONST              10 (False)
+                           946 KW_NAMES                11
+                           948 PRECALL                  1
+                           952 CALL                     1
+                           962 STORE_FAST               2 (results)
+                           964 JUMP_FORWARD            43 (to 1052)
+                       >>  966 PUSH_EXC_INFO
+               
+                91         968 LOAD_GLOBAL             14 (Exception)
+                           980 CHECK_EXC_MATCH
+                           982 POP_JUMP_FORWARD_IF_FALSE    30 (to 1044)
+                           984 STORE_FAST              11 (e)
+               
+                92         986 LOAD_GLOBAL              1 (NULL + logger)
+                           998 LOAD_ATTR               29 (exception)
+                          1008 LOAD_FAST               11 (e)
+                          1010 PRECALL                  1
+                          1014 CALL                     1
+                          1024 POP_TOP
+                          1026 POP_EXCEPT
+                          1028 LOAD_CONST               0 (None)
+                          1030 STORE_FAST              11 (e)
+                          1032 DELETE_FAST             11 (e)
+                          1034 JUMP_FORWARD             8 (to 1052)
+                       >> 1036 LOAD_CONST               0 (None)
+                          1038 STORE_FAST              11 (e)
+                          1040 DELETE_FAST             11 (e)
+                          1042 RERAISE                  1
+               
+                91     >> 1044 RERAISE                  0
+                       >> 1046 COPY                     3
+                          1048 POP_EXCEPT
+                          1050 RERAISE                  1
                
-                72          26 LOAD_FAST                1 (et)
-                            28 LOAD_ATTR                1 (tokenizer)
-                            38 LOAD_FAST                0 (self)
-                            40 LOAD_ATTR                2 (tokens)
-                            50 CONTAINS_OP              1
-                            52 POP_JUMP_FORWARD_IF_FALSE    44 (to 142)
-               
-                73          54 LOAD_FAST                1 (et)
-                            56 LOAD_ATTR                1 (tokenizer)
-                            66 LOAD_METHOD              3 (tokenize)
-                            88 LOAD_FAST                0 (self)
-                            90 LOAD_ATTR                4 (file)
-                           100 PRECALL                  1
-                           104 CALL                     1
-                           114 LOAD_FAST                0 (self)
-                           116 LOAD_ATTR                2 (tokens)
-                           126 LOAD_FAST                1 (et)
-                           128 LOAD_ATTR                1 (tokenizer)
-                           138 STORE_SUBSCR
-               
-                71     >>  142 LOAD_CONST               0 (None)
-                           144 LOAD_CONST               0 (None)
-                           146 LOAD_CONST               0 (None)
-                           148 PRECALL                  2
-                           152 CALL                     2
-                           162 POP_TOP
-                           164 JUMP_FORWARD            11 (to 188)
-                       >>  166 PUSH_EXC_INFO
-                           168 WITH_EXCEPT_START
-                           170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
-                           172 RERAISE                  2
-                       >>  174 COPY                     3
-                           176 POP_EXCEPT
-                           178 RERAISE                  1
-                       >>  180 POP_TOP
-                           182 POP_EXCEPT
-                           184 POP_TOP
-                           186 POP_TOP
-               
-                75     >>  188 LOAD_FAST                0 (self)
-                           190 LOAD_ATTR                2 (tokens)
-                           200 LOAD_FAST                1 (et)
-                           202 LOAD_ATTR                1 (tokenizer)
-                           212 BINARY_SUBSCR
-                           222 STORE_FAST               4 (tokens)
-               
-                77         224 LOAD_FAST                4 (tokens)
-                           226 GET_ITER
-                       >>  228 FOR_ITER               229 (to 688)
-                           230 STORE_FAST               5 (token)
-               
-                78         232 LOAD_FAST                3 (processed_values)
-                           234 LOAD_METHOD              5 (get)
-                           256 LOAD_FAST                5 (token)
-                           258 LOAD_METHOD              6 (val_hash)
-                           280 PRECALL                  0
-                           284 CALL                     0
-                           294 PRECALL                  1
-                           298 CALL                     1
-                           308 STORE_FAST               6 (is_known_content)
-               
-                79         310 LOAD_FAST                6 (is_known_content)
-                           312 POP_JUMP_FORWARD_IF_NONE     5 (to 324)
-                           314 LOAD_FAST                6 (is_known_content)
-                           316 LOAD_CONST               1 (False)
-                           318 IS_OP                    0
-                           320 POP_JUMP_FORWARD_IF_FALSE     1 (to 324)
-               
-                80         322 JUMP_BACKWARD           48 (to 228)
-               
-                82     >>  324 LOAD_CONST               1 (False)
-                           326 LOAD_FAST                3 (processed_values)
-                           328 LOAD_FAST                5 (token)
-                           330 LOAD_METHOD              6 (val_hash)
-                           352 PRECALL                  0
-                           356 CALL                     0
-                           366 STORE_SUBSCR
-               
-                84         370 NOP
-               
-                85         372 LOAD_FAST                1 (et)
-                           374 LOAD_ATTR                7 (engine)
-                           384 LOAD_METHOD              8 (search)
-                           406 LOAD_FAST                5 (token)
-                           408 PRECALL                  1
-                           412 CALL                     1
-                           422 STORE_FAST               7 (findings)
-               
-                86         424 LOAD_FAST                7 (findings)
-                           426 GET_ITER
-                       >>  428 FOR_ITER                85 (to 600)
-                           430 STORE_FAST               8 (finding)
-               
-                87         432 LOAD_FAST                8 (finding)
-                           434 LOAD_METHOD              9 (map_on_file)
-                           456 LOAD_FAST                0 (self)
-                           458 LOAD_ATTR                4 (file)
-                           468 LOAD_FAST                5 (token)
-                           470 LOAD_ATTR               10 (span)
-                           480 LOAD_CONST               2 (0)
-                           482 BINARY_SUBSCR
-                           492 KW_NAMES                 3
-                           494 PRECALL                  2
-                           498 CALL                     2
-                           508 POP_TOP
-               
-                88         510 LOAD_FAST                2 (results)
-                           512 LOAD_METHOD             11 (append)
-                           534 LOAD_FAST                8 (finding)
-                           536 PRECALL                  1
-                           540 CALL                     1
-                           550 POP_TOP
-               
-                89         552 LOAD_CONST               4 (True)
-                           554 LOAD_FAST                3 (processed_values)
-                           556 LOAD_FAST                5 (token)
-                           558 LOAD_METHOD              6 (val_hash)
-                           580 PRECALL                  0
-                           584 CALL                     0
-                           594 STORE_SUBSCR
-                           598 JUMP_BACKWARD           86 (to 428)
-               
-                86     >>  600 JUMP_BACKWARD          187 (to 228)
-                       >>  602 PUSH_EXC_INFO
-               
-                91         604 LOAD_GLOBAL             24 (Exception)
-                           616 CHECK_EXC_MATCH
-                           618 POP_JUMP_FORWARD_IF_FALSE    30 (to 680)
-                           620 STORE_FAST               9 (e)
-               
-                92         622 LOAD_GLOBAL             27 (NULL + logger)
-                           634 LOAD_ATTR               14 (error)
-                           644 LOAD_CONST               5 ('Unable to process token')
-                           646 PRECALL                  1
-                           650 CALL                     1
-                           660 POP_TOP
-               
-                93         662 POP_EXCEPT
-                           664 LOAD_CONST               0 (None)
-                           666 STORE_FAST               9 (e)
-                           668 DELETE_FAST              9 (e)
-                           670 JUMP_BACKWARD          222 (to 228)
-                       >>  672 LOAD_CONST               0 (None)
-                           674 STORE_FAST               9 (e)
-                           676 DELETE_FAST              9 (e)
-                           678 RERAISE                  1
-               
-                91     >>  680 RERAISE                  0
-                       >>  682 COPY                     3
-                           684 POP_EXCEPT
-                           686 RERAISE                  1
+                94     >> 1052 LOAD_GLOBAL             60 (PROFILER_ON)
+                          1064 POP_JUMP_FORWARD_IF_FALSE     1 (to 1068)
+               
+                95        1066 NOP
                
-                95     >>  688 LOAD_FAST                2 (results)
-                           690 RETURN_VALUE
+                97     >> 1068 LOAD_FAST                2 (results)
+                          1070 RETURN_VALUE
                ExceptionTable:
-                 24 to 140 -> 166 [1] lasti
-                 166 to 172 -> 174 [3] lasti
-                 180 to 180 -> 174 [3] lasti
-                 372 to 598 -> 602 [1]
-                 602 to 620 -> 682 [2] lasti
-                 622 to 660 -> 672 [2] lasti
-                 672 to 680 -> 682 [2] lasti
+                 920 to 962 -> 966 [0]
+                 966 to 984 -> 1046 [1] lasti
+                 986 to 1024 -> 1036 [1] lasti
+                 1036 to 1044 -> 1046 [1] lasti
                consts
                   None
-                  False
+                  'Starting analysis for '
+                  'Filepath as str expected'
+                  '/'
+                  ''
+                  ('path', 'relative_path')
                   0
-                  ('file', 'relative_start')
                   True
-                  'Unable to process token'
-               names      ('tokenizers_lock', 'tokenizer', 'tokens', 'tokenize', 'file', 'get', 'val_hash', 'engine', 'search', 'map_on_file', 'span', 'append', 'Exception', 'logger', 'error')
-               varnames   ('self', 'et', 'results', 'processed_values', 'tokens', 'token', 'is_known_content', 'findings', 'finding', 'e')
+                  ('deep_token_inspection',)
+                  ('ruleset',)
+                  False
+                  ('threaded',)
+               names      ('logger', 'level', 'logging', 'DEBUG', 'debug', 'isinstance', 'str', 'Exception', 'File', 'replace', 'workdir', 'length', 'FileAnalyzer', 'FullContentTokenizer', 'LexerTokenizer', 'RegexEngine', 'rulesets', 'get', 'RegexRulesetBuilder', 'ruleset_name', 'engines', 'items', 'name', 'add_engine', 'HashedSecretEngine', 'ruleset', 'HashedSecretsRulesetBuilder', 'SemanticEngine', 'process', 'exception', 'PROFILER_ON')
+               varnames   ('bundle', 'file', 'results', 'file_analyzer', 'fct', 'lex', 'regex_engine', 'eng', 'enabled', 'hashed_secret_engine', 'semantic_engine', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-               name       '_run_engine'
-               firstlineno 67
+               filename   '/app/deepsecrets/scan_modes/cli.py'
+               name       '_per_file_analyzer'
+               firstlineno 50
                lnotab
-                  0x02010401040210011c0158fe2e04240208014e010c0102022e02020134
-                  0108014e012a0130fd04051201280112fe0804
-            (None,)
-            (False,)
-         names      ('__name__', '__module__', '__qualname__', 'File', '__annotations__', 'List', 'EngineWithTokenizer', 'Dict', 'Type', 'Token', 'Optional', '__init__', 'IEngine', 'Tokenizer', 'add_engine', 'bool', 'Finding', 'process', '_run_engine')
+                  0x020234012e0204022a011e025a01160104021e011c0120020c0148ff12
+                  043c010401020220012e0220010c0148ff12032e0220011e013002020130
+                  0112013aff08030e010202
+            ('return', None)
+         names      ('__name__', '__module__', '__qualname__', 'engines_enabled', 'Dict', 'Type', 'bool', '__annotations__', 'rulesets', 'str', 'List', 'prepare_for_scan', 'DotWiz', 'analyzer_bundle', 'staticmethod', 'Any', 'Finding', '_per_file_analyzer', '__classcell__')
          varnames   ()
          freevars   ()
-         cellvars   ()
-         filename   '/app/deepsecrets/core/utils/file_analyzer.py'
-         name       'FileAnalyzer'
-         firstlineno 23
-         lnotab 0x0c010a01160126010a021e0b20041e17
-      'FileAnalyzer'
-      None
-   names      ('multiprocessing', 'RLock', 'multiprocessing.pool', 'Pool', 'typing', 'Dict', 'List', 'Optional', 'Type', 'pydantic', 'BaseModel', 'deepsecrets', 'logger', 'deepsecrets.core.engines.iengine', 'IEngine', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.finding', 'Finding', 'deepsecrets.core.model.token', 'Token', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'EngineWithTokenizer', 'FileAnalyzer')
+         cellvars   ('__class__',)
+         filename   '/app/deepsecrets/scan_modes/cli.py'
+         name       'CliScanMode'
+         firstlineno 21
+         lnotab 0x0e011e011e02080f100a02011aff0e01
+      'CliScanMode'
+   names      ('logging', 'os', 'typing', 'Any', 'Dict', 'List', 'Type', 'dotwiz', 'DotWiz', 'deepsecrets', 'PROFILER_ON', 'logger', 'deepsecrets.core.engines.hashed_secret', 'HashedSecretEngine', 'deepsecrets.core.engines.regex', 'RegexEngine', 'deepsecrets.core.engines.semantic', 'SemanticEngine', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.finding', 'Finding', 'deepsecrets.core.modes.iscan_mode', 'ScanMode', 'deepsecrets.core.rulesets.hashed_secrets', 'HashedSecretsRulesetBuilder', 'deepsecrets.core.rulesets.regex', 'RegexRulesetBuilder', 'deepsecrets.core.tokenizers.full_content', 'FullContentTokenizer', 'deepsecrets.core.tokenizers.lexer', 'LexerTokenizer', 'deepsecrets.core.utils.file_analyzer', 'FileAnalyzer', 'CliScanMode')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/app/deepsecrets/core/utils/file_analyzer.py'
+   filename   '/app/deepsecrets/scan_modes/cli.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0118020c020c010c010c010c010c010c031c08
+   lnotab
+      0x00ff02010801080118020c0210010c010c010c010c010c010c010c010c
+      010c010c010c03
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.1.0/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.1.0/deepsecrets/core/utils/file_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,11 +85,11 @@
                 findings: List[Finding] = et.engine.search(token)
                 for finding in findings:
                     finding.map_on_file(file=self.file, relative_start=token.span[0])
                     results.append(finding)
                     processed_values[token.val_hash()] = True
 
             except Exception as e:
-                logger.error('Unable to process token')
+                logger.exception('Unable to process token')
                 continue
 
         return results
```

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/fs.py` & `deepsecrets-1.1.0/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.1.0/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.1.0/deepsecrets/rules/excluded_paths.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {'insert': "[(31, OrderedDict([('name', 'Postman collection files'), ('pattern', "*

 * *           "'.*postman_collection\\\\.json$')]))]"}*

```diff
@@ -118,9 +118,13 @@
     {
         "name": "Path excluded",
         "pattern": ".*pbxproj$"
     },
     {
         "name": "Path excluded",
         "pattern": ".*go\\.sum$"
+    },
+    {
+        "name": "Postman collection files",
+        "pattern": ".*postman_collection\\.json$"
     }
 ]
```

### Comparing `deepsecrets-1.0.6/deepsecrets/rules/regexes.json` & `deepsecrets-1.1.0/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.1.0/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.6/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.1.0/deepsecrets/scan_modes/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from typing import Any, Dict, List, Type
 
 from dotwiz import DotWiz
 
 from deepsecrets import PROFILER_ON, logger
 from deepsecrets.core.engines.hashed_secret import HashedSecretEngine
@@ -44,15 +45,16 @@
             rulesets=self.rulesets,
         )
         return bundle
 
 
     @staticmethod
     def _per_file_analyzer(bundle, file: Any) -> List[Finding]:
-        logger.debug(f'Starting analysis for {file}')
+        if logger.level == logging.DEBUG:
+            logger.debug(f'Starting analysis for {file}')
 
         results: List[Finding] = []
 
         if not isinstance(file, str):
             raise Exception('Filepath as str expected')
 
         file = File(path=file, relative_path=file.replace(f'{bundle.workdir}/', ''))
@@ -83,13 +85,13 @@
             if eng == SemanticEngine.name:
                 semantic_engine = SemanticEngine(regex_engine)
                 file_analyzer.add_engine(semantic_engine, [lex])
 
         try:
             results = file_analyzer.process(threaded=False)
         except Exception as e:
-            logger.error(e)
+            logger.exception(e)
 
         if PROFILER_ON:
             pass
 
         return results
```

### Comparing `deepsecrets-1.0.6/pyproject.toml` & `deepsecrets-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.0.6"
+version = "1.1.0"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
@@ -33,14 +33,17 @@
 pydantic = "^1.10.4"
 pyyaml = "^5.4.1"
 pygments = "^2.14.0"
 ordered-set = "^4.1.0"
 dotwiz = "^0.4.0"
 mmh3 = "^3.0.0"
 regex = "^2023.3.23"
+jsx-lexer = "^2.0.1"
+aenum = "^3.1.15"
+puppetparser = "^0.2.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 coverage = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `deepsecrets-1.0.6/PKG-INFO` & `deepsecrets-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.0.6
+Version: 1.1.0
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
@@ -12,17 +12,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
+Requires-Dist: aenum (>=3.1.15,<4.0.0)
 Requires-Dist: dotwiz (>=0.4.0,<0.5.0)
+Requires-Dist: jsx-lexer (>=2.0.1,<3.0.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
+Requires-Dist: puppetparser (>=0.2.0,<0.3.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Project-URL: Bug Tracker, https://github.com/avito-tech/deepsecrets/issues
 Project-URL: Homepage, https://github.com/avito-tech/deepsecrets
 Description-Content-Type: text/markdown
```

