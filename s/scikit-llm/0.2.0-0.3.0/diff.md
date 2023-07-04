# Comparing `tmp/scikit-llm-0.2.0.tar.gz` & `tmp/scikit-llm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.2.0.tar", last modified: Sun Jun 11 19:20:41 2023, max compression
+gzip compressed data, was "scikit-llm-0.3.0.tar", last modified: Tue Jul  4 20:13:20 2023, max compression
```

## Comparing `scikit-llm-0.2.0.tar` & `scikit-llm-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,60 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.985105 scikit-llm-0.2.0/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.2.0/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    11027 2023-06-11 19:20:41.984647 scikit-llm-0.2.0/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    10473 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/README.md
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1927 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/pyproject.toml
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.966612 scikit-llm-0.2.0/scikit_llm.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    11027 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1027 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      102 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-06-11 19:20:41.000000 scikit-llm-0.2.0/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-06-11 19:20:41.985282 scikit-llm-0.2.0/setup.cfg
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.969728 scikit-llm-0.2.0/skllm/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      305 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/completions.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-06-11 11:27:57.000000 scikit-llm-0.2.0/skllm/config.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.973225 scikit-llm-0.2.0/skllm/datasets/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      273 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/datasets/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.2.0/skllm/datasets/multi_class.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.2.0/skllm/datasets/multi_label.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.2.0/skllm/datasets/summarization.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      818 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/datasets/translation.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      992 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/gpt4all_client.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.975263 scikit-llm-0.2.0/skllm/memory/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       49 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3269 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/_annoy.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1027 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/memory/base.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.976609 scikit-llm-0.2.0/skllm/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4007 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/skllm/models/gpt_dyn_few_shot_clf.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1865 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/models/gpt_few_shot_clf.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)    11346 2023-06-08 20:44:51.000000 scikit-llm-0.2.0/skllm/models/gpt_zero_shot_clf.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.979474 scikit-llm-0.2.0/skllm/openai/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2941 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/base_gpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2513 2023-06-08 21:17:13.000000 scikit-llm-0.2.0/skllm/openai/chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      310 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/credentials.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1441 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/embeddings.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1200 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/openai/mixin.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.981300 scikit-llm-0.2.0/skllm/preprocessing/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      183 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/preprocessing/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1380 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_summarizer.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1011 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_translator.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3044 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/preprocessing/gpt_vectorizer.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.982214 scikit-llm-0.2.0/skllm/prompts/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3381 2023-05-30 12:28:04.000000 scikit-llm-0.2.0/skllm/prompts/builders.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     3608 2023-06-04 11:52:37.000000 scikit-llm-0.2.0/skllm/prompts/templates.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      996 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/skllm/utils.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-11 19:20:41.984075 scikit-llm-0.2.0/tests/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1763 2023-06-08 16:25:48.000000 scikit-llm-0.2.0/tests/test_chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1821 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/tests/test_gpt_few_shot_clf.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     4480 2023-06-11 19:20:26.000000 scikit-llm-0.2.0/tests/test_gpt_zero_shot_clf.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1077 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    12301 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    11747 2023-07-04 20:09:01.000000 scikit-llm-0.3.0/README.md
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1983 2023-07-04 20:12:37.000000 scikit-llm-0.3.0/pyproject.toml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/scikit_llm.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    12301 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1231 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      149 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        6 2023-07-04 20:13:20.000000 scikit-llm-0.3.0/scikit_llm.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      317 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      740 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/completions.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2960 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/config.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/datasets/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      273 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5870 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/multi_class.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1438 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/multi_label.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2729 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/summarization.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      818 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/datasets/translation.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/google/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1403 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/google/completions.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      507 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/google/tuning.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      992 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/gpt4all_client.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/memory/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       49 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3269 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/_annoy.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1027 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/memory/base.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.022403 scikit-llm-0.3.0/skllm/models/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5956 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/_base.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/models/gpt/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      260 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4049 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_dyn_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1827 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5829 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/gpt/gpt_zero_shot_clf.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/models/palm/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      122 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4854 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/palm_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2313 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/models/palm/palm_est.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/openai/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2829 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/base_gpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2074 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/chatgpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      730 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/openai/credentials.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1441 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/openai/embeddings.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1200 2023-06-17 21:25:38.000000 scikit-llm-0.3.0/skllm/openai/mixin.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/preprocessing/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      183 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2237 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_summarizer.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1400 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_translator.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3044 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/preprocessing/gpt_vectorizer.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/skllm/prompts/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4130 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/skllm/prompts/builders.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4310 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/prompts/templates.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1697 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/skllm/utils.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-04 20:13:20.026403 scikit-llm-0.3.0/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1763 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/tests/test_chatgpt.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1821 2023-06-17 15:57:54.000000 scikit-llm-0.3.0/tests/test_gpt_few_shot_clf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4376 2023-07-04 20:07:18.000000 scikit-llm-0.3.0/tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.2.0/LICENSE` & `scikit-llm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/PKG-INFO` & `scikit-llm-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7363 696b  : 2.1.Name: scik
 00000020: 6974 2d6c 6c6d 0a56 6572 7369 6f6e 3a20  it-llm.Version: 
-00000030: 302e 322e 300a 5375 6d6d 6172 793a 2053  0.2.0.Summary: S
+00000030: 302e 332e 300a 5375 6d6d 6172 793a 2053  0.3.0.Summary: S
 00000040: 6369 6b69 742d 4c4c 4d3a 2053 6561 6d6c  cikit-LLM: Seaml
 00000050: 6573 736c 7920 696e 7465 6772 6174 6520  essly integrate 
 00000060: 706f 7765 7266 756c 206c 616e 6775 6167  powerful languag
 00000070: 6520 6d6f 6465 6c73 206c 696b 6520 4368  e models like Ch
 00000080: 6174 4750 5420 696e 746f 2073 6369 6b69  atGPT into sciki
 00000090: 742d 6c65 6172 6e20 666f 7220 656e 6861  t-learn for enha
 000000a0: 6e63 6564 2074 6578 7420 616e 616c 7973  nced text analys
@@ -60,631 +60,710 @@
 000003b0: 6f6a 6563 7420 696e 2074 6865 2066 6f6c  oject in the fol
 000003c0: 6c6f 7769 6e67 2077 6179 733a 0a0a 2d20  lowing ways:..- 
 000003d0: e2ad 9020 5374 6172 2053 6369 6b69 742d  ... Star Scikit-
 000003e0: 4c4c 4d20 6f6e 2047 6974 4875 6220 2863  LLM on GitHub (c
 000003f0: 6c69 636b 2074 6865 2073 7461 7220 6275  lick the star bu
 00000400: 7474 6f6e 2069 6e20 7468 6520 746f 7020  tton in the top 
 00000410: 7269 6768 7420 636f 726e 6572 290a 2d20  right corner).- 
-00000420: f09f 90a6 2043 6865 636b 206f 7574 206f  .... Check out o
-00000430: 7572 2072 656c 6174 6564 2070 726f 6a65  ur related proje
-00000440: 6374 202d 205b 4661 6c63 6f6e 2041 7574  ct - [Falcon Aut
-00000450: 6f4d 4c5d 2868 7474 7073 3a2f 2f67 6974  oML](https://git
-00000460: 6875 622e 636f 6d2f 4f4b 5541 312f 6661  hub.com/OKUA1/fa
-00000470: 6c63 6f6e 290a 2d20 f09f 92a1 2050 726f  lcon).- .... Pro
-00000480: 7669 6465 2079 6f75 7220 6665 6564 6261  vide your feedba
-00000490: 636b 206f 7220 7072 6f70 6f73 6520 6964  ck or propose id
-000004a0: 6561 7320 696e 2074 6865 205b 6973 7375  eas in the [issu
-000004b0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000004c0: 7562 2e63 6f6d 2f69 7279 6e61 2d6b 6f6e  ub.com/iryna-kon
-000004d0: 6472 2f73 6369 6b69 742d 6c6c 6d2f 6973  dr/scikit-llm/is
-000004e0: 7375 6573 2920 7365 6374 696f 6e20 6f72  sues) section or
-000004f0: 205b 4469 7363 6f72 645d 2868 7474 7073   [Discord](https
-00000500: 3a2f 2f64 6973 636f 7264 2e67 672f 5944  ://discord.gg/YD
-00000510: 4162 7775 574b 3756 290a 2d20 f09f 9497  AbwuWK7V).- ....
-00000520: 2050 6f73 7420 6162 6f75 7420 5363 696b   Post about Scik
-00000530: 6974 2d4c 4c4d 206f 6e20 4c69 6e6b 6564  it-LLM on Linked
-00000540: 496e 206f 7220 6f74 6865 7220 706c 6174  In or other plat
-00000550: 666f 726d 730a 0a23 2320 446f 6375 6d65  forms..## Docume
-00000560: 6e74 6174 696f 6e20 f09f 939a 0a0a 2323  ntation ......##
-00000570: 2320 436f 6e66 6967 7572 696e 6720 4f70  # Configuring Op
-00000580: 656e 4149 2041 5049 204b 6579 0a0a 4174  enAI API Key..At
-00000590: 2074 6865 206d 6f6d 656e 7420 7468 6520   the moment the 
-000005a0: 6d61 6a6f 7269 7479 206f 6620 7468 6520  majority of the 
-000005b0: 5363 696b 6974 2d4c 4c4d 2065 7374 696d  Scikit-LLM estim
-000005c0: 6174 6f72 7320 6172 6520 6f6e 6c79 2063  ators are only c
-000005d0: 6f6d 7061 7469 626c 6520 7769 7468 2073  ompatible with s
-000005e0: 6f6d 6520 6f66 2074 6865 204f 7065 6e41  ome of the OpenA
-000005f0: 4920 6d6f 6465 6c73 2e20 4865 6e63 652c  I models. Hence,
-00000600: 2061 2075 7365 722d 7072 6f76 6964 6564   a user-provided
-00000610: 204f 7065 6e41 4920 4150 4920 6b65 7920   OpenAI API key 
-00000620: 6973 2072 6571 7569 7265 642e 0a0a 6060  is required...``
-00000630: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
-00000640: 6c6d 2e63 6f6e 6669 6720 696d 706f 7274  lm.config import
-00000650: 2053 4b4c 4c4d 436f 6e66 6967 0a0a 534b   SKLLMConfig..SK
-00000660: 4c4c 4d43 6f6e 6669 672e 7365 745f 6f70  LLMConfig.set_op
-00000670: 656e 6169 5f6b 6579 2822 3c59 4f55 525f  enai_key("<YOUR_
-00000680: 4b45 593e 2229 0a53 4b4c 4c4d 436f 6e66  KEY>").SKLLMConf
-00000690: 6967 2e73 6574 5f6f 7065 6e61 695f 6f72  ig.set_openai_or
-000006a0: 6728 223c 594f 5552 5f4f 5247 414e 4953  g("<YOUR_ORGANIS
-000006b0: 4154 494f 4e3e 2229 0a60 6060 0a0a 2a2a  ATION>").```..**
-000006c0: 496d 706f 7274 616e 7420 6e6f 7469 6365  Important notice
-000006d0: 3a2a 2a0a 0a2d 2049 6620 796f 7520 6861  :**..- If you ha
-000006e0: 7665 2061 2066 7265 6520 7472 6961 6c20  ve a free trial 
-000006f0: 4f70 656e 4149 2061 6363 6f75 6e74 2c20  OpenAI account, 
-00000700: 7468 6520 5b72 6174 6520 6c69 6d69 7473  the [rate limits
-00000710: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
-00000720: 726d 2e6f 7065 6e61 692e 636f 6d2f 646f  rm.openai.com/do
-00000730: 6373 2f67 7569 6465 732f 7261 7465 2d6c  cs/guides/rate-l
-00000740: 696d 6974 732f 6f76 6572 7669 6577 2920  imits/overview) 
-00000750: 6172 6520 6e6f 7420 7375 6666 6963 6965  are not sufficie
-00000760: 6e74 2028 7370 6563 6966 6963 616c 6c79  nt (specifically
-00000770: 2033 2072 6571 7565 7374 7320 7065 7220   3 requests per 
-00000780: 6d69 6e75 7465 292e 2050 6c65 6173 6520  minute). Please 
-00000790: 7377 6974 6368 2074 6f20 7468 6520 2270  switch to the "p
-000007a0: 6179 2061 7320 796f 7520 676f 2220 706c  ay as you go" pl
-000007b0: 616e 2066 6972 7374 2e0a 2d20 5768 656e  an first..- When
-000007c0: 2063 616c 6c69 6e67 2060 534b 4c4c 4d43   calling `SKLLMC
-000007d0: 6f6e 6669 672e 7365 745f 6f70 656e 6169  onfig.set_openai
-000007e0: 5f6f 7267 602c 2079 6f75 2068 6176 6520  _org`, you have 
-000007f0: 746f 2070 726f 7669 6465 2079 6f75 7220  to provide your 
-00000800: 6f72 6761 6e69 7a61 7469 6f6e 2049 4420  organization ID 
-00000810: 616e 6420 2a2a 4e4f 542a 2a20 7468 6520  and **NOT** the 
-00000820: 6e61 6d65 2e20 596f 7520 6361 6e20 6669  name. You can fi
-00000830: 6e64 2079 6f75 7220 4944 205b 6865 7265  nd your ID [here
-00000840: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
-00000850: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
-00000860: 636f 756e 742f 6f72 672d 7365 7474 696e  count/org-settin
-00000870: 6773 292e 0a0a 2323 2320 5573 696e 6720  gs)...### Using 
-00000880: 4750 5434 414c 4c0a 0a49 6e20 6164 6469  GPT4ALL..In addi
-00000890: 7469 6f6e 2074 6f20 4f70 656e 4149 2c20  tion to OpenAI, 
-000008a0: 736f 6d65 206f 6620 7468 6520 6d6f 6465  some of the mode
-000008b0: 6c73 2063 616e 2075 7365 205b 6770 7434  ls can use [gpt4
-000008c0: 616c 6c5d 2868 7474 7073 3a2f 2f67 7074  all](https://gpt
-000008d0: 3461 6c6c 2e69 6f2f 696e 6465 782e 6874  4all.io/index.ht
-000008e0: 6d6c 2920 6173 2061 2062 6163 6b65 6e64  ml) as a backend
-000008f0: 2e0a 0a2a 2a54 6869 7320 6665 6174 7572  ...**This featur
-00000900: 6520 6973 2063 6f6e 7369 6465 7265 6420  e is considered 
-00000910: 6869 676c 7920 6578 7065 7269 6d65 6e74  higly experiment
-00000920: 616c 212a 2a0a 0a49 6e20 6f72 6465 7220  al!**..In order 
-00000930: 746f 2075 7365 2067 7074 3461 6c6c 2c20  to use gpt4all, 
-00000940: 796f 7520 6e65 6564 2074 6f20 696e 7374  you need to inst
-00000950: 616c 6c20 7468 6520 636f 7272 6573 706f  all the correspo
-00000960: 6e64 696e 6720 7375 626d 6f64 756c 653a  nding submodule:
-00000970: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00000980: 7374 616c 6c20 2273 6369 6b69 742d 6c6c  stall "scikit-ll
-00000990: 6d5b 6770 7434 616c 6c5d 220a 6060 600a  m[gpt4all]".```.
-000009a0: 0a49 6e20 6f72 6465 7220 746f 2073 7769  .In order to swi
-000009b0: 7463 6820 6672 6f6d 204f 7065 6e41 4920  tch from OpenAI 
-000009c0: 746f 2047 5054 3441 4c4c 206d 6f64 656c  to GPT4ALL model
-000009d0: 2c20 7369 6d70 6c79 2070 726f 7669 6465  , simply provide
-000009e0: 2061 2073 7472 696e 6720 6f66 2074 6865   a string of the
-000009f0: 2066 6f72 6d61 7420 6067 7074 3461 6c6c   format `gpt4all
-00000a00: 3a3a 3c6d 6f64 656c 5f6e 616d 653e 6020  ::<model_name>` 
-00000a10: 6173 2061 6e20 6172 6775 6d65 6e74 2e20  as an argument. 
-00000a20: 5768 696c 6520 7468 6520 6d6f 6465 6c20  While the model 
-00000a30: 7275 6e73 2063 6f6d 706c 6574 656c 7920  runs completely 
-00000a40: 6c6f 6361 6c6c 792c 2074 6865 2065 7374  locally, the est
-00000a50: 696d 6174 6f72 2073 7469 6c6c 2074 7265  imator still tre
-00000a60: 6174 7320 6974 2061 7320 616e 204f 7065  ats it as an Ope
-00000a70: 6e41 4920 656e 6470 6f69 6e74 2061 6e64  nAI endpoint and
-00000a80: 2077 696c 6c20 7472 7920 746f 2063 6865   will try to che
-00000a90: 636b 2074 6861 7420 7468 6520 4150 4920  ck that the API 
-00000aa0: 6b65 7920 6973 2070 7265 7365 6e74 2e20  key is present. 
-00000ab0: 596f 7520 6361 6e20 7072 6f76 6964 6520  You can provide 
-00000ac0: 616e 7920 7374 7269 6e67 2061 7320 6120  any string as a 
-00000ad0: 6b65 792e 0a0a 6060 6070 7974 686f 6e0a  key...```python.
-00000ae0: 534b 4c4c 4d43 6f6e 6669 672e 7365 745f  SKLLMConfig.set_
-00000af0: 6f70 656e 6169 5f6b 6579 2822 616e 7920  openai_key("any 
-00000b00: 7374 7269 6e67 2229 0a53 4b4c 4c4d 436f  string").SKLLMCo
-00000b10: 6e66 6967 2e73 6574 5f6f 7065 6e61 695f  nfig.set_openai_
-00000b20: 6f72 6728 2261 6e79 2073 7472 696e 6722  org("any string"
-00000b30: 290a 0a5a 6572 6f53 686f 7447 5054 436c  )..ZeroShotGPTCl
-00000b40: 6173 7369 6669 6572 286f 7065 6e61 695f  assifier(openai_
-00000b50: 6d6f 6465 6c3d 2267 7074 3461 6c6c 3a3a  model="gpt4all::
-00000b60: 6767 6d6c 2d67 7074 3461 6c6c 2d6a 2d76  ggml-gpt4all-j-v
-00000b70: 312e 332d 6772 6f6f 7679 2229 0a60 6060  1.3-groovy").```
-00000b80: 0a0a 5768 656e 2072 756e 6e69 6e67 2066  ..When running f
-00000b90: 6f72 2074 6865 2066 6972 7374 2074 696d  or the first tim
-00000ba0: 652c 2074 6865 206d 6f64 656c 2066 696c  e, the model fil
-00000bb0: 6520 7769 6c6c 2062 6520 646f 776e 6c6f  e will be downlo
-00000bc0: 6164 6564 2061 7574 6f6d 6174 6961 6c6c  aded automatiall
-00000bd0: 792e 0a0a 4174 2074 6865 206d 6f6d 656e  y...At the momen
-00000be0: 7420 6f6e 6c79 2074 6865 2066 6f6c 6c6f  t only the follo
-00000bf0: 7769 6e67 2065 7374 696d 6174 6f72 7320  wing estimators 
-00000c00: 7375 7070 6f72 7420 6770 7434 616c 6c20  support gpt4all 
-00000c10: 6173 2061 2062 6163 6b65 6e64 3a0a 0a2d  as a backend:..-
-00000c20: 2060 5a65 726f 5368 6f74 4750 5443 6c61   `ZeroShotGPTCla
-00000c30: 7373 6966 6965 7260 0a2d 2060 4d75 6c74  ssifier`.- `Mult
-00000c40: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
-00000c50: 5443 6c61 7373 6966 6965 7260 0a2d 2060  TClassifier`.- `
-00000c60: 4665 7753 686f 7447 5054 436c 6173 7369  FewShotGPTClassi
-00000c70: 6669 6572 600a 0a57 6865 6e20 7573 696e  fier`..When usin
-00000c80: 6720 6770 7434 616c 6c20 706c 6561 7365  g gpt4all please
-00000c90: 206b 6565 7020 7468 6520 666f 6c6c 6f77   keep the follow
-00000ca0: 696e 6720 696e 206d 696e 643a 0a0a 312e  ing in mind:..1.
-00000cb0: 204e 6f74 2061 6c6c 2067 7074 3461 6c6c   Not all gpt4all
-00000cc0: 206d 6f64 656c 7320 6172 6520 636f 6d6d   models are comm
-00000cd0: 6572 6369 616c 6c79 206c 6963 656e 7361  ercially licensa
-00000ce0: 626c 652c 2070 6c65 6173 6520 636f 6e73  ble, please cons
-00000cf0: 756c 7420 6770 7434 616c 6c20 7765 6273  ult gpt4all webs
-00000d00: 6974 6520 666f 7220 6d6f 7265 2064 6574  ite for more det
-00000d10: 6169 6c73 2e0a 322e 2054 6865 2061 6363  ails..2. The acc
-00000d20: 7572 6163 7920 6f66 2074 6865 206d 6f64  uracy of the mod
-00000d30: 656c 7320 6d61 7920 6265 206d 7563 6820  els may be much 
-00000d40: 6c6f 7765 7220 636f 6d70 6172 6564 2074  lower compared t
-00000d50: 6f20 6f6e 6573 2070 726f 7669 6465 6420  o ones provided 
-00000d60: 6279 204f 7065 6e41 4920 2865 7370 6563  by OpenAI (espec
-00000d70: 6961 6c6c 7920 6770 742d 3429 2e0a 332e  ially gpt-4)..3.
-00000d80: 204e 6f74 2061 6c6c 206f 6620 7468 6520   Not all of the 
-00000d90: 6176 6169 6c61 626c 6520 6d6f 6465 6c73  available models
-00000da0: 2077 6572 6520 7465 7374 6564 2c20 736f   were tested, so
-00000db0: 6d65 206d 6179 206e 6f74 2077 6f72 6b20  me may not work 
-00000dc0: 7769 7468 2073 6369 6b69 742d 6c6c 6d20  with scikit-llm 
-00000dd0: 6174 2061 6c6c 2e0a 0a23 2323 205a 6572  at all...### Zer
-00000de0: 6f2d 5368 6f74 2054 6578 7420 436c 6173  o-Shot Text Clas
-00000df0: 7369 6669 6361 7469 6f6e 0a0a 4f6e 6520  sification..One 
-00000e00: 6f66 2074 6865 2070 6f77 6572 6675 6c20  of the powerful 
-00000e10: 4368 6174 4750 5420 6665 6174 7572 6573  ChatGPT features
-00000e20: 2069 7320 7468 6520 6162 696c 6974 7920   is the ability 
-00000e30: 746f 2070 6572 666f 726d 2074 6578 7420  to perform text 
-00000e40: 636c 6173 7369 6669 6361 7469 6f6e 2077  classification w
-00000e50: 6974 686f 7574 2062 6569 6e67 2072 652d  ithout being re-
-00000e60: 7472 6169 6e65 642e 2046 6f72 2074 6861  trained. For tha
-00000e70: 742c 2074 6865 206f 6e6c 7920 7265 7175  t, the only requ
-00000e80: 6972 656d 656e 7420 6973 2074 6861 7420  irement is that 
-00000e90: 7468 6520 6c61 6265 6c73 206d 7573 7420  the labels must 
-00000ea0: 6265 2064 6573 6372 6970 7469 7665 2e0a  be descriptive..
-00000eb0: 0a57 6520 7072 6f76 6964 6520 6120 636c  .We provide a cl
-00000ec0: 6173 7320 605a 6572 6f53 686f 7447 5054  ass `ZeroShotGPT
-00000ed0: 436c 6173 7369 6669 6572 6020 7468 6174  Classifier` that
-00000ee0: 2061 6c6c 6f77 7320 746f 2063 7265 6174   allows to creat
-00000ef0: 6520 7375 6368 2061 206d 6f64 656c 2061  e such a model a
-00000f00: 7320 6120 7265 6775 6c61 7220 7363 696b  s a regular scik
-00000f10: 6974 2d6c 6561 726e 2063 6c61 7373 6966  it-learn classif
-00000f20: 6965 722e 0a0a 4578 616d 706c 6520 313a  ier...Example 1:
-00000f30: 2054 7261 696e 696e 6720 6173 2061 2072   Training as a r
-00000f40: 6567 756c 6172 2063 6c61 7373 6966 6965  egular classifie
-00000f50: 720a 0a60 6060 7079 7468 6f6e 0a66 726f  r..```python.fro
-00000f60: 6d20 736b 6c6c 6d20 696d 706f 7274 205a  m skllm import Z
-00000f70: 6572 6f53 686f 7447 5054 436c 6173 7369  eroShotGPTClassi
-00000f80: 6669 6572 0a66 726f 6d20 736b 6c6c 6d2e  fier.from skllm.
-00000f90: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
-00000fa0: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
-00000fb0: 6f6e 5f64 6174 6173 6574 0a0a 2320 6465  on_dataset..# de
-00000fc0: 6d6f 2073 656e 7469 6d65 6e74 2061 6e61  mo sentiment ana
-00000fd0: 6c79 7369 7320 6461 7461 7365 740a 2320  lysis dataset.# 
-00000fe0: 6c61 6265 6c73 3a20 706f 7369 7469 7665  labels: positive
-00000ff0: 2c20 6e65 6761 7469 7665 2c20 6e65 7574  , negative, neut
-00001000: 7261 6c0a 582c 2079 203d 2067 6574 5f63  ral.X, y = get_c
-00001010: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
-00001020: 7461 7365 7428 290a 0a63 6c66 203d 205a  taset()..clf = Z
-00001030: 6572 6f53 686f 7447 5054 436c 6173 7369  eroShotGPTClassi
-00001040: 6669 6572 286f 7065 6e61 695f 6d6f 6465  fier(openai_mode
-00001050: 6c3d 2267 7074 2d33 2e35 2d74 7572 626f  l="gpt-3.5-turbo
-00001060: 2229 0a63 6c66 2e66 6974 2858 2c20 7929  ").clf.fit(X, y)
-00001070: 0a6c 6162 656c 7320 3d20 636c 662e 7072  .labels = clf.pr
-00001080: 6564 6963 7428 5829 0a60 6060 0a0a 5363  edict(X).```..Sc
-00001090: 696b 6974 2d4c 4c4d 2077 696c 6c20 6175  ikit-LLM will au
-000010a0: 746f 6d61 7469 6361 6c6c 7920 7175 6572  tomatically quer
-000010b0: 7920 7468 6520 4f70 656e 4149 2041 5049  y the OpenAI API
-000010c0: 2061 6e64 2074 7261 6e73 666f 726d 2074   and transform t
-000010d0: 6865 2072 6573 706f 6e73 6520 696e 746f  he response into
-000010e0: 2061 2072 6567 756c 6172 206c 6973 7420   a regular list 
-000010f0: 6f66 206c 6162 656c 732e 0a0a 4164 6469  of labels...Addi
-00001100: 7469 6f6e 616c 6c79 2c20 5363 696b 6974  tionally, Scikit
-00001110: 2d4c 4c4d 2077 696c 6c20 656e 7375 7265  -LLM will ensure
-00001120: 2074 6861 7420 7468 6520 6f62 7461 696e   that the obtain
-00001130: 6564 2072 6573 706f 6e73 6520 636f 6e74  ed response cont
-00001140: 6169 6e73 2061 2076 616c 6964 206c 6162  ains a valid lab
-00001150: 656c 2e20 4966 2074 6869 7320 6973 206e  el. If this is n
-00001160: 6f74 2074 6865 2063 6173 652c 2061 206c  ot the case, a l
-00001170: 6162 656c 2077 696c 6c20 6265 2073 656c  abel will be sel
-00001180: 6563 7465 6420 7261 6e64 6f6d 6c79 2028  ected randomly (
-00001190: 6c61 6265 6c20 7072 6f62 6162 696c 6974  label probabilit
-000011a0: 6965 7320 6172 6520 7072 6f70 6f72 7469  ies are proporti
-000011b0: 6f6e 616c 2074 6f20 6c61 6265 6c20 6f63  onal to label oc
-000011c0: 6375 7272 656e 6365 7320 696e 2074 6865  currences in the
-000011d0: 2074 7261 696e 696e 6720 7365 7429 2e0a   training set)..
-000011e0: 0a45 7861 6d70 6c65 2032 3a20 5472 6169  .Example 2: Trai
-000011f0: 6e69 6e67 2077 6974 686f 7574 206c 6162  ning without lab
-00001200: 656c 6564 2064 6174 610a 0a53 696e 6365  eled data..Since
-00001210: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001220: 7461 2069 7320 6e6f 7420 7374 7269 6374  ta is not strict
-00001230: 6c79 2072 6571 7569 7265 642c 2069 7420  ly required, it 
-00001240: 6361 6e20 6265 2066 756c 6c79 206f 6d6d  can be fully omm
-00001250: 6974 6564 2e20 5468 6520 6f6e 6c79 2074  ited. The only t
-00001260: 6869 6e67 2074 6861 7420 6861 7320 746f  hing that has to
-00001270: 2062 6520 7072 6f76 6964 6564 2069 7320   be provided is 
-00001280: 7468 6520 6c69 7374 206f 6620 6361 6e64  the list of cand
-00001290: 6964 6174 6520 6c61 6265 6c73 2e0a 0a60  idate labels...`
-000012a0: 6060 7079 7468 6f6e 0a66 726f 6d20 736b  ``python.from sk
-000012b0: 6c6c 6d20 696d 706f 7274 205a 6572 6f53  llm import ZeroS
-000012c0: 686f 7447 5054 436c 6173 7369 6669 6572  hotGPTClassifier
-000012d0: 0a66 726f 6d20 736b 6c6c 6d2e 6461 7461  .from skllm.data
-000012e0: 7365 7473 2069 6d70 6f72 7420 6765 745f  sets import get_
-000012f0: 636c 6173 7369 6669 6361 7469 6f6e 5f64  classification_d
-00001300: 6174 6173 6574 0a0a 582c 205f 203d 2067  ataset..X, _ = g
-00001310: 6574 5f63 6c61 7373 6966 6963 6174 696f  et_classificatio
-00001320: 6e5f 6461 7461 7365 7428 290a 0a63 6c66  n_dataset()..clf
-00001330: 203d 205a 6572 6f53 686f 7447 5054 436c   = ZeroShotGPTCl
-00001340: 6173 7369 6669 6572 2829 0a63 6c66 2e66  assifier().clf.f
-00001350: 6974 284e 6f6e 652c 205b 2270 6f73 6974  it(None, ["posit
-00001360: 6976 6522 2c20 226e 6567 6174 6976 6522  ive", "negative"
-00001370: 2c20 226e 6575 7472 616c 225d 290a 6c61  , "neutral"]).la
-00001380: 6265 6c73 203d 2063 6c66 2e70 7265 6469  bels = clf.predi
-00001390: 6374 2858 290a 6060 600a 0a2a 2a4e 6f74  ct(X).```..**Not
-000013a0: 653a 2a2a 2075 6e6c 696b 6520 696e 2061  e:** unlike in a
-000013b0: 2074 7970 6963 616c 2073 7570 6572 7669   typical supervi
-000013c0: 7365 6420 7365 7474 696e 672c 2074 6865  sed setting, the
-000013d0: 2070 6572 666f 726d 616e 6365 206f 6620   performance of 
-000013e0: 6120 7a65 726f 2d73 686f 7420 636c 6173  a zero-shot clas
-000013f0: 7369 6669 6572 2067 7265 6174 6c79 2064  sifier greatly d
-00001400: 6570 656e 6473 206f 6e20 686f 7720 7468  epends on how th
-00001410: 6520 6c61 6265 6c20 6974 7365 6c66 2069  e label itself i
-00001420: 7320 7374 7275 6374 7572 6564 2e20 4974  s structured. It
-00001430: 2068 6173 2074 6f20 6265 2065 7870 7265   has to be expre
-00001440: 7373 6564 2069 6e20 6e61 7475 7261 6c20  ssed in natural 
-00001450: 6c61 6e67 7561 6765 2c20 6265 2064 6573  language, be des
-00001460: 6372 6970 7469 7665 2061 6e64 2073 656c  criptive and sel
-00001470: 662d 6578 706c 616e 6174 6f72 792e 2046  f-explanatory. F
-00001480: 6f72 2065 7861 6d70 6c65 2c20 696e 2074  or example, in t
-00001490: 6865 2070 7265 7669 6f75 7320 7365 6d61  he previous sema
-000014a0: 6e74 6963 2063 6c61 7373 6966 6963 6174  ntic classificat
-000014b0: 696f 6e20 7461 736b 2c20 6974 2063 6f75  ion task, it cou
-000014c0: 6c64 2062 6520 6265 6e65 6669 6369 616c  ld be beneficial
-000014d0: 2074 6f20 7472 616e 7366 6f72 6d20 6120   to transform a 
-000014e0: 6c61 6265 6c20 6672 6f6d 2060 223c 7365  label from `"<se
-000014f0: 6d61 6e74 6963 733e 2260 2074 6f20 6022  mantics>"` to `"
-00001500: 7468 6520 7365 6d61 6e74 6963 7320 6f66  the semantics of
-00001510: 2074 6865 2070 726f 7669 6465 6420 7465   the provided te
-00001520: 7874 2069 7320 3c73 656d 616e 7469 6373  xt is <semantics
-00001530: 3e22 602e 0a0a 2323 2320 4d75 6c74 692d  >"`...### Multi-
-00001540: 4c61 6265 6c20 5a65 726f 2d53 686f 7420  Label Zero-Shot 
-00001550: 5465 7874 2043 6c61 7373 6966 6963 6174  Text Classificat
-00001560: 696f 6e0a 0a57 6974 6820 6120 636c 6173  ion..With a clas
-00001570: 7320 604d 756c 7469 4c61 6265 6c5a 6572  s `MultiLabelZer
-00001580: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001590: 6572 6020 6974 2069 7320 706f 7373 6962  er` it is possib
-000015a0: 6c65 2074 6f20 7065 7266 6f72 6d20 7468  le to perform th
-000015b0: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
-000015c0: 2069 6e20 6d75 6c74 692d 6c61 6265 6c20   in multi-label 
-000015d0: 7365 7474 696e 672c 2077 6869 6368 206d  setting, which m
-000015e0: 6561 6e73 2074 6861 7420 6561 6368 2073  eans that each s
-000015f0: 616d 706c 6520 6d69 6768 7420 6265 2061  ample might be a
-00001600: 7373 6967 6e65 6420 746f 206f 6e65 206f  ssigned to one o
-00001610: 7220 7365 7665 7261 6c20 6469 7374 696e  r several distin
-00001620: 6374 2063 6c61 7373 6573 2e0a 0a45 7861  ct classes...Exa
-00001630: 6d70 6c65 3a0a 0a60 6060 7079 7468 6f6e  mple:..```python
-00001640: 0a66 726f 6d20 736b 6c6c 6d20 696d 706f  .from skllm impo
-00001650: 7274 204d 756c 7469 4c61 6265 6c5a 6572  rt MultiLabelZer
-00001660: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001670: 6572 0a66 726f 6d20 736b 6c6c 6d2e 6461  er.from skllm.da
-00001680: 7461 7365 7473 2069 6d70 6f72 7420 6765  tasets import ge
-00001690: 745f 6d75 6c74 696c 6162 656c 5f63 6c61  t_multilabel_cla
-000016a0: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
-000016b0: 7365 740a 0a58 2c20 7920 3d20 6765 745f  set..X, y = get_
-000016c0: 6d75 6c74 696c 6162 656c 5f63 6c61 7373  multilabel_class
-000016d0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
-000016e0: 7428 290a 0a63 6c66 203d 204d 756c 7469  t()..clf = Multi
-000016f0: 4c61 6265 6c5a 6572 6f53 686f 7447 5054  LabelZeroShotGPT
-00001700: 436c 6173 7369 6669 6572 286d 6178 5f6c  Classifier(max_l
-00001710: 6162 656c 733d 3329 0a63 6c66 2e66 6974  abels=3).clf.fit
-00001720: 2858 2c20 7929 0a6c 6162 656c 7320 3d20  (X, y).labels = 
-00001730: 636c 662e 7072 6564 6963 7428 5829 0a60  clf.predict(X).`
-00001740: 6060 0a0a 5369 6d69 6c61 726c 7920 746f  ``..Similarly to
-00001750: 2074 6865 2060 5a65 726f 5368 6f74 4750   the `ZeroShotGP
-00001760: 5443 6c61 7373 6966 6965 7260 2069 7420  TClassifier` it 
-00001770: 6973 2073 7566 6669 6369 656e 7420 6966  is sufficient if
-00001780: 206f 6e6c 7920 6361 6e64 6964 6174 6520   only candidate 
-00001790: 6c61 6265 6c73 2061 7265 2070 726f 7669  labels are provi
-000017a0: 6465 642e 2048 6f77 6576 6572 2c20 7468  ded. However, th
-000017b0: 6973 2074 696d 6520 7468 6520 636c 6173  is time the clas
-000017c0: 7369 6669 6572 2065 7870 6563 7473 2060  sifier expects `
-000017d0: 7960 206f 6620 6120 7479 7065 2060 4c69  y` of a type `Li
-000017e0: 7374 5b4c 6973 745b 7374 725d 5d60 2e0a  st[List[str]]`..
-000017f0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00001800: 736b 6c6c 6d20 696d 706f 7274 204d 756c  skllm import Mul
-00001810: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
-00001820: 5054 436c 6173 7369 6669 6572 0a66 726f  PTClassifier.fro
-00001830: 6d20 736b 6c6c 6d2e 6461 7461 7365 7473  m skllm.datasets
-00001840: 2069 6d70 6f72 7420 6765 745f 6d75 6c74   import get_mult
-00001850: 696c 6162 656c 5f63 6c61 7373 6966 6963  ilabel_classific
-00001860: 6174 696f 6e5f 6461 7461 7365 740a 0a58  ation_dataset..X
-00001870: 2c20 5f20 3d20 6765 745f 6d75 6c74 696c  , _ = get_multil
-00001880: 6162 656c 5f63 6c61 7373 6966 6963 6174  abel_classificat
-00001890: 696f 6e5f 6461 7461 7365 7428 290a 6361  ion_dataset().ca
-000018a0: 6e64 6964 6174 655f 6c61 6265 6c73 203d  ndidate_labels =
-000018b0: 205b 0a20 2020 2022 5175 616c 6974 7922   [.    "Quality"
-000018c0: 2c0a 2020 2020 2250 7269 6365 222c 0a20  ,.    "Price",. 
-000018d0: 2020 2022 4465 6c69 7665 7279 222c 0a20     "Delivery",. 
-000018e0: 2020 2022 5365 7276 6963 6522 2c0a 2020     "Service",.  
-000018f0: 2020 2250 726f 6475 6374 2056 6172 6965    "Product Varie
-00001900: 7479 222c 0a20 2020 2022 4375 7374 6f6d  ty",.    "Custom
-00001910: 6572 2053 7570 706f 7274 222c 0a20 2020  er Support",.   
-00001920: 2022 5061 636b 6167 696e 6722 2c0a 2020   "Packaging",.  
-00001930: 2020 2255 7365 7220 4578 7065 7269 656e    "User Experien
-00001940: 6365 222c 0a20 2020 2022 5265 7475 726e  ce",.    "Return
-00001950: 2050 6f6c 6963 7922 2c0a 2020 2020 2250   Policy",.    "P
-00001960: 726f 6475 6374 2049 6e66 6f72 6d61 7469  roduct Informati
-00001970: 6f6e 222c 0a5d 0a63 6c66 203d 204d 756c  on",.].clf = Mul
-00001980: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
-00001990: 5054 436c 6173 7369 6669 6572 286d 6178  PTClassifier(max
-000019a0: 5f6c 6162 656c 733d 3329 0a63 6c66 2e66  _labels=3).clf.f
-000019b0: 6974 284e 6f6e 652c 205b 6361 6e64 6964  it(None, [candid
-000019c0: 6174 655f 6c61 6265 6c73 5d29 0a6c 6162  ate_labels]).lab
-000019d0: 656c 7320 3d20 636c 662e 7072 6564 6963  els = clf.predic
-000019e0: 7428 5829 0a60 6060 0a0a 2323 2320 4665  t(X).```..### Fe
-000019f0: 772d 5368 6f74 2054 6578 7420 436c 6173  w-Shot Text Clas
-00001a00: 7369 6669 6361 7469 6f6e 0a0a 5769 7468  sification..With
-00001a10: 2060 4665 7753 686f 7447 5054 436c 6173   `FewShotGPTClas
-00001a20: 7369 6669 6572 6020 6974 2069 7320 706f  sifier` it is po
-00001a30: 7373 6962 6c65 2074 6f20 7065 7266 6f72  ssible to perfor
-00001a40: 6d20 6120 6665 772d 7368 6f74 2063 6c61  m a few-shot cla
-00001a50: 7373 6966 6963 6174 696f 6e2c 2077 6869  ssification, whi
-00001a60: 6368 206d 6561 6e73 2074 6861 7420 7468  ch means that th
-00001a70: 6520 7472 6169 6e69 6e67 2073 616d 706c  e training sampl
-00001a80: 6573 2077 696c 6c20 6265 2061 6464 6564  es will be added
-00001a90: 2074 6f20 7072 6f6d 7074 2061 6e64 2070   to prompt and p
-00001aa0: 6173 7365 6420 746f 2074 6865 206d 6f64  assed to the mod
-00001ab0: 656c 2e0a 0a60 6060 7079 7468 6f6e 0a66  el...```python.f
-00001ac0: 726f 6d20 736b 6c6c 6d20 696d 706f 7274  rom skllm import
-00001ad0: 2046 6577 5368 6f74 4750 5443 6c61 7373   FewShotGPTClass
-00001ae0: 6966 6965 720a 6672 6f6d 2073 6b6c 6c6d  ifier.from skllm
-00001af0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
-00001b00: 2067 6574 5f63 6c61 7373 6966 6963 6174   get_classificat
-00001b10: 696f 6e5f 6461 7461 7365 740a 0a58 2c20  ion_dataset..X, 
-00001b20: 7920 3d20 6765 745f 636c 6173 7369 6669  y = get_classifi
-00001b30: 6361 7469 6f6e 5f64 6174 6173 6574 2829  cation_dataset()
-00001b40: 0a0a 636c 6620 3d20 4665 7753 686f 7447  ..clf = FewShotG
-00001b50: 5054 436c 6173 7369 6669 6572 286f 7065  PTClassifier(ope
-00001b60: 6e61 695f 6d6f 6465 6c3d 2267 7074 2d33  nai_model="gpt-3
-00001b70: 2e35 2d74 7572 626f 2229 0a63 6c66 2e66  .5-turbo").clf.f
-00001b80: 6974 2858 2c20 7929 0a6c 6162 656c 7320  it(X, y).labels 
-00001b90: 3d20 636c 662e 7072 6564 6963 7428 5829  = clf.predict(X)
-00001ba0: 0a60 6060 0a0a 5768 696c 6520 7468 6520  .```..While the 
-00001bb0: 6170 6920 7265 6d61 696e 7320 7468 6520  api remains the 
-00001bc0: 7361 6d65 2061 7320 666f 7220 7468 6520  same as for the 
-00001bd0: 7a65 726f 2073 686f 7420 636c 6173 7369  zero shot classi
-00001be0: 6669 6572 2c20 7468 6572 6520 6172 6520  fier, there are 
-00001bf0: 6120 6665 7720 7468 696e 6773 2074 6f20  a few things to 
-00001c00: 7461 6b65 2069 6e74 6f20 6163 636f 756e  take into accoun
-00001c10: 743a 0a0a 2d20 7468 6520 2274 7261 696e  t:..- the "train
-00001c20: 696e 6722 2072 6571 7569 7265 7320 736f  ing" requires so
-00001c30: 6d65 206c 6162 656c 6c65 6420 7472 6169  me labelled trai
-00001c40: 6e69 6e67 2064 6174 613b 0a2d 2074 6865  ning data;.- the
-00001c50: 2074 7261 696e 696e 6720 7365 7420 7368   training set sh
-00001c60: 6f75 6c64 2062 6520 736d 616c 6c20 656e  ould be small en
-00001c70: 6f75 6768 2074 6f20 6669 7420 696e 746f  ough to fit into
-00001c80: 2061 2073 696e 676c 6520 7072 6f6d 7074   a single prompt
-00001c90: 2028 7765 2072 6563 6f6d 6d65 6e64 2075   (we recommend u
-00001ca0: 7020 746f 2031 3020 7361 6d70 6c65 7320  p to 10 samples 
-00001cb0: 7065 7220 6c61 6265 6c29 3b0a 2d20 6265  per label);.- be
-00001cc0: 6361 7573 6520 6f66 2074 6865 2073 6967  cause of the sig
-00001cd0: 6e69 6669 6361 6e74 6c79 206c 6172 6765  nificantly large
-00001ce0: 7220 7072 6f6d 7074 2c20 7468 6520 696e  r prompt, the in
-00001cf0: 6665 7265 6e63 6520 7461 6b65 7320 6c6f  ference takes lo
-00001d00: 6e67 6572 2061 6e64 2063 6f6e 7375 6d65  nger and consume
-00001d10: 7320 6869 6768 6572 2061 6d6f 756e 7420  s higher amount 
-00001d20: 6f66 2074 6f6b 656e 732e 0a0a 4e6f 7465  of tokens...Note
-00001d30: 3a20 6173 2074 6865 206d 6f64 656c 2069  : as the model i
-00001d40: 7320 6e6f 7420 6265 696e 6720 7265 2d74  s not being re-t
-00001d50: 7261 696e 6564 2c20 6275 7420 7573 6573  rained, but uses
-00001d60: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001d70: 7461 2064 7572 696e 6720 696e 6665 7265  ta during infere
-00001d80: 6e63 652c 206f 6e65 2063 6f75 6c64 2073  nce, one could s
-00001d90: 6179 2074 6861 7420 7468 6973 2069 7320  ay that this is 
-00001da0: 7374 696c 6c20 6120 2864 6966 6665 7265  still a (differe
-00001db0: 6e74 2920 7a65 726f 2d73 686f 7420 6170  nt) zero-shot ap
-00001dc0: 7072 6f61 6368 2e0a 0a23 2323 2044 796e  proach...### Dyn
-00001dd0: 616d 6963 2046 6577 2d53 686f 7420 5465  amic Few-Shot Te
-00001de0: 7874 2043 6c61 7373 6966 6963 6174 696f  xt Classificatio
-00001df0: 6e0a 0a60 4479 6e61 6d69 6346 6577 5368  n..`DynamicFewSh
-00001e00: 6f74 4750 5443 6c61 7373 6966 6965 7260  otGPTClassifier`
-00001e10: 2064 796e 616d 6963 616c 6c79 2073 656c   dynamically sel
-00001e20: 6563 7473 204e 2073 616d 706c 6573 2070  ects N samples p
-00001e30: 6572 2063 6c61 7373 2074 6f20 696e 636c  er class to incl
-00001e40: 7564 6520 696e 2074 6865 2070 726f 6d70  ude in the promp
-00001e50: 742e 2054 6869 7320 616c 6c6f 7773 2074  t. This allows t
-00001e60: 6865 2066 6577 2d73 686f 7420 636c 6173  he few-shot clas
-00001e70: 7369 6669 6572 2074 6f20 7363 616c 6520  sifier to scale 
-00001e80: 746f 2064 6174 6173 6574 7320 7468 6174  to datasets that
-00001e90: 2061 7265 2074 6f6f 206c 6172 6765 2066   are too large f
-00001ea0: 6f72 2074 6865 2073 7461 6e64 6172 6420  or the standard 
-00001eb0: 636f 6e74 6578 7420 7769 6e64 6f77 206f  context window o
-00001ec0: 6620 4c4c 4d73 2e0a 0a2a 486f 7720 646f  f LLMs...*How do
-00001ed0: 6573 2069 7420 776f 726b 3f2a 0a0a 4475  es it work?*..Du
-00001ee0: 7269 6e67 2066 6974 7469 6e67 2c20 7468  ring fitting, th
-00001ef0: 6520 7768 6f6c 6520 6461 7461 7365 7420  e whole dataset 
-00001f00: 6973 2070 6172 7469 7469 6f6e 6564 2062  is partitioned b
-00001f10: 7920 636c 6173 732c 2076 6563 746f 7269  y class, vectori
-00001f20: 7a65 642c 2061 6e64 2073 746f 7265 642e  zed, and stored.
-00001f30: 0a0a 4475 7269 6e67 2069 6e66 6572 656e  ..During inferen
-00001f40: 6365 2c20 7468 6520 5b61 6e6e 6f79 5d28  ce, the [annoy](
-00001f50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001f60: 6f6d 2f73 706f 7469 6679 2f61 6e6e 6f79  om/spotify/annoy
-00001f70: 2920 6c69 6272 6172 7920 6973 2075 7365  ) library is use
-00001f80: 6420 666f 7220 6661 7374 206e 6569 6768  d for fast neigh
-00001f90: 626f 7220 6c6f 6f6b 7570 2c20 7768 6963  bor lookup, whic
-00001fa0: 6820 616c 6c6f 7773 2069 6e63 6c75 6469  h allows includi
-00001fb0: 6e67 206f 6e6c 7920 7468 6520 6d6f 7374  ng only the most
-00001fc0: 2073 696d 696c 6172 2065 7861 6d70 6c65   similar example
-00001fd0: 7320 696e 2074 6865 2070 726f 6d70 742e  s in the prompt.
-00001fe0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001ff0: 2073 6b6c 6c6d 2069 6d70 6f72 7420 4479   skllm import Dy
-00002000: 6e61 6d69 6346 6577 5368 6f74 4750 5443  namicFewShotGPTC
-00002010: 6c61 7373 6966 6965 720a 6672 6f6d 2073  lassifier.from s
-00002020: 6b6c 6c6d 2e64 6174 6173 6574 7320 696d  kllm.datasets im
-00002030: 706f 7274 2067 6574 5f63 6c61 7373 6966  port get_classif
-00002040: 6963 6174 696f 6e5f 6461 7461 7365 740a  ication_dataset.
-00002050: 0a58 2c20 7920 3d20 6765 745f 636c 6173  .X, y = get_clas
-00002060: 7369 6669 6361 7469 6f6e 5f64 6174 6173  sification_datas
-00002070: 6574 2829 0a0a 636c 6620 3d20 4479 6e61  et()..clf = Dyna
-00002080: 6d69 6346 6577 5368 6f74 4750 5443 6c61  micFewShotGPTCla
-00002090: 7373 6966 6965 7228 6e5f 6578 616d 706c  ssifier(n_exampl
-000020a0: 6573 3d33 290a 636c 662e 6669 7428 582c  es=3).clf.fit(X,
-000020b0: 2079 290a 6c61 6265 6c73 203d 2063 6c66   y).labels = clf
-000020c0: 2e70 7265 6469 6374 2858 290a 6060 600a  .predict(X).```.
-000020d0: 0a23 2323 2054 6578 7420 5665 6374 6f72  .### Text Vector
-000020e0: 697a 6174 696f 6e0a 0a41 7320 616e 2061  ization..As an a
-000020f0: 6c74 6572 6e61 7469 7665 2074 6f20 7573  lternative to us
-00002100: 696e 6720 4750 5420 6173 2061 2063 6c61  ing GPT as a cla
-00002110: 7373 6966 6965 722c 2069 7420 6361 6e20  ssifier, it can 
-00002120: 6265 2075 7365 6420 736f 6c65 6c79 2066  be used solely f
-00002130: 6f72 2064 6174 6120 7072 6570 726f 6365  or data preproce
-00002140: 7373 696e 672e 2060 4750 5456 6563 746f  ssing. `GPTVecto
-00002150: 7269 7a65 7260 2061 6c6c 6f77 7320 746f  rizer` allows to
-00002160: 2065 6d62 6564 2061 2063 6875 6e6b 206f   embed a chunk o
-00002170: 6620 7465 7874 206f 6620 6172 6269 7472  f text of arbitr
-00002180: 6172 7920 6c65 6e67 7468 2074 6f20 6120  ary length to a 
-00002190: 6669 7865 642d 6469 6d65 6e73 696f 6e61  fixed-dimensiona
-000021a0: 6c20 7665 6374 6f72 2c20 7468 6174 2063  l vector, that c
-000021b0: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
-000021c0: 7669 7274 7561 6c6c 7920 616e 7920 636c  virtually any cl
-000021d0: 6173 7369 6669 6361 7469 6f6e 206f 7220  assification or 
-000021e0: 7265 6772 6573 7369 6f6e 206d 6f64 656c  regression model
-000021f0: 2e0a 0a45 7861 6d70 6c65 2031 3a20 456d  ...Example 1: Em
-00002200: 6265 6464 696e 6720 7468 6520 7465 7874  bedding the text
-00002210: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00002220: 2073 6b6c 6c6d 2e70 7265 7072 6f63 6573   skllm.preproces
-00002230: 7369 6e67 2069 6d70 6f72 7420 4750 5456  sing import GPTV
-00002240: 6563 746f 7269 7a65 720a 0a6d 6f64 656c  ectorizer..model
-00002250: 203d 2047 5054 5665 6374 6f72 697a 6572   = GPTVectorizer
-00002260: 2829 0a76 6563 746f 7273 203d 206d 6f64  ().vectors = mod
-00002270: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
-00002280: 2858 290a 6060 600a 0a45 7861 6d70 6c65  (X).```..Example
-00002290: 2032 3a20 436f 6d62 696e 696e 6720 7468   2: Combining th
-000022a0: 6520 5665 6374 6f72 697a 6572 2077 6974  e Vectorizer wit
-000022b0: 6820 7468 6520 5847 426f 6f73 7420 436c  h the XGBoost Cl
-000022c0: 6173 7369 6669 6572 2069 6e20 6120 536b  assifier in a Sk
-000022d0: 6c65 6172 6e20 5069 7065 6c69 6e65 0a0a  learn Pipeline..
-000022e0: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
-000022f0: 6b6c 6561 726e 2e70 6970 656c 696e 6520  klearn.pipeline 
-00002300: 696d 706f 7274 2050 6970 656c 696e 650a  import Pipeline.
-00002310: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
-00002320: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
-00002330: 7420 4c61 6265 6c45 6e63 6f64 6572 0a66  t LabelEncoder.f
-00002340: 726f 6d20 7867 626f 6f73 7420 696d 706f  rom xgboost impo
-00002350: 7274 2058 4742 436c 6173 7369 6669 6572  rt XGBClassifier
-00002360: 0a0a 6c65 203d 204c 6162 656c 456e 636f  ..le = LabelEnco
-00002370: 6465 7228 290a 795f 7472 6169 6e5f 656e  der().y_train_en
-00002380: 636f 6465 6420 3d20 6c65 2e66 6974 5f74  coded = le.fit_t
-00002390: 7261 6e73 666f 726d 2879 5f74 7261 696e  ransform(y_train
-000023a0: 290a 795f 7465 7374 5f65 6e63 6f64 6564  ).y_test_encoded
-000023b0: 203d 206c 652e 7472 616e 7366 6f72 6d28   = le.transform(
-000023c0: 795f 7465 7374 290a 0a73 7465 7073 203d  y_test)..steps =
-000023d0: 205b 2822 4750 5422 2c20 4750 5456 6563   [("GPT", GPTVec
-000023e0: 746f 7269 7a65 7228 2929 2c20 2822 436c  torizer()), ("Cl
-000023f0: 6622 2c20 5847 4243 6c61 7373 6966 6965  f", XGBClassifie
-00002400: 7228 2929 5d0a 636c 6620 3d20 5069 7065  r())].clf = Pipe
-00002410: 6c69 6e65 2873 7465 7073 290a 636c 662e  line(steps).clf.
-00002420: 6669 7428 585f 7472 6169 6e2c 2079 5f74  fit(X_train, y_t
-00002430: 7261 696e 5f65 6e63 6f64 6564 290a 7968  rain_encoded).yh
-00002440: 203d 2063 6c66 2e70 7265 6469 6374 2858   = clf.predict(X
-00002450: 5f74 6573 7429 0a60 6060 0a0a 2323 2320  _test).```..### 
-00002460: 5465 7874 2053 756d 6d61 7269 7a61 7469  Text Summarizati
-00002470: 6f6e 0a0a 4750 5420 6578 6365 6c73 2061  on..GPT excels a
-00002480: 7420 7065 7266 6f72 6d69 6e67 2073 756d  t performing sum
-00002490: 6d61 7269 7a61 7469 6f6e 2074 6173 6b73  marization tasks
-000024a0: 2e20 5468 6572 6566 6f72 652c 2077 6520  . Therefore, we 
-000024b0: 7072 6f76 6964 6520 6047 5054 5375 6d6d  provide `GPTSumm
-000024c0: 6172 697a 6572 6020 7468 6174 2063 616e  arizer` that can
-000024d0: 2062 6520 7573 6564 2062 6f74 6820 6173   be used both as
-000024e0: 2073 7461 6e64 2d61 6c6f 6e65 2065 7374   stand-alone est
-000024f0: 696d 6174 6f72 2c20 6f72 2061 7320 6120  imator, or as a 
-00002500: 7072 6570 726f 6365 7373 6f72 2028 696e  preprocessor (in
-00002510: 2074 6869 7320 6361 7365 2077 6520 6361   this case we ca
-00002520: 6e20 6d61 6b65 2061 6e20 616e 616c 6f67  n make an analog
-00002530: 7920 7769 7468 2061 2064 696d 656e 7369  y with a dimensi
-00002540: 6f6e 616c 6974 7920 7265 6475 6374 696f  onality reductio
-00002550: 6e20 7072 6570 726f 6365 7373 6f72 292e  n preprocessor).
-00002560: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
-00002570: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
-00002580: 2e70 7265 7072 6f63 6573 7369 6e67 2069  .preprocessing i
-00002590: 6d70 6f72 7420 4750 5453 756d 6d61 7269  mport GPTSummari
-000025a0: 7a65 720a 6672 6f6d 2073 6b6c 6c6d 2e64  zer.from skllm.d
-000025b0: 6174 6173 6574 7320 696d 706f 7274 2067  atasets import g
-000025c0: 6574 5f73 756d 6d61 7269 7a61 7469 6f6e  et_summarization
-000025d0: 5f64 6174 6173 6574 0a0a 5820 3d20 6765  _dataset..X = ge
-000025e0: 745f 7375 6d6d 6172 697a 6174 696f 6e5f  t_summarization_
-000025f0: 6461 7461 7365 7428 290a 7320 3d20 4750  dataset().s = GP
-00002600: 5453 756d 6d61 7269 7a65 7228 6f70 656e  TSummarizer(open
-00002610: 6169 5f6d 6f64 656c 3d22 6770 742d 332e  ai_model="gpt-3.
-00002620: 352d 7475 7262 6f22 2c20 6d61 785f 776f  5-turbo", max_wo
-00002630: 7264 733d 3135 290a 7375 6d6d 6172 6965  rds=15).summarie
-00002640: 7320 3d20 732e 6669 745f 7472 616e 7366  s = s.fit_transf
-00002650: 6f72 6d28 5829 0a60 6060 0a0a 506c 6561  orm(X).```..Plea
-00002660: 7365 2062 6520 6177 6172 6520 7468 6174  se be aware that
-00002670: 2074 6865 2060 6d61 785f 776f 7264 7360   the `max_words`
-00002680: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
-00002690: 7365 7473 2061 2073 6f66 7420 6c69 6d69  sets a soft limi
-000026a0: 742c 2077 6869 6368 2069 7320 6e6f 7420  t, which is not 
-000026b0: 7374 7269 6374 6c79 2065 6e66 6f72 6365  strictly enforce
-000026c0: 6420 6f75 7473 6964 6520 6f66 2074 6865  d outside of the
-000026d0: 2070 726f 6d70 742e 2054 6865 7265 666f   prompt. Therefo
-000026e0: 7265 2c20 696e 2073 6f6d 6520 6361 7365  re, in some case
-000026f0: 732c 2074 6865 2061 6374 7561 6c20 6e75  s, the actual nu
-00002700: 6d62 6572 206f 6620 776f 7264 7320 6d69  mber of words mi
-00002710: 6768 7420 6265 2073 6c69 6768 746c 7920  ght be slightly 
-00002720: 6869 6768 6572 2e0a 0a23 2323 2054 6578  higher...### Tex
-00002730: 7420 5472 616e 736c 6174 696f 6e0a 0a47  t Translation..G
-00002740: 5054 206d 6f64 656c 7320 6861 7665 2064  PT models have d
-00002750: 656d 6f6e 7374 7261 7465 6420 7468 6569  emonstrated thei
-00002760: 7220 6566 6665 6374 6976 656e 6573 7320  r effectiveness 
-00002770: 696e 2074 7261 6e73 6c61 7469 6f6e 2074  in translation t
-00002780: 6173 6b73 2062 7920 6765 6e65 7261 7469  asks by generati
-00002790: 6e67 2061 6363 7572 6174 6520 7472 616e  ng accurate tran
-000027a0: 736c 6174 696f 6e73 2061 6372 6f73 7320  slations across 
-000027b0: 7661 7269 6f75 7320 6c61 6e67 7561 6765  various language
-000027c0: 732e 2054 6875 732c 2077 6520 6164 6465  s. Thus, we adde
-000027d0: 6420 6047 5054 5472 616e 736c 6174 6f72  d `GPTTranslator
-000027e0: 6020 7468 6174 2061 6c6c 6f77 7320 7472  ` that allows tr
-000027f0: 616e 736c 6174 696e 6720 616e 2061 7262  anslating an arb
-00002800: 6974 7261 7479 2074 6578 7420 696e 746f  itraty text into
-00002810: 2061 206c 616e 6775 6167 6520 6f66 2069   a language of i
-00002820: 6e74 6572 6573 742e 0a0a 4578 616d 706c  nterest...Exampl
-00002830: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00002840: 6f6d 2073 6b6c 6c6d 2e70 7265 7072 6f63  om skllm.preproc
-00002850: 6573 7369 6e67 2069 6d70 6f72 7420 4750  essing import GP
-00002860: 5454 7261 6e73 6c61 746f 720a 6672 6f6d  TTranslator.from
-00002870: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
-00002880: 696d 706f 7274 2067 6574 5f74 7261 6e73  import get_trans
-00002890: 6c61 7469 6f6e 5f64 6174 6173 6574 0a0a  lation_dataset..
-000028a0: 5820 3d20 6765 745f 7472 616e 736c 6174  X = get_translat
-000028b0: 696f 6e5f 6461 7461 7365 7428 290a 7420  ion_dataset().t 
-000028c0: 3d20 4750 5454 7261 6e73 6c61 746f 7228  = GPTTranslator(
-000028d0: 6f70 656e 6169 5f6d 6f64 656c 3d22 6770  openai_model="gp
-000028e0: 742d 332e 352d 7475 7262 6f22 2c20 6f75  t-3.5-turbo", ou
-000028f0: 7470 7574 5f6c 616e 6775 6167 653d 2245  tput_language="E
-00002900: 6e67 6c69 7368 2229 0a74 7261 6e73 6c61  nglish").transla
-00002910: 7465 645f 7465 7874 203d 2074 2e66 6974  ted_text = t.fit
-00002920: 5f74 7261 6e73 666f 726d 2858 290a 6060  _transform(X).``
-00002930: 600a 0a23 2320 526f 6164 6d61 7020 f09f  `..## Roadmap ..
-00002940: a7ad 0a0a 2d20 5b78 5d20 5a65 726f 2d53  ....- [x] Zero-S
-00002950: 686f 7420 436c 6173 7369 6669 6361 7469  hot Classificati
-00002960: 6f6e 2077 6974 6820 4f70 656e 4149 2047  on with OpenAI G
-00002970: 5054 2033 2f34 0a20 202d 205b 785d 204d  PT 3/4.  - [x] M
-00002980: 756c 7469 636c 6173 7320 636c 6173 7369  ulticlass classi
-00002990: 6669 6361 7469 6f6e 0a20 202d 205b 785d  fication.  - [x]
-000029a0: 204d 756c 7469 2d6c 6162 656c 2063 6c61   Multi-label cla
-000029b0: 7373 6966 6963 6174 696f 6e0a 2d20 5b20  ssification.- [ 
-000029c0: 5d20 4665 772d 5368 6f74 2063 6c61 7373  ] Few-Shot class
-000029d0: 6966 6965 720a 2020 2d20 5b78 5d20 4d75  ifier.  - [x] Mu
-000029e0: 6c74 6963 6c61 7373 2063 6c61 7373 6966  lticlass classif
-000029f0: 6963 6174 696f 6e0a 2020 2d20 5b20 5d20  ication.  - [ ] 
-00002a00: 4d75 6c74 692d 6c61 6265 6c20 636c 6173  Multi-label clas
-00002a10: 7369 6669 6361 7469 6f6e 0a2d 205b 785d  sification.- [x]
-00002a20: 2047 5054 2056 6563 746f 7269 7a65 720a   GPT Vectorizer.
-00002a30: 2d20 5b78 5d20 4368 6174 4750 5420 6d6f  - [x] ChatGPT mo
-00002a40: 6465 6c73 0a2d 205b 205d 2049 6e73 7472  dels.- [ ] Instr
-00002a50: 7563 7447 5054 206d 6f64 656c 730a 2d20  uctGPT models.- 
-00002a60: 5b20 5d20 496e 7374 7275 6374 4750 5420  [ ] InstructGPT 
-00002a70: 4669 6e65 2d74 756e 696e 6720 286f 7074  Fine-tuning (opt
-00002a80: 696f 6e61 6c29 0a2d 205b 205d 204f 7065  ional).- [ ] Ope
-00002a90: 6e20 736f 7572 6365 206d 6f64 656c 730a  n source models.
-00002aa0: 0a2a 5468 6520 6f72 6465 7220 6f66 2074  .*The order of t
-00002ab0: 6865 2065 6c65 6d65 6e74 7320 696e 2074  he elements in t
-00002ac0: 6865 2072 6f61 646d 6170 2069 7320 6172  he roadmap is ar
-00002ad0: 6269 7472 6172 7920 616e 6420 646f 6573  bitrary and does
-00002ae0: 206e 6f74 2072 6566 6c65 6374 2074 6865   not reflect the
-00002af0: 2070 6c61 6e6e 6564 206f 7264 6572 206f   planned order o
-00002b00: 6620 696d 706c 656d 656e 7461 7469 6f6e  f implementation
-00002b10: 2e2a 0a                                  .*.
+00000420: f09f 92a1 2050 726f 7669 6465 2079 6f75  .... Provide you
+00000430: 7220 6665 6564 6261 636b 206f 7220 7072  r feedback or pr
+00000440: 6f70 6f73 6520 6964 6561 7320 696e 2074  opose ideas in t
+00000450: 6865 205b 6973 7375 6573 5d28 6874 7470  he [issues](http
+00000460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00000470: 7279 6e61 2d6b 6f6e 6472 2f73 6369 6b69  ryna-kondr/sciki
+00000480: 742d 6c6c 6d2f 6973 7375 6573 2920 7365  t-llm/issues) se
+00000490: 6374 696f 6e20 6f72 205b 4469 7363 6f72  ction or [Discor
+000004a0: 645d 2868 7474 7073 3a2f 2f64 6973 636f  d](https://disco
+000004b0: 7264 2e67 672f 5944 4162 7775 574b 3756  rd.gg/YDAbwuWK7V
+000004c0: 290a 2d20 f09f 93b0 2050 6f73 7420 6162  ).- .... Post ab
+000004d0: 6f75 7420 5363 696b 6974 2d4c 4c4d 206f  out Scikit-LLM o
+000004e0: 6e20 4c69 6e6b 6564 496e 206f 7220 6f74  n LinkedIn or ot
+000004f0: 6865 7220 706c 6174 666f 726d 730a 0a23  her platforms..#
+00000500: 2320 4f75 7220 5265 6c61 7465 6420 5072  # Our Related Pr
+00000510: 6f6a 6563 7473 20f0 9f94 970a 0a3c 6120  ojects ......<a 
+00000520: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000530: 7468 7562 2e63 6f6d 2f4f 4b55 4131 2f66  thub.com/OKUA1/f
+00000540: 616c 636f 6e22 3e3c 696d 6720 7372 633d  alcon"><img src=
+00000550: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000560: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000570: 6f6d 2f67 6973 742f 4f4b 5541 312f 3632  om/gist/OKUA1/62
+00000580: 3634 6139 3561 3861 6264 3232 3563 3734  64a95a8abd225c74
+00000590: 3431 3161 3262 3730 3762 3032 3432 2f72  411a2b707b0242/r
+000005a0: 6177 2f33 6365 6462 3533 3533 3863 6230  aw/3cedb53538cb0
+000005b0: 3436 3536 6364 3964 3764 3037 6536 3937  4656cd9d7d07e697
+000005c0: 6537 3236 3839 3663 6539 662f 6661 6c63  e726896ce9f/falc
+000005d0: 6f6e 5f6c 6967 6874 2e73 7667 222f 3e3c  on_light.svg"/><
+000005e0: 2f61 3e20 3c62 723e 0a3c 6120 6872 6566  /a> <br>.<a href
+000005f0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000600: 2e63 6f6d 2f4f 4b55 4131 2f61 6765 6e74  .com/OKUA1/agent
+00000610: 5f64 696e 676f 223e 3c69 6d67 2073 7263  _dingo"><img src
+00000620: 3d22 6874 7470 733a 2f2f 6769 7374 2e67  ="https://gist.g
+00000630: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000640: 2e63 6f6d 2f4f 4b55 4131 2f36 3236 3461  .com/OKUA1/6264a
+00000650: 3935 6138 6162 6432 3235 6337 3434 3131  95a8abd225c74411
+00000660: 6132 6237 3037 6230 3234 322f 7261 772f  a2b707b0242/raw/
+00000670: 3162 3233 3161 6162 3731 3866 6361 6236  1b231aab718fcab6
+00000680: 3234 6661 6133 3364 3963 3130 6430 6565  24faa33d9c10d0ee
+00000690: 6531 3763 6131 3630 2f64 696e 676f 5f6c  e17ca160/dingo_l
+000006a0: 6967 6874 2e73 7667 222f 3e3c 2f61 3e0a  ight.svg"/></a>.
+000006b0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
+000006c0: 6e20 f09f 939a 0a0a 2323 2320 436f 6e66  n ......### Conf
+000006d0: 6967 7572 696e 6720 4f70 656e 4149 2041  iguring OpenAI A
+000006e0: 5049 204b 6579 0a0a 4174 2074 6865 206d  PI Key..At the m
+000006f0: 6f6d 656e 7420 7468 6520 6d61 6a6f 7269  oment the majori
+00000700: 7479 206f 6620 7468 6520 5363 696b 6974  ty of the Scikit
+00000710: 2d4c 4c4d 2065 7374 696d 6174 6f72 7320  -LLM estimators 
+00000720: 6172 6520 6f6e 6c79 2063 6f6d 7061 7469  are only compati
+00000730: 626c 6520 7769 7468 2073 6f6d 6520 6f66  ble with some of
+00000740: 2074 6865 204f 7065 6e41 4920 6d6f 6465   the OpenAI mode
+00000750: 6c73 2e20 4865 6e63 652c 2061 2075 7365  ls. Hence, a use
+00000760: 722d 7072 6f76 6964 6564 204f 7065 6e41  r-provided OpenA
+00000770: 4920 4150 4920 6b65 7920 6973 2072 6571  I API key is req
+00000780: 7569 7265 642e 0a0a 6060 6070 7974 686f  uired...```pytho
+00000790: 6e0a 6672 6f6d 2073 6b6c 6c6d 2e63 6f6e  n.from skllm.con
+000007a0: 6669 6720 696d 706f 7274 2053 4b4c 4c4d  fig import SKLLM
+000007b0: 436f 6e66 6967 0a0a 534b 4c4c 4d43 6f6e  Config..SKLLMCon
+000007c0: 6669 672e 7365 745f 6f70 656e 6169 5f6b  fig.set_openai_k
+000007d0: 6579 2822 3c59 4f55 525f 4b45 593e 2229  ey("<YOUR_KEY>")
+000007e0: 0a53 4b4c 4c4d 436f 6e66 6967 2e73 6574  .SKLLMConfig.set
+000007f0: 5f6f 7065 6e61 695f 6f72 6728 223c 594f  _openai_org("<YO
+00000800: 5552 5f4f 5247 414e 4953 4154 494f 4e3e  UR_ORGANISATION>
+00000810: 2229 0a60 6060 0a0a 2a2a 496d 706f 7274  ").```..**Import
+00000820: 616e 7420 6e6f 7469 6365 3a2a 2a0a 0a2d  ant notice:**..-
+00000830: 2049 6620 796f 7520 6861 7665 2061 2066   If you have a f
+00000840: 7265 6520 7472 6961 6c20 4f70 656e 4149  ree trial OpenAI
+00000850: 2061 6363 6f75 6e74 2c20 7468 6520 5b72   account, the [r
+00000860: 6174 6520 6c69 6d69 7473 5d28 6874 7470  ate limits](http
+00000870: 733a 2f2f 706c 6174 666f 726d 2e6f 7065  s://platform.ope
+00000880: 6e61 692e 636f 6d2f 646f 6373 2f67 7569  nai.com/docs/gui
+00000890: 6465 732f 7261 7465 2d6c 696d 6974 732f  des/rate-limits/
+000008a0: 6f76 6572 7669 6577 2920 6172 6520 6e6f  overview) are no
+000008b0: 7420 7375 6666 6963 6965 6e74 2028 7370  t sufficient (sp
+000008c0: 6563 6966 6963 616c 6c79 2033 2072 6571  ecifically 3 req
+000008d0: 7565 7374 7320 7065 7220 6d69 6e75 7465  uests per minute
+000008e0: 292e 2050 6c65 6173 6520 7377 6974 6368  ). Please switch
+000008f0: 2074 6f20 7468 6520 2270 6179 2061 7320   to the "pay as 
+00000900: 796f 7520 676f 2220 706c 616e 2066 6972  you go" plan fir
+00000910: 7374 2e0a 2d20 5768 656e 2063 616c 6c69  st..- When calli
+00000920: 6e67 2060 534b 4c4c 4d43 6f6e 6669 672e  ng `SKLLMConfig.
+00000930: 7365 745f 6f70 656e 6169 5f6f 7267 602c  set_openai_org`,
+00000940: 2079 6f75 2068 6176 6520 746f 2070 726f   you have to pro
+00000950: 7669 6465 2079 6f75 7220 6f72 6761 6e69  vide your organi
+00000960: 7a61 7469 6f6e 2049 4420 616e 6420 2a2a  zation ID and **
+00000970: 4e4f 542a 2a20 7468 6520 6e61 6d65 2e20  NOT** the name. 
+00000980: 596f 7520 6361 6e20 6669 6e64 2079 6f75  You can find you
+00000990: 7220 4944 205b 6865 7265 5d28 6874 7470  r ID [here](http
+000009a0: 733a 2f2f 706c 6174 666f 726d 2e6f 7065  s://platform.ope
+000009b0: 6e61 692e 636f 6d2f 6163 636f 756e 742f  nai.com/account/
+000009c0: 6f72 672d 7365 7474 696e 6773 292e 0a0a  org-settings)...
+000009d0: 2323 2320 5573 696e 6720 417a 7572 6520  ### Using Azure 
+000009e0: 4f70 656e 4149 0a0a 6060 6070 7974 686f  OpenAI..```pytho
+000009f0: 6e0a 6672 6f6d 2073 6b6c 6c6d 2e63 6f6e  n.from skllm.con
+00000a00: 6669 6720 696d 706f 7274 2053 4b4c 4c4d  fig import SKLLM
+00000a10: 436f 6e66 6967 0a0a 534b 4c4c 4d43 6f6e  Config..SKLLMCon
+00000a20: 6669 672e 7365 745f 6f70 656e 6169 5f6b  fig.set_openai_k
+00000a30: 6579 2822 3c59 4f55 525f 4b45 593e 2229  ey("<YOUR_KEY>")
+00000a40: 2023 7573 6520 617a 7572 6520 6b65 7920   #use azure key 
+00000a50: 696e 7374 6561 640a 534b 4c4c 4d43 6f6e  instead.SKLLMCon
+00000a60: 6669 672e 7365 745f 617a 7572 655f 6170  fig.set_azure_ap
+00000a70: 695f 6261 7365 2822 3c41 5049 5f42 4153  i_base("<API_BAS
+00000a80: 453e 2229 0a0a 2320 7374 6172 7420 7769  E>")..# start wi
+00000a90: 7468 2022 617a 7572 653a 3a22 2070 7265  th "azure::" pre
+00000aa0: 6669 7820 7768 656e 2073 6574 7469 6e67  fix when setting
+00000ab0: 2074 6865 206d 6f64 656c 206e 616d 650a   the model name.
+00000ac0: 6d6f 6465 6c5f 6e61 6d65 203d 2022 617a  model_name = "az
+00000ad0: 7572 653a 3a3c 6d6f 6465 6c5f 6e61 6d65  ure::<model_name
+00000ae0: 3e22 0a23 2065 2e67 2e20 5a65 726f 5368  >".# e.g. ZeroSh
+00000af0: 6f74 4750 5443 6c61 7373 6966 6965 7228  otGPTClassifier(
+00000b00: 6f70 656e 6169 5f6d 6f64 656c 3d22 617a  openai_model="az
+00000b10: 7572 653a 3a67 7074 2d33 2e35 2d74 7572  ure::gpt-3.5-tur
+00000b20: 626f 2229 0a60 6060 0a0a 4e6f 7465 3a20  bo").```..Note: 
+00000b30: 417a 7572 6520 4f70 656e 4149 2069 7320  Azure OpenAI is 
+00000b40: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00000b50: 2074 6865 2070 7265 7072 6f63 6573 736f   the preprocesso
+00000b60: 7273 2061 7420 7468 6520 6d6f 6d65 6e74  rs at the moment
+00000b70: 2e0a 0a23 2323 2055 7369 6e67 2047 5054  ...### Using GPT
+00000b80: 3441 4c4c 0a0a 496e 2061 6464 6974 696f  4ALL..In additio
+00000b90: 6e20 746f 204f 7065 6e41 492c 2073 6f6d  n to OpenAI, som
+00000ba0: 6520 6f66 2074 6865 206d 6f64 656c 7320  e of the models 
+00000bb0: 6361 6e20 7573 6520 5b67 7074 3461 6c6c  can use [gpt4all
+00000bc0: 5d28 6874 7470 733a 2f2f 6770 7434 616c  ](https://gpt4al
+00000bd0: 6c2e 696f 2f69 6e64 6578 2e68 746d 6c29  l.io/index.html)
+00000be0: 2061 7320 6120 6261 636b 656e 642e 0a0a   as a backend...
+00000bf0: 2a2a 5468 6973 2066 6561 7475 7265 2069  **This feature i
+00000c00: 7320 636f 6e73 6964 6572 6564 2068 6967  s considered hig
+00000c10: 6c79 2065 7870 6572 696d 656e 7461 6c21  ly experimental!
+00000c20: 2a2a 0a0a 496e 206f 7264 6572 2074 6f20  **..In order to 
+00000c30: 7573 6520 6770 7434 616c 6c2c 2079 6f75  use gpt4all, you
+00000c40: 206e 6565 6420 746f 2069 6e73 7461 6c6c   need to install
+00000c50: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00000c60: 6e67 2073 7562 6d6f 6475 6c65 3a0a 0a60  ng submodule:..`
+00000c70: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00000c80: 6c6c 2022 7363 696b 6974 2d6c 6c6d 5b67  ll "scikit-llm[g
+00000c90: 7074 3461 6c6c 5d22 0a60 6060 0a0a 496e  pt4all]".```..In
+00000ca0: 206f 7264 6572 2074 6f20 7377 6974 6368   order to switch
+00000cb0: 2066 726f 6d20 4f70 656e 4149 2074 6f20   from OpenAI to 
+00000cc0: 4750 5434 414c 4c20 6d6f 6465 6c2c 2073  GPT4ALL model, s
+00000cd0: 696d 706c 7920 7072 6f76 6964 6520 6120  imply provide a 
+00000ce0: 7374 7269 6e67 206f 6620 7468 6520 666f  string of the fo
+00000cf0: 726d 6174 2060 6770 7434 616c 6c3a 3a3c  rmat `gpt4all::<
+00000d00: 6d6f 6465 6c5f 6e61 6d65 3e60 2061 7320  model_name>` as 
+00000d10: 616e 2061 7267 756d 656e 742e 2057 6869  an argument. Whi
+00000d20: 6c65 2074 6865 206d 6f64 656c 2072 756e  le the model run
+00000d30: 7320 636f 6d70 6c65 7465 6c79 206c 6f63  s completely loc
+00000d40: 616c 6c79 2c20 7468 6520 6573 7469 6d61  ally, the estima
+00000d50: 746f 7220 7374 696c 6c20 7472 6561 7473  tor still treats
+00000d60: 2069 7420 6173 2061 6e20 4f70 656e 4149   it as an OpenAI
+00000d70: 2065 6e64 706f 696e 7420 616e 6420 7769   endpoint and wi
+00000d80: 6c6c 2074 7279 2074 6f20 6368 6563 6b20  ll try to check 
+00000d90: 7468 6174 2074 6865 2041 5049 206b 6579  that the API key
+00000da0: 2069 7320 7072 6573 656e 742e 2059 6f75   is present. You
+00000db0: 2063 616e 2070 726f 7669 6465 2061 6e79   can provide any
+00000dc0: 2073 7472 696e 6720 6173 2061 206b 6579   string as a key
+00000dd0: 2e0a 0a60 6060 7079 7468 6f6e 0a53 4b4c  ...```python.SKL
+00000de0: 4c4d 436f 6e66 6967 2e73 6574 5f6f 7065  LMConfig.set_ope
+00000df0: 6e61 695f 6b65 7928 2261 6e79 2073 7472  nai_key("any str
+00000e00: 696e 6722 290a 534b 4c4c 4d43 6f6e 6669  ing").SKLLMConfi
+00000e10: 672e 7365 745f 6f70 656e 6169 5f6f 7267  g.set_openai_org
+00000e20: 2822 616e 7920 7374 7269 6e67 2229 0a0a  ("any string")..
+00000e30: 5a65 726f 5368 6f74 4750 5443 6c61 7373  ZeroShotGPTClass
+00000e40: 6966 6965 7228 6f70 656e 6169 5f6d 6f64  ifier(openai_mod
+00000e50: 656c 3d22 6770 7434 616c 6c3a 3a67 676d  el="gpt4all::ggm
+00000e60: 6c2d 6770 7434 616c 6c2d 6a2d 7631 2e33  l-gpt4all-j-v1.3
+00000e70: 2d67 726f 6f76 7922 290a 6060 600a 0a57  -groovy").```..W
+00000e80: 6865 6e20 7275 6e6e 696e 6720 666f 7220  hen running for 
+00000e90: 7468 6520 6669 7273 7420 7469 6d65 2c20  the first time, 
+00000ea0: 7468 6520 6d6f 6465 6c20 6669 6c65 2077  the model file w
+00000eb0: 696c 6c20 6265 2064 6f77 6e6c 6f61 6465  ill be downloade
+00000ec0: 6420 6175 746f 6d61 7469 616c 6c79 2e0a  d automatially..
+00000ed0: 0a57 6865 6e20 7573 696e 6720 6770 7434  .When using gpt4
+00000ee0: 616c 6c20 706c 6561 7365 206b 6565 7020  all please keep 
+00000ef0: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+00000f00: 206d 696e 643a 0a0a 312e 204e 6f74 2061   mind:..1. Not a
+00000f10: 6c6c 2067 7074 3461 6c6c 206d 6f64 656c  ll gpt4all model
+00000f20: 7320 6172 6520 636f 6d6d 6572 6369 616c  s are commercial
+00000f30: 6c79 206c 6963 656e 7361 626c 652c 2070  ly licensable, p
+00000f40: 6c65 6173 6520 636f 6e73 756c 7420 6770  lease consult gp
+00000f50: 7434 616c 6c20 7765 6273 6974 6520 666f  t4all website fo
+00000f60: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
+00000f70: 322e 2054 6865 2061 6363 7572 6163 7920  2. The accuracy 
+00000f80: 6f66 2074 6865 206d 6f64 656c 7320 6d61  of the models ma
+00000f90: 7920 6265 206d 7563 6820 6c6f 7765 7220  y be much lower 
+00000fa0: 636f 6d70 6172 6564 2074 6f20 6f6e 6573  compared to ones
+00000fb0: 2070 726f 7669 6465 6420 6279 204f 7065   provided by Ope
+00000fc0: 6e41 4920 2865 7370 6563 6961 6c6c 7920  nAI (especially 
+00000fd0: 6770 742d 3429 2e0a 332e 204e 6f74 2061  gpt-4)..3. Not a
+00000fe0: 6c6c 206f 6620 7468 6520 6176 6169 6c61  ll of the availa
+00000ff0: 626c 6520 6d6f 6465 6c73 2077 6572 6520  ble models were 
+00001000: 7465 7374 6564 2c20 736f 6d65 206d 6179  tested, some may
+00001010: 206e 6f74 2077 6f72 6b20 7769 7468 2073   not work with s
+00001020: 6369 6b69 742d 6c6c 6d20 6174 2061 6c6c  cikit-llm at all
+00001030: 2e0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
+00001040: 206d 6f64 656c 7320 6279 2061 206e 6f6e   models by a non
+00001050: 2d73 7461 6e64 6172 6420 6261 636b 656e  -standard backen
+00001060: 640a 0a41 7420 7468 6520 6d6f 6d65 6e74  d..At the moment
+00001070: 206f 6e6c 7920 7468 6520 666f 6c6c 6f77   only the follow
+00001080: 696e 6720 6573 7469 6d61 746f 7273 2073  ing estimators s
+00001090: 7570 706f 7274 206e 6f6e 2d73 7461 6e64  upport non-stand
+000010a0: 6172 6420 6261 636b 656e 6473 2028 6770  ard backends (gp
+000010b0: 7434 616c 6c2c 2061 7a75 7265 293a 0a0a  t4all, azure):..
+000010c0: 2d20 605a 6572 6f53 686f 7447 5054 436c  - `ZeroShotGPTCl
+000010d0: 6173 7369 6669 6572 600a 2d20 604d 756c  assifier`.- `Mul
+000010e0: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
+000010f0: 5054 436c 6173 7369 6669 6572 600a 2d20  PTClassifier`.- 
+00001100: 6046 6577 5368 6f74 4750 5443 6c61 7373  `FewShotGPTClass
+00001110: 6966 6965 7260 0a0a 2323 2320 5a65 726f  ifier`..### Zero
+00001120: 2d53 686f 7420 5465 7874 2043 6c61 7373  -Shot Text Class
+00001130: 6966 6963 6174 696f 6e0a 0a4f 6e65 206f  ification..One o
+00001140: 6620 7468 6520 706f 7765 7266 756c 2043  f the powerful C
+00001150: 6861 7447 5054 2066 6561 7475 7265 7320  hatGPT features 
+00001160: 6973 2074 6865 2061 6269 6c69 7479 2074  is the ability t
+00001170: 6f20 7065 7266 6f72 6d20 7465 7874 2063  o perform text c
+00001180: 6c61 7373 6966 6963 6174 696f 6e20 7769  lassification wi
+00001190: 7468 6f75 7420 6265 696e 6720 7265 2d74  thout being re-t
+000011a0: 7261 696e 6564 2e20 466f 7220 7468 6174  rained. For that
+000011b0: 2c20 7468 6520 6f6e 6c79 2072 6571 7569  , the only requi
+000011c0: 7265 6d65 6e74 2069 7320 7468 6174 2074  rement is that t
+000011d0: 6865 206c 6162 656c 7320 6d75 7374 2062  he labels must b
+000011e0: 6520 6465 7363 7269 7074 6976 652e 0a0a  e descriptive...
+000011f0: 5765 2070 726f 7669 6465 2061 2063 6c61  We provide a cla
+00001200: 7373 2060 5a65 726f 5368 6f74 4750 5443  ss `ZeroShotGPTC
+00001210: 6c61 7373 6966 6965 7260 2074 6861 7420  lassifier` that 
+00001220: 616c 6c6f 7773 2074 6f20 6372 6561 7465  allows to create
+00001230: 2073 7563 6820 6120 6d6f 6465 6c20 6173   such a model as
+00001240: 2061 2072 6567 756c 6172 2073 6369 6b69   a regular sciki
+00001250: 742d 6c65 6172 6e20 636c 6173 7369 6669  t-learn classifi
+00001260: 6572 2e0a 0a45 7861 6d70 6c65 2031 3a20  er...Example 1: 
+00001270: 5472 6169 6e69 6e67 2061 7320 6120 7265  Training as a re
+00001280: 6775 6c61 7220 636c 6173 7369 6669 6572  gular classifier
+00001290: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000012a0: 2073 6b6c 6c6d 2069 6d70 6f72 7420 5a65   skllm import Ze
+000012b0: 726f 5368 6f74 4750 5443 6c61 7373 6966  roShotGPTClassif
+000012c0: 6965 720a 6672 6f6d 2073 6b6c 6c6d 2e64  ier.from skllm.d
+000012d0: 6174 6173 6574 7320 696d 706f 7274 2067  atasets import g
+000012e0: 6574 5f63 6c61 7373 6966 6963 6174 696f  et_classificatio
+000012f0: 6e5f 6461 7461 7365 740a 0a23 2064 656d  n_dataset..# dem
+00001300: 6f20 7365 6e74 696d 656e 7420 616e 616c  o sentiment anal
+00001310: 7973 6973 2064 6174 6173 6574 0a23 206c  ysis dataset.# l
+00001320: 6162 656c 733a 2070 6f73 6974 6976 652c  abels: positive,
+00001330: 206e 6567 6174 6976 652c 206e 6575 7472   negative, neutr
+00001340: 616c 0a58 2c20 7920 3d20 6765 745f 636c  al.X, y = get_cl
+00001350: 6173 7369 6669 6361 7469 6f6e 5f64 6174  assification_dat
+00001360: 6173 6574 2829 0a0a 636c 6620 3d20 5a65  aset()..clf = Ze
+00001370: 726f 5368 6f74 4750 5443 6c61 7373 6966  roShotGPTClassif
+00001380: 6965 7228 6f70 656e 6169 5f6d 6f64 656c  ier(openai_model
+00001390: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+000013a0: 290a 636c 662e 6669 7428 582c 2079 290a  ).clf.fit(X, y).
+000013b0: 6c61 6265 6c73 203d 2063 6c66 2e70 7265  labels = clf.pre
+000013c0: 6469 6374 2858 290a 6060 600a 0a53 6369  dict(X).```..Sci
+000013d0: 6b69 742d 4c4c 4d20 7769 6c6c 2061 7574  kit-LLM will aut
+000013e0: 6f6d 6174 6963 616c 6c79 2071 7565 7279  omatically query
+000013f0: 2074 6865 204f 7065 6e41 4920 4150 4920   the OpenAI API 
+00001400: 616e 6420 7472 616e 7366 6f72 6d20 7468  and transform th
+00001410: 6520 7265 7370 6f6e 7365 2069 6e74 6f20  e response into 
+00001420: 6120 7265 6775 6c61 7220 6c69 7374 206f  a regular list o
+00001430: 6620 6c61 6265 6c73 2e0a 0a41 6464 6974  f labels...Addit
+00001440: 696f 6e61 6c6c 792c 2053 6369 6b69 742d  ionally, Scikit-
+00001450: 4c4c 4d20 7769 6c6c 2065 6e73 7572 6520  LLM will ensure 
+00001460: 7468 6174 2074 6865 206f 6274 6169 6e65  that the obtaine
+00001470: 6420 7265 7370 6f6e 7365 2063 6f6e 7461  d response conta
+00001480: 696e 7320 6120 7661 6c69 6420 6c61 6265  ins a valid labe
+00001490: 6c2e 2049 6620 7468 6973 2069 7320 6e6f  l. If this is no
+000014a0: 7420 7468 6520 6361 7365 2c20 6120 6c61  t the case, a la
+000014b0: 6265 6c20 7769 6c6c 2062 6520 7365 6c65  bel will be sele
+000014c0: 6374 6564 2072 616e 646f 6d6c 7920 286c  cted randomly (l
+000014d0: 6162 656c 2070 726f 6261 6269 6c69 7469  abel probabiliti
+000014e0: 6573 2061 7265 2070 726f 706f 7274 696f  es are proportio
+000014f0: 6e61 6c20 746f 206c 6162 656c 206f 6363  nal to label occ
+00001500: 7572 7265 6e63 6573 2069 6e20 7468 6520  urrences in the 
+00001510: 7472 6169 6e69 6e67 2073 6574 292e 0a0a  training set)...
+00001520: 4578 616d 706c 6520 323a 2054 7261 696e  Example 2: Train
+00001530: 696e 6720 7769 7468 6f75 7420 6c61 6265  ing without labe
+00001540: 6c65 6420 6461 7461 0a0a 5369 6e63 6520  led data..Since 
+00001550: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
+00001560: 6120 6973 206e 6f74 2073 7472 6963 746c  a is not strictl
+00001570: 7920 7265 7175 6972 6564 2c20 6974 2063  y required, it c
+00001580: 616e 2062 6520 6675 6c6c 7920 6f6d 6d69  an be fully ommi
+00001590: 7465 642e 2054 6865 206f 6e6c 7920 7468  ted. The only th
+000015a0: 696e 6720 7468 6174 2068 6173 2074 6f20  ing that has to 
+000015b0: 6265 2070 726f 7669 6465 6420 6973 2074  be provided is t
+000015c0: 6865 206c 6973 7420 6f66 2063 616e 6469  he list of candi
+000015d0: 6461 7465 206c 6162 656c 732e 0a0a 6060  date labels...``
+000015e0: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+000015f0: 6c6d 2069 6d70 6f72 7420 5a65 726f 5368  lm import ZeroSh
+00001600: 6f74 4750 5443 6c61 7373 6966 6965 720a  otGPTClassifier.
+00001610: 6672 6f6d 2073 6b6c 6c6d 2e64 6174 6173  from skllm.datas
+00001620: 6574 7320 696d 706f 7274 2067 6574 5f63  ets import get_c
+00001630: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
+00001640: 7461 7365 740a 0a58 2c20 5f20 3d20 6765  taset..X, _ = ge
+00001650: 745f 636c 6173 7369 6669 6361 7469 6f6e  t_classification
+00001660: 5f64 6174 6173 6574 2829 0a0a 636c 6620  _dataset()..clf 
+00001670: 3d20 5a65 726f 5368 6f74 4750 5443 6c61  = ZeroShotGPTCla
+00001680: 7373 6966 6965 7228 290a 636c 662e 6669  ssifier().clf.fi
+00001690: 7428 4e6f 6e65 2c20 5b22 706f 7369 7469  t(None, ["positi
+000016a0: 7665 222c 2022 6e65 6761 7469 7665 222c  ve", "negative",
+000016b0: 2022 6e65 7574 7261 6c22 5d29 0a6c 6162   "neutral"]).lab
+000016c0: 656c 7320 3d20 636c 662e 7072 6564 6963  els = clf.predic
+000016d0: 7428 5829 0a60 6060 0a0a 2a2a 4e6f 7465  t(X).```..**Note
+000016e0: 3a2a 2a20 756e 6c69 6b65 2069 6e20 6120  :** unlike in a 
+000016f0: 7479 7069 6361 6c20 7375 7065 7276 6973  typical supervis
+00001700: 6564 2073 6574 7469 6e67 2c20 7468 6520  ed setting, the 
+00001710: 7065 7266 6f72 6d61 6e63 6520 6f66 2061  performance of a
+00001720: 207a 6572 6f2d 7368 6f74 2063 6c61 7373   zero-shot class
+00001730: 6966 6965 7220 6772 6561 746c 7920 6465  ifier greatly de
+00001740: 7065 6e64 7320 6f6e 2068 6f77 2074 6865  pends on how the
+00001750: 206c 6162 656c 2069 7473 656c 6620 6973   label itself is
+00001760: 2073 7472 7563 7475 7265 642e 2049 7420   structured. It 
+00001770: 6861 7320 746f 2062 6520 6578 7072 6573  has to be expres
+00001780: 7365 6420 696e 206e 6174 7572 616c 206c  sed in natural l
+00001790: 616e 6775 6167 652c 2062 6520 6465 7363  anguage, be desc
+000017a0: 7269 7074 6976 6520 616e 6420 7365 6c66  riptive and self
+000017b0: 2d65 7870 6c61 6e61 746f 7279 2e20 466f  -explanatory. Fo
+000017c0: 7220 6578 616d 706c 652c 2069 6e20 7468  r example, in th
+000017d0: 6520 7072 6576 696f 7573 2073 656d 616e  e previous seman
+000017e0: 7469 6320 636c 6173 7369 6669 6361 7469  tic classificati
+000017f0: 6f6e 2074 6173 6b2c 2069 7420 636f 756c  on task, it coul
+00001800: 6420 6265 2062 656e 6566 6963 6961 6c20  d be beneficial 
+00001810: 746f 2074 7261 6e73 666f 726d 2061 206c  to transform a l
+00001820: 6162 656c 2066 726f 6d20 6022 3c73 656d  abel from `"<sem
+00001830: 616e 7469 6373 3e22 6020 746f 2060 2274  antics>"` to `"t
+00001840: 6865 2073 656d 616e 7469 6373 206f 6620  he semantics of 
+00001850: 7468 6520 7072 6f76 6964 6564 2074 6578  the provided tex
+00001860: 7420 6973 203c 7365 6d61 6e74 6963 733e  t is <semantics>
+00001870: 2260 2e0a 0a23 2323 204d 756c 7469 2d4c  "`...### Multi-L
+00001880: 6162 656c 205a 6572 6f2d 5368 6f74 2054  abel Zero-Shot T
+00001890: 6578 7420 436c 6173 7369 6669 6361 7469  ext Classificati
+000018a0: 6f6e 0a0a 5769 7468 2061 2063 6c61 7373  on..With a class
+000018b0: 2060 4d75 6c74 694c 6162 656c 5a65 726f   `MultiLabelZero
+000018c0: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+000018d0: 7260 2069 7420 6973 2070 6f73 7369 626c  r` it is possibl
+000018e0: 6520 746f 2070 6572 666f 726d 2074 6865  e to perform the
+000018f0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00001900: 696e 206d 756c 7469 2d6c 6162 656c 2073  in multi-label s
+00001910: 6574 7469 6e67 2c20 7768 6963 6820 6d65  etting, which me
+00001920: 616e 7320 7468 6174 2065 6163 6820 7361  ans that each sa
+00001930: 6d70 6c65 206d 6967 6874 2062 6520 6173  mple might be as
+00001940: 7369 676e 6564 2074 6f20 6f6e 6520 6f72  signed to one or
+00001950: 2073 6576 6572 616c 2064 6973 7469 6e63   several distinc
+00001960: 7420 636c 6173 7365 732e 0a0a 4578 616d  t classes...Exam
+00001970: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00001980: 6672 6f6d 2073 6b6c 6c6d 2069 6d70 6f72  from skllm impor
+00001990: 7420 4d75 6c74 694c 6162 656c 5a65 726f  t MultiLabelZero
+000019a0: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+000019b0: 720a 6672 6f6d 2073 6b6c 6c6d 2e64 6174  r.from skllm.dat
+000019c0: 6173 6574 7320 696d 706f 7274 2067 6574  asets import get
+000019d0: 5f6d 756c 7469 6c61 6265 6c5f 636c 6173  _multilabel_clas
+000019e0: 7369 6669 6361 7469 6f6e 5f64 6174 6173  sification_datas
+000019f0: 6574 0a0a 582c 2079 203d 2067 6574 5f6d  et..X, y = get_m
+00001a00: 756c 7469 6c61 6265 6c5f 636c 6173 7369  ultilabel_classi
+00001a10: 6669 6361 7469 6f6e 5f64 6174 6173 6574  fication_dataset
+00001a20: 2829 0a0a 636c 6620 3d20 4d75 6c74 694c  ()..clf = MultiL
+00001a30: 6162 656c 5a65 726f 5368 6f74 4750 5443  abelZeroShotGPTC
+00001a40: 6c61 7373 6966 6965 7228 6d61 785f 6c61  lassifier(max_la
+00001a50: 6265 6c73 3d33 290a 636c 662e 6669 7428  bels=3).clf.fit(
+00001a60: 582c 2079 290a 6c61 6265 6c73 203d 2063  X, y).labels = c
+00001a70: 6c66 2e70 7265 6469 6374 2858 290a 6060  lf.predict(X).``
+00001a80: 600a 0a53 696d 696c 6172 6c79 2074 6f20  `..Similarly to 
+00001a90: 7468 6520 605a 6572 6f53 686f 7447 5054  the `ZeroShotGPT
+00001aa0: 436c 6173 7369 6669 6572 6020 6974 2069  Classifier` it i
+00001ab0: 7320 7375 6666 6963 6965 6e74 2069 6620  s sufficient if 
+00001ac0: 6f6e 6c79 2063 616e 6469 6461 7465 206c  only candidate l
+00001ad0: 6162 656c 7320 6172 6520 7072 6f76 6964  abels are provid
+00001ae0: 6564 2e20 486f 7765 7665 722c 2074 6869  ed. However, thi
+00001af0: 7320 7469 6d65 2074 6865 2063 6c61 7373  s time the class
+00001b00: 6966 6965 7220 6578 7065 6374 7320 6079  ifier expects `y
+00001b10: 6020 6f66 2061 2074 7970 6520 604c 6973  ` of a type `Lis
+00001b20: 745b 4c69 7374 5b73 7472 5d5d 602e 0a0a  t[List[str]]`...
+00001b30: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
+00001b40: 6b6c 6c6d 2069 6d70 6f72 7420 4d75 6c74  kllm import Mult
+00001b50: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
+00001b60: 5443 6c61 7373 6966 6965 720a 6672 6f6d  TClassifier.from
+00001b70: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
+00001b80: 696d 706f 7274 2067 6574 5f6d 756c 7469  import get_multi
+00001b90: 6c61 6265 6c5f 636c 6173 7369 6669 6361  label_classifica
+00001ba0: 7469 6f6e 5f64 6174 6173 6574 0a0a 582c  tion_dataset..X,
+00001bb0: 205f 203d 2067 6574 5f6d 756c 7469 6c61   _ = get_multila
+00001bc0: 6265 6c5f 636c 6173 7369 6669 6361 7469  bel_classificati
+00001bd0: 6f6e 5f64 6174 6173 6574 2829 0a63 616e  on_dataset().can
+00001be0: 6469 6461 7465 5f6c 6162 656c 7320 3d20  didate_labels = 
+00001bf0: 5b0a 2020 2020 2251 7561 6c69 7479 222c  [.    "Quality",
+00001c00: 0a20 2020 2022 5072 6963 6522 2c0a 2020  .    "Price",.  
+00001c10: 2020 2244 656c 6976 6572 7922 2c0a 2020    "Delivery",.  
+00001c20: 2020 2253 6572 7669 6365 222c 0a20 2020    "Service",.   
+00001c30: 2022 5072 6f64 7563 7420 5661 7269 6574   "Product Variet
+00001c40: 7922 2c0a 2020 2020 2243 7573 746f 6d65  y",.    "Custome
+00001c50: 7220 5375 7070 6f72 7422 2c0a 2020 2020  r Support",.    
+00001c60: 2250 6163 6b61 6769 6e67 222c 0a20 2020  "Packaging",.   
+00001c70: 2022 5573 6572 2045 7870 6572 6965 6e63   "User Experienc
+00001c80: 6522 2c0a 2020 2020 2252 6574 7572 6e20  e",.    "Return 
+00001c90: 506f 6c69 6379 222c 0a20 2020 2022 5072  Policy",.    "Pr
+00001ca0: 6f64 7563 7420 496e 666f 726d 6174 696f  oduct Informatio
+00001cb0: 6e22 2c0a 5d0a 636c 6620 3d20 4d75 6c74  n",.].clf = Mult
+00001cc0: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
+00001cd0: 5443 6c61 7373 6966 6965 7228 6d61 785f  TClassifier(max_
+00001ce0: 6c61 6265 6c73 3d33 290a 636c 662e 6669  labels=3).clf.fi
+00001cf0: 7428 4e6f 6e65 2c20 5b63 616e 6469 6461  t(None, [candida
+00001d00: 7465 5f6c 6162 656c 735d 290a 6c61 6265  te_labels]).labe
+00001d10: 6c73 203d 2063 6c66 2e70 7265 6469 6374  ls = clf.predict
+00001d20: 2858 290a 6060 600a 0a23 2323 2046 6577  (X).```..### Few
+00001d30: 2d53 686f 7420 5465 7874 2043 6c61 7373  -Shot Text Class
+00001d40: 6966 6963 6174 696f 6e0a 0a57 6974 6820  ification..With 
+00001d50: 6046 6577 5368 6f74 4750 5443 6c61 7373  `FewShotGPTClass
+00001d60: 6966 6965 7260 2069 7420 6973 2070 6f73  ifier` it is pos
+00001d70: 7369 626c 6520 746f 2070 6572 666f 726d  sible to perform
+00001d80: 2061 2066 6577 2d73 686f 7420 636c 6173   a few-shot clas
+00001d90: 7369 6669 6361 7469 6f6e 2c20 7768 6963  sification, whic
+00001da0: 6820 6d65 616e 7320 7468 6174 2074 6865  h means that the
+00001db0: 2074 7261 696e 696e 6720 7361 6d70 6c65   training sample
+00001dc0: 7320 7769 6c6c 2062 6520 6164 6465 6420  s will be added 
+00001dd0: 746f 2070 726f 6d70 7420 616e 6420 7061  to prompt and pa
+00001de0: 7373 6564 2074 6f20 7468 6520 6d6f 6465  ssed to the mode
+00001df0: 6c2e 0a0a 6060 6070 7974 686f 6e0a 6672  l...```python.fr
+00001e00: 6f6d 2073 6b6c 6c6d 2069 6d70 6f72 7420  om skllm import 
+00001e10: 4665 7753 686f 7447 5054 436c 6173 7369  FewShotGPTClassi
+00001e20: 6669 6572 0a66 726f 6d20 736b 6c6c 6d2e  fier.from skllm.
+00001e30: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
+00001e40: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
+00001e50: 6f6e 5f64 6174 6173 6574 0a0a 582c 2079  on_dataset..X, y
+00001e60: 203d 2067 6574 5f63 6c61 7373 6966 6963   = get_classific
+00001e70: 6174 696f 6e5f 6461 7461 7365 7428 290a  ation_dataset().
+00001e80: 0a63 6c66 203d 2046 6577 5368 6f74 4750  .clf = FewShotGP
+00001e90: 5443 6c61 7373 6966 6965 7228 6f70 656e  TClassifier(open
+00001ea0: 6169 5f6d 6f64 656c 3d22 6770 742d 332e  ai_model="gpt-3.
+00001eb0: 352d 7475 7262 6f22 290a 636c 662e 6669  5-turbo").clf.fi
+00001ec0: 7428 582c 2079 290a 6c61 6265 6c73 203d  t(X, y).labels =
+00001ed0: 2063 6c66 2e70 7265 6469 6374 2858 290a   clf.predict(X).
+00001ee0: 6060 600a 0a57 6869 6c65 2074 6865 2061  ```..While the a
+00001ef0: 7069 2072 656d 6169 6e73 2074 6865 2073  pi remains the s
+00001f00: 616d 6520 6173 2066 6f72 2074 6865 207a  ame as for the z
+00001f10: 6572 6f20 7368 6f74 2063 6c61 7373 6966  ero shot classif
+00001f20: 6965 722c 2074 6865 7265 2061 7265 2061  ier, there are a
+00001f30: 2066 6577 2074 6869 6e67 7320 746f 2074   few things to t
+00001f40: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
+00001f50: 3a0a 0a2d 2074 6865 2022 7472 6169 6e69  :..- the "traini
+00001f60: 6e67 2220 7265 7175 6972 6573 2073 6f6d  ng" requires som
+00001f70: 6520 6c61 6265 6c6c 6564 2074 7261 696e  e labelled train
+00001f80: 696e 6720 6461 7461 3b0a 2d20 7468 6520  ing data;.- the 
+00001f90: 7472 6169 6e69 6e67 2073 6574 2073 686f  training set sho
+00001fa0: 756c 6420 6265 2073 6d61 6c6c 2065 6e6f  uld be small eno
+00001fb0: 7567 6820 746f 2066 6974 2069 6e74 6f20  ugh to fit into 
+00001fc0: 6120 7369 6e67 6c65 2070 726f 6d70 7420  a single prompt 
+00001fd0: 2877 6520 7265 636f 6d6d 656e 6420 7570  (we recommend up
+00001fe0: 2074 6f20 3130 2073 616d 706c 6573 2070   to 10 samples p
+00001ff0: 6572 206c 6162 656c 293b 0a2d 2062 6563  er label);.- bec
+00002000: 6175 7365 206f 6620 7468 6520 7369 676e  ause of the sign
+00002010: 6966 6963 616e 746c 7920 6c61 7267 6572  ificantly larger
+00002020: 2070 726f 6d70 742c 2074 6865 2069 6e66   prompt, the inf
+00002030: 6572 656e 6365 2074 616b 6573 206c 6f6e  erence takes lon
+00002040: 6765 7220 616e 6420 636f 6e73 756d 6573  ger and consumes
+00002050: 2068 6967 6865 7220 616d 6f75 6e74 206f   higher amount o
+00002060: 6620 746f 6b65 6e73 2e0a 0a4e 6f74 653a  f tokens...Note:
+00002070: 2061 7320 7468 6520 6d6f 6465 6c20 6973   as the model is
+00002080: 206e 6f74 2062 6569 6e67 2072 652d 7472   not being re-tr
+00002090: 6169 6e65 642c 2062 7574 2075 7365 7320  ained, but uses 
+000020a0: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
+000020b0: 6120 6475 7269 6e67 2069 6e66 6572 656e  a during inferen
+000020c0: 6365 2c20 6f6e 6520 636f 756c 6420 7361  ce, one could sa
+000020d0: 7920 7468 6174 2074 6869 7320 6973 2073  y that this is s
+000020e0: 7469 6c6c 2061 2028 6469 6666 6572 656e  till a (differen
+000020f0: 7429 207a 6572 6f2d 7368 6f74 2061 7070  t) zero-shot app
+00002100: 726f 6163 682e 0a0a 2323 2320 4479 6e61  roach...### Dyna
+00002110: 6d69 6320 4665 772d 5368 6f74 2054 6578  mic Few-Shot Tex
+00002120: 7420 436c 6173 7369 6669 6361 7469 6f6e  t Classification
+00002130: 0a0a 6044 796e 616d 6963 4665 7753 686f  ..`DynamicFewSho
+00002140: 7447 5054 436c 6173 7369 6669 6572 6020  tGPTClassifier` 
+00002150: 6479 6e61 6d69 6361 6c6c 7920 7365 6c65  dynamically sele
+00002160: 6374 7320 4e20 7361 6d70 6c65 7320 7065  cts N samples pe
+00002170: 7220 636c 6173 7320 746f 2069 6e63 6c75  r class to inclu
+00002180: 6465 2069 6e20 7468 6520 7072 6f6d 7074  de in the prompt
+00002190: 2e20 5468 6973 2061 6c6c 6f77 7320 7468  . This allows th
+000021a0: 6520 6665 772d 7368 6f74 2063 6c61 7373  e few-shot class
+000021b0: 6966 6965 7220 746f 2073 6361 6c65 2074  ifier to scale t
+000021c0: 6f20 6461 7461 7365 7473 2074 6861 7420  o datasets that 
+000021d0: 6172 6520 746f 6f20 6c61 7267 6520 666f  are too large fo
+000021e0: 7220 7468 6520 7374 616e 6461 7264 2063  r the standard c
+000021f0: 6f6e 7465 7874 2077 696e 646f 7720 6f66  ontext window of
+00002200: 204c 4c4d 732e 0a0a 2a48 6f77 2064 6f65   LLMs...*How doe
+00002210: 7320 6974 2077 6f72 6b3f 2a0a 0a44 7572  s it work?*..Dur
+00002220: 696e 6720 6669 7474 696e 672c 2074 6865  ing fitting, the
+00002230: 2077 686f 6c65 2064 6174 6173 6574 2069   whole dataset i
+00002240: 7320 7061 7274 6974 696f 6e65 6420 6279  s partitioned by
+00002250: 2063 6c61 7373 2c20 7665 6374 6f72 697a   class, vectoriz
+00002260: 6564 2c20 616e 6420 7374 6f72 6564 2e0a  ed, and stored..
+00002270: 0a44 7572 696e 6720 696e 6665 7265 6e63  .During inferenc
+00002280: 652c 2074 6865 205b 616e 6e6f 795d 2868  e, the [annoy](h
+00002290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000022a0: 6d2f 7370 6f74 6966 792f 616e 6e6f 7929  m/spotify/annoy)
+000022b0: 206c 6962 7261 7279 2069 7320 7573 6564   library is used
+000022c0: 2066 6f72 2066 6173 7420 6e65 6967 6862   for fast neighb
+000022d0: 6f72 206c 6f6f 6b75 702c 2077 6869 6368  or lookup, which
+000022e0: 2061 6c6c 6f77 7320 696e 636c 7564 696e   allows includin
+000022f0: 6720 6f6e 6c79 2074 6865 206d 6f73 7420  g only the most 
+00002300: 7369 6d69 6c61 7220 6578 616d 706c 6573  similar examples
+00002310: 2069 6e20 7468 6520 7072 6f6d 7074 2e0a   in the prompt..
+00002320: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00002330: 736b 6c6c 6d20 696d 706f 7274 2044 796e  skllm import Dyn
+00002340: 616d 6963 4665 7753 686f 7447 5054 436c  amicFewShotGPTCl
+00002350: 6173 7369 6669 6572 0a66 726f 6d20 736b  assifier.from sk
+00002360: 6c6c 6d2e 6461 7461 7365 7473 2069 6d70  llm.datasets imp
+00002370: 6f72 7420 6765 745f 636c 6173 7369 6669  ort get_classifi
+00002380: 6361 7469 6f6e 5f64 6174 6173 6574 0a0a  cation_dataset..
+00002390: 582c 2079 203d 2067 6574 5f63 6c61 7373  X, y = get_class
+000023a0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
+000023b0: 7428 290a 0a63 6c66 203d 2044 796e 616d  t()..clf = Dynam
+000023c0: 6963 4665 7753 686f 7447 5054 436c 6173  icFewShotGPTClas
+000023d0: 7369 6669 6572 286e 5f65 7861 6d70 6c65  sifier(n_example
+000023e0: 733d 3329 0a63 6c66 2e66 6974 2858 2c20  s=3).clf.fit(X, 
+000023f0: 7929 0a6c 6162 656c 7320 3d20 636c 662e  y).labels = clf.
+00002400: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
+00002410: 2323 2320 5465 7874 2043 6c61 7373 6966  ### Text Classif
+00002420: 6963 6174 696f 6e20 7769 7468 2047 6f6f  ication with Goo
+00002430: 676c 6520 5061 4c4d 2032 0a0a 4174 2074  gle PaLM 2..At t
+00002440: 6865 206d 6f6d 656e 7420 3320 5061 4c4d  he moment 3 PaLM
+00002450: 2062 6173 6564 206d 6f64 656c 7320 6172   based models ar
+00002460: 6520 6176 6169 6c61 626c 6520 696e 2074  e available in t
+00002470: 6573 7420 6d6f 6465 3a0a 2d20 605a 6572  est mode:.- `Zer
+00002480: 6f53 686f 7450 614c 4d43 6c61 7373 6966  oShotPaLMClassif
+00002490: 6965 7260 202d 207a 6572 6f2d 7368 6f74  ier` - zero-shot
+000024a0: 2074 6578 7420 636c 6173 7369 6669 6361   text classifica
+000024b0: 7469 6f6e 2077 6974 6820 5061 4c4d 2032  tion with PaLM 2
+000024c0: 3b0a 2d20 6050 614c 4d43 6c61 7373 6966  ;.- `PaLMClassif
+000024d0: 6965 7260 202d 2066 696e 652d 7475 6e61  ier` - fine-tuna
+000024e0: 626c 6520 7465 7874 2063 6c61 7373 6966  ble text classif
+000024f0: 6965 7220 7769 7468 2050 614c 4d20 323b  ier with PaLM 2;
+00002500: 0a2d 2060 5061 4c4d 6020 2d20 6669 6e65  .- `PaLM` - fine
+00002510: 2d74 756e 6162 6c65 2065 7374 696d 6174  -tunable estimat
+00002520: 6f72 2074 6861 7420 6361 6e20 6265 2074  or that can be t
+00002530: 7261 696e 6564 206f 6e20 6172 6269 7472  rained on arbitr
+00002540: 6172 7920 7465 7874 2069 6e70 7574 2d6f  ary text input-o
+00002550: 7574 7075 7420 7061 6972 732e 0a0a 4578  utput pairs...Ex
+00002560: 616d 706c 653a 200a 0a60 6060 7079 7468  ample: ..```pyth
+00002570: 6f6e 0a66 726f 6d20 736b 6c6c 6d2e 6d6f  on.from skllm.mo
+00002580: 6465 6c73 2e70 616c 6d20 696d 706f 7274  dels.palm import
+00002590: 2050 614c 4d43 6c61 7373 6966 6965 720a   PaLMClassifier.
+000025a0: 6672 6f6d 2073 6b6c 6c6d 2e64 6174 6173  from skllm.datas
+000025b0: 6574 7320 696d 706f 7274 2067 6574 5f63  ets import get_c
+000025c0: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
+000025d0: 7461 7365 740a 0a58 2c20 7920 3d20 6765  taset..X, y = ge
+000025e0: 745f 636c 6173 7369 6669 6361 7469 6f6e  t_classification
+000025f0: 5f64 6174 6173 6574 2829 0a0a 636c 6620  _dataset()..clf 
+00002600: 3d20 5061 4c4d 436c 6173 7369 6669 6572  = PaLMClassifier
+00002610: 286e 5f75 7064 6174 655f 7374 6570 733d  (n_update_steps=
+00002620: 3130 3029 0a63 6c66 2e66 6974 2858 2c20  100).clf.fit(X, 
+00002630: 7929 0a6c 6162 656c 7320 3d20 636c 662e  y).labels = clf.
+00002640: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
+00002650: 4120 6d6f 7265 2064 6574 6169 6c65 6420  A more detailed 
+00002660: 646f 6375 6d65 6e74 6174 696f 6e20 7769  documentation wi
+00002670: 6c6c 2066 6f6c 6c6f 7720 736f 6f6e 2e20  ll follow soon. 
+00002680: 466f 7220 6e6f 772c 2070 6c65 6173 6520  For now, please 
+00002690: 7265 6665 7220 746f 206f 7572 205b 6f66  refer to our [of
+000026a0: 6669 6369 616c 2067 7569 6465 206f 6e20  ficial guide on 
+000026b0: 4d65 6469 756d 5d28 6874 7470 733a 2f2f  Medium](https://
+000026c0: 6d65 6469 756d 2e63 6f6d 2f40 6972 796e  medium.com/@iryn
+000026d0: 6132 3330 3532 3029 2e0a 0a23 2323 2054  a230520)...### T
+000026e0: 6578 7420 5665 6374 6f72 697a 6174 696f  ext Vectorizatio
+000026f0: 6e0a 0a41 7320 616e 2061 6c74 6572 6e61  n..As an alterna
+00002700: 7469 7665 2074 6f20 7573 696e 6720 4750  tive to using GP
+00002710: 5420 6173 2061 2063 6c61 7373 6966 6965  T as a classifie
+00002720: 722c 2069 7420 6361 6e20 6265 2075 7365  r, it can be use
+00002730: 6420 736f 6c65 6c79 2066 6f72 2064 6174  d solely for dat
+00002740: 6120 7072 6570 726f 6365 7373 696e 672e  a preprocessing.
+00002750: 2060 4750 5456 6563 746f 7269 7a65 7260   `GPTVectorizer`
+00002760: 2061 6c6c 6f77 7320 746f 2065 6d62 6564   allows to embed
+00002770: 2061 2063 6875 6e6b 206f 6620 7465 7874   a chunk of text
+00002780: 206f 6620 6172 6269 7472 6172 7920 6c65   of arbitrary le
+00002790: 6e67 7468 2074 6f20 6120 6669 7865 642d  ngth to a fixed-
+000027a0: 6469 6d65 6e73 696f 6e61 6c20 7665 6374  dimensional vect
+000027b0: 6f72 2c20 7468 6174 2063 616e 2062 6520  or, that can be 
+000027c0: 7573 6564 2077 6974 6820 7669 7274 7561  used with virtua
+000027d0: 6c6c 7920 616e 7920 636c 6173 7369 6669  lly any classifi
+000027e0: 6361 7469 6f6e 206f 7220 7265 6772 6573  cation or regres
+000027f0: 7369 6f6e 206d 6f64 656c 2e0a 0a45 7861  sion model...Exa
+00002800: 6d70 6c65 2031 3a20 456d 6265 6464 696e  mple 1: Embeddin
+00002810: 6720 7468 6520 7465 7874 0a0a 6060 6070  g the text..```p
+00002820: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
+00002830: 2e70 7265 7072 6f63 6573 7369 6e67 2069  .preprocessing i
+00002840: 6d70 6f72 7420 4750 5456 6563 746f 7269  mport GPTVectori
+00002850: 7a65 720a 0a6d 6f64 656c 203d 2047 5054  zer..model = GPT
+00002860: 5665 6374 6f72 697a 6572 2829 0a76 6563  Vectorizer().vec
+00002870: 746f 7273 203d 206d 6f64 656c 2e66 6974  tors = model.fit
+00002880: 5f74 7261 6e73 666f 726d 2858 290a 6060  _transform(X).``
+00002890: 600a 0a45 7861 6d70 6c65 2032 3a20 436f  `..Example 2: Co
+000028a0: 6d62 696e 696e 6720 7468 6520 5665 6374  mbining the Vect
+000028b0: 6f72 697a 6572 2077 6974 6820 7468 6520  orizer with the 
+000028c0: 5847 426f 6f73 7420 436c 6173 7369 6669  XGBoost Classifi
+000028d0: 6572 2069 6e20 6120 536b 6c65 6172 6e20  er in a Sklearn 
+000028e0: 5069 7065 6c69 6e65 0a0a 6060 6070 7974  Pipeline..```pyt
+000028f0: 686f 6e0a 6672 6f6d 2073 6b6c 6561 726e  hon.from sklearn
+00002900: 2e70 6970 656c 696e 6520 696d 706f 7274  .pipeline import
+00002910: 2050 6970 656c 696e 650a 6672 6f6d 2073   Pipeline.from s
+00002920: 6b6c 6561 726e 2e70 7265 7072 6f63 6573  klearn.preproces
+00002930: 7369 6e67 2069 6d70 6f72 7420 4c61 6265  sing import Labe
+00002940: 6c45 6e63 6f64 6572 0a66 726f 6d20 7867  lEncoder.from xg
+00002950: 626f 6f73 7420 696d 706f 7274 2058 4742  boost import XGB
+00002960: 436c 6173 7369 6669 6572 0a0a 6c65 203d  Classifier..le =
+00002970: 204c 6162 656c 456e 636f 6465 7228 290a   LabelEncoder().
+00002980: 795f 7472 6169 6e5f 656e 636f 6465 6420  y_train_encoded 
+00002990: 3d20 6c65 2e66 6974 5f74 7261 6e73 666f  = le.fit_transfo
+000029a0: 726d 2879 5f74 7261 696e 290a 795f 7465  rm(y_train).y_te
+000029b0: 7374 5f65 6e63 6f64 6564 203d 206c 652e  st_encoded = le.
+000029c0: 7472 616e 7366 6f72 6d28 795f 7465 7374  transform(y_test
+000029d0: 290a 0a73 7465 7073 203d 205b 2822 4750  )..steps = [("GP
+000029e0: 5422 2c20 4750 5456 6563 746f 7269 7a65  T", GPTVectorize
+000029f0: 7228 2929 2c20 2822 436c 6622 2c20 5847  r()), ("Clf", XG
+00002a00: 4243 6c61 7373 6966 6965 7228 2929 5d0a  BClassifier())].
+00002a10: 636c 6620 3d20 5069 7065 6c69 6e65 2873  clf = Pipeline(s
+00002a20: 7465 7073 290a 636c 662e 6669 7428 585f  teps).clf.fit(X_
+00002a30: 7472 6169 6e2c 2079 5f74 7261 696e 5f65  train, y_train_e
+00002a40: 6e63 6f64 6564 290a 7968 203d 2063 6c66  ncoded).yh = clf
+00002a50: 2e70 7265 6469 6374 2858 5f74 6573 7429  .predict(X_test)
+00002a60: 0a60 6060 0a0a 2323 2320 5465 7874 2053  .```..### Text S
+00002a70: 756d 6d61 7269 7a61 7469 6f6e 0a0a 4750  ummarization..GP
+00002a80: 5420 6578 6365 6c73 2061 7420 7065 7266  T excels at perf
+00002a90: 6f72 6d69 6e67 2073 756d 6d61 7269 7a61  orming summariza
+00002aa0: 7469 6f6e 2074 6173 6b73 2e20 5468 6572  tion tasks. Ther
+00002ab0: 6566 6f72 652c 2077 6520 7072 6f76 6964  efore, we provid
+00002ac0: 6520 6047 5054 5375 6d6d 6172 697a 6572  e `GPTSummarizer
+00002ad0: 6020 7468 6174 2063 616e 2062 6520 7573  ` that can be us
+00002ae0: 6564 2062 6f74 6820 6173 2073 7461 6e64  ed both as stand
+00002af0: 2d61 6c6f 6e65 2065 7374 696d 6174 6f72  -alone estimator
+00002b00: 2c20 6f72 2061 7320 6120 7072 6570 726f  , or as a prepro
+00002b10: 6365 7373 6f72 2028 696e 2074 6869 7320  cessor (in this 
+00002b20: 6361 7365 2077 6520 6361 6e20 6d61 6b65  case we can make
+00002b30: 2061 6e20 616e 616c 6f67 7920 7769 7468   an analogy with
+00002b40: 2061 2064 696d 656e 7369 6f6e 616c 6974   a dimensionalit
+00002b50: 7920 7265 6475 6374 696f 6e20 7072 6570  y reduction prep
+00002b60: 726f 6365 7373 6f72 292e 0a0a 4578 616d  rocessor)...Exam
+00002b70: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00002b80: 6672 6f6d 2073 6b6c 6c6d 2e70 7265 7072  from skllm.prepr
+00002b90: 6f63 6573 7369 6e67 2069 6d70 6f72 7420  ocessing import 
+00002ba0: 4750 5453 756d 6d61 7269 7a65 720a 6672  GPTSummarizer.fr
+00002bb0: 6f6d 2073 6b6c 6c6d 2e64 6174 6173 6574  om skllm.dataset
+00002bc0: 7320 696d 706f 7274 2067 6574 5f73 756d  s import get_sum
+00002bd0: 6d61 7269 7a61 7469 6f6e 5f64 6174 6173  marization_datas
+00002be0: 6574 0a0a 5820 3d20 6765 745f 7375 6d6d  et..X = get_summ
+00002bf0: 6172 697a 6174 696f 6e5f 6461 7461 7365  arization_datase
+00002c00: 7428 290a 7320 3d20 4750 5453 756d 6d61  t().s = GPTSumma
+00002c10: 7269 7a65 7228 6f70 656e 6169 5f6d 6f64  rizer(openai_mod
+00002c20: 656c 3d22 6770 742d 332e 352d 7475 7262  el="gpt-3.5-turb
+00002c30: 6f22 2c20 6d61 785f 776f 7264 733d 3135  o", max_words=15
+00002c40: 290a 7375 6d6d 6172 6965 7320 3d20 732e  ).summaries = s.
+00002c50: 6669 745f 7472 616e 7366 6f72 6d28 5829  fit_transform(X)
+00002c60: 0a60 6060 0a0a 506c 6561 7365 2062 6520  .```..Please be 
+00002c70: 6177 6172 6520 7468 6174 2074 6865 2060  aware that the `
+00002c80: 6d61 785f 776f 7264 7360 2068 7970 6572  max_words` hyper
+00002c90: 7061 7261 6d65 7465 7220 7365 7473 2061  parameter sets a
+00002ca0: 2073 6f66 7420 6c69 6d69 742c 2077 6869   soft limit, whi
+00002cb0: 6368 2069 7320 6e6f 7420 7374 7269 6374  ch is not strict
+00002cc0: 6c79 2065 6e66 6f72 6365 6420 6f75 7473  ly enforced outs
+00002cd0: 6964 6520 6f66 2074 6865 2070 726f 6d70  ide of the promp
+00002ce0: 742e 2054 6865 7265 666f 7265 2c20 696e  t. Therefore, in
+00002cf0: 2073 6f6d 6520 6361 7365 732c 2074 6865   some cases, the
+00002d00: 2061 6374 7561 6c20 6e75 6d62 6572 206f   actual number o
+00002d10: 6620 776f 7264 7320 6d69 6768 7420 6265  f words might be
+00002d20: 2073 6c69 6768 746c 7920 6869 6768 6572   slightly higher
+00002d30: 2e0a 0a49 7420 6973 2070 6f73 7369 626c  ...It is possibl
+00002d40: 6520 746f 2067 656e 6572 6174 6520 6120  e to generate a 
+00002d50: 7375 6d6d 6172 792c 2065 6d70 6861 7369  summary, emphasi
+00002d60: 7a69 6e67 2061 2073 7065 6369 6669 6320  zing a specific 
+00002d70: 636f 6e63 6570 742c 2062 7920 7072 6f76  concept, by prov
+00002d80: 6964 696e 6720 616e 206f 7074 696f 6e61  iding an optiona
+00002d90: 6c20 7061 7261 6d65 7465 7220 6066 6f63  l parameter `foc
+00002da0: 7573 603a 0a0a 6060 6070 7974 686f 6e0a  us`:..```python.
+00002db0: 7320 3d20 4750 5453 756d 6d61 7269 7a65  s = GPTSummarize
+00002dc0: 7228 6f70 656e 6169 5f6d 6f64 656c 3d22  r(openai_model="
+00002dd0: 6770 742d 332e 352d 7475 7262 6f22 2c20  gpt-3.5-turbo", 
+00002de0: 6d61 785f 776f 7264 733d 3135 2c20 666f  max_words=15, fo
+00002df0: 6375 733d 2261 7070 6c65 7322 290a 6060  cus="apples").``
+00002e00: 600a 0a23 2323 2054 6578 7420 5472 616e  `..### Text Tran
+00002e10: 736c 6174 696f 6e0a 0a47 5054 206d 6f64  slation..GPT mod
+00002e20: 656c 7320 6861 7665 2064 656d 6f6e 7374  els have demonst
+00002e30: 7261 7465 6420 7468 6569 7220 6566 6665  rated their effe
+00002e40: 6374 6976 656e 6573 7320 696e 2074 7261  ctiveness in tra
+00002e50: 6e73 6c61 7469 6f6e 2074 6173 6b73 2062  nslation tasks b
+00002e60: 7920 6765 6e65 7261 7469 6e67 2061 6363  y generating acc
+00002e70: 7572 6174 6520 7472 616e 736c 6174 696f  urate translatio
+00002e80: 6e73 2061 6372 6f73 7320 7661 7269 6f75  ns across variou
+00002e90: 7320 6c61 6e67 7561 6765 732e 2054 6875  s languages. Thu
+00002ea0: 732c 2077 6520 6164 6465 6420 6047 5054  s, we added `GPT
+00002eb0: 5472 616e 736c 6174 6f72 6020 7468 6174  Translator` that
+00002ec0: 2061 6c6c 6f77 7320 7472 616e 736c 6174   allows translat
+00002ed0: 696e 6720 616e 2061 7262 6974 7261 7479  ing an arbitraty
+00002ee0: 2074 6578 7420 696e 746f 2061 206c 616e   text into a lan
+00002ef0: 6775 6167 6520 6f66 2069 6e74 6572 6573  guage of interes
+00002f00: 742e 0a0a 4578 616d 706c 653a 0a0a 6060  t...Example:..``
+00002f10: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+00002f20: 6c6d 2e70 7265 7072 6f63 6573 7369 6e67  lm.preprocessing
+00002f30: 2069 6d70 6f72 7420 4750 5454 7261 6e73   import GPTTrans
+00002f40: 6c61 746f 720a 6672 6f6d 2073 6b6c 6c6d  lator.from skllm
+00002f50: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00002f60: 2067 6574 5f74 7261 6e73 6c61 7469 6f6e   get_translation
+00002f70: 5f64 6174 6173 6574 0a0a 5820 3d20 6765  _dataset..X = ge
+00002f80: 745f 7472 616e 736c 6174 696f 6e5f 6461  t_translation_da
+00002f90: 7461 7365 7428 290a 7420 3d20 4750 5454  taset().t = GPTT
+00002fa0: 7261 6e73 6c61 746f 7228 6f70 656e 6169  ranslator(openai
+00002fb0: 5f6d 6f64 656c 3d22 6770 742d 332e 352d  _model="gpt-3.5-
+00002fc0: 7475 7262 6f22 2c20 6f75 7470 7574 5f6c  turbo", output_l
+00002fd0: 616e 6775 6167 653d 2245 6e67 6c69 7368  anguage="English
+00002fe0: 2229 0a74 7261 6e73 6c61 7465 645f 7465  ").translated_te
+00002ff0: 7874 203d 2074 2e66 6974 5f74 7261 6e73  xt = t.fit_trans
+00003000: 666f 726d 2858 290a 6060 600a 0a         form(X).```..
```

### Comparing `scikit-llm-0.2.0/README.md` & `scikit-llm-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,631 +25,711 @@
 00000180: 7468 6520 7072 6f6a 6563 7420 696e 2074  the project in t
 00000190: 6865 2066 6f6c 6c6f 7769 6e67 2077 6179  he following way
 000001a0: 733a 0a0a 2d20 e2ad 9020 5374 6172 2053  s:..- ... Star S
 000001b0: 6369 6b69 742d 4c4c 4d20 6f6e 2047 6974  cikit-LLM on Git
 000001c0: 4875 6220 2863 6c69 636b 2074 6865 2073  Hub (click the s
 000001d0: 7461 7220 6275 7474 6f6e 2069 6e20 7468  tar button in th
 000001e0: 6520 746f 7020 7269 6768 7420 636f 726e  e top right corn
-000001f0: 6572 290a 2d20 f09f 90a6 2043 6865 636b  er).- .... Check
-00000200: 206f 7574 206f 7572 2072 656c 6174 6564   out our related
-00000210: 2070 726f 6a65 6374 202d 205b 4661 6c63   project - [Falc
-00000220: 6f6e 2041 7574 6f4d 4c5d 2868 7474 7073  on AutoML](https
-00000230: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4b  ://github.com/OK
-00000240: 5541 312f 6661 6c63 6f6e 290a 2d20 f09f  UA1/falcon).- ..
-00000250: 92a1 2050 726f 7669 6465 2079 6f75 7220  .. Provide your 
-00000260: 6665 6564 6261 636b 206f 7220 7072 6f70  feedback or prop
-00000270: 6f73 6520 6964 6561 7320 696e 2074 6865  ose ideas in the
-00000280: 205b 6973 7375 6573 5d28 6874 7470 733a   [issues](https:
-00000290: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7279  //github.com/iry
-000002a0: 6e61 2d6b 6f6e 6472 2f73 6369 6b69 742d  na-kondr/scikit-
-000002b0: 6c6c 6d2f 6973 7375 6573 2920 7365 6374  llm/issues) sect
-000002c0: 696f 6e20 6f72 205b 4469 7363 6f72 645d  ion or [Discord]
-000002d0: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
-000002e0: 2e67 672f 5944 4162 7775 574b 3756 290a  .gg/YDAbwuWK7V).
-000002f0: 2d20 f09f 9497 2050 6f73 7420 6162 6f75  - .... Post abou
-00000300: 7420 5363 696b 6974 2d4c 4c4d 206f 6e20  t Scikit-LLM on 
-00000310: 4c69 6e6b 6564 496e 206f 7220 6f74 6865  LinkedIn or othe
-00000320: 7220 706c 6174 666f 726d 730a 0a23 2320  r platforms..## 
-00000330: 446f 6375 6d65 6e74 6174 696f 6e20 f09f  Documentation ..
-00000340: 939a 0a0a 2323 2320 436f 6e66 6967 7572  ....### Configur
-00000350: 696e 6720 4f70 656e 4149 2041 5049 204b  ing OpenAI API K
-00000360: 6579 0a0a 4174 2074 6865 206d 6f6d 656e  ey..At the momen
-00000370: 7420 7468 6520 6d61 6a6f 7269 7479 206f  t the majority o
-00000380: 6620 7468 6520 5363 696b 6974 2d4c 4c4d  f the Scikit-LLM
-00000390: 2065 7374 696d 6174 6f72 7320 6172 6520   estimators are 
-000003a0: 6f6e 6c79 2063 6f6d 7061 7469 626c 6520  only compatible 
-000003b0: 7769 7468 2073 6f6d 6520 6f66 2074 6865  with some of the
-000003c0: 204f 7065 6e41 4920 6d6f 6465 6c73 2e20   OpenAI models. 
-000003d0: 4865 6e63 652c 2061 2075 7365 722d 7072  Hence, a user-pr
-000003e0: 6f76 6964 6564 204f 7065 6e41 4920 4150  ovided OpenAI AP
-000003f0: 4920 6b65 7920 6973 2072 6571 7569 7265  I key is require
-00000400: 642e 0a0a 6060 6070 7974 686f 6e0a 6672  d...```python.fr
-00000410: 6f6d 2073 6b6c 6c6d 2e63 6f6e 6669 6720  om skllm.config 
-00000420: 696d 706f 7274 2053 4b4c 4c4d 436f 6e66  import SKLLMConf
-00000430: 6967 0a0a 534b 4c4c 4d43 6f6e 6669 672e  ig..SKLLMConfig.
-00000440: 7365 745f 6f70 656e 6169 5f6b 6579 2822  set_openai_key("
-00000450: 3c59 4f55 525f 4b45 593e 2229 0a53 4b4c  <YOUR_KEY>").SKL
-00000460: 4c4d 436f 6e66 6967 2e73 6574 5f6f 7065  LMConfig.set_ope
-00000470: 6e61 695f 6f72 6728 223c 594f 5552 5f4f  nai_org("<YOUR_O
-00000480: 5247 414e 4953 4154 494f 4e3e 2229 0a60  RGANISATION>").`
-00000490: 6060 0a0a 2a2a 496d 706f 7274 616e 7420  ``..**Important 
-000004a0: 6e6f 7469 6365 3a2a 2a0a 0a2d 2049 6620  notice:**..- If 
-000004b0: 796f 7520 6861 7665 2061 2066 7265 6520  you have a free 
-000004c0: 7472 6961 6c20 4f70 656e 4149 2061 6363  trial OpenAI acc
-000004d0: 6f75 6e74 2c20 7468 6520 5b72 6174 6520  ount, the [rate 
-000004e0: 6c69 6d69 7473 5d28 6874 7470 733a 2f2f  limits](https://
-000004f0: 706c 6174 666f 726d 2e6f 7065 6e61 692e  platform.openai.
-00000500: 636f 6d2f 646f 6373 2f67 7569 6465 732f  com/docs/guides/
-00000510: 7261 7465 2d6c 696d 6974 732f 6f76 6572  rate-limits/over
-00000520: 7669 6577 2920 6172 6520 6e6f 7420 7375  view) are not su
-00000530: 6666 6963 6965 6e74 2028 7370 6563 6966  fficient (specif
-00000540: 6963 616c 6c79 2033 2072 6571 7565 7374  ically 3 request
-00000550: 7320 7065 7220 6d69 6e75 7465 292e 2050  s per minute). P
-00000560: 6c65 6173 6520 7377 6974 6368 2074 6f20  lease switch to 
-00000570: 7468 6520 2270 6179 2061 7320 796f 7520  the "pay as you 
-00000580: 676f 2220 706c 616e 2066 6972 7374 2e0a  go" plan first..
-00000590: 2d20 5768 656e 2063 616c 6c69 6e67 2060  - When calling `
-000005a0: 534b 4c4c 4d43 6f6e 6669 672e 7365 745f  SKLLMConfig.set_
-000005b0: 6f70 656e 6169 5f6f 7267 602c 2079 6f75  openai_org`, you
-000005c0: 2068 6176 6520 746f 2070 726f 7669 6465   have to provide
-000005d0: 2079 6f75 7220 6f72 6761 6e69 7a61 7469   your organizati
-000005e0: 6f6e 2049 4420 616e 6420 2a2a 4e4f 542a  on ID and **NOT*
-000005f0: 2a20 7468 6520 6e61 6d65 2e20 596f 7520  * the name. You 
-00000600: 6361 6e20 6669 6e64 2079 6f75 7220 4944  can find your ID
-00000610: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-00000620: 706c 6174 666f 726d 2e6f 7065 6e61 692e  platform.openai.
-00000630: 636f 6d2f 6163 636f 756e 742f 6f72 672d  com/account/org-
-00000640: 7365 7474 696e 6773 292e 0a0a 2323 2320  settings)...### 
-00000650: 5573 696e 6720 4750 5434 414c 4c0a 0a49  Using GPT4ALL..I
-00000660: 6e20 6164 6469 7469 6f6e 2074 6f20 4f70  n addition to Op
-00000670: 656e 4149 2c20 736f 6d65 206f 6620 7468  enAI, some of th
-00000680: 6520 6d6f 6465 6c73 2063 616e 2075 7365  e models can use
-00000690: 205b 6770 7434 616c 6c5d 2868 7474 7073   [gpt4all](https
-000006a0: 3a2f 2f67 7074 3461 6c6c 2e69 6f2f 696e  ://gpt4all.io/in
-000006b0: 6465 782e 6874 6d6c 2920 6173 2061 2062  dex.html) as a b
-000006c0: 6163 6b65 6e64 2e0a 0a2a 2a54 6869 7320  ackend...**This 
-000006d0: 6665 6174 7572 6520 6973 2063 6f6e 7369  feature is consi
-000006e0: 6465 7265 6420 6869 676c 7920 6578 7065  dered higly expe
-000006f0: 7269 6d65 6e74 616c 212a 2a0a 0a49 6e20  rimental!**..In 
-00000700: 6f72 6465 7220 746f 2075 7365 2067 7074  order to use gpt
-00000710: 3461 6c6c 2c20 796f 7520 6e65 6564 2074  4all, you need t
-00000720: 6f20 696e 7374 616c 6c20 7468 6520 636f  o install the co
-00000730: 7272 6573 706f 6e64 696e 6720 7375 626d  rresponding subm
-00000740: 6f64 756c 653a 0a0a 6060 6062 6173 680a  odule:..```bash.
-00000750: 7069 7020 696e 7374 616c 6c20 2273 6369  pip install "sci
-00000760: 6b69 742d 6c6c 6d5b 6770 7434 616c 6c5d  kit-llm[gpt4all]
-00000770: 220a 6060 600a 0a49 6e20 6f72 6465 7220  ".```..In order 
-00000780: 746f 2073 7769 7463 6820 6672 6f6d 204f  to switch from O
-00000790: 7065 6e41 4920 746f 2047 5054 3441 4c4c  penAI to GPT4ALL
-000007a0: 206d 6f64 656c 2c20 7369 6d70 6c79 2070   model, simply p
-000007b0: 726f 7669 6465 2061 2073 7472 696e 6720  rovide a string 
-000007c0: 6f66 2074 6865 2066 6f72 6d61 7420 6067  of the format `g
-000007d0: 7074 3461 6c6c 3a3a 3c6d 6f64 656c 5f6e  pt4all::<model_n
-000007e0: 616d 653e 6020 6173 2061 6e20 6172 6775  ame>` as an argu
-000007f0: 6d65 6e74 2e20 5768 696c 6520 7468 6520  ment. While the 
-00000800: 6d6f 6465 6c20 7275 6e73 2063 6f6d 706c  model runs compl
-00000810: 6574 656c 7920 6c6f 6361 6c6c 792c 2074  etely locally, t
-00000820: 6865 2065 7374 696d 6174 6f72 2073 7469  he estimator sti
-00000830: 6c6c 2074 7265 6174 7320 6974 2061 7320  ll treats it as 
-00000840: 616e 204f 7065 6e41 4920 656e 6470 6f69  an OpenAI endpoi
-00000850: 6e74 2061 6e64 2077 696c 6c20 7472 7920  nt and will try 
-00000860: 746f 2063 6865 636b 2074 6861 7420 7468  to check that th
-00000870: 6520 4150 4920 6b65 7920 6973 2070 7265  e API key is pre
-00000880: 7365 6e74 2e20 596f 7520 6361 6e20 7072  sent. You can pr
-00000890: 6f76 6964 6520 616e 7920 7374 7269 6e67  ovide any string
-000008a0: 2061 7320 6120 6b65 792e 0a0a 6060 6070   as a key...```p
-000008b0: 7974 686f 6e0a 534b 4c4c 4d43 6f6e 6669  ython.SKLLMConfi
-000008c0: 672e 7365 745f 6f70 656e 6169 5f6b 6579  g.set_openai_key
-000008d0: 2822 616e 7920 7374 7269 6e67 2229 0a53  ("any string").S
-000008e0: 4b4c 4c4d 436f 6e66 6967 2e73 6574 5f6f  KLLMConfig.set_o
-000008f0: 7065 6e61 695f 6f72 6728 2261 6e79 2073  penai_org("any s
-00000900: 7472 696e 6722 290a 0a5a 6572 6f53 686f  tring")..ZeroSho
-00000910: 7447 5054 436c 6173 7369 6669 6572 286f  tGPTClassifier(o
-00000920: 7065 6e61 695f 6d6f 6465 6c3d 2267 7074  penai_model="gpt
-00000930: 3461 6c6c 3a3a 6767 6d6c 2d67 7074 3461  4all::ggml-gpt4a
-00000940: 6c6c 2d6a 2d76 312e 332d 6772 6f6f 7679  ll-j-v1.3-groovy
-00000950: 2229 0a60 6060 0a0a 5768 656e 2072 756e  ").```..When run
-00000960: 6e69 6e67 2066 6f72 2074 6865 2066 6972  ning for the fir
-00000970: 7374 2074 696d 652c 2074 6865 206d 6f64  st time, the mod
-00000980: 656c 2066 696c 6520 7769 6c6c 2062 6520  el file will be 
-00000990: 646f 776e 6c6f 6164 6564 2061 7574 6f6d  downloaded autom
-000009a0: 6174 6961 6c6c 792e 0a0a 4174 2074 6865  atially...At the
-000009b0: 206d 6f6d 656e 7420 6f6e 6c79 2074 6865   moment only the
-000009c0: 2066 6f6c 6c6f 7769 6e67 2065 7374 696d   following estim
-000009d0: 6174 6f72 7320 7375 7070 6f72 7420 6770  ators support gp
-000009e0: 7434 616c 6c20 6173 2061 2062 6163 6b65  t4all as a backe
-000009f0: 6e64 3a0a 0a2d 2060 5a65 726f 5368 6f74  nd:..- `ZeroShot
-00000a00: 4750 5443 6c61 7373 6966 6965 7260 0a2d  GPTClassifier`.-
-00000a10: 2060 4d75 6c74 694c 6162 656c 5a65 726f   `MultiLabelZero
-00000a20: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
-00000a30: 7260 0a2d 2060 4665 7753 686f 7447 5054  r`.- `FewShotGPT
-00000a40: 436c 6173 7369 6669 6572 600a 0a57 6865  Classifier`..Whe
-00000a50: 6e20 7573 696e 6720 6770 7434 616c 6c20  n using gpt4all 
-00000a60: 706c 6561 7365 206b 6565 7020 7468 6520  please keep the 
-00000a70: 666f 6c6c 6f77 696e 6720 696e 206d 696e  following in min
-00000a80: 643a 0a0a 312e 204e 6f74 2061 6c6c 2067  d:..1. Not all g
-00000a90: 7074 3461 6c6c 206d 6f64 656c 7320 6172  pt4all models ar
-00000aa0: 6520 636f 6d6d 6572 6369 616c 6c79 206c  e commercially l
-00000ab0: 6963 656e 7361 626c 652c 2070 6c65 6173  icensable, pleas
-00000ac0: 6520 636f 6e73 756c 7420 6770 7434 616c  e consult gpt4al
-00000ad0: 6c20 7765 6273 6974 6520 666f 7220 6d6f  l website for mo
-00000ae0: 7265 2064 6574 6169 6c73 2e0a 322e 2054  re details..2. T
-00000af0: 6865 2061 6363 7572 6163 7920 6f66 2074  he accuracy of t
-00000b00: 6865 206d 6f64 656c 7320 6d61 7920 6265  he models may be
-00000b10: 206d 7563 6820 6c6f 7765 7220 636f 6d70   much lower comp
-00000b20: 6172 6564 2074 6f20 6f6e 6573 2070 726f  ared to ones pro
-00000b30: 7669 6465 6420 6279 204f 7065 6e41 4920  vided by OpenAI 
-00000b40: 2865 7370 6563 6961 6c6c 7920 6770 742d  (especially gpt-
-00000b50: 3429 2e0a 332e 204e 6f74 2061 6c6c 206f  4)..3. Not all o
-00000b60: 6620 7468 6520 6176 6169 6c61 626c 6520  f the available 
-00000b70: 6d6f 6465 6c73 2077 6572 6520 7465 7374  models were test
-00000b80: 6564 2c20 736f 6d65 206d 6179 206e 6f74  ed, some may not
-00000b90: 2077 6f72 6b20 7769 7468 2073 6369 6b69   work with sciki
-00000ba0: 742d 6c6c 6d20 6174 2061 6c6c 2e0a 0a23  t-llm at all...#
-00000bb0: 2323 205a 6572 6f2d 5368 6f74 2054 6578  ## Zero-Shot Tex
-00000bc0: 7420 436c 6173 7369 6669 6361 7469 6f6e  t Classification
-00000bd0: 0a0a 4f6e 6520 6f66 2074 6865 2070 6f77  ..One of the pow
-00000be0: 6572 6675 6c20 4368 6174 4750 5420 6665  erful ChatGPT fe
-00000bf0: 6174 7572 6573 2069 7320 7468 6520 6162  atures is the ab
-00000c00: 696c 6974 7920 746f 2070 6572 666f 726d  ility to perform
-00000c10: 2074 6578 7420 636c 6173 7369 6669 6361   text classifica
-00000c20: 7469 6f6e 2077 6974 686f 7574 2062 6569  tion without bei
-00000c30: 6e67 2072 652d 7472 6169 6e65 642e 2046  ng re-trained. F
-00000c40: 6f72 2074 6861 742c 2074 6865 206f 6e6c  or that, the onl
-00000c50: 7920 7265 7175 6972 656d 656e 7420 6973  y requirement is
-00000c60: 2074 6861 7420 7468 6520 6c61 6265 6c73   that the labels
-00000c70: 206d 7573 7420 6265 2064 6573 6372 6970   must be descrip
-00000c80: 7469 7665 2e0a 0a57 6520 7072 6f76 6964  tive...We provid
-00000c90: 6520 6120 636c 6173 7320 605a 6572 6f53  e a class `ZeroS
-00000ca0: 686f 7447 5054 436c 6173 7369 6669 6572  hotGPTClassifier
-00000cb0: 6020 7468 6174 2061 6c6c 6f77 7320 746f  ` that allows to
-00000cc0: 2063 7265 6174 6520 7375 6368 2061 206d   create such a m
-00000cd0: 6f64 656c 2061 7320 6120 7265 6775 6c61  odel as a regula
-00000ce0: 7220 7363 696b 6974 2d6c 6561 726e 2063  r scikit-learn c
-00000cf0: 6c61 7373 6966 6965 722e 0a0a 4578 616d  lassifier...Exam
-00000d00: 706c 6520 313a 2054 7261 696e 696e 6720  ple 1: Training 
-00000d10: 6173 2061 2072 6567 756c 6172 2063 6c61  as a regular cla
-00000d20: 7373 6966 6965 720a 0a60 6060 7079 7468  ssifier..```pyth
-00000d30: 6f6e 0a66 726f 6d20 736b 6c6c 6d20 696d  on.from skllm im
-00000d40: 706f 7274 205a 6572 6f53 686f 7447 5054  port ZeroShotGPT
-00000d50: 436c 6173 7369 6669 6572 0a66 726f 6d20  Classifier.from 
-00000d60: 736b 6c6c 6d2e 6461 7461 7365 7473 2069  skllm.datasets i
-00000d70: 6d70 6f72 7420 6765 745f 636c 6173 7369  mport get_classi
-00000d80: 6669 6361 7469 6f6e 5f64 6174 6173 6574  fication_dataset
-00000d90: 0a0a 2320 6465 6d6f 2073 656e 7469 6d65  ..# demo sentime
-00000da0: 6e74 2061 6e61 6c79 7369 7320 6461 7461  nt analysis data
-00000db0: 7365 740a 2320 6c61 6265 6c73 3a20 706f  set.# labels: po
-00000dc0: 7369 7469 7665 2c20 6e65 6761 7469 7665  sitive, negative
-00000dd0: 2c20 6e65 7574 7261 6c0a 582c 2079 203d  , neutral.X, y =
-00000de0: 2067 6574 5f63 6c61 7373 6966 6963 6174   get_classificat
-00000df0: 696f 6e5f 6461 7461 7365 7428 290a 0a63  ion_dataset()..c
-00000e00: 6c66 203d 205a 6572 6f53 686f 7447 5054  lf = ZeroShotGPT
-00000e10: 436c 6173 7369 6669 6572 286f 7065 6e61  Classifier(opena
-00000e20: 695f 6d6f 6465 6c3d 2267 7074 2d33 2e35  i_model="gpt-3.5
-00000e30: 2d74 7572 626f 2229 0a63 6c66 2e66 6974  -turbo").clf.fit
-00000e40: 2858 2c20 7929 0a6c 6162 656c 7320 3d20  (X, y).labels = 
-00000e50: 636c 662e 7072 6564 6963 7428 5829 0a60  clf.predict(X).`
-00000e60: 6060 0a0a 5363 696b 6974 2d4c 4c4d 2077  ``..Scikit-LLM w
-00000e70: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
-00000e80: 7920 7175 6572 7920 7468 6520 4f70 656e  y query the Open
-00000e90: 4149 2041 5049 2061 6e64 2074 7261 6e73  AI API and trans
-00000ea0: 666f 726d 2074 6865 2072 6573 706f 6e73  form the respons
-00000eb0: 6520 696e 746f 2061 2072 6567 756c 6172  e into a regular
-00000ec0: 206c 6973 7420 6f66 206c 6162 656c 732e   list of labels.
-00000ed0: 0a0a 4164 6469 7469 6f6e 616c 6c79 2c20  ..Additionally, 
-00000ee0: 5363 696b 6974 2d4c 4c4d 2077 696c 6c20  Scikit-LLM will 
-00000ef0: 656e 7375 7265 2074 6861 7420 7468 6520  ensure that the 
-00000f00: 6f62 7461 696e 6564 2072 6573 706f 6e73  obtained respons
-00000f10: 6520 636f 6e74 6169 6e73 2061 2076 616c  e contains a val
-00000f20: 6964 206c 6162 656c 2e20 4966 2074 6869  id label. If thi
-00000f30: 7320 6973 206e 6f74 2074 6865 2063 6173  s is not the cas
-00000f40: 652c 2061 206c 6162 656c 2077 696c 6c20  e, a label will 
-00000f50: 6265 2073 656c 6563 7465 6420 7261 6e64  be selected rand
-00000f60: 6f6d 6c79 2028 6c61 6265 6c20 7072 6f62  omly (label prob
-00000f70: 6162 696c 6974 6965 7320 6172 6520 7072  abilities are pr
-00000f80: 6f70 6f72 7469 6f6e 616c 2074 6f20 6c61  oportional to la
-00000f90: 6265 6c20 6f63 6375 7272 656e 6365 7320  bel occurrences 
-00000fa0: 696e 2074 6865 2074 7261 696e 696e 6720  in the training 
-00000fb0: 7365 7429 2e0a 0a45 7861 6d70 6c65 2032  set)...Example 2
-00000fc0: 3a20 5472 6169 6e69 6e67 2077 6974 686f  : Training witho
-00000fd0: 7574 206c 6162 656c 6564 2064 6174 610a  ut labeled data.
-00000fe0: 0a53 696e 6365 2074 6865 2074 7261 696e  .Since the train
-00000ff0: 696e 6720 6461 7461 2069 7320 6e6f 7420  ing data is not 
-00001000: 7374 7269 6374 6c79 2072 6571 7569 7265  strictly require
-00001010: 642c 2069 7420 6361 6e20 6265 2066 756c  d, it can be ful
-00001020: 6c79 206f 6d6d 6974 6564 2e20 5468 6520  ly ommited. The 
-00001030: 6f6e 6c79 2074 6869 6e67 2074 6861 7420  only thing that 
-00001040: 6861 7320 746f 2062 6520 7072 6f76 6964  has to be provid
-00001050: 6564 2069 7320 7468 6520 6c69 7374 206f  ed is the list o
-00001060: 6620 6361 6e64 6964 6174 6520 6c61 6265  f candidate labe
-00001070: 6c73 2e0a 0a60 6060 7079 7468 6f6e 0a66  ls...```python.f
-00001080: 726f 6d20 736b 6c6c 6d20 696d 706f 7274  rom skllm import
-00001090: 205a 6572 6f53 686f 7447 5054 436c 6173   ZeroShotGPTClas
-000010a0: 7369 6669 6572 0a66 726f 6d20 736b 6c6c  sifier.from skll
-000010b0: 6d2e 6461 7461 7365 7473 2069 6d70 6f72  m.datasets impor
-000010c0: 7420 6765 745f 636c 6173 7369 6669 6361  t get_classifica
-000010d0: 7469 6f6e 5f64 6174 6173 6574 0a0a 582c  tion_dataset..X,
-000010e0: 205f 203d 2067 6574 5f63 6c61 7373 6966   _ = get_classif
-000010f0: 6963 6174 696f 6e5f 6461 7461 7365 7428  ication_dataset(
-00001100: 290a 0a63 6c66 203d 205a 6572 6f53 686f  )..clf = ZeroSho
-00001110: 7447 5054 436c 6173 7369 6669 6572 2829  tGPTClassifier()
-00001120: 0a63 6c66 2e66 6974 284e 6f6e 652c 205b  .clf.fit(None, [
-00001130: 2270 6f73 6974 6976 6522 2c20 226e 6567  "positive", "neg
-00001140: 6174 6976 6522 2c20 226e 6575 7472 616c  ative", "neutral
-00001150: 225d 290a 6c61 6265 6c73 203d 2063 6c66  "]).labels = clf
-00001160: 2e70 7265 6469 6374 2858 290a 6060 600a  .predict(X).```.
-00001170: 0a2a 2a4e 6f74 653a 2a2a 2075 6e6c 696b  .**Note:** unlik
-00001180: 6520 696e 2061 2074 7970 6963 616c 2073  e in a typical s
-00001190: 7570 6572 7669 7365 6420 7365 7474 696e  upervised settin
-000011a0: 672c 2074 6865 2070 6572 666f 726d 616e  g, the performan
-000011b0: 6365 206f 6620 6120 7a65 726f 2d73 686f  ce of a zero-sho
-000011c0: 7420 636c 6173 7369 6669 6572 2067 7265  t classifier gre
-000011d0: 6174 6c79 2064 6570 656e 6473 206f 6e20  atly depends on 
-000011e0: 686f 7720 7468 6520 6c61 6265 6c20 6974  how the label it
-000011f0: 7365 6c66 2069 7320 7374 7275 6374 7572  self is structur
-00001200: 6564 2e20 4974 2068 6173 2074 6f20 6265  ed. It has to be
-00001210: 2065 7870 7265 7373 6564 2069 6e20 6e61   expressed in na
-00001220: 7475 7261 6c20 6c61 6e67 7561 6765 2c20  tural language, 
-00001230: 6265 2064 6573 6372 6970 7469 7665 2061  be descriptive a
-00001240: 6e64 2073 656c 662d 6578 706c 616e 6174  nd self-explanat
-00001250: 6f72 792e 2046 6f72 2065 7861 6d70 6c65  ory. For example
-00001260: 2c20 696e 2074 6865 2070 7265 7669 6f75  , in the previou
-00001270: 7320 7365 6d61 6e74 6963 2063 6c61 7373  s semantic class
-00001280: 6966 6963 6174 696f 6e20 7461 736b 2c20  ification task, 
-00001290: 6974 2063 6f75 6c64 2062 6520 6265 6e65  it could be bene
-000012a0: 6669 6369 616c 2074 6f20 7472 616e 7366  ficial to transf
-000012b0: 6f72 6d20 6120 6c61 6265 6c20 6672 6f6d  orm a label from
-000012c0: 2060 223c 7365 6d61 6e74 6963 733e 2260   `"<semantics>"`
-000012d0: 2074 6f20 6022 7468 6520 7365 6d61 6e74   to `"the semant
-000012e0: 6963 7320 6f66 2074 6865 2070 726f 7669  ics of the provi
-000012f0: 6465 6420 7465 7874 2069 7320 3c73 656d  ded text is <sem
-00001300: 616e 7469 6373 3e22 602e 0a0a 2323 2320  antics>"`...### 
-00001310: 4d75 6c74 692d 4c61 6265 6c20 5a65 726f  Multi-Label Zero
-00001320: 2d53 686f 7420 5465 7874 2043 6c61 7373  -Shot Text Class
-00001330: 6966 6963 6174 696f 6e0a 0a57 6974 6820  ification..With 
-00001340: 6120 636c 6173 7320 604d 756c 7469 4c61  a class `MultiLa
-00001350: 6265 6c5a 6572 6f53 686f 7447 5054 436c  belZeroShotGPTCl
-00001360: 6173 7369 6669 6572 6020 6974 2069 7320  assifier` it is 
-00001370: 706f 7373 6962 6c65 2074 6f20 7065 7266  possible to perf
-00001380: 6f72 6d20 7468 6520 636c 6173 7369 6669  orm the classifi
-00001390: 6361 7469 6f6e 2069 6e20 6d75 6c74 692d  cation in multi-
-000013a0: 6c61 6265 6c20 7365 7474 696e 672c 2077  label setting, w
-000013b0: 6869 6368 206d 6561 6e73 2074 6861 7420  hich means that 
-000013c0: 6561 6368 2073 616d 706c 6520 6d69 6768  each sample migh
-000013d0: 7420 6265 2061 7373 6967 6e65 6420 746f  t be assigned to
-000013e0: 206f 6e65 206f 7220 7365 7665 7261 6c20   one or several 
-000013f0: 6469 7374 696e 6374 2063 6c61 7373 6573  distinct classes
-00001400: 2e0a 0a45 7861 6d70 6c65 3a0a 0a60 6060  ...Example:..```
-00001410: 7079 7468 6f6e 0a66 726f 6d20 736b 6c6c  python.from skll
-00001420: 6d20 696d 706f 7274 204d 756c 7469 4c61  m import MultiLa
-00001430: 6265 6c5a 6572 6f53 686f 7447 5054 436c  belZeroShotGPTCl
-00001440: 6173 7369 6669 6572 0a66 726f 6d20 736b  assifier.from sk
-00001450: 6c6c 6d2e 6461 7461 7365 7473 2069 6d70  llm.datasets imp
-00001460: 6f72 7420 6765 745f 6d75 6c74 696c 6162  ort get_multilab
-00001470: 656c 5f63 6c61 7373 6966 6963 6174 696f  el_classificatio
-00001480: 6e5f 6461 7461 7365 740a 0a58 2c20 7920  n_dataset..X, y 
-00001490: 3d20 6765 745f 6d75 6c74 696c 6162 656c  = get_multilabel
-000014a0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-000014b0: 6461 7461 7365 7428 290a 0a63 6c66 203d  dataset()..clf =
-000014c0: 204d 756c 7469 4c61 6265 6c5a 6572 6f53   MultiLabelZeroS
-000014d0: 686f 7447 5054 436c 6173 7369 6669 6572  hotGPTClassifier
-000014e0: 286d 6178 5f6c 6162 656c 733d 3329 0a63  (max_labels=3).c
-000014f0: 6c66 2e66 6974 2858 2c20 7929 0a6c 6162  lf.fit(X, y).lab
-00001500: 656c 7320 3d20 636c 662e 7072 6564 6963  els = clf.predic
-00001510: 7428 5829 0a60 6060 0a0a 5369 6d69 6c61  t(X).```..Simila
-00001520: 726c 7920 746f 2074 6865 2060 5a65 726f  rly to the `Zero
-00001530: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
-00001540: 7260 2069 7420 6973 2073 7566 6669 6369  r` it is suffici
-00001550: 656e 7420 6966 206f 6e6c 7920 6361 6e64  ent if only cand
-00001560: 6964 6174 6520 6c61 6265 6c73 2061 7265  idate labels are
-00001570: 2070 726f 7669 6465 642e 2048 6f77 6576   provided. Howev
-00001580: 6572 2c20 7468 6973 2074 696d 6520 7468  er, this time th
-00001590: 6520 636c 6173 7369 6669 6572 2065 7870  e classifier exp
-000015a0: 6563 7473 2060 7960 206f 6620 6120 7479  ects `y` of a ty
-000015b0: 7065 2060 4c69 7374 5b4c 6973 745b 7374  pe `List[List[st
-000015c0: 725d 5d60 2e0a 0a60 6060 7079 7468 6f6e  r]]`...```python
-000015d0: 0a66 726f 6d20 736b 6c6c 6d20 696d 706f  .from skllm impo
-000015e0: 7274 204d 756c 7469 4c61 6265 6c5a 6572  rt MultiLabelZer
-000015f0: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001600: 6572 0a66 726f 6d20 736b 6c6c 6d2e 6461  er.from skllm.da
-00001610: 7461 7365 7473 2069 6d70 6f72 7420 6765  tasets import ge
-00001620: 745f 6d75 6c74 696c 6162 656c 5f63 6c61  t_multilabel_cla
-00001630: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
-00001640: 7365 740a 0a58 2c20 5f20 3d20 6765 745f  set..X, _ = get_
-00001650: 6d75 6c74 696c 6162 656c 5f63 6c61 7373  multilabel_class
-00001660: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
-00001670: 7428 290a 6361 6e64 6964 6174 655f 6c61  t().candidate_la
-00001680: 6265 6c73 203d 205b 0a20 2020 2022 5175  bels = [.    "Qu
-00001690: 616c 6974 7922 2c0a 2020 2020 2250 7269  ality",.    "Pri
-000016a0: 6365 222c 0a20 2020 2022 4465 6c69 7665  ce",.    "Delive
-000016b0: 7279 222c 0a20 2020 2022 5365 7276 6963  ry",.    "Servic
-000016c0: 6522 2c0a 2020 2020 2250 726f 6475 6374  e",.    "Product
-000016d0: 2056 6172 6965 7479 222c 0a20 2020 2022   Variety",.    "
-000016e0: 4375 7374 6f6d 6572 2053 7570 706f 7274  Customer Support
-000016f0: 222c 0a20 2020 2022 5061 636b 6167 696e  ",.    "Packagin
-00001700: 6722 2c0a 2020 2020 2255 7365 7220 4578  g",.    "User Ex
-00001710: 7065 7269 656e 6365 222c 0a20 2020 2022  perience",.    "
-00001720: 5265 7475 726e 2050 6f6c 6963 7922 2c0a  Return Policy",.
-00001730: 2020 2020 2250 726f 6475 6374 2049 6e66      "Product Inf
-00001740: 6f72 6d61 7469 6f6e 222c 0a5d 0a63 6c66  ormation",.].clf
-00001750: 203d 204d 756c 7469 4c61 6265 6c5a 6572   = MultiLabelZer
-00001760: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001770: 6572 286d 6178 5f6c 6162 656c 733d 3329  er(max_labels=3)
-00001780: 0a63 6c66 2e66 6974 284e 6f6e 652c 205b  .clf.fit(None, [
-00001790: 6361 6e64 6964 6174 655f 6c61 6265 6c73  candidate_labels
-000017a0: 5d29 0a6c 6162 656c 7320 3d20 636c 662e  ]).labels = clf.
-000017b0: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
-000017c0: 2323 2320 4665 772d 5368 6f74 2054 6578  ### Few-Shot Tex
-000017d0: 7420 436c 6173 7369 6669 6361 7469 6f6e  t Classification
-000017e0: 0a0a 5769 7468 2060 4665 7753 686f 7447  ..With `FewShotG
-000017f0: 5054 436c 6173 7369 6669 6572 6020 6974  PTClassifier` it
-00001800: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
-00001810: 7065 7266 6f72 6d20 6120 6665 772d 7368  perform a few-sh
-00001820: 6f74 2063 6c61 7373 6966 6963 6174 696f  ot classificatio
-00001830: 6e2c 2077 6869 6368 206d 6561 6e73 2074  n, which means t
-00001840: 6861 7420 7468 6520 7472 6169 6e69 6e67  hat the training
-00001850: 2073 616d 706c 6573 2077 696c 6c20 6265   samples will be
-00001860: 2061 6464 6564 2074 6f20 7072 6f6d 7074   added to prompt
-00001870: 2061 6e64 2070 6173 7365 6420 746f 2074   and passed to t
-00001880: 6865 206d 6f64 656c 2e0a 0a60 6060 7079  he model...```py
-00001890: 7468 6f6e 0a66 726f 6d20 736b 6c6c 6d20  thon.from skllm 
-000018a0: 696d 706f 7274 2046 6577 5368 6f74 4750  import FewShotGP
-000018b0: 5443 6c61 7373 6966 6965 720a 6672 6f6d  TClassifier.from
-000018c0: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
-000018d0: 696d 706f 7274 2067 6574 5f63 6c61 7373  import get_class
-000018e0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
-000018f0: 740a 0a58 2c20 7920 3d20 6765 745f 636c  t..X, y = get_cl
-00001900: 6173 7369 6669 6361 7469 6f6e 5f64 6174  assification_dat
-00001910: 6173 6574 2829 0a0a 636c 6620 3d20 4665  aset()..clf = Fe
-00001920: 7753 686f 7447 5054 436c 6173 7369 6669  wShotGPTClassifi
-00001930: 6572 286f 7065 6e61 695f 6d6f 6465 6c3d  er(openai_model=
-00001940: 2267 7074 2d33 2e35 2d74 7572 626f 2229  "gpt-3.5-turbo")
-00001950: 0a63 6c66 2e66 6974 2858 2c20 7929 0a6c  .clf.fit(X, y).l
-00001960: 6162 656c 7320 3d20 636c 662e 7072 6564  abels = clf.pred
-00001970: 6963 7428 5829 0a60 6060 0a0a 5768 696c  ict(X).```..Whil
-00001980: 6520 7468 6520 6170 6920 7265 6d61 696e  e the api remain
-00001990: 7320 7468 6520 7361 6d65 2061 7320 666f  s the same as fo
-000019a0: 7220 7468 6520 7a65 726f 2073 686f 7420  r the zero shot 
-000019b0: 636c 6173 7369 6669 6572 2c20 7468 6572  classifier, ther
-000019c0: 6520 6172 6520 6120 6665 7720 7468 696e  e are a few thin
-000019d0: 6773 2074 6f20 7461 6b65 2069 6e74 6f20  gs to take into 
-000019e0: 6163 636f 756e 743a 0a0a 2d20 7468 6520  account:..- the 
-000019f0: 2274 7261 696e 696e 6722 2072 6571 7569  "training" requi
-00001a00: 7265 7320 736f 6d65 206c 6162 656c 6c65  res some labelle
-00001a10: 6420 7472 6169 6e69 6e67 2064 6174 613b  d training data;
-00001a20: 0a2d 2074 6865 2074 7261 696e 696e 6720  .- the training 
-00001a30: 7365 7420 7368 6f75 6c64 2062 6520 736d  set should be sm
-00001a40: 616c 6c20 656e 6f75 6768 2074 6f20 6669  all enough to fi
-00001a50: 7420 696e 746f 2061 2073 696e 676c 6520  t into a single 
-00001a60: 7072 6f6d 7074 2028 7765 2072 6563 6f6d  prompt (we recom
-00001a70: 6d65 6e64 2075 7020 746f 2031 3020 7361  mend up to 10 sa
-00001a80: 6d70 6c65 7320 7065 7220 6c61 6265 6c29  mples per label)
-00001a90: 3b0a 2d20 6265 6361 7573 6520 6f66 2074  ;.- because of t
-00001aa0: 6865 2073 6967 6e69 6669 6361 6e74 6c79  he significantly
-00001ab0: 206c 6172 6765 7220 7072 6f6d 7074 2c20   larger prompt, 
-00001ac0: 7468 6520 696e 6665 7265 6e63 6520 7461  the inference ta
-00001ad0: 6b65 7320 6c6f 6e67 6572 2061 6e64 2063  kes longer and c
-00001ae0: 6f6e 7375 6d65 7320 6869 6768 6572 2061  onsumes higher a
-00001af0: 6d6f 756e 7420 6f66 2074 6f6b 656e 732e  mount of tokens.
-00001b00: 0a0a 4e6f 7465 3a20 6173 2074 6865 206d  ..Note: as the m
-00001b10: 6f64 656c 2069 7320 6e6f 7420 6265 696e  odel is not bein
-00001b20: 6720 7265 2d74 7261 696e 6564 2c20 6275  g re-trained, bu
-00001b30: 7420 7573 6573 2074 6865 2074 7261 696e  t uses the train
-00001b40: 696e 6720 6461 7461 2064 7572 696e 6720  ing data during 
-00001b50: 696e 6665 7265 6e63 652c 206f 6e65 2063  inference, one c
-00001b60: 6f75 6c64 2073 6179 2074 6861 7420 7468  ould say that th
-00001b70: 6973 2069 7320 7374 696c 6c20 6120 2864  is is still a (d
-00001b80: 6966 6665 7265 6e74 2920 7a65 726f 2d73  ifferent) zero-s
-00001b90: 686f 7420 6170 7072 6f61 6368 2e0a 0a23  hot approach...#
-00001ba0: 2323 2044 796e 616d 6963 2046 6577 2d53  ## Dynamic Few-S
-00001bb0: 686f 7420 5465 7874 2043 6c61 7373 6966  hot Text Classif
-00001bc0: 6963 6174 696f 6e0a 0a60 4479 6e61 6d69  ication..`Dynami
-00001bd0: 6346 6577 5368 6f74 4750 5443 6c61 7373  cFewShotGPTClass
-00001be0: 6966 6965 7260 2064 796e 616d 6963 616c  ifier` dynamical
-00001bf0: 6c79 2073 656c 6563 7473 204e 2073 616d  ly selects N sam
-00001c00: 706c 6573 2070 6572 2063 6c61 7373 2074  ples per class t
-00001c10: 6f20 696e 636c 7564 6520 696e 2074 6865  o include in the
-00001c20: 2070 726f 6d70 742e 2054 6869 7320 616c   prompt. This al
-00001c30: 6c6f 7773 2074 6865 2066 6577 2d73 686f  lows the few-sho
-00001c40: 7420 636c 6173 7369 6669 6572 2074 6f20  t classifier to 
-00001c50: 7363 616c 6520 746f 2064 6174 6173 6574  scale to dataset
-00001c60: 7320 7468 6174 2061 7265 2074 6f6f 206c  s that are too l
-00001c70: 6172 6765 2066 6f72 2074 6865 2073 7461  arge for the sta
-00001c80: 6e64 6172 6420 636f 6e74 6578 7420 7769  ndard context wi
-00001c90: 6e64 6f77 206f 6620 4c4c 4d73 2e0a 0a2a  ndow of LLMs...*
-00001ca0: 486f 7720 646f 6573 2069 7420 776f 726b  How does it work
-00001cb0: 3f2a 0a0a 4475 7269 6e67 2066 6974 7469  ?*..During fitti
-00001cc0: 6e67 2c20 7468 6520 7768 6f6c 6520 6461  ng, the whole da
-00001cd0: 7461 7365 7420 6973 2070 6172 7469 7469  taset is partiti
-00001ce0: 6f6e 6564 2062 7920 636c 6173 732c 2076  oned by class, v
-00001cf0: 6563 746f 7269 7a65 642c 2061 6e64 2073  ectorized, and s
-00001d00: 746f 7265 642e 0a0a 4475 7269 6e67 2069  tored...During i
-00001d10: 6e66 6572 656e 6365 2c20 7468 6520 5b61  nference, the [a
-00001d20: 6e6e 6f79 5d28 6874 7470 733a 2f2f 6769  nnoy](https://gi
-00001d30: 7468 7562 2e63 6f6d 2f73 706f 7469 6679  thub.com/spotify
-00001d40: 2f61 6e6e 6f79 2920 6c69 6272 6172 7920  /annoy) library 
-00001d50: 6973 2075 7365 6420 666f 7220 6661 7374  is used for fast
-00001d60: 206e 6569 6768 626f 7220 6c6f 6f6b 7570   neighbor lookup
-00001d70: 2c20 7768 6963 6820 616c 6c6f 7773 2069  , which allows i
-00001d80: 6e63 6c75 6469 6e67 206f 6e6c 7920 7468  ncluding only th
-00001d90: 6520 6d6f 7374 2073 696d 696c 6172 2065  e most similar e
-00001da0: 7861 6d70 6c65 7320 696e 2074 6865 2070  xamples in the p
-00001db0: 726f 6d70 742e 0a0a 6060 6070 7974 686f  rompt...```pytho
-00001dc0: 6e0a 6672 6f6d 2073 6b6c 6c6d 2069 6d70  n.from skllm imp
-00001dd0: 6f72 7420 4479 6e61 6d69 6346 6577 5368  ort DynamicFewSh
-00001de0: 6f74 4750 5443 6c61 7373 6966 6965 720a  otGPTClassifier.
-00001df0: 6672 6f6d 2073 6b6c 6c6d 2e64 6174 6173  from skllm.datas
-00001e00: 6574 7320 696d 706f 7274 2067 6574 5f63  ets import get_c
-00001e10: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
-00001e20: 7461 7365 740a 0a58 2c20 7920 3d20 6765  taset..X, y = ge
-00001e30: 745f 636c 6173 7369 6669 6361 7469 6f6e  t_classification
-00001e40: 5f64 6174 6173 6574 2829 0a0a 636c 6620  _dataset()..clf 
-00001e50: 3d20 4479 6e61 6d69 6346 6577 5368 6f74  = DynamicFewShot
-00001e60: 4750 5443 6c61 7373 6966 6965 7228 6e5f  GPTClassifier(n_
-00001e70: 6578 616d 706c 6573 3d33 290a 636c 662e  examples=3).clf.
-00001e80: 6669 7428 582c 2079 290a 6c61 6265 6c73  fit(X, y).labels
-00001e90: 203d 2063 6c66 2e70 7265 6469 6374 2858   = clf.predict(X
-00001ea0: 290a 6060 600a 0a23 2323 2054 6578 7420  ).```..### Text 
-00001eb0: 5665 6374 6f72 697a 6174 696f 6e0a 0a41  Vectorization..A
-00001ec0: 7320 616e 2061 6c74 6572 6e61 7469 7665  s an alternative
-00001ed0: 2074 6f20 7573 696e 6720 4750 5420 6173   to using GPT as
-00001ee0: 2061 2063 6c61 7373 6966 6965 722c 2069   a classifier, i
-00001ef0: 7420 6361 6e20 6265 2075 7365 6420 736f  t can be used so
-00001f00: 6c65 6c79 2066 6f72 2064 6174 6120 7072  lely for data pr
-00001f10: 6570 726f 6365 7373 696e 672e 2060 4750  eprocessing. `GP
-00001f20: 5456 6563 746f 7269 7a65 7260 2061 6c6c  TVectorizer` all
-00001f30: 6f77 7320 746f 2065 6d62 6564 2061 2063  ows to embed a c
-00001f40: 6875 6e6b 206f 6620 7465 7874 206f 6620  hunk of text of 
-00001f50: 6172 6269 7472 6172 7920 6c65 6e67 7468  arbitrary length
-00001f60: 2074 6f20 6120 6669 7865 642d 6469 6d65   to a fixed-dime
-00001f70: 6e73 696f 6e61 6c20 7665 6374 6f72 2c20  nsional vector, 
-00001f80: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00001f90: 2077 6974 6820 7669 7274 7561 6c6c 7920   with virtually 
-00001fa0: 616e 7920 636c 6173 7369 6669 6361 7469  any classificati
-00001fb0: 6f6e 206f 7220 7265 6772 6573 7369 6f6e  on or regression
-00001fc0: 206d 6f64 656c 2e0a 0a45 7861 6d70 6c65   model...Example
-00001fd0: 2031 3a20 456d 6265 6464 696e 6720 7468   1: Embedding th
-00001fe0: 6520 7465 7874 0a0a 6060 6070 7974 686f  e text..```pytho
-00001ff0: 6e0a 6672 6f6d 2073 6b6c 6c6d 2e70 7265  n.from skllm.pre
-00002000: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
-00002010: 7420 4750 5456 6563 746f 7269 7a65 720a  t GPTVectorizer.
-00002020: 0a6d 6f64 656c 203d 2047 5054 5665 6374  .model = GPTVect
-00002030: 6f72 697a 6572 2829 0a76 6563 746f 7273  orizer().vectors
-00002040: 203d 206d 6f64 656c 2e66 6974 5f74 7261   = model.fit_tra
-00002050: 6e73 666f 726d 2858 290a 6060 600a 0a45  nsform(X).```..E
-00002060: 7861 6d70 6c65 2032 3a20 436f 6d62 696e  xample 2: Combin
-00002070: 696e 6720 7468 6520 5665 6374 6f72 697a  ing the Vectoriz
-00002080: 6572 2077 6974 6820 7468 6520 5847 426f  er with the XGBo
-00002090: 6f73 7420 436c 6173 7369 6669 6572 2069  ost Classifier i
-000020a0: 6e20 6120 536b 6c65 6172 6e20 5069 7065  n a Sklearn Pipe
-000020b0: 6c69 6e65 0a0a 6060 6070 7974 686f 6e0a  line..```python.
-000020c0: 6672 6f6d 2073 6b6c 6561 726e 2e70 6970  from sklearn.pip
-000020d0: 656c 696e 6520 696d 706f 7274 2050 6970  eline import Pip
-000020e0: 656c 696e 650a 6672 6f6d 2073 6b6c 6561  eline.from sklea
-000020f0: 726e 2e70 7265 7072 6f63 6573 7369 6e67  rn.preprocessing
-00002100: 2069 6d70 6f72 7420 4c61 6265 6c45 6e63   import LabelEnc
-00002110: 6f64 6572 0a66 726f 6d20 7867 626f 6f73  oder.from xgboos
-00002120: 7420 696d 706f 7274 2058 4742 436c 6173  t import XGBClas
-00002130: 7369 6669 6572 0a0a 6c65 203d 204c 6162  sifier..le = Lab
-00002140: 656c 456e 636f 6465 7228 290a 795f 7472  elEncoder().y_tr
-00002150: 6169 6e5f 656e 636f 6465 6420 3d20 6c65  ain_encoded = le
-00002160: 2e66 6974 5f74 7261 6e73 666f 726d 2879  .fit_transform(y
-00002170: 5f74 7261 696e 290a 795f 7465 7374 5f65  _train).y_test_e
-00002180: 6e63 6f64 6564 203d 206c 652e 7472 616e  ncoded = le.tran
-00002190: 7366 6f72 6d28 795f 7465 7374 290a 0a73  sform(y_test)..s
-000021a0: 7465 7073 203d 205b 2822 4750 5422 2c20  teps = [("GPT", 
-000021b0: 4750 5456 6563 746f 7269 7a65 7228 2929  GPTVectorizer())
-000021c0: 2c20 2822 436c 6622 2c20 5847 4243 6c61  , ("Clf", XGBCla
-000021d0: 7373 6966 6965 7228 2929 5d0a 636c 6620  ssifier())].clf 
-000021e0: 3d20 5069 7065 6c69 6e65 2873 7465 7073  = Pipeline(steps
-000021f0: 290a 636c 662e 6669 7428 585f 7472 6169  ).clf.fit(X_trai
-00002200: 6e2c 2079 5f74 7261 696e 5f65 6e63 6f64  n, y_train_encod
-00002210: 6564 290a 7968 203d 2063 6c66 2e70 7265  ed).yh = clf.pre
-00002220: 6469 6374 2858 5f74 6573 7429 0a60 6060  dict(X_test).```
-00002230: 0a0a 2323 2320 5465 7874 2053 756d 6d61  ..### Text Summa
-00002240: 7269 7a61 7469 6f6e 0a0a 4750 5420 6578  rization..GPT ex
-00002250: 6365 6c73 2061 7420 7065 7266 6f72 6d69  cels at performi
-00002260: 6e67 2073 756d 6d61 7269 7a61 7469 6f6e  ng summarization
-00002270: 2074 6173 6b73 2e20 5468 6572 6566 6f72   tasks. Therefor
-00002280: 652c 2077 6520 7072 6f76 6964 6520 6047  e, we provide `G
-00002290: 5054 5375 6d6d 6172 697a 6572 6020 7468  PTSummarizer` th
-000022a0: 6174 2063 616e 2062 6520 7573 6564 2062  at can be used b
-000022b0: 6f74 6820 6173 2073 7461 6e64 2d61 6c6f  oth as stand-alo
-000022c0: 6e65 2065 7374 696d 6174 6f72 2c20 6f72  ne estimator, or
-000022d0: 2061 7320 6120 7072 6570 726f 6365 7373   as a preprocess
-000022e0: 6f72 2028 696e 2074 6869 7320 6361 7365  or (in this case
-000022f0: 2077 6520 6361 6e20 6d61 6b65 2061 6e20   we can make an 
-00002300: 616e 616c 6f67 7920 7769 7468 2061 2064  analogy with a d
-00002310: 696d 656e 7369 6f6e 616c 6974 7920 7265  imensionality re
-00002320: 6475 6374 696f 6e20 7072 6570 726f 6365  duction preproce
-00002330: 7373 6f72 292e 0a0a 4578 616d 706c 653a  ssor)...Example:
-00002340: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00002350: 2073 6b6c 6c6d 2e70 7265 7072 6f63 6573   skllm.preproces
-00002360: 7369 6e67 2069 6d70 6f72 7420 4750 5453  sing import GPTS
-00002370: 756d 6d61 7269 7a65 720a 6672 6f6d 2073  ummarizer.from s
-00002380: 6b6c 6c6d 2e64 6174 6173 6574 7320 696d  kllm.datasets im
-00002390: 706f 7274 2067 6574 5f73 756d 6d61 7269  port get_summari
-000023a0: 7a61 7469 6f6e 5f64 6174 6173 6574 0a0a  zation_dataset..
-000023b0: 5820 3d20 6765 745f 7375 6d6d 6172 697a  X = get_summariz
-000023c0: 6174 696f 6e5f 6461 7461 7365 7428 290a  ation_dataset().
-000023d0: 7320 3d20 4750 5453 756d 6d61 7269 7a65  s = GPTSummarize
-000023e0: 7228 6f70 656e 6169 5f6d 6f64 656c 3d22  r(openai_model="
-000023f0: 6770 742d 332e 352d 7475 7262 6f22 2c20  gpt-3.5-turbo", 
-00002400: 6d61 785f 776f 7264 733d 3135 290a 7375  max_words=15).su
-00002410: 6d6d 6172 6965 7320 3d20 732e 6669 745f  mmaries = s.fit_
-00002420: 7472 616e 7366 6f72 6d28 5829 0a60 6060  transform(X).```
-00002430: 0a0a 506c 6561 7365 2062 6520 6177 6172  ..Please be awar
-00002440: 6520 7468 6174 2074 6865 2060 6d61 785f  e that the `max_
-00002450: 776f 7264 7360 2068 7970 6572 7061 7261  words` hyperpara
-00002460: 6d65 7465 7220 7365 7473 2061 2073 6f66  meter sets a sof
-00002470: 7420 6c69 6d69 742c 2077 6869 6368 2069  t limit, which i
-00002480: 7320 6e6f 7420 7374 7269 6374 6c79 2065  s not strictly e
-00002490: 6e66 6f72 6365 6420 6f75 7473 6964 6520  nforced outside 
-000024a0: 6f66 2074 6865 2070 726f 6d70 742e 2054  of the prompt. T
-000024b0: 6865 7265 666f 7265 2c20 696e 2073 6f6d  herefore, in som
-000024c0: 6520 6361 7365 732c 2074 6865 2061 6374  e cases, the act
-000024d0: 7561 6c20 6e75 6d62 6572 206f 6620 776f  ual number of wo
-000024e0: 7264 7320 6d69 6768 7420 6265 2073 6c69  rds might be sli
-000024f0: 6768 746c 7920 6869 6768 6572 2e0a 0a23  ghtly higher...#
-00002500: 2323 2054 6578 7420 5472 616e 736c 6174  ## Text Translat
-00002510: 696f 6e0a 0a47 5054 206d 6f64 656c 7320  ion..GPT models 
-00002520: 6861 7665 2064 656d 6f6e 7374 7261 7465  have demonstrate
-00002530: 6420 7468 6569 7220 6566 6665 6374 6976  d their effectiv
-00002540: 656e 6573 7320 696e 2074 7261 6e73 6c61  eness in transla
-00002550: 7469 6f6e 2074 6173 6b73 2062 7920 6765  tion tasks by ge
-00002560: 6e65 7261 7469 6e67 2061 6363 7572 6174  nerating accurat
-00002570: 6520 7472 616e 736c 6174 696f 6e73 2061  e translations a
-00002580: 6372 6f73 7320 7661 7269 6f75 7320 6c61  cross various la
-00002590: 6e67 7561 6765 732e 2054 6875 732c 2077  nguages. Thus, w
-000025a0: 6520 6164 6465 6420 6047 5054 5472 616e  e added `GPTTran
-000025b0: 736c 6174 6f72 6020 7468 6174 2061 6c6c  slator` that all
-000025c0: 6f77 7320 7472 616e 736c 6174 696e 6720  ows translating 
-000025d0: 616e 2061 7262 6974 7261 7479 2074 6578  an arbitraty tex
-000025e0: 7420 696e 746f 2061 206c 616e 6775 6167  t into a languag
-000025f0: 6520 6f66 2069 6e74 6572 6573 742e 0a0a  e of interest...
-00002600: 4578 616d 706c 653a 0a0a 6060 6070 7974  Example:..```pyt
-00002610: 686f 6e0a 6672 6f6d 2073 6b6c 6c6d 2e70  hon.from skllm.p
-00002620: 7265 7072 6f63 6573 7369 6e67 2069 6d70  reprocessing imp
-00002630: 6f72 7420 4750 5454 7261 6e73 6c61 746f  ort GPTTranslato
-00002640: 720a 6672 6f6d 2073 6b6c 6c6d 2e64 6174  r.from skllm.dat
-00002650: 6173 6574 7320 696d 706f 7274 2067 6574  asets import get
-00002660: 5f74 7261 6e73 6c61 7469 6f6e 5f64 6174  _translation_dat
-00002670: 6173 6574 0a0a 5820 3d20 6765 745f 7472  aset..X = get_tr
-00002680: 616e 736c 6174 696f 6e5f 6461 7461 7365  anslation_datase
-00002690: 7428 290a 7420 3d20 4750 5454 7261 6e73  t().t = GPTTrans
-000026a0: 6c61 746f 7228 6f70 656e 6169 5f6d 6f64  lator(openai_mod
-000026b0: 656c 3d22 6770 742d 332e 352d 7475 7262  el="gpt-3.5-turb
-000026c0: 6f22 2c20 6f75 7470 7574 5f6c 616e 6775  o", output_langu
-000026d0: 6167 653d 2245 6e67 6c69 7368 2229 0a74  age="English").t
-000026e0: 7261 6e73 6c61 7465 645f 7465 7874 203d  ranslated_text =
-000026f0: 2074 2e66 6974 5f74 7261 6e73 666f 726d   t.fit_transform
-00002700: 2858 290a 6060 600a 0a23 2320 526f 6164  (X).```..## Road
-00002710: 6d61 7020 f09f a7ad 0a0a 2d20 5b78 5d20  map ......- [x] 
-00002720: 5a65 726f 2d53 686f 7420 436c 6173 7369  Zero-Shot Classi
-00002730: 6669 6361 7469 6f6e 2077 6974 6820 4f70  fication with Op
-00002740: 656e 4149 2047 5054 2033 2f34 0a20 202d  enAI GPT 3/4.  -
-00002750: 205b 785d 204d 756c 7469 636c 6173 7320   [x] Multiclass 
-00002760: 636c 6173 7369 6669 6361 7469 6f6e 0a20  classification. 
-00002770: 202d 205b 785d 204d 756c 7469 2d6c 6162   - [x] Multi-lab
-00002780: 656c 2063 6c61 7373 6966 6963 6174 696f  el classificatio
-00002790: 6e0a 2d20 5b20 5d20 4665 772d 5368 6f74  n.- [ ] Few-Shot
-000027a0: 2063 6c61 7373 6966 6965 720a 2020 2d20   classifier.  - 
-000027b0: 5b78 5d20 4d75 6c74 6963 6c61 7373 2063  [x] Multiclass c
-000027c0: 6c61 7373 6966 6963 6174 696f 6e0a 2020  lassification.  
-000027d0: 2d20 5b20 5d20 4d75 6c74 692d 6c61 6265  - [ ] Multi-labe
-000027e0: 6c20 636c 6173 7369 6669 6361 7469 6f6e  l classification
-000027f0: 0a2d 205b 785d 2047 5054 2056 6563 746f  .- [x] GPT Vecto
-00002800: 7269 7a65 720a 2d20 5b78 5d20 4368 6174  rizer.- [x] Chat
-00002810: 4750 5420 6d6f 6465 6c73 0a2d 205b 205d  GPT models.- [ ]
-00002820: 2049 6e73 7472 7563 7447 5054 206d 6f64   InstructGPT mod
-00002830: 656c 730a 2d20 5b20 5d20 496e 7374 7275  els.- [ ] Instru
-00002840: 6374 4750 5420 4669 6e65 2d74 756e 696e  ctGPT Fine-tunin
-00002850: 6720 286f 7074 696f 6e61 6c29 0a2d 205b  g (optional).- [
-00002860: 205d 204f 7065 6e20 736f 7572 6365 206d   ] Open source m
-00002870: 6f64 656c 730a 0a2a 5468 6520 6f72 6465  odels..*The orde
-00002880: 7220 6f66 2074 6865 2065 6c65 6d65 6e74  r of the element
-00002890: 7320 696e 2074 6865 2072 6f61 646d 6170  s in the roadmap
-000028a0: 2069 7320 6172 6269 7472 6172 7920 616e   is arbitrary an
-000028b0: 6420 646f 6573 206e 6f74 2072 6566 6c65  d does not refle
-000028c0: 6374 2074 6865 2070 6c61 6e6e 6564 206f  ct the planned o
-000028d0: 7264 6572 206f 6620 696d 706c 656d 656e  rder of implemen
-000028e0: 7461 7469 6f6e 2e2a 0a                   tation.*.
+000001f0: 6572 290a 2d20 f09f 92a1 2050 726f 7669  er).- .... Provi
+00000200: 6465 2079 6f75 7220 6665 6564 6261 636b  de your feedback
+00000210: 206f 7220 7072 6f70 6f73 6520 6964 6561   or propose idea
+00000220: 7320 696e 2074 6865 205b 6973 7375 6573  s in the [issues
+00000230: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000240: 2e63 6f6d 2f69 7279 6e61 2d6b 6f6e 6472  .com/iryna-kondr
+00000250: 2f73 6369 6b69 742d 6c6c 6d2f 6973 7375  /scikit-llm/issu
+00000260: 6573 2920 7365 6374 696f 6e20 6f72 205b  es) section or [
+00000270: 4469 7363 6f72 645d 2868 7474 7073 3a2f  Discord](https:/
+00000280: 2f64 6973 636f 7264 2e67 672f 5944 4162  /discord.gg/YDAb
+00000290: 7775 574b 3756 290a 2d20 f09f 93b0 2050  wuWK7V).- .... P
+000002a0: 6f73 7420 6162 6f75 7420 5363 696b 6974  ost about Scikit
+000002b0: 2d4c 4c4d 206f 6e20 4c69 6e6b 6564 496e  -LLM on LinkedIn
+000002c0: 206f 7220 6f74 6865 7220 706c 6174 666f   or other platfo
+000002d0: 726d 730a 0a23 2320 4f75 7220 5265 6c61  rms..## Our Rela
+000002e0: 7465 6420 5072 6f6a 6563 7473 20f0 9f94  ted Projects ...
+000002f0: 970a 0a3c 6120 6872 6566 3d22 6874 7470  ...<a href="http
+00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+00000310: 4b55 4131 2f66 616c 636f 6e22 3e3c 696d  KUA1/falcon"><im
+00000320: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000330: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000340: 7465 6e74 2e63 6f6d 2f67 6973 742f 4f4b  tent.com/gist/OK
+00000350: 5541 312f 3632 3634 6139 3561 3861 6264  UA1/6264a95a8abd
+00000360: 3232 3563 3734 3431 3161 3262 3730 3762  225c74411a2b707b
+00000370: 3032 3432 2f72 6177 2f33 6365 6462 3533  0242/raw/3cedb53
+00000380: 3533 3863 6230 3436 3536 6364 3964 3764  538cb04656cd9d7d
+00000390: 3037 6536 3937 6537 3236 3839 3663 6539  07e697e726896ce9
+000003a0: 662f 6661 6c63 6f6e 5f6c 6967 6874 2e73  f/falcon_light.s
+000003b0: 7667 222f 3e3c 2f61 3e20 3c62 723e 0a3c  vg"/></a> <br>.<
+000003c0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000003d0: 6769 7468 7562 2e63 6f6d 2f4f 4b55 4131  github.com/OKUA1
+000003e0: 2f61 6765 6e74 5f64 696e 676f 223e 3c69  /agent_dingo"><i
+000003f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000400: 6769 7374 2e67 6974 6875 6275 7365 7263  gist.githubuserc
+00000410: 6f6e 7465 6e74 2e63 6f6d 2f4f 4b55 4131  ontent.com/OKUA1
+00000420: 2f36 3236 3461 3935 6138 6162 6432 3235  /6264a95a8abd225
+00000430: 6337 3434 3131 6132 6237 3037 6230 3234  c74411a2b707b024
+00000440: 322f 7261 772f 3162 3233 3161 6162 3731  2/raw/1b231aab71
+00000450: 3866 6361 6236 3234 6661 6133 3364 3963  8fcab624faa33d9c
+00000460: 3130 6430 6565 6531 3763 6131 3630 2f64  10d0eee17ca160/d
+00000470: 696e 676f 5f6c 6967 6874 2e73 7667 222f  ingo_light.svg"/
+00000480: 3e3c 2f61 3e0a 0a23 2320 446f 6375 6d65  ></a>..## Docume
+00000490: 6e74 6174 696f 6e20 f09f 939a 0a0a 2323  ntation ......##
+000004a0: 2320 436f 6e66 6967 7572 696e 6720 4f70  # Configuring Op
+000004b0: 656e 4149 2041 5049 204b 6579 0a0a 4174  enAI API Key..At
+000004c0: 2074 6865 206d 6f6d 656e 7420 7468 6520   the moment the 
+000004d0: 6d61 6a6f 7269 7479 206f 6620 7468 6520  majority of the 
+000004e0: 5363 696b 6974 2d4c 4c4d 2065 7374 696d  Scikit-LLM estim
+000004f0: 6174 6f72 7320 6172 6520 6f6e 6c79 2063  ators are only c
+00000500: 6f6d 7061 7469 626c 6520 7769 7468 2073  ompatible with s
+00000510: 6f6d 6520 6f66 2074 6865 204f 7065 6e41  ome of the OpenA
+00000520: 4920 6d6f 6465 6c73 2e20 4865 6e63 652c  I models. Hence,
+00000530: 2061 2075 7365 722d 7072 6f76 6964 6564   a user-provided
+00000540: 204f 7065 6e41 4920 4150 4920 6b65 7920   OpenAI API key 
+00000550: 6973 2072 6571 7569 7265 642e 0a0a 6060  is required...``
+00000560: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+00000570: 6c6d 2e63 6f6e 6669 6720 696d 706f 7274  lm.config import
+00000580: 2053 4b4c 4c4d 436f 6e66 6967 0a0a 534b   SKLLMConfig..SK
+00000590: 4c4c 4d43 6f6e 6669 672e 7365 745f 6f70  LLMConfig.set_op
+000005a0: 656e 6169 5f6b 6579 2822 3c59 4f55 525f  enai_key("<YOUR_
+000005b0: 4b45 593e 2229 0a53 4b4c 4c4d 436f 6e66  KEY>").SKLLMConf
+000005c0: 6967 2e73 6574 5f6f 7065 6e61 695f 6f72  ig.set_openai_or
+000005d0: 6728 223c 594f 5552 5f4f 5247 414e 4953  g("<YOUR_ORGANIS
+000005e0: 4154 494f 4e3e 2229 0a60 6060 0a0a 2a2a  ATION>").```..**
+000005f0: 496d 706f 7274 616e 7420 6e6f 7469 6365  Important notice
+00000600: 3a2a 2a0a 0a2d 2049 6620 796f 7520 6861  :**..- If you ha
+00000610: 7665 2061 2066 7265 6520 7472 6961 6c20  ve a free trial 
+00000620: 4f70 656e 4149 2061 6363 6f75 6e74 2c20  OpenAI account, 
+00000630: 7468 6520 5b72 6174 6520 6c69 6d69 7473  the [rate limits
+00000640: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
+00000650: 726d 2e6f 7065 6e61 692e 636f 6d2f 646f  rm.openai.com/do
+00000660: 6373 2f67 7569 6465 732f 7261 7465 2d6c  cs/guides/rate-l
+00000670: 696d 6974 732f 6f76 6572 7669 6577 2920  imits/overview) 
+00000680: 6172 6520 6e6f 7420 7375 6666 6963 6965  are not sufficie
+00000690: 6e74 2028 7370 6563 6966 6963 616c 6c79  nt (specifically
+000006a0: 2033 2072 6571 7565 7374 7320 7065 7220   3 requests per 
+000006b0: 6d69 6e75 7465 292e 2050 6c65 6173 6520  minute). Please 
+000006c0: 7377 6974 6368 2074 6f20 7468 6520 2270  switch to the "p
+000006d0: 6179 2061 7320 796f 7520 676f 2220 706c  ay as you go" pl
+000006e0: 616e 2066 6972 7374 2e0a 2d20 5768 656e  an first..- When
+000006f0: 2063 616c 6c69 6e67 2060 534b 4c4c 4d43   calling `SKLLMC
+00000700: 6f6e 6669 672e 7365 745f 6f70 656e 6169  onfig.set_openai
+00000710: 5f6f 7267 602c 2079 6f75 2068 6176 6520  _org`, you have 
+00000720: 746f 2070 726f 7669 6465 2079 6f75 7220  to provide your 
+00000730: 6f72 6761 6e69 7a61 7469 6f6e 2049 4420  organization ID 
+00000740: 616e 6420 2a2a 4e4f 542a 2a20 7468 6520  and **NOT** the 
+00000750: 6e61 6d65 2e20 596f 7520 6361 6e20 6669  name. You can fi
+00000760: 6e64 2079 6f75 7220 4944 205b 6865 7265  nd your ID [here
+00000770: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
+00000780: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
+00000790: 636f 756e 742f 6f72 672d 7365 7474 696e  count/org-settin
+000007a0: 6773 292e 0a0a 2323 2320 5573 696e 6720  gs)...### Using 
+000007b0: 417a 7572 6520 4f70 656e 4149 0a0a 6060  Azure OpenAI..``
+000007c0: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+000007d0: 6c6d 2e63 6f6e 6669 6720 696d 706f 7274  lm.config import
+000007e0: 2053 4b4c 4c4d 436f 6e66 6967 0a0a 534b   SKLLMConfig..SK
+000007f0: 4c4c 4d43 6f6e 6669 672e 7365 745f 6f70  LLMConfig.set_op
+00000800: 656e 6169 5f6b 6579 2822 3c59 4f55 525f  enai_key("<YOUR_
+00000810: 4b45 593e 2229 2023 7573 6520 617a 7572  KEY>") #use azur
+00000820: 6520 6b65 7920 696e 7374 6561 640a 534b  e key instead.SK
+00000830: 4c4c 4d43 6f6e 6669 672e 7365 745f 617a  LLMConfig.set_az
+00000840: 7572 655f 6170 695f 6261 7365 2822 3c41  ure_api_base("<A
+00000850: 5049 5f42 4153 453e 2229 0a0a 2320 7374  PI_BASE>")..# st
+00000860: 6172 7420 7769 7468 2022 617a 7572 653a  art with "azure:
+00000870: 3a22 2070 7265 6669 7820 7768 656e 2073  :" prefix when s
+00000880: 6574 7469 6e67 2074 6865 206d 6f64 656c  etting the model
+00000890: 206e 616d 650a 6d6f 6465 6c5f 6e61 6d65   name.model_name
+000008a0: 203d 2022 617a 7572 653a 3a3c 6d6f 6465   = "azure::<mode
+000008b0: 6c5f 6e61 6d65 3e22 0a23 2065 2e67 2e20  l_name>".# e.g. 
+000008c0: 5a65 726f 5368 6f74 4750 5443 6c61 7373  ZeroShotGPTClass
+000008d0: 6966 6965 7228 6f70 656e 6169 5f6d 6f64  ifier(openai_mod
+000008e0: 656c 3d22 617a 7572 653a 3a67 7074 2d33  el="azure::gpt-3
+000008f0: 2e35 2d74 7572 626f 2229 0a60 6060 0a0a  .5-turbo").```..
+00000900: 4e6f 7465 3a20 417a 7572 6520 4f70 656e  Note: Azure Open
+00000910: 4149 2069 7320 6e6f 7420 7375 7070 6f72  AI is not suppor
+00000920: 7465 6420 6279 2074 6865 2070 7265 7072  ted by the prepr
+00000930: 6f63 6573 736f 7273 2061 7420 7468 6520  ocessors at the 
+00000940: 6d6f 6d65 6e74 2e0a 0a23 2323 2055 7369  moment...### Usi
+00000950: 6e67 2047 5054 3441 4c4c 0a0a 496e 2061  ng GPT4ALL..In a
+00000960: 6464 6974 696f 6e20 746f 204f 7065 6e41  ddition to OpenA
+00000970: 492c 2073 6f6d 6520 6f66 2074 6865 206d  I, some of the m
+00000980: 6f64 656c 7320 6361 6e20 7573 6520 5b67  odels can use [g
+00000990: 7074 3461 6c6c 5d28 6874 7470 733a 2f2f  pt4all](https://
+000009a0: 6770 7434 616c 6c2e 696f 2f69 6e64 6578  gpt4all.io/index
+000009b0: 2e68 746d 6c29 2061 7320 6120 6261 636b  .html) as a back
+000009c0: 656e 642e 0a0a 2a2a 5468 6973 2066 6561  end...**This fea
+000009d0: 7475 7265 2069 7320 636f 6e73 6964 6572  ture is consider
+000009e0: 6564 2068 6967 6c79 2065 7870 6572 696d  ed higly experim
+000009f0: 656e 7461 6c21 2a2a 0a0a 496e 206f 7264  ental!**..In ord
+00000a00: 6572 2074 6f20 7573 6520 6770 7434 616c  er to use gpt4al
+00000a10: 6c2c 2079 6f75 206e 6565 6420 746f 2069  l, you need to i
+00000a20: 6e73 7461 6c6c 2074 6865 2063 6f72 7265  nstall the corre
+00000a30: 7370 6f6e 6469 6e67 2073 7562 6d6f 6475  sponding submodu
+00000a40: 6c65 3a0a 0a60 6060 6261 7368 0a70 6970  le:..```bash.pip
+00000a50: 2069 6e73 7461 6c6c 2022 7363 696b 6974   install "scikit
+00000a60: 2d6c 6c6d 5b67 7074 3461 6c6c 5d22 0a60  -llm[gpt4all]".`
+00000a70: 6060 0a0a 496e 206f 7264 6572 2074 6f20  ``..In order to 
+00000a80: 7377 6974 6368 2066 726f 6d20 4f70 656e  switch from Open
+00000a90: 4149 2074 6f20 4750 5434 414c 4c20 6d6f  AI to GPT4ALL mo
+00000aa0: 6465 6c2c 2073 696d 706c 7920 7072 6f76  del, simply prov
+00000ab0: 6964 6520 6120 7374 7269 6e67 206f 6620  ide a string of 
+00000ac0: 7468 6520 666f 726d 6174 2060 6770 7434  the format `gpt4
+00000ad0: 616c 6c3a 3a3c 6d6f 6465 6c5f 6e61 6d65  all::<model_name
+00000ae0: 3e60 2061 7320 616e 2061 7267 756d 656e  >` as an argumen
+00000af0: 742e 2057 6869 6c65 2074 6865 206d 6f64  t. While the mod
+00000b00: 656c 2072 756e 7320 636f 6d70 6c65 7465  el runs complete
+00000b10: 6c79 206c 6f63 616c 6c79 2c20 7468 6520  ly locally, the 
+00000b20: 6573 7469 6d61 746f 7220 7374 696c 6c20  estimator still 
+00000b30: 7472 6561 7473 2069 7420 6173 2061 6e20  treats it as an 
+00000b40: 4f70 656e 4149 2065 6e64 706f 696e 7420  OpenAI endpoint 
+00000b50: 616e 6420 7769 6c6c 2074 7279 2074 6f20  and will try to 
+00000b60: 6368 6563 6b20 7468 6174 2074 6865 2041  check that the A
+00000b70: 5049 206b 6579 2069 7320 7072 6573 656e  PI key is presen
+00000b80: 742e 2059 6f75 2063 616e 2070 726f 7669  t. You can provi
+00000b90: 6465 2061 6e79 2073 7472 696e 6720 6173  de any string as
+00000ba0: 2061 206b 6579 2e0a 0a60 6060 7079 7468   a key...```pyth
+00000bb0: 6f6e 0a53 4b4c 4c4d 436f 6e66 6967 2e73  on.SKLLMConfig.s
+00000bc0: 6574 5f6f 7065 6e61 695f 6b65 7928 2261  et_openai_key("a
+00000bd0: 6e79 2073 7472 696e 6722 290a 534b 4c4c  ny string").SKLL
+00000be0: 4d43 6f6e 6669 672e 7365 745f 6f70 656e  MConfig.set_open
+00000bf0: 6169 5f6f 7267 2822 616e 7920 7374 7269  ai_org("any stri
+00000c00: 6e67 2229 0a0a 5a65 726f 5368 6f74 4750  ng")..ZeroShotGP
+00000c10: 5443 6c61 7373 6966 6965 7228 6f70 656e  TClassifier(open
+00000c20: 6169 5f6d 6f64 656c 3d22 6770 7434 616c  ai_model="gpt4al
+00000c30: 6c3a 3a67 676d 6c2d 6770 7434 616c 6c2d  l::ggml-gpt4all-
+00000c40: 6a2d 7631 2e33 2d67 726f 6f76 7922 290a  j-v1.3-groovy").
+00000c50: 6060 600a 0a57 6865 6e20 7275 6e6e 696e  ```..When runnin
+00000c60: 6720 666f 7220 7468 6520 6669 7273 7420  g for the first 
+00000c70: 7469 6d65 2c20 7468 6520 6d6f 6465 6c20  time, the model 
+00000c80: 6669 6c65 2077 696c 6c20 6265 2064 6f77  file will be dow
+00000c90: 6e6c 6f61 6465 6420 6175 746f 6d61 7469  nloaded automati
+00000ca0: 616c 6c79 2e0a 0a57 6865 6e20 7573 696e  ally...When usin
+00000cb0: 6720 6770 7434 616c 6c20 706c 6561 7365  g gpt4all please
+00000cc0: 206b 6565 7020 7468 6520 666f 6c6c 6f77   keep the follow
+00000cd0: 696e 6720 696e 206d 696e 643a 0a0a 312e  ing in mind:..1.
+00000ce0: 204e 6f74 2061 6c6c 2067 7074 3461 6c6c   Not all gpt4all
+00000cf0: 206d 6f64 656c 7320 6172 6520 636f 6d6d   models are comm
+00000d00: 6572 6369 616c 6c79 206c 6963 656e 7361  ercially licensa
+00000d10: 626c 652c 2070 6c65 6173 6520 636f 6e73  ble, please cons
+00000d20: 756c 7420 6770 7434 616c 6c20 7765 6273  ult gpt4all webs
+00000d30: 6974 6520 666f 7220 6d6f 7265 2064 6574  ite for more det
+00000d40: 6169 6c73 2e0a 322e 2054 6865 2061 6363  ails..2. The acc
+00000d50: 7572 6163 7920 6f66 2074 6865 206d 6f64  uracy of the mod
+00000d60: 656c 7320 6d61 7920 6265 206d 7563 6820  els may be much 
+00000d70: 6c6f 7765 7220 636f 6d70 6172 6564 2074  lower compared t
+00000d80: 6f20 6f6e 6573 2070 726f 7669 6465 6420  o ones provided 
+00000d90: 6279 204f 7065 6e41 4920 2865 7370 6563  by OpenAI (espec
+00000da0: 6961 6c6c 7920 6770 742d 3429 2e0a 332e  ially gpt-4)..3.
+00000db0: 204e 6f74 2061 6c6c 206f 6620 7468 6520   Not all of the 
+00000dc0: 6176 6169 6c61 626c 6520 6d6f 6465 6c73  available models
+00000dd0: 2077 6572 6520 7465 7374 6564 2c20 736f   were tested, so
+00000de0: 6d65 206d 6179 206e 6f74 2077 6f72 6b20  me may not work 
+00000df0: 7769 7468 2073 6369 6b69 742d 6c6c 6d20  with scikit-llm 
+00000e00: 6174 2061 6c6c 2e0a 0a23 2323 2053 7570  at all...### Sup
+00000e10: 706f 7274 6564 206d 6f64 656c 7320 6279  ported models by
+00000e20: 2061 206e 6f6e 2d73 7461 6e64 6172 6420   a non-standard 
+00000e30: 6261 636b 656e 640a 0a41 7420 7468 6520  backend..At the 
+00000e40: 6d6f 6d65 6e74 206f 6e6c 7920 7468 6520  moment only the 
+00000e50: 666f 6c6c 6f77 696e 6720 6573 7469 6d61  following estima
+00000e60: 746f 7273 2073 7570 706f 7274 206e 6f6e  tors support non
+00000e70: 2d73 7461 6e64 6172 6420 6261 636b 656e  -standard backen
+00000e80: 6473 2028 6770 7434 616c 6c2c 2061 7a75  ds (gpt4all, azu
+00000e90: 7265 293a 0a0a 2d20 605a 6572 6f53 686f  re):..- `ZeroSho
+00000ea0: 7447 5054 436c 6173 7369 6669 6572 600a  tGPTClassifier`.
+00000eb0: 2d20 604d 756c 7469 4c61 6265 6c5a 6572  - `MultiLabelZer
+00000ec0: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
+00000ed0: 6572 600a 2d20 6046 6577 5368 6f74 4750  er`.- `FewShotGP
+00000ee0: 5443 6c61 7373 6966 6965 7260 0a0a 2323  TClassifier`..##
+00000ef0: 2320 5a65 726f 2d53 686f 7420 5465 7874  # Zero-Shot Text
+00000f00: 2043 6c61 7373 6966 6963 6174 696f 6e0a   Classification.
+00000f10: 0a4f 6e65 206f 6620 7468 6520 706f 7765  .One of the powe
+00000f20: 7266 756c 2043 6861 7447 5054 2066 6561  rful ChatGPT fea
+00000f30: 7475 7265 7320 6973 2074 6865 2061 6269  tures is the abi
+00000f40: 6c69 7479 2074 6f20 7065 7266 6f72 6d20  lity to perform 
+00000f50: 7465 7874 2063 6c61 7373 6966 6963 6174  text classificat
+00000f60: 696f 6e20 7769 7468 6f75 7420 6265 696e  ion without bein
+00000f70: 6720 7265 2d74 7261 696e 6564 2e20 466f  g re-trained. Fo
+00000f80: 7220 7468 6174 2c20 7468 6520 6f6e 6c79  r that, the only
+00000f90: 2072 6571 7569 7265 6d65 6e74 2069 7320   requirement is 
+00000fa0: 7468 6174 2074 6865 206c 6162 656c 7320  that the labels 
+00000fb0: 6d75 7374 2062 6520 6465 7363 7269 7074  must be descript
+00000fc0: 6976 652e 0a0a 5765 2070 726f 7669 6465  ive...We provide
+00000fd0: 2061 2063 6c61 7373 2060 5a65 726f 5368   a class `ZeroSh
+00000fe0: 6f74 4750 5443 6c61 7373 6966 6965 7260  otGPTClassifier`
+00000ff0: 2074 6861 7420 616c 6c6f 7773 2074 6f20   that allows to 
+00001000: 6372 6561 7465 2073 7563 6820 6120 6d6f  create such a mo
+00001010: 6465 6c20 6173 2061 2072 6567 756c 6172  del as a regular
+00001020: 2073 6369 6b69 742d 6c65 6172 6e20 636c   scikit-learn cl
+00001030: 6173 7369 6669 6572 2e0a 0a45 7861 6d70  assifier...Examp
+00001040: 6c65 2031 3a20 5472 6169 6e69 6e67 2061  le 1: Training a
+00001050: 7320 6120 7265 6775 6c61 7220 636c 6173  s a regular clas
+00001060: 7369 6669 6572 0a0a 6060 6070 7974 686f  sifier..```pytho
+00001070: 6e0a 6672 6f6d 2073 6b6c 6c6d 2069 6d70  n.from skllm imp
+00001080: 6f72 7420 5a65 726f 5368 6f74 4750 5443  ort ZeroShotGPTC
+00001090: 6c61 7373 6966 6965 720a 6672 6f6d 2073  lassifier.from s
+000010a0: 6b6c 6c6d 2e64 6174 6173 6574 7320 696d  kllm.datasets im
+000010b0: 706f 7274 2067 6574 5f63 6c61 7373 6966  port get_classif
+000010c0: 6963 6174 696f 6e5f 6461 7461 7365 740a  ication_dataset.
+000010d0: 0a23 2064 656d 6f20 7365 6e74 696d 656e  .# demo sentimen
+000010e0: 7420 616e 616c 7973 6973 2064 6174 6173  t analysis datas
+000010f0: 6574 0a23 206c 6162 656c 733a 2070 6f73  et.# labels: pos
+00001100: 6974 6976 652c 206e 6567 6174 6976 652c  itive, negative,
+00001110: 206e 6575 7472 616c 0a58 2c20 7920 3d20   neutral.X, y = 
+00001120: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
+00001130: 6f6e 5f64 6174 6173 6574 2829 0a0a 636c  on_dataset()..cl
+00001140: 6620 3d20 5a65 726f 5368 6f74 4750 5443  f = ZeroShotGPTC
+00001150: 6c61 7373 6966 6965 7228 6f70 656e 6169  lassifier(openai
+00001160: 5f6d 6f64 656c 3d22 6770 742d 332e 352d  _model="gpt-3.5-
+00001170: 7475 7262 6f22 290a 636c 662e 6669 7428  turbo").clf.fit(
+00001180: 582c 2079 290a 6c61 6265 6c73 203d 2063  X, y).labels = c
+00001190: 6c66 2e70 7265 6469 6374 2858 290a 6060  lf.predict(X).``
+000011a0: 600a 0a53 6369 6b69 742d 4c4c 4d20 7769  `..Scikit-LLM wi
+000011b0: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+000011c0: 2071 7565 7279 2074 6865 204f 7065 6e41   query the OpenA
+000011d0: 4920 4150 4920 616e 6420 7472 616e 7366  I API and transf
+000011e0: 6f72 6d20 7468 6520 7265 7370 6f6e 7365  orm the response
+000011f0: 2069 6e74 6f20 6120 7265 6775 6c61 7220   into a regular 
+00001200: 6c69 7374 206f 6620 6c61 6265 6c73 2e0a  list of labels..
+00001210: 0a41 6464 6974 696f 6e61 6c6c 792c 2053  .Additionally, S
+00001220: 6369 6b69 742d 4c4c 4d20 7769 6c6c 2065  cikit-LLM will e
+00001230: 6e73 7572 6520 7468 6174 2074 6865 206f  nsure that the o
+00001240: 6274 6169 6e65 6420 7265 7370 6f6e 7365  btained response
+00001250: 2063 6f6e 7461 696e 7320 6120 7661 6c69   contains a vali
+00001260: 6420 6c61 6265 6c2e 2049 6620 7468 6973  d label. If this
+00001270: 2069 7320 6e6f 7420 7468 6520 6361 7365   is not the case
+00001280: 2c20 6120 6c61 6265 6c20 7769 6c6c 2062  , a label will b
+00001290: 6520 7365 6c65 6374 6564 2072 616e 646f  e selected rando
+000012a0: 6d6c 7920 286c 6162 656c 2070 726f 6261  mly (label proba
+000012b0: 6269 6c69 7469 6573 2061 7265 2070 726f  bilities are pro
+000012c0: 706f 7274 696f 6e61 6c20 746f 206c 6162  portional to lab
+000012d0: 656c 206f 6363 7572 7265 6e63 6573 2069  el occurrences i
+000012e0: 6e20 7468 6520 7472 6169 6e69 6e67 2073  n the training s
+000012f0: 6574 292e 0a0a 4578 616d 706c 6520 323a  et)...Example 2:
+00001300: 2054 7261 696e 696e 6720 7769 7468 6f75   Training withou
+00001310: 7420 6c61 6265 6c65 6420 6461 7461 0a0a  t labeled data..
+00001320: 5369 6e63 6520 7468 6520 7472 6169 6e69  Since the traini
+00001330: 6e67 2064 6174 6120 6973 206e 6f74 2073  ng data is not s
+00001340: 7472 6963 746c 7920 7265 7175 6972 6564  trictly required
+00001350: 2c20 6974 2063 616e 2062 6520 6675 6c6c  , it can be full
+00001360: 7920 6f6d 6d69 7465 642e 2054 6865 206f  y ommited. The o
+00001370: 6e6c 7920 7468 696e 6720 7468 6174 2068  nly thing that h
+00001380: 6173 2074 6f20 6265 2070 726f 7669 6465  as to be provide
+00001390: 6420 6973 2074 6865 206c 6973 7420 6f66  d is the list of
+000013a0: 2063 616e 6469 6461 7465 206c 6162 656c   candidate label
+000013b0: 732e 0a0a 6060 6070 7974 686f 6e0a 6672  s...```python.fr
+000013c0: 6f6d 2073 6b6c 6c6d 2069 6d70 6f72 7420  om skllm import 
+000013d0: 5a65 726f 5368 6f74 4750 5443 6c61 7373  ZeroShotGPTClass
+000013e0: 6966 6965 720a 6672 6f6d 2073 6b6c 6c6d  ifier.from skllm
+000013f0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00001400: 2067 6574 5f63 6c61 7373 6966 6963 6174   get_classificat
+00001410: 696f 6e5f 6461 7461 7365 740a 0a58 2c20  ion_dataset..X, 
+00001420: 5f20 3d20 6765 745f 636c 6173 7369 6669  _ = get_classifi
+00001430: 6361 7469 6f6e 5f64 6174 6173 6574 2829  cation_dataset()
+00001440: 0a0a 636c 6620 3d20 5a65 726f 5368 6f74  ..clf = ZeroShot
+00001450: 4750 5443 6c61 7373 6966 6965 7228 290a  GPTClassifier().
+00001460: 636c 662e 6669 7428 4e6f 6e65 2c20 5b22  clf.fit(None, ["
+00001470: 706f 7369 7469 7665 222c 2022 6e65 6761  positive", "nega
+00001480: 7469 7665 222c 2022 6e65 7574 7261 6c22  tive", "neutral"
+00001490: 5d29 0a6c 6162 656c 7320 3d20 636c 662e  ]).labels = clf.
+000014a0: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
+000014b0: 2a2a 4e6f 7465 3a2a 2a20 756e 6c69 6b65  **Note:** unlike
+000014c0: 2069 6e20 6120 7479 7069 6361 6c20 7375   in a typical su
+000014d0: 7065 7276 6973 6564 2073 6574 7469 6e67  pervised setting
+000014e0: 2c20 7468 6520 7065 7266 6f72 6d61 6e63  , the performanc
+000014f0: 6520 6f66 2061 207a 6572 6f2d 7368 6f74  e of a zero-shot
+00001500: 2063 6c61 7373 6966 6965 7220 6772 6561   classifier grea
+00001510: 746c 7920 6465 7065 6e64 7320 6f6e 2068  tly depends on h
+00001520: 6f77 2074 6865 206c 6162 656c 2069 7473  ow the label its
+00001530: 656c 6620 6973 2073 7472 7563 7475 7265  elf is structure
+00001540: 642e 2049 7420 6861 7320 746f 2062 6520  d. It has to be 
+00001550: 6578 7072 6573 7365 6420 696e 206e 6174  expressed in nat
+00001560: 7572 616c 206c 616e 6775 6167 652c 2062  ural language, b
+00001570: 6520 6465 7363 7269 7074 6976 6520 616e  e descriptive an
+00001580: 6420 7365 6c66 2d65 7870 6c61 6e61 746f  d self-explanato
+00001590: 7279 2e20 466f 7220 6578 616d 706c 652c  ry. For example,
+000015a0: 2069 6e20 7468 6520 7072 6576 696f 7573   in the previous
+000015b0: 2073 656d 616e 7469 6320 636c 6173 7369   semantic classi
+000015c0: 6669 6361 7469 6f6e 2074 6173 6b2c 2069  fication task, i
+000015d0: 7420 636f 756c 6420 6265 2062 656e 6566  t could be benef
+000015e0: 6963 6961 6c20 746f 2074 7261 6e73 666f  icial to transfo
+000015f0: 726d 2061 206c 6162 656c 2066 726f 6d20  rm a label from 
+00001600: 6022 3c73 656d 616e 7469 6373 3e22 6020  `"<semantics>"` 
+00001610: 746f 2060 2274 6865 2073 656d 616e 7469  to `"the semanti
+00001620: 6373 206f 6620 7468 6520 7072 6f76 6964  cs of the provid
+00001630: 6564 2074 6578 7420 6973 203c 7365 6d61  ed text is <sema
+00001640: 6e74 6963 733e 2260 2e0a 0a23 2323 204d  ntics>"`...### M
+00001650: 756c 7469 2d4c 6162 656c 205a 6572 6f2d  ulti-Label Zero-
+00001660: 5368 6f74 2054 6578 7420 436c 6173 7369  Shot Text Classi
+00001670: 6669 6361 7469 6f6e 0a0a 5769 7468 2061  fication..With a
+00001680: 2063 6c61 7373 2060 4d75 6c74 694c 6162   class `MultiLab
+00001690: 656c 5a65 726f 5368 6f74 4750 5443 6c61  elZeroShotGPTCla
+000016a0: 7373 6966 6965 7260 2069 7420 6973 2070  ssifier` it is p
+000016b0: 6f73 7369 626c 6520 746f 2070 6572 666f  ossible to perfo
+000016c0: 726d 2074 6865 2063 6c61 7373 6966 6963  rm the classific
+000016d0: 6174 696f 6e20 696e 206d 756c 7469 2d6c  ation in multi-l
+000016e0: 6162 656c 2073 6574 7469 6e67 2c20 7768  abel setting, wh
+000016f0: 6963 6820 6d65 616e 7320 7468 6174 2065  ich means that e
+00001700: 6163 6820 7361 6d70 6c65 206d 6967 6874  ach sample might
+00001710: 2062 6520 6173 7369 676e 6564 2074 6f20   be assigned to 
+00001720: 6f6e 6520 6f72 2073 6576 6572 616c 2064  one or several d
+00001730: 6973 7469 6e63 7420 636c 6173 7365 732e  istinct classes.
+00001740: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
+00001750: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
+00001760: 2069 6d70 6f72 7420 4d75 6c74 694c 6162   import MultiLab
+00001770: 656c 5a65 726f 5368 6f74 4750 5443 6c61  elZeroShotGPTCla
+00001780: 7373 6966 6965 720a 6672 6f6d 2073 6b6c  ssifier.from skl
+00001790: 6c6d 2e64 6174 6173 6574 7320 696d 706f  lm.datasets impo
+000017a0: 7274 2067 6574 5f6d 756c 7469 6c61 6265  rt get_multilabe
+000017b0: 6c5f 636c 6173 7369 6669 6361 7469 6f6e  l_classification
+000017c0: 5f64 6174 6173 6574 0a0a 582c 2079 203d  _dataset..X, y =
+000017d0: 2067 6574 5f6d 756c 7469 6c61 6265 6c5f   get_multilabel_
+000017e0: 636c 6173 7369 6669 6361 7469 6f6e 5f64  classification_d
+000017f0: 6174 6173 6574 2829 0a0a 636c 6620 3d20  ataset()..clf = 
+00001800: 4d75 6c74 694c 6162 656c 5a65 726f 5368  MultiLabelZeroSh
+00001810: 6f74 4750 5443 6c61 7373 6966 6965 7228  otGPTClassifier(
+00001820: 6d61 785f 6c61 6265 6c73 3d33 290a 636c  max_labels=3).cl
+00001830: 662e 6669 7428 582c 2079 290a 6c61 6265  f.fit(X, y).labe
+00001840: 6c73 203d 2063 6c66 2e70 7265 6469 6374  ls = clf.predict
+00001850: 2858 290a 6060 600a 0a53 696d 696c 6172  (X).```..Similar
+00001860: 6c79 2074 6f20 7468 6520 605a 6572 6f53  ly to the `ZeroS
+00001870: 686f 7447 5054 436c 6173 7369 6669 6572  hotGPTClassifier
+00001880: 6020 6974 2069 7320 7375 6666 6963 6965  ` it is sufficie
+00001890: 6e74 2069 6620 6f6e 6c79 2063 616e 6469  nt if only candi
+000018a0: 6461 7465 206c 6162 656c 7320 6172 6520  date labels are 
+000018b0: 7072 6f76 6964 6564 2e20 486f 7765 7665  provided. Howeve
+000018c0: 722c 2074 6869 7320 7469 6d65 2074 6865  r, this time the
+000018d0: 2063 6c61 7373 6966 6965 7220 6578 7065   classifier expe
+000018e0: 6374 7320 6079 6020 6f66 2061 2074 7970  cts `y` of a typ
+000018f0: 6520 604c 6973 745b 4c69 7374 5b73 7472  e `List[List[str
+00001900: 5d5d 602e 0a0a 6060 6070 7974 686f 6e0a  ]]`...```python.
+00001910: 6672 6f6d 2073 6b6c 6c6d 2069 6d70 6f72  from skllm impor
+00001920: 7420 4d75 6c74 694c 6162 656c 5a65 726f  t MultiLabelZero
+00001930: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+00001940: 720a 6672 6f6d 2073 6b6c 6c6d 2e64 6174  r.from skllm.dat
+00001950: 6173 6574 7320 696d 706f 7274 2067 6574  asets import get
+00001960: 5f6d 756c 7469 6c61 6265 6c5f 636c 6173  _multilabel_clas
+00001970: 7369 6669 6361 7469 6f6e 5f64 6174 6173  sification_datas
+00001980: 6574 0a0a 582c 205f 203d 2067 6574 5f6d  et..X, _ = get_m
+00001990: 756c 7469 6c61 6265 6c5f 636c 6173 7369  ultilabel_classi
+000019a0: 6669 6361 7469 6f6e 5f64 6174 6173 6574  fication_dataset
+000019b0: 2829 0a63 616e 6469 6461 7465 5f6c 6162  ().candidate_lab
+000019c0: 656c 7320 3d20 5b0a 2020 2020 2251 7561  els = [.    "Qua
+000019d0: 6c69 7479 222c 0a20 2020 2022 5072 6963  lity",.    "Pric
+000019e0: 6522 2c0a 2020 2020 2244 656c 6976 6572  e",.    "Deliver
+000019f0: 7922 2c0a 2020 2020 2253 6572 7669 6365  y",.    "Service
+00001a00: 222c 0a20 2020 2022 5072 6f64 7563 7420  ",.    "Product 
+00001a10: 5661 7269 6574 7922 2c0a 2020 2020 2243  Variety",.    "C
+00001a20: 7573 746f 6d65 7220 5375 7070 6f72 7422  ustomer Support"
+00001a30: 2c0a 2020 2020 2250 6163 6b61 6769 6e67  ,.    "Packaging
+00001a40: 222c 0a20 2020 2022 5573 6572 2045 7870  ",.    "User Exp
+00001a50: 6572 6965 6e63 6522 2c0a 2020 2020 2252  erience",.    "R
+00001a60: 6574 7572 6e20 506f 6c69 6379 222c 0a20  eturn Policy",. 
+00001a70: 2020 2022 5072 6f64 7563 7420 496e 666f     "Product Info
+00001a80: 726d 6174 696f 6e22 2c0a 5d0a 636c 6620  rmation",.].clf 
+00001a90: 3d20 4d75 6c74 694c 6162 656c 5a65 726f  = MultiLabelZero
+00001aa0: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+00001ab0: 7228 6d61 785f 6c61 6265 6c73 3d33 290a  r(max_labels=3).
+00001ac0: 636c 662e 6669 7428 4e6f 6e65 2c20 5b63  clf.fit(None, [c
+00001ad0: 616e 6469 6461 7465 5f6c 6162 656c 735d  andidate_labels]
+00001ae0: 290a 6c61 6265 6c73 203d 2063 6c66 2e70  ).labels = clf.p
+00001af0: 7265 6469 6374 2858 290a 6060 600a 0a23  redict(X).```..#
+00001b00: 2323 2046 6577 2d53 686f 7420 5465 7874  ## Few-Shot Text
+00001b10: 2043 6c61 7373 6966 6963 6174 696f 6e0a   Classification.
+00001b20: 0a57 6974 6820 6046 6577 5368 6f74 4750  .With `FewShotGP
+00001b30: 5443 6c61 7373 6966 6965 7260 2069 7420  TClassifier` it 
+00001b40: 6973 2070 6f73 7369 626c 6520 746f 2070  is possible to p
+00001b50: 6572 666f 726d 2061 2066 6577 2d73 686f  erform a few-sho
+00001b60: 7420 636c 6173 7369 6669 6361 7469 6f6e  t classification
+00001b70: 2c20 7768 6963 6820 6d65 616e 7320 7468  , which means th
+00001b80: 6174 2074 6865 2074 7261 696e 696e 6720  at the training 
+00001b90: 7361 6d70 6c65 7320 7769 6c6c 2062 6520  samples will be 
+00001ba0: 6164 6465 6420 746f 2070 726f 6d70 7420  added to prompt 
+00001bb0: 616e 6420 7061 7373 6564 2074 6f20 7468  and passed to th
+00001bc0: 6520 6d6f 6465 6c2e 0a0a 6060 6070 7974  e model...```pyt
+00001bd0: 686f 6e0a 6672 6f6d 2073 6b6c 6c6d 2069  hon.from skllm i
+00001be0: 6d70 6f72 7420 4665 7753 686f 7447 5054  mport FewShotGPT
+00001bf0: 436c 6173 7369 6669 6572 0a66 726f 6d20  Classifier.from 
+00001c00: 736b 6c6c 6d2e 6461 7461 7365 7473 2069  skllm.datasets i
+00001c10: 6d70 6f72 7420 6765 745f 636c 6173 7369  mport get_classi
+00001c20: 6669 6361 7469 6f6e 5f64 6174 6173 6574  fication_dataset
+00001c30: 0a0a 582c 2079 203d 2067 6574 5f63 6c61  ..X, y = get_cla
+00001c40: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
+00001c50: 7365 7428 290a 0a63 6c66 203d 2046 6577  set()..clf = Few
+00001c60: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+00001c70: 7228 6f70 656e 6169 5f6d 6f64 656c 3d22  r(openai_model="
+00001c80: 6770 742d 332e 352d 7475 7262 6f22 290a  gpt-3.5-turbo").
+00001c90: 636c 662e 6669 7428 582c 2079 290a 6c61  clf.fit(X, y).la
+00001ca0: 6265 6c73 203d 2063 6c66 2e70 7265 6469  bels = clf.predi
+00001cb0: 6374 2858 290a 6060 600a 0a57 6869 6c65  ct(X).```..While
+00001cc0: 2074 6865 2061 7069 2072 656d 6169 6e73   the api remains
+00001cd0: 2074 6865 2073 616d 6520 6173 2066 6f72   the same as for
+00001ce0: 2074 6865 207a 6572 6f20 7368 6f74 2063   the zero shot c
+00001cf0: 6c61 7373 6966 6965 722c 2074 6865 7265  lassifier, there
+00001d00: 2061 7265 2061 2066 6577 2074 6869 6e67   are a few thing
+00001d10: 7320 746f 2074 616b 6520 696e 746f 2061  s to take into a
+00001d20: 6363 6f75 6e74 3a0a 0a2d 2074 6865 2022  ccount:..- the "
+00001d30: 7472 6169 6e69 6e67 2220 7265 7175 6972  training" requir
+00001d40: 6573 2073 6f6d 6520 6c61 6265 6c6c 6564  es some labelled
+00001d50: 2074 7261 696e 696e 6720 6461 7461 3b0a   training data;.
+00001d60: 2d20 7468 6520 7472 6169 6e69 6e67 2073  - the training s
+00001d70: 6574 2073 686f 756c 6420 6265 2073 6d61  et should be sma
+00001d80: 6c6c 2065 6e6f 7567 6820 746f 2066 6974  ll enough to fit
+00001d90: 2069 6e74 6f20 6120 7369 6e67 6c65 2070   into a single p
+00001da0: 726f 6d70 7420 2877 6520 7265 636f 6d6d  rompt (we recomm
+00001db0: 656e 6420 7570 2074 6f20 3130 2073 616d  end up to 10 sam
+00001dc0: 706c 6573 2070 6572 206c 6162 656c 293b  ples per label);
+00001dd0: 0a2d 2062 6563 6175 7365 206f 6620 7468  .- because of th
+00001de0: 6520 7369 676e 6966 6963 616e 746c 7920  e significantly 
+00001df0: 6c61 7267 6572 2070 726f 6d70 742c 2074  larger prompt, t
+00001e00: 6865 2069 6e66 6572 656e 6365 2074 616b  he inference tak
+00001e10: 6573 206c 6f6e 6765 7220 616e 6420 636f  es longer and co
+00001e20: 6e73 756d 6573 2068 6967 6865 7220 616d  nsumes higher am
+00001e30: 6f75 6e74 206f 6620 746f 6b65 6e73 2e0a  ount of tokens..
+00001e40: 0a4e 6f74 653a 2061 7320 7468 6520 6d6f  .Note: as the mo
+00001e50: 6465 6c20 6973 206e 6f74 2062 6569 6e67  del is not being
+00001e60: 2072 652d 7472 6169 6e65 642c 2062 7574   re-trained, but
+00001e70: 2075 7365 7320 7468 6520 7472 6169 6e69   uses the traini
+00001e80: 6e67 2064 6174 6120 6475 7269 6e67 2069  ng data during i
+00001e90: 6e66 6572 656e 6365 2c20 6f6e 6520 636f  nference, one co
+00001ea0: 756c 6420 7361 7920 7468 6174 2074 6869  uld say that thi
+00001eb0: 7320 6973 2073 7469 6c6c 2061 2028 6469  s is still a (di
+00001ec0: 6666 6572 656e 7429 207a 6572 6f2d 7368  fferent) zero-sh
+00001ed0: 6f74 2061 7070 726f 6163 682e 0a0a 2323  ot approach...##
+00001ee0: 2320 4479 6e61 6d69 6320 4665 772d 5368  # Dynamic Few-Sh
+00001ef0: 6f74 2054 6578 7420 436c 6173 7369 6669  ot Text Classifi
+00001f00: 6361 7469 6f6e 0a0a 6044 796e 616d 6963  cation..`Dynamic
+00001f10: 4665 7753 686f 7447 5054 436c 6173 7369  FewShotGPTClassi
+00001f20: 6669 6572 6020 6479 6e61 6d69 6361 6c6c  fier` dynamicall
+00001f30: 7920 7365 6c65 6374 7320 4e20 7361 6d70  y selects N samp
+00001f40: 6c65 7320 7065 7220 636c 6173 7320 746f  les per class to
+00001f50: 2069 6e63 6c75 6465 2069 6e20 7468 6520   include in the 
+00001f60: 7072 6f6d 7074 2e20 5468 6973 2061 6c6c  prompt. This all
+00001f70: 6f77 7320 7468 6520 6665 772d 7368 6f74  ows the few-shot
+00001f80: 2063 6c61 7373 6966 6965 7220 746f 2073   classifier to s
+00001f90: 6361 6c65 2074 6f20 6461 7461 7365 7473  cale to datasets
+00001fa0: 2074 6861 7420 6172 6520 746f 6f20 6c61   that are too la
+00001fb0: 7267 6520 666f 7220 7468 6520 7374 616e  rge for the stan
+00001fc0: 6461 7264 2063 6f6e 7465 7874 2077 696e  dard context win
+00001fd0: 646f 7720 6f66 204c 4c4d 732e 0a0a 2a48  dow of LLMs...*H
+00001fe0: 6f77 2064 6f65 7320 6974 2077 6f72 6b3f  ow does it work?
+00001ff0: 2a0a 0a44 7572 696e 6720 6669 7474 696e  *..During fittin
+00002000: 672c 2074 6865 2077 686f 6c65 2064 6174  g, the whole dat
+00002010: 6173 6574 2069 7320 7061 7274 6974 696f  aset is partitio
+00002020: 6e65 6420 6279 2063 6c61 7373 2c20 7665  ned by class, ve
+00002030: 6374 6f72 697a 6564 2c20 616e 6420 7374  ctorized, and st
+00002040: 6f72 6564 2e0a 0a44 7572 696e 6720 696e  ored...During in
+00002050: 6665 7265 6e63 652c 2074 6865 205b 616e  ference, the [an
+00002060: 6e6f 795d 2868 7474 7073 3a2f 2f67 6974  noy](https://git
+00002070: 6875 622e 636f 6d2f 7370 6f74 6966 792f  hub.com/spotify/
+00002080: 616e 6e6f 7929 206c 6962 7261 7279 2069  annoy) library i
+00002090: 7320 7573 6564 2066 6f72 2066 6173 7420  s used for fast 
+000020a0: 6e65 6967 6862 6f72 206c 6f6f 6b75 702c  neighbor lookup,
+000020b0: 2077 6869 6368 2061 6c6c 6f77 7320 696e   which allows in
+000020c0: 636c 7564 696e 6720 6f6e 6c79 2074 6865  cluding only the
+000020d0: 206d 6f73 7420 7369 6d69 6c61 7220 6578   most similar ex
+000020e0: 616d 706c 6573 2069 6e20 7468 6520 7072  amples in the pr
+000020f0: 6f6d 7074 2e0a 0a60 6060 7079 7468 6f6e  ompt...```python
+00002100: 0a66 726f 6d20 736b 6c6c 6d20 696d 706f  .from skllm impo
+00002110: 7274 2044 796e 616d 6963 4665 7753 686f  rt DynamicFewSho
+00002120: 7447 5054 436c 6173 7369 6669 6572 0a66  tGPTClassifier.f
+00002130: 726f 6d20 736b 6c6c 6d2e 6461 7461 7365  rom skllm.datase
+00002140: 7473 2069 6d70 6f72 7420 6765 745f 636c  ts import get_cl
+00002150: 6173 7369 6669 6361 7469 6f6e 5f64 6174  assification_dat
+00002160: 6173 6574 0a0a 582c 2079 203d 2067 6574  aset..X, y = get
+00002170: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00002180: 6461 7461 7365 7428 290a 0a63 6c66 203d  dataset()..clf =
+00002190: 2044 796e 616d 6963 4665 7753 686f 7447   DynamicFewShotG
+000021a0: 5054 436c 6173 7369 6669 6572 286e 5f65  PTClassifier(n_e
+000021b0: 7861 6d70 6c65 733d 3329 0a63 6c66 2e66  xamples=3).clf.f
+000021c0: 6974 2858 2c20 7929 0a6c 6162 656c 7320  it(X, y).labels 
+000021d0: 3d20 636c 662e 7072 6564 6963 7428 5829  = clf.predict(X)
+000021e0: 0a60 6060 0a0a 2323 2320 5465 7874 2043  .```..### Text C
+000021f0: 6c61 7373 6966 6963 6174 696f 6e20 7769  lassification wi
+00002200: 7468 2047 6f6f 676c 6520 5061 4c4d 2032  th Google PaLM 2
+00002210: 0a0a 4174 2074 6865 206d 6f6d 656e 7420  ..At the moment 
+00002220: 3320 5061 4c4d 2062 6173 6564 206d 6f64  3 PaLM based mod
+00002230: 656c 7320 6172 6520 6176 6169 6c61 626c  els are availabl
+00002240: 6520 696e 2074 6573 7420 6d6f 6465 3a0a  e in test mode:.
+00002250: 2d20 605a 6572 6f53 686f 7450 614c 4d43  - `ZeroShotPaLMC
+00002260: 6c61 7373 6966 6965 7260 202d 207a 6572  lassifier` - zer
+00002270: 6f2d 7368 6f74 2074 6578 7420 636c 6173  o-shot text clas
+00002280: 7369 6669 6361 7469 6f6e 2077 6974 6820  sification with 
+00002290: 5061 4c4d 2032 3b0a 2d20 6050 614c 4d43  PaLM 2;.- `PaLMC
+000022a0: 6c61 7373 6966 6965 7260 202d 2066 696e  lassifier` - fin
+000022b0: 652d 7475 6e61 626c 6520 7465 7874 2063  e-tunable text c
+000022c0: 6c61 7373 6966 6965 7220 7769 7468 2050  lassifier with P
+000022d0: 614c 4d20 323b 0a2d 2060 5061 4c4d 6020  aLM 2;.- `PaLM` 
+000022e0: 2d20 6669 6e65 2d74 756e 6162 6c65 2065  - fine-tunable e
+000022f0: 7374 696d 6174 6f72 2074 6861 7420 6361  stimator that ca
+00002300: 6e20 6265 2074 7261 696e 6564 206f 6e20  n be trained on 
+00002310: 6172 6269 7472 6172 7920 7465 7874 2069  arbitrary text i
+00002320: 6e70 7574 2d6f 7574 7075 7420 7061 6972  nput-output pair
+00002330: 732e 0a0a 4578 616d 706c 653a 200a 0a60  s...Example: ..`
+00002340: 6060 7079 7468 6f6e 0a66 726f 6d20 736b  ``python.from sk
+00002350: 6c6c 6d2e 6d6f 6465 6c73 2e70 616c 6d20  llm.models.palm 
+00002360: 696d 706f 7274 2050 614c 4d43 6c61 7373  import PaLMClass
+00002370: 6966 6965 720a 6672 6f6d 2073 6b6c 6c6d  ifier.from skllm
+00002380: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00002390: 2067 6574 5f63 6c61 7373 6966 6963 6174   get_classificat
+000023a0: 696f 6e5f 6461 7461 7365 740a 0a58 2c20  ion_dataset..X, 
+000023b0: 7920 3d20 6765 745f 636c 6173 7369 6669  y = get_classifi
+000023c0: 6361 7469 6f6e 5f64 6174 6173 6574 2829  cation_dataset()
+000023d0: 0a0a 636c 6620 3d20 5061 4c4d 436c 6173  ..clf = PaLMClas
+000023e0: 7369 6669 6572 286e 5f75 7064 6174 655f  sifier(n_update_
+000023f0: 7374 6570 733d 3130 3029 0a63 6c66 2e66  steps=100).clf.f
+00002400: 6974 2858 2c20 7929 0a6c 6162 656c 7320  it(X, y).labels 
+00002410: 3d20 636c 662e 7072 6564 6963 7428 5829  = clf.predict(X)
+00002420: 0a60 6060 0a0a 4120 6d6f 7265 2064 6574  .```..A more det
+00002430: 6169 6c65 6420 646f 6375 6d65 6e74 6174  ailed documentat
+00002440: 696f 6e20 7769 6c6c 2066 6f6c 6c6f 7720  ion will follow 
+00002450: 736f 6f6e 2e20 466f 7220 6e6f 772c 2070  soon. For now, p
+00002460: 6c65 6173 6520 7265 6665 7220 746f 206f  lease refer to o
+00002470: 7572 205b 6f66 6669 6369 616c 2067 7569  ur [official gui
+00002480: 6465 206f 6e20 4d65 6469 756d 5d28 6874  de on Medium](ht
+00002490: 7470 733a 2f2f 6d65 6469 756d 2e63 6f6d  tps://medium.com
+000024a0: 2f40 6972 796e 6132 3330 3532 3029 2e0a  /@iryna230520)..
+000024b0: 0a23 2323 2054 6578 7420 5665 6374 6f72  .### Text Vector
+000024c0: 697a 6174 696f 6e0a 0a41 7320 616e 2061  ization..As an a
+000024d0: 6c74 6572 6e61 7469 7665 2074 6f20 7573  lternative to us
+000024e0: 696e 6720 4750 5420 6173 2061 2063 6c61  ing GPT as a cla
+000024f0: 7373 6966 6965 722c 2069 7420 6361 6e20  ssifier, it can 
+00002500: 6265 2075 7365 6420 736f 6c65 6c79 2066  be used solely f
+00002510: 6f72 2064 6174 6120 7072 6570 726f 6365  or data preproce
+00002520: 7373 696e 672e 2060 4750 5456 6563 746f  ssing. `GPTVecto
+00002530: 7269 7a65 7260 2061 6c6c 6f77 7320 746f  rizer` allows to
+00002540: 2065 6d62 6564 2061 2063 6875 6e6b 206f   embed a chunk o
+00002550: 6620 7465 7874 206f 6620 6172 6269 7472  f text of arbitr
+00002560: 6172 7920 6c65 6e67 7468 2074 6f20 6120  ary length to a 
+00002570: 6669 7865 642d 6469 6d65 6e73 696f 6e61  fixed-dimensiona
+00002580: 6c20 7665 6374 6f72 2c20 7468 6174 2063  l vector, that c
+00002590: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
+000025a0: 7669 7274 7561 6c6c 7920 616e 7920 636c  virtually any cl
+000025b0: 6173 7369 6669 6361 7469 6f6e 206f 7220  assification or 
+000025c0: 7265 6772 6573 7369 6f6e 206d 6f64 656c  regression model
+000025d0: 2e0a 0a45 7861 6d70 6c65 2031 3a20 456d  ...Example 1: Em
+000025e0: 6265 6464 696e 6720 7468 6520 7465 7874  bedding the text
+000025f0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00002600: 2073 6b6c 6c6d 2e70 7265 7072 6f63 6573   skllm.preproces
+00002610: 7369 6e67 2069 6d70 6f72 7420 4750 5456  sing import GPTV
+00002620: 6563 746f 7269 7a65 720a 0a6d 6f64 656c  ectorizer..model
+00002630: 203d 2047 5054 5665 6374 6f72 697a 6572   = GPTVectorizer
+00002640: 2829 0a76 6563 746f 7273 203d 206d 6f64  ().vectors = mod
+00002650: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
+00002660: 2858 290a 6060 600a 0a45 7861 6d70 6c65  (X).```..Example
+00002670: 2032 3a20 436f 6d62 696e 696e 6720 7468   2: Combining th
+00002680: 6520 5665 6374 6f72 697a 6572 2077 6974  e Vectorizer wit
+00002690: 6820 7468 6520 5847 426f 6f73 7420 436c  h the XGBoost Cl
+000026a0: 6173 7369 6669 6572 2069 6e20 6120 536b  assifier in a Sk
+000026b0: 6c65 6172 6e20 5069 7065 6c69 6e65 0a0a  learn Pipeline..
+000026c0: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
+000026d0: 6b6c 6561 726e 2e70 6970 656c 696e 6520  klearn.pipeline 
+000026e0: 696d 706f 7274 2050 6970 656c 696e 650a  import Pipeline.
+000026f0: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
+00002700: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
+00002710: 7420 4c61 6265 6c45 6e63 6f64 6572 0a66  t LabelEncoder.f
+00002720: 726f 6d20 7867 626f 6f73 7420 696d 706f  rom xgboost impo
+00002730: 7274 2058 4742 436c 6173 7369 6669 6572  rt XGBClassifier
+00002740: 0a0a 6c65 203d 204c 6162 656c 456e 636f  ..le = LabelEnco
+00002750: 6465 7228 290a 795f 7472 6169 6e5f 656e  der().y_train_en
+00002760: 636f 6465 6420 3d20 6c65 2e66 6974 5f74  coded = le.fit_t
+00002770: 7261 6e73 666f 726d 2879 5f74 7261 696e  ransform(y_train
+00002780: 290a 795f 7465 7374 5f65 6e63 6f64 6564  ).y_test_encoded
+00002790: 203d 206c 652e 7472 616e 7366 6f72 6d28   = le.transform(
+000027a0: 795f 7465 7374 290a 0a73 7465 7073 203d  y_test)..steps =
+000027b0: 205b 2822 4750 5422 2c20 4750 5456 6563   [("GPT", GPTVec
+000027c0: 746f 7269 7a65 7228 2929 2c20 2822 436c  torizer()), ("Cl
+000027d0: 6622 2c20 5847 4243 6c61 7373 6966 6965  f", XGBClassifie
+000027e0: 7228 2929 5d0a 636c 6620 3d20 5069 7065  r())].clf = Pipe
+000027f0: 6c69 6e65 2873 7465 7073 290a 636c 662e  line(steps).clf.
+00002800: 6669 7428 585f 7472 6169 6e2c 2079 5f74  fit(X_train, y_t
+00002810: 7261 696e 5f65 6e63 6f64 6564 290a 7968  rain_encoded).yh
+00002820: 203d 2063 6c66 2e70 7265 6469 6374 2858   = clf.predict(X
+00002830: 5f74 6573 7429 0a60 6060 0a0a 2323 2320  _test).```..### 
+00002840: 5465 7874 2053 756d 6d61 7269 7a61 7469  Text Summarizati
+00002850: 6f6e 0a0a 4750 5420 6578 6365 6c73 2061  on..GPT excels a
+00002860: 7420 7065 7266 6f72 6d69 6e67 2073 756d  t performing sum
+00002870: 6d61 7269 7a61 7469 6f6e 2074 6173 6b73  marization tasks
+00002880: 2e20 5468 6572 6566 6f72 652c 2077 6520  . Therefore, we 
+00002890: 7072 6f76 6964 6520 6047 5054 5375 6d6d  provide `GPTSumm
+000028a0: 6172 697a 6572 6020 7468 6174 2063 616e  arizer` that can
+000028b0: 2062 6520 7573 6564 2062 6f74 6820 6173   be used both as
+000028c0: 2073 7461 6e64 2d61 6c6f 6e65 2065 7374   stand-alone est
+000028d0: 696d 6174 6f72 2c20 6f72 2061 7320 6120  imator, or as a 
+000028e0: 7072 6570 726f 6365 7373 6f72 2028 696e  preprocessor (in
+000028f0: 2074 6869 7320 6361 7365 2077 6520 6361   this case we ca
+00002900: 6e20 6d61 6b65 2061 6e20 616e 616c 6f67  n make an analog
+00002910: 7920 7769 7468 2061 2064 696d 656e 7369  y with a dimensi
+00002920: 6f6e 616c 6974 7920 7265 6475 6374 696f  onality reductio
+00002930: 6e20 7072 6570 726f 6365 7373 6f72 292e  n preprocessor).
+00002940: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
+00002950: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
+00002960: 2e70 7265 7072 6f63 6573 7369 6e67 2069  .preprocessing i
+00002970: 6d70 6f72 7420 4750 5453 756d 6d61 7269  mport GPTSummari
+00002980: 7a65 720a 6672 6f6d 2073 6b6c 6c6d 2e64  zer.from skllm.d
+00002990: 6174 6173 6574 7320 696d 706f 7274 2067  atasets import g
+000029a0: 6574 5f73 756d 6d61 7269 7a61 7469 6f6e  et_summarization
+000029b0: 5f64 6174 6173 6574 0a0a 5820 3d20 6765  _dataset..X = ge
+000029c0: 745f 7375 6d6d 6172 697a 6174 696f 6e5f  t_summarization_
+000029d0: 6461 7461 7365 7428 290a 7320 3d20 4750  dataset().s = GP
+000029e0: 5453 756d 6d61 7269 7a65 7228 6f70 656e  TSummarizer(open
+000029f0: 6169 5f6d 6f64 656c 3d22 6770 742d 332e  ai_model="gpt-3.
+00002a00: 352d 7475 7262 6f22 2c20 6d61 785f 776f  5-turbo", max_wo
+00002a10: 7264 733d 3135 290a 7375 6d6d 6172 6965  rds=15).summarie
+00002a20: 7320 3d20 732e 6669 745f 7472 616e 7366  s = s.fit_transf
+00002a30: 6f72 6d28 5829 0a60 6060 0a0a 506c 6561  orm(X).```..Plea
+00002a40: 7365 2062 6520 6177 6172 6520 7468 6174  se be aware that
+00002a50: 2074 6865 2060 6d61 785f 776f 7264 7360   the `max_words`
+00002a60: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
+00002a70: 7365 7473 2061 2073 6f66 7420 6c69 6d69  sets a soft limi
+00002a80: 742c 2077 6869 6368 2069 7320 6e6f 7420  t, which is not 
+00002a90: 7374 7269 6374 6c79 2065 6e66 6f72 6365  strictly enforce
+00002aa0: 6420 6f75 7473 6964 6520 6f66 2074 6865  d outside of the
+00002ab0: 2070 726f 6d70 742e 2054 6865 7265 666f   prompt. Therefo
+00002ac0: 7265 2c20 696e 2073 6f6d 6520 6361 7365  re, in some case
+00002ad0: 732c 2074 6865 2061 6374 7561 6c20 6e75  s, the actual nu
+00002ae0: 6d62 6572 206f 6620 776f 7264 7320 6d69  mber of words mi
+00002af0: 6768 7420 6265 2073 6c69 6768 746c 7920  ght be slightly 
+00002b00: 6869 6768 6572 2e0a 0a49 7420 6973 2070  higher...It is p
+00002b10: 6f73 7369 626c 6520 746f 2067 656e 6572  ossible to gener
+00002b20: 6174 6520 6120 7375 6d6d 6172 792c 2065  ate a summary, e
+00002b30: 6d70 6861 7369 7a69 6e67 2061 2073 7065  mphasizing a spe
+00002b40: 6369 6669 6320 636f 6e63 6570 742c 2062  cific concept, b
+00002b50: 7920 7072 6f76 6964 696e 6720 616e 206f  y providing an o
+00002b60: 7074 696f 6e61 6c20 7061 7261 6d65 7465  ptional paramete
+00002b70: 7220 6066 6f63 7573 603a 0a0a 6060 6070  r `focus`:..```p
+00002b80: 7974 686f 6e0a 7320 3d20 4750 5453 756d  ython.s = GPTSum
+00002b90: 6d61 7269 7a65 7228 6f70 656e 6169 5f6d  marizer(openai_m
+00002ba0: 6f64 656c 3d22 6770 742d 332e 352d 7475  odel="gpt-3.5-tu
+00002bb0: 7262 6f22 2c20 6d61 785f 776f 7264 733d  rbo", max_words=
+00002bc0: 3135 2c20 666f 6375 733d 2261 7070 6c65  15, focus="apple
+00002bd0: 7322 290a 6060 600a 0a23 2323 2054 6578  s").```..### Tex
+00002be0: 7420 5472 616e 736c 6174 696f 6e0a 0a47  t Translation..G
+00002bf0: 5054 206d 6f64 656c 7320 6861 7665 2064  PT models have d
+00002c00: 656d 6f6e 7374 7261 7465 6420 7468 6569  emonstrated thei
+00002c10: 7220 6566 6665 6374 6976 656e 6573 7320  r effectiveness 
+00002c20: 696e 2074 7261 6e73 6c61 7469 6f6e 2074  in translation t
+00002c30: 6173 6b73 2062 7920 6765 6e65 7261 7469  asks by generati
+00002c40: 6e67 2061 6363 7572 6174 6520 7472 616e  ng accurate tran
+00002c50: 736c 6174 696f 6e73 2061 6372 6f73 7320  slations across 
+00002c60: 7661 7269 6f75 7320 6c61 6e67 7561 6765  various language
+00002c70: 732e 2054 6875 732c 2077 6520 6164 6465  s. Thus, we adde
+00002c80: 6420 6047 5054 5472 616e 736c 6174 6f72  d `GPTTranslator
+00002c90: 6020 7468 6174 2061 6c6c 6f77 7320 7472  ` that allows tr
+00002ca0: 616e 736c 6174 696e 6720 616e 2061 7262  anslating an arb
+00002cb0: 6974 7261 7479 2074 6578 7420 696e 746f  itraty text into
+00002cc0: 2061 206c 616e 6775 6167 6520 6f66 2069   a language of i
+00002cd0: 6e74 6572 6573 742e 0a0a 4578 616d 706c  nterest...Exampl
+00002ce0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
+00002cf0: 6f6d 2073 6b6c 6c6d 2e70 7265 7072 6f63  om skllm.preproc
+00002d00: 6573 7369 6e67 2069 6d70 6f72 7420 4750  essing import GP
+00002d10: 5454 7261 6e73 6c61 746f 720a 6672 6f6d  TTranslator.from
+00002d20: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
+00002d30: 696d 706f 7274 2067 6574 5f74 7261 6e73  import get_trans
+00002d40: 6c61 7469 6f6e 5f64 6174 6173 6574 0a0a  lation_dataset..
+00002d50: 5820 3d20 6765 745f 7472 616e 736c 6174  X = get_translat
+00002d60: 696f 6e5f 6461 7461 7365 7428 290a 7420  ion_dataset().t 
+00002d70: 3d20 4750 5454 7261 6e73 6c61 746f 7228  = GPTTranslator(
+00002d80: 6f70 656e 6169 5f6d 6f64 656c 3d22 6770  openai_model="gp
+00002d90: 742d 332e 352d 7475 7262 6f22 2c20 6f75  t-3.5-turbo", ou
+00002da0: 7470 7574 5f6c 616e 6775 6167 653d 2245  tput_language="E
+00002db0: 6e67 6c69 7368 2229 0a74 7261 6e73 6c61  nglish").transla
+00002dc0: 7465 645f 7465 7874 203d 2074 2e66 6974  ted_text = t.fit
+00002dd0: 5f74 7261 6e73 666f 726d 2858 290a 6060  _transform(X).``
+00002de0: 600a 0a                                  `..
```

### Comparing `scikit-llm-0.2.0/pyproject.toml` & `scikit-llm-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 [project]
 dependencies = [
   "scikit-learn>=1.1.0",
   "pandas>=1.5.0",
   "openai>=0.27.0",
   "tqdm>=4.60.0",
   "annoy>=1.17.2",
+  "google-cloud-aiplatform>=1.27.0",
+  "vertexai<0.1.0"
 ]
 name = "scikit-llm"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
 ]
 description = "Scikit-LLM: Seamlessly integrate powerful language models like ChatGPT into scikit-learn for enhanced text analysis tasks."
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `scikit-llm-0.2.0/scikit_llm.egg-info/PKG-INFO` & `scikit-llm-0.3.0/scikit_llm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7363 696b  : 2.1.Name: scik
 00000020: 6974 2d6c 6c6d 0a56 6572 7369 6f6e 3a20  it-llm.Version: 
-00000030: 302e 322e 300a 5375 6d6d 6172 793a 2053  0.2.0.Summary: S
+00000030: 302e 332e 300a 5375 6d6d 6172 793a 2053  0.3.0.Summary: S
 00000040: 6369 6b69 742d 4c4c 4d3a 2053 6561 6d6c  cikit-LLM: Seaml
 00000050: 6573 736c 7920 696e 7465 6772 6174 6520  essly integrate 
 00000060: 706f 7765 7266 756c 206c 616e 6775 6167  powerful languag
 00000070: 6520 6d6f 6465 6c73 206c 696b 6520 4368  e models like Ch
 00000080: 6174 4750 5420 696e 746f 2073 6369 6b69  atGPT into sciki
 00000090: 742d 6c65 6172 6e20 666f 7220 656e 6861  t-learn for enha
 000000a0: 6e63 6564 2074 6578 7420 616e 616c 7973  nced text analys
@@ -60,631 +60,710 @@
 000003b0: 6f6a 6563 7420 696e 2074 6865 2066 6f6c  oject in the fol
 000003c0: 6c6f 7769 6e67 2077 6179 733a 0a0a 2d20  lowing ways:..- 
 000003d0: e2ad 9020 5374 6172 2053 6369 6b69 742d  ... Star Scikit-
 000003e0: 4c4c 4d20 6f6e 2047 6974 4875 6220 2863  LLM on GitHub (c
 000003f0: 6c69 636b 2074 6865 2073 7461 7220 6275  lick the star bu
 00000400: 7474 6f6e 2069 6e20 7468 6520 746f 7020  tton in the top 
 00000410: 7269 6768 7420 636f 726e 6572 290a 2d20  right corner).- 
-00000420: f09f 90a6 2043 6865 636b 206f 7574 206f  .... Check out o
-00000430: 7572 2072 656c 6174 6564 2070 726f 6a65  ur related proje
-00000440: 6374 202d 205b 4661 6c63 6f6e 2041 7574  ct - [Falcon Aut
-00000450: 6f4d 4c5d 2868 7474 7073 3a2f 2f67 6974  oML](https://git
-00000460: 6875 622e 636f 6d2f 4f4b 5541 312f 6661  hub.com/OKUA1/fa
-00000470: 6c63 6f6e 290a 2d20 f09f 92a1 2050 726f  lcon).- .... Pro
-00000480: 7669 6465 2079 6f75 7220 6665 6564 6261  vide your feedba
-00000490: 636b 206f 7220 7072 6f70 6f73 6520 6964  ck or propose id
-000004a0: 6561 7320 696e 2074 6865 205b 6973 7375  eas in the [issu
-000004b0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000004c0: 7562 2e63 6f6d 2f69 7279 6e61 2d6b 6f6e  ub.com/iryna-kon
-000004d0: 6472 2f73 6369 6b69 742d 6c6c 6d2f 6973  dr/scikit-llm/is
-000004e0: 7375 6573 2920 7365 6374 696f 6e20 6f72  sues) section or
-000004f0: 205b 4469 7363 6f72 645d 2868 7474 7073   [Discord](https
-00000500: 3a2f 2f64 6973 636f 7264 2e67 672f 5944  ://discord.gg/YD
-00000510: 4162 7775 574b 3756 290a 2d20 f09f 9497  AbwuWK7V).- ....
-00000520: 2050 6f73 7420 6162 6f75 7420 5363 696b   Post about Scik
-00000530: 6974 2d4c 4c4d 206f 6e20 4c69 6e6b 6564  it-LLM on Linked
-00000540: 496e 206f 7220 6f74 6865 7220 706c 6174  In or other plat
-00000550: 666f 726d 730a 0a23 2320 446f 6375 6d65  forms..## Docume
-00000560: 6e74 6174 696f 6e20 f09f 939a 0a0a 2323  ntation ......##
-00000570: 2320 436f 6e66 6967 7572 696e 6720 4f70  # Configuring Op
-00000580: 656e 4149 2041 5049 204b 6579 0a0a 4174  enAI API Key..At
-00000590: 2074 6865 206d 6f6d 656e 7420 7468 6520   the moment the 
-000005a0: 6d61 6a6f 7269 7479 206f 6620 7468 6520  majority of the 
-000005b0: 5363 696b 6974 2d4c 4c4d 2065 7374 696d  Scikit-LLM estim
-000005c0: 6174 6f72 7320 6172 6520 6f6e 6c79 2063  ators are only c
-000005d0: 6f6d 7061 7469 626c 6520 7769 7468 2073  ompatible with s
-000005e0: 6f6d 6520 6f66 2074 6865 204f 7065 6e41  ome of the OpenA
-000005f0: 4920 6d6f 6465 6c73 2e20 4865 6e63 652c  I models. Hence,
-00000600: 2061 2075 7365 722d 7072 6f76 6964 6564   a user-provided
-00000610: 204f 7065 6e41 4920 4150 4920 6b65 7920   OpenAI API key 
-00000620: 6973 2072 6571 7569 7265 642e 0a0a 6060  is required...``
-00000630: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
-00000640: 6c6d 2e63 6f6e 6669 6720 696d 706f 7274  lm.config import
-00000650: 2053 4b4c 4c4d 436f 6e66 6967 0a0a 534b   SKLLMConfig..SK
-00000660: 4c4c 4d43 6f6e 6669 672e 7365 745f 6f70  LLMConfig.set_op
-00000670: 656e 6169 5f6b 6579 2822 3c59 4f55 525f  enai_key("<YOUR_
-00000680: 4b45 593e 2229 0a53 4b4c 4c4d 436f 6e66  KEY>").SKLLMConf
-00000690: 6967 2e73 6574 5f6f 7065 6e61 695f 6f72  ig.set_openai_or
-000006a0: 6728 223c 594f 5552 5f4f 5247 414e 4953  g("<YOUR_ORGANIS
-000006b0: 4154 494f 4e3e 2229 0a60 6060 0a0a 2a2a  ATION>").```..**
-000006c0: 496d 706f 7274 616e 7420 6e6f 7469 6365  Important notice
-000006d0: 3a2a 2a0a 0a2d 2049 6620 796f 7520 6861  :**..- If you ha
-000006e0: 7665 2061 2066 7265 6520 7472 6961 6c20  ve a free trial 
-000006f0: 4f70 656e 4149 2061 6363 6f75 6e74 2c20  OpenAI account, 
-00000700: 7468 6520 5b72 6174 6520 6c69 6d69 7473  the [rate limits
-00000710: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
-00000720: 726d 2e6f 7065 6e61 692e 636f 6d2f 646f  rm.openai.com/do
-00000730: 6373 2f67 7569 6465 732f 7261 7465 2d6c  cs/guides/rate-l
-00000740: 696d 6974 732f 6f76 6572 7669 6577 2920  imits/overview) 
-00000750: 6172 6520 6e6f 7420 7375 6666 6963 6965  are not sufficie
-00000760: 6e74 2028 7370 6563 6966 6963 616c 6c79  nt (specifically
-00000770: 2033 2072 6571 7565 7374 7320 7065 7220   3 requests per 
-00000780: 6d69 6e75 7465 292e 2050 6c65 6173 6520  minute). Please 
-00000790: 7377 6974 6368 2074 6f20 7468 6520 2270  switch to the "p
-000007a0: 6179 2061 7320 796f 7520 676f 2220 706c  ay as you go" pl
-000007b0: 616e 2066 6972 7374 2e0a 2d20 5768 656e  an first..- When
-000007c0: 2063 616c 6c69 6e67 2060 534b 4c4c 4d43   calling `SKLLMC
-000007d0: 6f6e 6669 672e 7365 745f 6f70 656e 6169  onfig.set_openai
-000007e0: 5f6f 7267 602c 2079 6f75 2068 6176 6520  _org`, you have 
-000007f0: 746f 2070 726f 7669 6465 2079 6f75 7220  to provide your 
-00000800: 6f72 6761 6e69 7a61 7469 6f6e 2049 4420  organization ID 
-00000810: 616e 6420 2a2a 4e4f 542a 2a20 7468 6520  and **NOT** the 
-00000820: 6e61 6d65 2e20 596f 7520 6361 6e20 6669  name. You can fi
-00000830: 6e64 2079 6f75 7220 4944 205b 6865 7265  nd your ID [here
-00000840: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
-00000850: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
-00000860: 636f 756e 742f 6f72 672d 7365 7474 696e  count/org-settin
-00000870: 6773 292e 0a0a 2323 2320 5573 696e 6720  gs)...### Using 
-00000880: 4750 5434 414c 4c0a 0a49 6e20 6164 6469  GPT4ALL..In addi
-00000890: 7469 6f6e 2074 6f20 4f70 656e 4149 2c20  tion to OpenAI, 
-000008a0: 736f 6d65 206f 6620 7468 6520 6d6f 6465  some of the mode
-000008b0: 6c73 2063 616e 2075 7365 205b 6770 7434  ls can use [gpt4
-000008c0: 616c 6c5d 2868 7474 7073 3a2f 2f67 7074  all](https://gpt
-000008d0: 3461 6c6c 2e69 6f2f 696e 6465 782e 6874  4all.io/index.ht
-000008e0: 6d6c 2920 6173 2061 2062 6163 6b65 6e64  ml) as a backend
-000008f0: 2e0a 0a2a 2a54 6869 7320 6665 6174 7572  ...**This featur
-00000900: 6520 6973 2063 6f6e 7369 6465 7265 6420  e is considered 
-00000910: 6869 676c 7920 6578 7065 7269 6d65 6e74  higly experiment
-00000920: 616c 212a 2a0a 0a49 6e20 6f72 6465 7220  al!**..In order 
-00000930: 746f 2075 7365 2067 7074 3461 6c6c 2c20  to use gpt4all, 
-00000940: 796f 7520 6e65 6564 2074 6f20 696e 7374  you need to inst
-00000950: 616c 6c20 7468 6520 636f 7272 6573 706f  all the correspo
-00000960: 6e64 696e 6720 7375 626d 6f64 756c 653a  nding submodule:
-00000970: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00000980: 7374 616c 6c20 2273 6369 6b69 742d 6c6c  stall "scikit-ll
-00000990: 6d5b 6770 7434 616c 6c5d 220a 6060 600a  m[gpt4all]".```.
-000009a0: 0a49 6e20 6f72 6465 7220 746f 2073 7769  .In order to swi
-000009b0: 7463 6820 6672 6f6d 204f 7065 6e41 4920  tch from OpenAI 
-000009c0: 746f 2047 5054 3441 4c4c 206d 6f64 656c  to GPT4ALL model
-000009d0: 2c20 7369 6d70 6c79 2070 726f 7669 6465  , simply provide
-000009e0: 2061 2073 7472 696e 6720 6f66 2074 6865   a string of the
-000009f0: 2066 6f72 6d61 7420 6067 7074 3461 6c6c   format `gpt4all
-00000a00: 3a3a 3c6d 6f64 656c 5f6e 616d 653e 6020  ::<model_name>` 
-00000a10: 6173 2061 6e20 6172 6775 6d65 6e74 2e20  as an argument. 
-00000a20: 5768 696c 6520 7468 6520 6d6f 6465 6c20  While the model 
-00000a30: 7275 6e73 2063 6f6d 706c 6574 656c 7920  runs completely 
-00000a40: 6c6f 6361 6c6c 792c 2074 6865 2065 7374  locally, the est
-00000a50: 696d 6174 6f72 2073 7469 6c6c 2074 7265  imator still tre
-00000a60: 6174 7320 6974 2061 7320 616e 204f 7065  ats it as an Ope
-00000a70: 6e41 4920 656e 6470 6f69 6e74 2061 6e64  nAI endpoint and
-00000a80: 2077 696c 6c20 7472 7920 746f 2063 6865   will try to che
-00000a90: 636b 2074 6861 7420 7468 6520 4150 4920  ck that the API 
-00000aa0: 6b65 7920 6973 2070 7265 7365 6e74 2e20  key is present. 
-00000ab0: 596f 7520 6361 6e20 7072 6f76 6964 6520  You can provide 
-00000ac0: 616e 7920 7374 7269 6e67 2061 7320 6120  any string as a 
-00000ad0: 6b65 792e 0a0a 6060 6070 7974 686f 6e0a  key...```python.
-00000ae0: 534b 4c4c 4d43 6f6e 6669 672e 7365 745f  SKLLMConfig.set_
-00000af0: 6f70 656e 6169 5f6b 6579 2822 616e 7920  openai_key("any 
-00000b00: 7374 7269 6e67 2229 0a53 4b4c 4c4d 436f  string").SKLLMCo
-00000b10: 6e66 6967 2e73 6574 5f6f 7065 6e61 695f  nfig.set_openai_
-00000b20: 6f72 6728 2261 6e79 2073 7472 696e 6722  org("any string"
-00000b30: 290a 0a5a 6572 6f53 686f 7447 5054 436c  )..ZeroShotGPTCl
-00000b40: 6173 7369 6669 6572 286f 7065 6e61 695f  assifier(openai_
-00000b50: 6d6f 6465 6c3d 2267 7074 3461 6c6c 3a3a  model="gpt4all::
-00000b60: 6767 6d6c 2d67 7074 3461 6c6c 2d6a 2d76  ggml-gpt4all-j-v
-00000b70: 312e 332d 6772 6f6f 7679 2229 0a60 6060  1.3-groovy").```
-00000b80: 0a0a 5768 656e 2072 756e 6e69 6e67 2066  ..When running f
-00000b90: 6f72 2074 6865 2066 6972 7374 2074 696d  or the first tim
-00000ba0: 652c 2074 6865 206d 6f64 656c 2066 696c  e, the model fil
-00000bb0: 6520 7769 6c6c 2062 6520 646f 776e 6c6f  e will be downlo
-00000bc0: 6164 6564 2061 7574 6f6d 6174 6961 6c6c  aded automatiall
-00000bd0: 792e 0a0a 4174 2074 6865 206d 6f6d 656e  y...At the momen
-00000be0: 7420 6f6e 6c79 2074 6865 2066 6f6c 6c6f  t only the follo
-00000bf0: 7769 6e67 2065 7374 696d 6174 6f72 7320  wing estimators 
-00000c00: 7375 7070 6f72 7420 6770 7434 616c 6c20  support gpt4all 
-00000c10: 6173 2061 2062 6163 6b65 6e64 3a0a 0a2d  as a backend:..-
-00000c20: 2060 5a65 726f 5368 6f74 4750 5443 6c61   `ZeroShotGPTCla
-00000c30: 7373 6966 6965 7260 0a2d 2060 4d75 6c74  ssifier`.- `Mult
-00000c40: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
-00000c50: 5443 6c61 7373 6966 6965 7260 0a2d 2060  TClassifier`.- `
-00000c60: 4665 7753 686f 7447 5054 436c 6173 7369  FewShotGPTClassi
-00000c70: 6669 6572 600a 0a57 6865 6e20 7573 696e  fier`..When usin
-00000c80: 6720 6770 7434 616c 6c20 706c 6561 7365  g gpt4all please
-00000c90: 206b 6565 7020 7468 6520 666f 6c6c 6f77   keep the follow
-00000ca0: 696e 6720 696e 206d 696e 643a 0a0a 312e  ing in mind:..1.
-00000cb0: 204e 6f74 2061 6c6c 2067 7074 3461 6c6c   Not all gpt4all
-00000cc0: 206d 6f64 656c 7320 6172 6520 636f 6d6d   models are comm
-00000cd0: 6572 6369 616c 6c79 206c 6963 656e 7361  ercially licensa
-00000ce0: 626c 652c 2070 6c65 6173 6520 636f 6e73  ble, please cons
-00000cf0: 756c 7420 6770 7434 616c 6c20 7765 6273  ult gpt4all webs
-00000d00: 6974 6520 666f 7220 6d6f 7265 2064 6574  ite for more det
-00000d10: 6169 6c73 2e0a 322e 2054 6865 2061 6363  ails..2. The acc
-00000d20: 7572 6163 7920 6f66 2074 6865 206d 6f64  uracy of the mod
-00000d30: 656c 7320 6d61 7920 6265 206d 7563 6820  els may be much 
-00000d40: 6c6f 7765 7220 636f 6d70 6172 6564 2074  lower compared t
-00000d50: 6f20 6f6e 6573 2070 726f 7669 6465 6420  o ones provided 
-00000d60: 6279 204f 7065 6e41 4920 2865 7370 6563  by OpenAI (espec
-00000d70: 6961 6c6c 7920 6770 742d 3429 2e0a 332e  ially gpt-4)..3.
-00000d80: 204e 6f74 2061 6c6c 206f 6620 7468 6520   Not all of the 
-00000d90: 6176 6169 6c61 626c 6520 6d6f 6465 6c73  available models
-00000da0: 2077 6572 6520 7465 7374 6564 2c20 736f   were tested, so
-00000db0: 6d65 206d 6179 206e 6f74 2077 6f72 6b20  me may not work 
-00000dc0: 7769 7468 2073 6369 6b69 742d 6c6c 6d20  with scikit-llm 
-00000dd0: 6174 2061 6c6c 2e0a 0a23 2323 205a 6572  at all...### Zer
-00000de0: 6f2d 5368 6f74 2054 6578 7420 436c 6173  o-Shot Text Clas
-00000df0: 7369 6669 6361 7469 6f6e 0a0a 4f6e 6520  sification..One 
-00000e00: 6f66 2074 6865 2070 6f77 6572 6675 6c20  of the powerful 
-00000e10: 4368 6174 4750 5420 6665 6174 7572 6573  ChatGPT features
-00000e20: 2069 7320 7468 6520 6162 696c 6974 7920   is the ability 
-00000e30: 746f 2070 6572 666f 726d 2074 6578 7420  to perform text 
-00000e40: 636c 6173 7369 6669 6361 7469 6f6e 2077  classification w
-00000e50: 6974 686f 7574 2062 6569 6e67 2072 652d  ithout being re-
-00000e60: 7472 6169 6e65 642e 2046 6f72 2074 6861  trained. For tha
-00000e70: 742c 2074 6865 206f 6e6c 7920 7265 7175  t, the only requ
-00000e80: 6972 656d 656e 7420 6973 2074 6861 7420  irement is that 
-00000e90: 7468 6520 6c61 6265 6c73 206d 7573 7420  the labels must 
-00000ea0: 6265 2064 6573 6372 6970 7469 7665 2e0a  be descriptive..
-00000eb0: 0a57 6520 7072 6f76 6964 6520 6120 636c  .We provide a cl
-00000ec0: 6173 7320 605a 6572 6f53 686f 7447 5054  ass `ZeroShotGPT
-00000ed0: 436c 6173 7369 6669 6572 6020 7468 6174  Classifier` that
-00000ee0: 2061 6c6c 6f77 7320 746f 2063 7265 6174   allows to creat
-00000ef0: 6520 7375 6368 2061 206d 6f64 656c 2061  e such a model a
-00000f00: 7320 6120 7265 6775 6c61 7220 7363 696b  s a regular scik
-00000f10: 6974 2d6c 6561 726e 2063 6c61 7373 6966  it-learn classif
-00000f20: 6965 722e 0a0a 4578 616d 706c 6520 313a  ier...Example 1:
-00000f30: 2054 7261 696e 696e 6720 6173 2061 2072   Training as a r
-00000f40: 6567 756c 6172 2063 6c61 7373 6966 6965  egular classifie
-00000f50: 720a 0a60 6060 7079 7468 6f6e 0a66 726f  r..```python.fro
-00000f60: 6d20 736b 6c6c 6d20 696d 706f 7274 205a  m skllm import Z
-00000f70: 6572 6f53 686f 7447 5054 436c 6173 7369  eroShotGPTClassi
-00000f80: 6669 6572 0a66 726f 6d20 736b 6c6c 6d2e  fier.from skllm.
-00000f90: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
-00000fa0: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
-00000fb0: 6f6e 5f64 6174 6173 6574 0a0a 2320 6465  on_dataset..# de
-00000fc0: 6d6f 2073 656e 7469 6d65 6e74 2061 6e61  mo sentiment ana
-00000fd0: 6c79 7369 7320 6461 7461 7365 740a 2320  lysis dataset.# 
-00000fe0: 6c61 6265 6c73 3a20 706f 7369 7469 7665  labels: positive
-00000ff0: 2c20 6e65 6761 7469 7665 2c20 6e65 7574  , negative, neut
-00001000: 7261 6c0a 582c 2079 203d 2067 6574 5f63  ral.X, y = get_c
-00001010: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
-00001020: 7461 7365 7428 290a 0a63 6c66 203d 205a  taset()..clf = Z
-00001030: 6572 6f53 686f 7447 5054 436c 6173 7369  eroShotGPTClassi
-00001040: 6669 6572 286f 7065 6e61 695f 6d6f 6465  fier(openai_mode
-00001050: 6c3d 2267 7074 2d33 2e35 2d74 7572 626f  l="gpt-3.5-turbo
-00001060: 2229 0a63 6c66 2e66 6974 2858 2c20 7929  ").clf.fit(X, y)
-00001070: 0a6c 6162 656c 7320 3d20 636c 662e 7072  .labels = clf.pr
-00001080: 6564 6963 7428 5829 0a60 6060 0a0a 5363  edict(X).```..Sc
-00001090: 696b 6974 2d4c 4c4d 2077 696c 6c20 6175  ikit-LLM will au
-000010a0: 746f 6d61 7469 6361 6c6c 7920 7175 6572  tomatically quer
-000010b0: 7920 7468 6520 4f70 656e 4149 2041 5049  y the OpenAI API
-000010c0: 2061 6e64 2074 7261 6e73 666f 726d 2074   and transform t
-000010d0: 6865 2072 6573 706f 6e73 6520 696e 746f  he response into
-000010e0: 2061 2072 6567 756c 6172 206c 6973 7420   a regular list 
-000010f0: 6f66 206c 6162 656c 732e 0a0a 4164 6469  of labels...Addi
-00001100: 7469 6f6e 616c 6c79 2c20 5363 696b 6974  tionally, Scikit
-00001110: 2d4c 4c4d 2077 696c 6c20 656e 7375 7265  -LLM will ensure
-00001120: 2074 6861 7420 7468 6520 6f62 7461 696e   that the obtain
-00001130: 6564 2072 6573 706f 6e73 6520 636f 6e74  ed response cont
-00001140: 6169 6e73 2061 2076 616c 6964 206c 6162  ains a valid lab
-00001150: 656c 2e20 4966 2074 6869 7320 6973 206e  el. If this is n
-00001160: 6f74 2074 6865 2063 6173 652c 2061 206c  ot the case, a l
-00001170: 6162 656c 2077 696c 6c20 6265 2073 656c  abel will be sel
-00001180: 6563 7465 6420 7261 6e64 6f6d 6c79 2028  ected randomly (
-00001190: 6c61 6265 6c20 7072 6f62 6162 696c 6974  label probabilit
-000011a0: 6965 7320 6172 6520 7072 6f70 6f72 7469  ies are proporti
-000011b0: 6f6e 616c 2074 6f20 6c61 6265 6c20 6f63  onal to label oc
-000011c0: 6375 7272 656e 6365 7320 696e 2074 6865  currences in the
-000011d0: 2074 7261 696e 696e 6720 7365 7429 2e0a   training set)..
-000011e0: 0a45 7861 6d70 6c65 2032 3a20 5472 6169  .Example 2: Trai
-000011f0: 6e69 6e67 2077 6974 686f 7574 206c 6162  ning without lab
-00001200: 656c 6564 2064 6174 610a 0a53 696e 6365  eled data..Since
-00001210: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001220: 7461 2069 7320 6e6f 7420 7374 7269 6374  ta is not strict
-00001230: 6c79 2072 6571 7569 7265 642c 2069 7420  ly required, it 
-00001240: 6361 6e20 6265 2066 756c 6c79 206f 6d6d  can be fully omm
-00001250: 6974 6564 2e20 5468 6520 6f6e 6c79 2074  ited. The only t
-00001260: 6869 6e67 2074 6861 7420 6861 7320 746f  hing that has to
-00001270: 2062 6520 7072 6f76 6964 6564 2069 7320   be provided is 
-00001280: 7468 6520 6c69 7374 206f 6620 6361 6e64  the list of cand
-00001290: 6964 6174 6520 6c61 6265 6c73 2e0a 0a60  idate labels...`
-000012a0: 6060 7079 7468 6f6e 0a66 726f 6d20 736b  ``python.from sk
-000012b0: 6c6c 6d20 696d 706f 7274 205a 6572 6f53  llm import ZeroS
-000012c0: 686f 7447 5054 436c 6173 7369 6669 6572  hotGPTClassifier
-000012d0: 0a66 726f 6d20 736b 6c6c 6d2e 6461 7461  .from skllm.data
-000012e0: 7365 7473 2069 6d70 6f72 7420 6765 745f  sets import get_
-000012f0: 636c 6173 7369 6669 6361 7469 6f6e 5f64  classification_d
-00001300: 6174 6173 6574 0a0a 582c 205f 203d 2067  ataset..X, _ = g
-00001310: 6574 5f63 6c61 7373 6966 6963 6174 696f  et_classificatio
-00001320: 6e5f 6461 7461 7365 7428 290a 0a63 6c66  n_dataset()..clf
-00001330: 203d 205a 6572 6f53 686f 7447 5054 436c   = ZeroShotGPTCl
-00001340: 6173 7369 6669 6572 2829 0a63 6c66 2e66  assifier().clf.f
-00001350: 6974 284e 6f6e 652c 205b 2270 6f73 6974  it(None, ["posit
-00001360: 6976 6522 2c20 226e 6567 6174 6976 6522  ive", "negative"
-00001370: 2c20 226e 6575 7472 616c 225d 290a 6c61  , "neutral"]).la
-00001380: 6265 6c73 203d 2063 6c66 2e70 7265 6469  bels = clf.predi
-00001390: 6374 2858 290a 6060 600a 0a2a 2a4e 6f74  ct(X).```..**Not
-000013a0: 653a 2a2a 2075 6e6c 696b 6520 696e 2061  e:** unlike in a
-000013b0: 2074 7970 6963 616c 2073 7570 6572 7669   typical supervi
-000013c0: 7365 6420 7365 7474 696e 672c 2074 6865  sed setting, the
-000013d0: 2070 6572 666f 726d 616e 6365 206f 6620   performance of 
-000013e0: 6120 7a65 726f 2d73 686f 7420 636c 6173  a zero-shot clas
-000013f0: 7369 6669 6572 2067 7265 6174 6c79 2064  sifier greatly d
-00001400: 6570 656e 6473 206f 6e20 686f 7720 7468  epends on how th
-00001410: 6520 6c61 6265 6c20 6974 7365 6c66 2069  e label itself i
-00001420: 7320 7374 7275 6374 7572 6564 2e20 4974  s structured. It
-00001430: 2068 6173 2074 6f20 6265 2065 7870 7265   has to be expre
-00001440: 7373 6564 2069 6e20 6e61 7475 7261 6c20  ssed in natural 
-00001450: 6c61 6e67 7561 6765 2c20 6265 2064 6573  language, be des
-00001460: 6372 6970 7469 7665 2061 6e64 2073 656c  criptive and sel
-00001470: 662d 6578 706c 616e 6174 6f72 792e 2046  f-explanatory. F
-00001480: 6f72 2065 7861 6d70 6c65 2c20 696e 2074  or example, in t
-00001490: 6865 2070 7265 7669 6f75 7320 7365 6d61  he previous sema
-000014a0: 6e74 6963 2063 6c61 7373 6966 6963 6174  ntic classificat
-000014b0: 696f 6e20 7461 736b 2c20 6974 2063 6f75  ion task, it cou
-000014c0: 6c64 2062 6520 6265 6e65 6669 6369 616c  ld be beneficial
-000014d0: 2074 6f20 7472 616e 7366 6f72 6d20 6120   to transform a 
-000014e0: 6c61 6265 6c20 6672 6f6d 2060 223c 7365  label from `"<se
-000014f0: 6d61 6e74 6963 733e 2260 2074 6f20 6022  mantics>"` to `"
-00001500: 7468 6520 7365 6d61 6e74 6963 7320 6f66  the semantics of
-00001510: 2074 6865 2070 726f 7669 6465 6420 7465   the provided te
-00001520: 7874 2069 7320 3c73 656d 616e 7469 6373  xt is <semantics
-00001530: 3e22 602e 0a0a 2323 2320 4d75 6c74 692d  >"`...### Multi-
-00001540: 4c61 6265 6c20 5a65 726f 2d53 686f 7420  Label Zero-Shot 
-00001550: 5465 7874 2043 6c61 7373 6966 6963 6174  Text Classificat
-00001560: 696f 6e0a 0a57 6974 6820 6120 636c 6173  ion..With a clas
-00001570: 7320 604d 756c 7469 4c61 6265 6c5a 6572  s `MultiLabelZer
-00001580: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001590: 6572 6020 6974 2069 7320 706f 7373 6962  er` it is possib
-000015a0: 6c65 2074 6f20 7065 7266 6f72 6d20 7468  le to perform th
-000015b0: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
-000015c0: 2069 6e20 6d75 6c74 692d 6c61 6265 6c20   in multi-label 
-000015d0: 7365 7474 696e 672c 2077 6869 6368 206d  setting, which m
-000015e0: 6561 6e73 2074 6861 7420 6561 6368 2073  eans that each s
-000015f0: 616d 706c 6520 6d69 6768 7420 6265 2061  ample might be a
-00001600: 7373 6967 6e65 6420 746f 206f 6e65 206f  ssigned to one o
-00001610: 7220 7365 7665 7261 6c20 6469 7374 696e  r several distin
-00001620: 6374 2063 6c61 7373 6573 2e0a 0a45 7861  ct classes...Exa
-00001630: 6d70 6c65 3a0a 0a60 6060 7079 7468 6f6e  mple:..```python
-00001640: 0a66 726f 6d20 736b 6c6c 6d20 696d 706f  .from skllm impo
-00001650: 7274 204d 756c 7469 4c61 6265 6c5a 6572  rt MultiLabelZer
-00001660: 6f53 686f 7447 5054 436c 6173 7369 6669  oShotGPTClassifi
-00001670: 6572 0a66 726f 6d20 736b 6c6c 6d2e 6461  er.from skllm.da
-00001680: 7461 7365 7473 2069 6d70 6f72 7420 6765  tasets import ge
-00001690: 745f 6d75 6c74 696c 6162 656c 5f63 6c61  t_multilabel_cla
-000016a0: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
-000016b0: 7365 740a 0a58 2c20 7920 3d20 6765 745f  set..X, y = get_
-000016c0: 6d75 6c74 696c 6162 656c 5f63 6c61 7373  multilabel_class
-000016d0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
-000016e0: 7428 290a 0a63 6c66 203d 204d 756c 7469  t()..clf = Multi
-000016f0: 4c61 6265 6c5a 6572 6f53 686f 7447 5054  LabelZeroShotGPT
-00001700: 436c 6173 7369 6669 6572 286d 6178 5f6c  Classifier(max_l
-00001710: 6162 656c 733d 3329 0a63 6c66 2e66 6974  abels=3).clf.fit
-00001720: 2858 2c20 7929 0a6c 6162 656c 7320 3d20  (X, y).labels = 
-00001730: 636c 662e 7072 6564 6963 7428 5829 0a60  clf.predict(X).`
-00001740: 6060 0a0a 5369 6d69 6c61 726c 7920 746f  ``..Similarly to
-00001750: 2074 6865 2060 5a65 726f 5368 6f74 4750   the `ZeroShotGP
-00001760: 5443 6c61 7373 6966 6965 7260 2069 7420  TClassifier` it 
-00001770: 6973 2073 7566 6669 6369 656e 7420 6966  is sufficient if
-00001780: 206f 6e6c 7920 6361 6e64 6964 6174 6520   only candidate 
-00001790: 6c61 6265 6c73 2061 7265 2070 726f 7669  labels are provi
-000017a0: 6465 642e 2048 6f77 6576 6572 2c20 7468  ded. However, th
-000017b0: 6973 2074 696d 6520 7468 6520 636c 6173  is time the clas
-000017c0: 7369 6669 6572 2065 7870 6563 7473 2060  sifier expects `
-000017d0: 7960 206f 6620 6120 7479 7065 2060 4c69  y` of a type `Li
-000017e0: 7374 5b4c 6973 745b 7374 725d 5d60 2e0a  st[List[str]]`..
-000017f0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00001800: 736b 6c6c 6d20 696d 706f 7274 204d 756c  skllm import Mul
-00001810: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
-00001820: 5054 436c 6173 7369 6669 6572 0a66 726f  PTClassifier.fro
-00001830: 6d20 736b 6c6c 6d2e 6461 7461 7365 7473  m skllm.datasets
-00001840: 2069 6d70 6f72 7420 6765 745f 6d75 6c74   import get_mult
-00001850: 696c 6162 656c 5f63 6c61 7373 6966 6963  ilabel_classific
-00001860: 6174 696f 6e5f 6461 7461 7365 740a 0a58  ation_dataset..X
-00001870: 2c20 5f20 3d20 6765 745f 6d75 6c74 696c  , _ = get_multil
-00001880: 6162 656c 5f63 6c61 7373 6966 6963 6174  abel_classificat
-00001890: 696f 6e5f 6461 7461 7365 7428 290a 6361  ion_dataset().ca
-000018a0: 6e64 6964 6174 655f 6c61 6265 6c73 203d  ndidate_labels =
-000018b0: 205b 0a20 2020 2022 5175 616c 6974 7922   [.    "Quality"
-000018c0: 2c0a 2020 2020 2250 7269 6365 222c 0a20  ,.    "Price",. 
-000018d0: 2020 2022 4465 6c69 7665 7279 222c 0a20     "Delivery",. 
-000018e0: 2020 2022 5365 7276 6963 6522 2c0a 2020     "Service",.  
-000018f0: 2020 2250 726f 6475 6374 2056 6172 6965    "Product Varie
-00001900: 7479 222c 0a20 2020 2022 4375 7374 6f6d  ty",.    "Custom
-00001910: 6572 2053 7570 706f 7274 222c 0a20 2020  er Support",.   
-00001920: 2022 5061 636b 6167 696e 6722 2c0a 2020   "Packaging",.  
-00001930: 2020 2255 7365 7220 4578 7065 7269 656e    "User Experien
-00001940: 6365 222c 0a20 2020 2022 5265 7475 726e  ce",.    "Return
-00001950: 2050 6f6c 6963 7922 2c0a 2020 2020 2250   Policy",.    "P
-00001960: 726f 6475 6374 2049 6e66 6f72 6d61 7469  roduct Informati
-00001970: 6f6e 222c 0a5d 0a63 6c66 203d 204d 756c  on",.].clf = Mul
-00001980: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
-00001990: 5054 436c 6173 7369 6669 6572 286d 6178  PTClassifier(max
-000019a0: 5f6c 6162 656c 733d 3329 0a63 6c66 2e66  _labels=3).clf.f
-000019b0: 6974 284e 6f6e 652c 205b 6361 6e64 6964  it(None, [candid
-000019c0: 6174 655f 6c61 6265 6c73 5d29 0a6c 6162  ate_labels]).lab
-000019d0: 656c 7320 3d20 636c 662e 7072 6564 6963  els = clf.predic
-000019e0: 7428 5829 0a60 6060 0a0a 2323 2320 4665  t(X).```..### Fe
-000019f0: 772d 5368 6f74 2054 6578 7420 436c 6173  w-Shot Text Clas
-00001a00: 7369 6669 6361 7469 6f6e 0a0a 5769 7468  sification..With
-00001a10: 2060 4665 7753 686f 7447 5054 436c 6173   `FewShotGPTClas
-00001a20: 7369 6669 6572 6020 6974 2069 7320 706f  sifier` it is po
-00001a30: 7373 6962 6c65 2074 6f20 7065 7266 6f72  ssible to perfor
-00001a40: 6d20 6120 6665 772d 7368 6f74 2063 6c61  m a few-shot cla
-00001a50: 7373 6966 6963 6174 696f 6e2c 2077 6869  ssification, whi
-00001a60: 6368 206d 6561 6e73 2074 6861 7420 7468  ch means that th
-00001a70: 6520 7472 6169 6e69 6e67 2073 616d 706c  e training sampl
-00001a80: 6573 2077 696c 6c20 6265 2061 6464 6564  es will be added
-00001a90: 2074 6f20 7072 6f6d 7074 2061 6e64 2070   to prompt and p
-00001aa0: 6173 7365 6420 746f 2074 6865 206d 6f64  assed to the mod
-00001ab0: 656c 2e0a 0a60 6060 7079 7468 6f6e 0a66  el...```python.f
-00001ac0: 726f 6d20 736b 6c6c 6d20 696d 706f 7274  rom skllm import
-00001ad0: 2046 6577 5368 6f74 4750 5443 6c61 7373   FewShotGPTClass
-00001ae0: 6966 6965 720a 6672 6f6d 2073 6b6c 6c6d  ifier.from skllm
-00001af0: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
-00001b00: 2067 6574 5f63 6c61 7373 6966 6963 6174   get_classificat
-00001b10: 696f 6e5f 6461 7461 7365 740a 0a58 2c20  ion_dataset..X, 
-00001b20: 7920 3d20 6765 745f 636c 6173 7369 6669  y = get_classifi
-00001b30: 6361 7469 6f6e 5f64 6174 6173 6574 2829  cation_dataset()
-00001b40: 0a0a 636c 6620 3d20 4665 7753 686f 7447  ..clf = FewShotG
-00001b50: 5054 436c 6173 7369 6669 6572 286f 7065  PTClassifier(ope
-00001b60: 6e61 695f 6d6f 6465 6c3d 2267 7074 2d33  nai_model="gpt-3
-00001b70: 2e35 2d74 7572 626f 2229 0a63 6c66 2e66  .5-turbo").clf.f
-00001b80: 6974 2858 2c20 7929 0a6c 6162 656c 7320  it(X, y).labels 
-00001b90: 3d20 636c 662e 7072 6564 6963 7428 5829  = clf.predict(X)
-00001ba0: 0a60 6060 0a0a 5768 696c 6520 7468 6520  .```..While the 
-00001bb0: 6170 6920 7265 6d61 696e 7320 7468 6520  api remains the 
-00001bc0: 7361 6d65 2061 7320 666f 7220 7468 6520  same as for the 
-00001bd0: 7a65 726f 2073 686f 7420 636c 6173 7369  zero shot classi
-00001be0: 6669 6572 2c20 7468 6572 6520 6172 6520  fier, there are 
-00001bf0: 6120 6665 7720 7468 696e 6773 2074 6f20  a few things to 
-00001c00: 7461 6b65 2069 6e74 6f20 6163 636f 756e  take into accoun
-00001c10: 743a 0a0a 2d20 7468 6520 2274 7261 696e  t:..- the "train
-00001c20: 696e 6722 2072 6571 7569 7265 7320 736f  ing" requires so
-00001c30: 6d65 206c 6162 656c 6c65 6420 7472 6169  me labelled trai
-00001c40: 6e69 6e67 2064 6174 613b 0a2d 2074 6865  ning data;.- the
-00001c50: 2074 7261 696e 696e 6720 7365 7420 7368   training set sh
-00001c60: 6f75 6c64 2062 6520 736d 616c 6c20 656e  ould be small en
-00001c70: 6f75 6768 2074 6f20 6669 7420 696e 746f  ough to fit into
-00001c80: 2061 2073 696e 676c 6520 7072 6f6d 7074   a single prompt
-00001c90: 2028 7765 2072 6563 6f6d 6d65 6e64 2075   (we recommend u
-00001ca0: 7020 746f 2031 3020 7361 6d70 6c65 7320  p to 10 samples 
-00001cb0: 7065 7220 6c61 6265 6c29 3b0a 2d20 6265  per label);.- be
-00001cc0: 6361 7573 6520 6f66 2074 6865 2073 6967  cause of the sig
-00001cd0: 6e69 6669 6361 6e74 6c79 206c 6172 6765  nificantly large
-00001ce0: 7220 7072 6f6d 7074 2c20 7468 6520 696e  r prompt, the in
-00001cf0: 6665 7265 6e63 6520 7461 6b65 7320 6c6f  ference takes lo
-00001d00: 6e67 6572 2061 6e64 2063 6f6e 7375 6d65  nger and consume
-00001d10: 7320 6869 6768 6572 2061 6d6f 756e 7420  s higher amount 
-00001d20: 6f66 2074 6f6b 656e 732e 0a0a 4e6f 7465  of tokens...Note
-00001d30: 3a20 6173 2074 6865 206d 6f64 656c 2069  : as the model i
-00001d40: 7320 6e6f 7420 6265 696e 6720 7265 2d74  s not being re-t
-00001d50: 7261 696e 6564 2c20 6275 7420 7573 6573  rained, but uses
-00001d60: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-00001d70: 7461 2064 7572 696e 6720 696e 6665 7265  ta during infere
-00001d80: 6e63 652c 206f 6e65 2063 6f75 6c64 2073  nce, one could s
-00001d90: 6179 2074 6861 7420 7468 6973 2069 7320  ay that this is 
-00001da0: 7374 696c 6c20 6120 2864 6966 6665 7265  still a (differe
-00001db0: 6e74 2920 7a65 726f 2d73 686f 7420 6170  nt) zero-shot ap
-00001dc0: 7072 6f61 6368 2e0a 0a23 2323 2044 796e  proach...### Dyn
-00001dd0: 616d 6963 2046 6577 2d53 686f 7420 5465  amic Few-Shot Te
-00001de0: 7874 2043 6c61 7373 6966 6963 6174 696f  xt Classificatio
-00001df0: 6e0a 0a60 4479 6e61 6d69 6346 6577 5368  n..`DynamicFewSh
-00001e00: 6f74 4750 5443 6c61 7373 6966 6965 7260  otGPTClassifier`
-00001e10: 2064 796e 616d 6963 616c 6c79 2073 656c   dynamically sel
-00001e20: 6563 7473 204e 2073 616d 706c 6573 2070  ects N samples p
-00001e30: 6572 2063 6c61 7373 2074 6f20 696e 636c  er class to incl
-00001e40: 7564 6520 696e 2074 6865 2070 726f 6d70  ude in the promp
-00001e50: 742e 2054 6869 7320 616c 6c6f 7773 2074  t. This allows t
-00001e60: 6865 2066 6577 2d73 686f 7420 636c 6173  he few-shot clas
-00001e70: 7369 6669 6572 2074 6f20 7363 616c 6520  sifier to scale 
-00001e80: 746f 2064 6174 6173 6574 7320 7468 6174  to datasets that
-00001e90: 2061 7265 2074 6f6f 206c 6172 6765 2066   are too large f
-00001ea0: 6f72 2074 6865 2073 7461 6e64 6172 6420  or the standard 
-00001eb0: 636f 6e74 6578 7420 7769 6e64 6f77 206f  context window o
-00001ec0: 6620 4c4c 4d73 2e0a 0a2a 486f 7720 646f  f LLMs...*How do
-00001ed0: 6573 2069 7420 776f 726b 3f2a 0a0a 4475  es it work?*..Du
-00001ee0: 7269 6e67 2066 6974 7469 6e67 2c20 7468  ring fitting, th
-00001ef0: 6520 7768 6f6c 6520 6461 7461 7365 7420  e whole dataset 
-00001f00: 6973 2070 6172 7469 7469 6f6e 6564 2062  is partitioned b
-00001f10: 7920 636c 6173 732c 2076 6563 746f 7269  y class, vectori
-00001f20: 7a65 642c 2061 6e64 2073 746f 7265 642e  zed, and stored.
-00001f30: 0a0a 4475 7269 6e67 2069 6e66 6572 656e  ..During inferen
-00001f40: 6365 2c20 7468 6520 5b61 6e6e 6f79 5d28  ce, the [annoy](
-00001f50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001f60: 6f6d 2f73 706f 7469 6679 2f61 6e6e 6f79  om/spotify/annoy
-00001f70: 2920 6c69 6272 6172 7920 6973 2075 7365  ) library is use
-00001f80: 6420 666f 7220 6661 7374 206e 6569 6768  d for fast neigh
-00001f90: 626f 7220 6c6f 6f6b 7570 2c20 7768 6963  bor lookup, whic
-00001fa0: 6820 616c 6c6f 7773 2069 6e63 6c75 6469  h allows includi
-00001fb0: 6e67 206f 6e6c 7920 7468 6520 6d6f 7374  ng only the most
-00001fc0: 2073 696d 696c 6172 2065 7861 6d70 6c65   similar example
-00001fd0: 7320 696e 2074 6865 2070 726f 6d70 742e  s in the prompt.
-00001fe0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001ff0: 2073 6b6c 6c6d 2069 6d70 6f72 7420 4479   skllm import Dy
-00002000: 6e61 6d69 6346 6577 5368 6f74 4750 5443  namicFewShotGPTC
-00002010: 6c61 7373 6966 6965 720a 6672 6f6d 2073  lassifier.from s
-00002020: 6b6c 6c6d 2e64 6174 6173 6574 7320 696d  kllm.datasets im
-00002030: 706f 7274 2067 6574 5f63 6c61 7373 6966  port get_classif
-00002040: 6963 6174 696f 6e5f 6461 7461 7365 740a  ication_dataset.
-00002050: 0a58 2c20 7920 3d20 6765 745f 636c 6173  .X, y = get_clas
-00002060: 7369 6669 6361 7469 6f6e 5f64 6174 6173  sification_datas
-00002070: 6574 2829 0a0a 636c 6620 3d20 4479 6e61  et()..clf = Dyna
-00002080: 6d69 6346 6577 5368 6f74 4750 5443 6c61  micFewShotGPTCla
-00002090: 7373 6966 6965 7228 6e5f 6578 616d 706c  ssifier(n_exampl
-000020a0: 6573 3d33 290a 636c 662e 6669 7428 582c  es=3).clf.fit(X,
-000020b0: 2079 290a 6c61 6265 6c73 203d 2063 6c66   y).labels = clf
-000020c0: 2e70 7265 6469 6374 2858 290a 6060 600a  .predict(X).```.
-000020d0: 0a23 2323 2054 6578 7420 5665 6374 6f72  .### Text Vector
-000020e0: 697a 6174 696f 6e0a 0a41 7320 616e 2061  ization..As an a
-000020f0: 6c74 6572 6e61 7469 7665 2074 6f20 7573  lternative to us
-00002100: 696e 6720 4750 5420 6173 2061 2063 6c61  ing GPT as a cla
-00002110: 7373 6966 6965 722c 2069 7420 6361 6e20  ssifier, it can 
-00002120: 6265 2075 7365 6420 736f 6c65 6c79 2066  be used solely f
-00002130: 6f72 2064 6174 6120 7072 6570 726f 6365  or data preproce
-00002140: 7373 696e 672e 2060 4750 5456 6563 746f  ssing. `GPTVecto
-00002150: 7269 7a65 7260 2061 6c6c 6f77 7320 746f  rizer` allows to
-00002160: 2065 6d62 6564 2061 2063 6875 6e6b 206f   embed a chunk o
-00002170: 6620 7465 7874 206f 6620 6172 6269 7472  f text of arbitr
-00002180: 6172 7920 6c65 6e67 7468 2074 6f20 6120  ary length to a 
-00002190: 6669 7865 642d 6469 6d65 6e73 696f 6e61  fixed-dimensiona
-000021a0: 6c20 7665 6374 6f72 2c20 7468 6174 2063  l vector, that c
-000021b0: 616e 2062 6520 7573 6564 2077 6974 6820  an be used with 
-000021c0: 7669 7274 7561 6c6c 7920 616e 7920 636c  virtually any cl
-000021d0: 6173 7369 6669 6361 7469 6f6e 206f 7220  assification or 
-000021e0: 7265 6772 6573 7369 6f6e 206d 6f64 656c  regression model
-000021f0: 2e0a 0a45 7861 6d70 6c65 2031 3a20 456d  ...Example 1: Em
-00002200: 6265 6464 696e 6720 7468 6520 7465 7874  bedding the text
-00002210: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00002220: 2073 6b6c 6c6d 2e70 7265 7072 6f63 6573   skllm.preproces
-00002230: 7369 6e67 2069 6d70 6f72 7420 4750 5456  sing import GPTV
-00002240: 6563 746f 7269 7a65 720a 0a6d 6f64 656c  ectorizer..model
-00002250: 203d 2047 5054 5665 6374 6f72 697a 6572   = GPTVectorizer
-00002260: 2829 0a76 6563 746f 7273 203d 206d 6f64  ().vectors = mod
-00002270: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
-00002280: 2858 290a 6060 600a 0a45 7861 6d70 6c65  (X).```..Example
-00002290: 2032 3a20 436f 6d62 696e 696e 6720 7468   2: Combining th
-000022a0: 6520 5665 6374 6f72 697a 6572 2077 6974  e Vectorizer wit
-000022b0: 6820 7468 6520 5847 426f 6f73 7420 436c  h the XGBoost Cl
-000022c0: 6173 7369 6669 6572 2069 6e20 6120 536b  assifier in a Sk
-000022d0: 6c65 6172 6e20 5069 7065 6c69 6e65 0a0a  learn Pipeline..
-000022e0: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
-000022f0: 6b6c 6561 726e 2e70 6970 656c 696e 6520  klearn.pipeline 
-00002300: 696d 706f 7274 2050 6970 656c 696e 650a  import Pipeline.
-00002310: 6672 6f6d 2073 6b6c 6561 726e 2e70 7265  from sklearn.pre
-00002320: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
-00002330: 7420 4c61 6265 6c45 6e63 6f64 6572 0a66  t LabelEncoder.f
-00002340: 726f 6d20 7867 626f 6f73 7420 696d 706f  rom xgboost impo
-00002350: 7274 2058 4742 436c 6173 7369 6669 6572  rt XGBClassifier
-00002360: 0a0a 6c65 203d 204c 6162 656c 456e 636f  ..le = LabelEnco
-00002370: 6465 7228 290a 795f 7472 6169 6e5f 656e  der().y_train_en
-00002380: 636f 6465 6420 3d20 6c65 2e66 6974 5f74  coded = le.fit_t
-00002390: 7261 6e73 666f 726d 2879 5f74 7261 696e  ransform(y_train
-000023a0: 290a 795f 7465 7374 5f65 6e63 6f64 6564  ).y_test_encoded
-000023b0: 203d 206c 652e 7472 616e 7366 6f72 6d28   = le.transform(
-000023c0: 795f 7465 7374 290a 0a73 7465 7073 203d  y_test)..steps =
-000023d0: 205b 2822 4750 5422 2c20 4750 5456 6563   [("GPT", GPTVec
-000023e0: 746f 7269 7a65 7228 2929 2c20 2822 436c  torizer()), ("Cl
-000023f0: 6622 2c20 5847 4243 6c61 7373 6966 6965  f", XGBClassifie
-00002400: 7228 2929 5d0a 636c 6620 3d20 5069 7065  r())].clf = Pipe
-00002410: 6c69 6e65 2873 7465 7073 290a 636c 662e  line(steps).clf.
-00002420: 6669 7428 585f 7472 6169 6e2c 2079 5f74  fit(X_train, y_t
-00002430: 7261 696e 5f65 6e63 6f64 6564 290a 7968  rain_encoded).yh
-00002440: 203d 2063 6c66 2e70 7265 6469 6374 2858   = clf.predict(X
-00002450: 5f74 6573 7429 0a60 6060 0a0a 2323 2320  _test).```..### 
-00002460: 5465 7874 2053 756d 6d61 7269 7a61 7469  Text Summarizati
-00002470: 6f6e 0a0a 4750 5420 6578 6365 6c73 2061  on..GPT excels a
-00002480: 7420 7065 7266 6f72 6d69 6e67 2073 756d  t performing sum
-00002490: 6d61 7269 7a61 7469 6f6e 2074 6173 6b73  marization tasks
-000024a0: 2e20 5468 6572 6566 6f72 652c 2077 6520  . Therefore, we 
-000024b0: 7072 6f76 6964 6520 6047 5054 5375 6d6d  provide `GPTSumm
-000024c0: 6172 697a 6572 6020 7468 6174 2063 616e  arizer` that can
-000024d0: 2062 6520 7573 6564 2062 6f74 6820 6173   be used both as
-000024e0: 2073 7461 6e64 2d61 6c6f 6e65 2065 7374   stand-alone est
-000024f0: 696d 6174 6f72 2c20 6f72 2061 7320 6120  imator, or as a 
-00002500: 7072 6570 726f 6365 7373 6f72 2028 696e  preprocessor (in
-00002510: 2074 6869 7320 6361 7365 2077 6520 6361   this case we ca
-00002520: 6e20 6d61 6b65 2061 6e20 616e 616c 6f67  n make an analog
-00002530: 7920 7769 7468 2061 2064 696d 656e 7369  y with a dimensi
-00002540: 6f6e 616c 6974 7920 7265 6475 6374 696f  onality reductio
-00002550: 6e20 7072 6570 726f 6365 7373 6f72 292e  n preprocessor).
-00002560: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
-00002570: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
-00002580: 2e70 7265 7072 6f63 6573 7369 6e67 2069  .preprocessing i
-00002590: 6d70 6f72 7420 4750 5453 756d 6d61 7269  mport GPTSummari
-000025a0: 7a65 720a 6672 6f6d 2073 6b6c 6c6d 2e64  zer.from skllm.d
-000025b0: 6174 6173 6574 7320 696d 706f 7274 2067  atasets import g
-000025c0: 6574 5f73 756d 6d61 7269 7a61 7469 6f6e  et_summarization
-000025d0: 5f64 6174 6173 6574 0a0a 5820 3d20 6765  _dataset..X = ge
-000025e0: 745f 7375 6d6d 6172 697a 6174 696f 6e5f  t_summarization_
-000025f0: 6461 7461 7365 7428 290a 7320 3d20 4750  dataset().s = GP
-00002600: 5453 756d 6d61 7269 7a65 7228 6f70 656e  TSummarizer(open
-00002610: 6169 5f6d 6f64 656c 3d22 6770 742d 332e  ai_model="gpt-3.
-00002620: 352d 7475 7262 6f22 2c20 6d61 785f 776f  5-turbo", max_wo
-00002630: 7264 733d 3135 290a 7375 6d6d 6172 6965  rds=15).summarie
-00002640: 7320 3d20 732e 6669 745f 7472 616e 7366  s = s.fit_transf
-00002650: 6f72 6d28 5829 0a60 6060 0a0a 506c 6561  orm(X).```..Plea
-00002660: 7365 2062 6520 6177 6172 6520 7468 6174  se be aware that
-00002670: 2074 6865 2060 6d61 785f 776f 7264 7360   the `max_words`
-00002680: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
-00002690: 7365 7473 2061 2073 6f66 7420 6c69 6d69  sets a soft limi
-000026a0: 742c 2077 6869 6368 2069 7320 6e6f 7420  t, which is not 
-000026b0: 7374 7269 6374 6c79 2065 6e66 6f72 6365  strictly enforce
-000026c0: 6420 6f75 7473 6964 6520 6f66 2074 6865  d outside of the
-000026d0: 2070 726f 6d70 742e 2054 6865 7265 666f   prompt. Therefo
-000026e0: 7265 2c20 696e 2073 6f6d 6520 6361 7365  re, in some case
-000026f0: 732c 2074 6865 2061 6374 7561 6c20 6e75  s, the actual nu
-00002700: 6d62 6572 206f 6620 776f 7264 7320 6d69  mber of words mi
-00002710: 6768 7420 6265 2073 6c69 6768 746c 7920  ght be slightly 
-00002720: 6869 6768 6572 2e0a 0a23 2323 2054 6578  higher...### Tex
-00002730: 7420 5472 616e 736c 6174 696f 6e0a 0a47  t Translation..G
-00002740: 5054 206d 6f64 656c 7320 6861 7665 2064  PT models have d
-00002750: 656d 6f6e 7374 7261 7465 6420 7468 6569  emonstrated thei
-00002760: 7220 6566 6665 6374 6976 656e 6573 7320  r effectiveness 
-00002770: 696e 2074 7261 6e73 6c61 7469 6f6e 2074  in translation t
-00002780: 6173 6b73 2062 7920 6765 6e65 7261 7469  asks by generati
-00002790: 6e67 2061 6363 7572 6174 6520 7472 616e  ng accurate tran
-000027a0: 736c 6174 696f 6e73 2061 6372 6f73 7320  slations across 
-000027b0: 7661 7269 6f75 7320 6c61 6e67 7561 6765  various language
-000027c0: 732e 2054 6875 732c 2077 6520 6164 6465  s. Thus, we adde
-000027d0: 6420 6047 5054 5472 616e 736c 6174 6f72  d `GPTTranslator
-000027e0: 6020 7468 6174 2061 6c6c 6f77 7320 7472  ` that allows tr
-000027f0: 616e 736c 6174 696e 6720 616e 2061 7262  anslating an arb
-00002800: 6974 7261 7479 2074 6578 7420 696e 746f  itraty text into
-00002810: 2061 206c 616e 6775 6167 6520 6f66 2069   a language of i
-00002820: 6e74 6572 6573 742e 0a0a 4578 616d 706c  nterest...Exampl
-00002830: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00002840: 6f6d 2073 6b6c 6c6d 2e70 7265 7072 6f63  om skllm.preproc
-00002850: 6573 7369 6e67 2069 6d70 6f72 7420 4750  essing import GP
-00002860: 5454 7261 6e73 6c61 746f 720a 6672 6f6d  TTranslator.from
-00002870: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
-00002880: 696d 706f 7274 2067 6574 5f74 7261 6e73  import get_trans
-00002890: 6c61 7469 6f6e 5f64 6174 6173 6574 0a0a  lation_dataset..
-000028a0: 5820 3d20 6765 745f 7472 616e 736c 6174  X = get_translat
-000028b0: 696f 6e5f 6461 7461 7365 7428 290a 7420  ion_dataset().t 
-000028c0: 3d20 4750 5454 7261 6e73 6c61 746f 7228  = GPTTranslator(
-000028d0: 6f70 656e 6169 5f6d 6f64 656c 3d22 6770  openai_model="gp
-000028e0: 742d 332e 352d 7475 7262 6f22 2c20 6f75  t-3.5-turbo", ou
-000028f0: 7470 7574 5f6c 616e 6775 6167 653d 2245  tput_language="E
-00002900: 6e67 6c69 7368 2229 0a74 7261 6e73 6c61  nglish").transla
-00002910: 7465 645f 7465 7874 203d 2074 2e66 6974  ted_text = t.fit
-00002920: 5f74 7261 6e73 666f 726d 2858 290a 6060  _transform(X).``
-00002930: 600a 0a23 2320 526f 6164 6d61 7020 f09f  `..## Roadmap ..
-00002940: a7ad 0a0a 2d20 5b78 5d20 5a65 726f 2d53  ....- [x] Zero-S
-00002950: 686f 7420 436c 6173 7369 6669 6361 7469  hot Classificati
-00002960: 6f6e 2077 6974 6820 4f70 656e 4149 2047  on with OpenAI G
-00002970: 5054 2033 2f34 0a20 202d 205b 785d 204d  PT 3/4.  - [x] M
-00002980: 756c 7469 636c 6173 7320 636c 6173 7369  ulticlass classi
-00002990: 6669 6361 7469 6f6e 0a20 202d 205b 785d  fication.  - [x]
-000029a0: 204d 756c 7469 2d6c 6162 656c 2063 6c61   Multi-label cla
-000029b0: 7373 6966 6963 6174 696f 6e0a 2d20 5b20  ssification.- [ 
-000029c0: 5d20 4665 772d 5368 6f74 2063 6c61 7373  ] Few-Shot class
-000029d0: 6966 6965 720a 2020 2d20 5b78 5d20 4d75  ifier.  - [x] Mu
-000029e0: 6c74 6963 6c61 7373 2063 6c61 7373 6966  lticlass classif
-000029f0: 6963 6174 696f 6e0a 2020 2d20 5b20 5d20  ication.  - [ ] 
-00002a00: 4d75 6c74 692d 6c61 6265 6c20 636c 6173  Multi-label clas
-00002a10: 7369 6669 6361 7469 6f6e 0a2d 205b 785d  sification.- [x]
-00002a20: 2047 5054 2056 6563 746f 7269 7a65 720a   GPT Vectorizer.
-00002a30: 2d20 5b78 5d20 4368 6174 4750 5420 6d6f  - [x] ChatGPT mo
-00002a40: 6465 6c73 0a2d 205b 205d 2049 6e73 7472  dels.- [ ] Instr
-00002a50: 7563 7447 5054 206d 6f64 656c 730a 2d20  uctGPT models.- 
-00002a60: 5b20 5d20 496e 7374 7275 6374 4750 5420  [ ] InstructGPT 
-00002a70: 4669 6e65 2d74 756e 696e 6720 286f 7074  Fine-tuning (opt
-00002a80: 696f 6e61 6c29 0a2d 205b 205d 204f 7065  ional).- [ ] Ope
-00002a90: 6e20 736f 7572 6365 206d 6f64 656c 730a  n source models.
-00002aa0: 0a2a 5468 6520 6f72 6465 7220 6f66 2074  .*The order of t
-00002ab0: 6865 2065 6c65 6d65 6e74 7320 696e 2074  he elements in t
-00002ac0: 6865 2072 6f61 646d 6170 2069 7320 6172  he roadmap is ar
-00002ad0: 6269 7472 6172 7920 616e 6420 646f 6573  bitrary and does
-00002ae0: 206e 6f74 2072 6566 6c65 6374 2074 6865   not reflect the
-00002af0: 2070 6c61 6e6e 6564 206f 7264 6572 206f   planned order o
-00002b00: 6620 696d 706c 656d 656e 7461 7469 6f6e  f implementation
-00002b10: 2e2a 0a                                  .*.
+00000420: f09f 92a1 2050 726f 7669 6465 2079 6f75  .... Provide you
+00000430: 7220 6665 6564 6261 636b 206f 7220 7072  r feedback or pr
+00000440: 6f70 6f73 6520 6964 6561 7320 696e 2074  opose ideas in t
+00000450: 6865 205b 6973 7375 6573 5d28 6874 7470  he [issues](http
+00000460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00000470: 7279 6e61 2d6b 6f6e 6472 2f73 6369 6b69  ryna-kondr/sciki
+00000480: 742d 6c6c 6d2f 6973 7375 6573 2920 7365  t-llm/issues) se
+00000490: 6374 696f 6e20 6f72 205b 4469 7363 6f72  ction or [Discor
+000004a0: 645d 2868 7474 7073 3a2f 2f64 6973 636f  d](https://disco
+000004b0: 7264 2e67 672f 5944 4162 7775 574b 3756  rd.gg/YDAbwuWK7V
+000004c0: 290a 2d20 f09f 93b0 2050 6f73 7420 6162  ).- .... Post ab
+000004d0: 6f75 7420 5363 696b 6974 2d4c 4c4d 206f  out Scikit-LLM o
+000004e0: 6e20 4c69 6e6b 6564 496e 206f 7220 6f74  n LinkedIn or ot
+000004f0: 6865 7220 706c 6174 666f 726d 730a 0a23  her platforms..#
+00000500: 2320 4f75 7220 5265 6c61 7465 6420 5072  # Our Related Pr
+00000510: 6f6a 6563 7473 20f0 9f94 970a 0a3c 6120  ojects ......<a 
+00000520: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000530: 7468 7562 2e63 6f6d 2f4f 4b55 4131 2f66  thub.com/OKUA1/f
+00000540: 616c 636f 6e22 3e3c 696d 6720 7372 633d  alcon"><img src=
+00000550: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000560: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000570: 6f6d 2f67 6973 742f 4f4b 5541 312f 3632  om/gist/OKUA1/62
+00000580: 3634 6139 3561 3861 6264 3232 3563 3734  64a95a8abd225c74
+00000590: 3431 3161 3262 3730 3762 3032 3432 2f72  411a2b707b0242/r
+000005a0: 6177 2f33 6365 6462 3533 3533 3863 6230  aw/3cedb53538cb0
+000005b0: 3436 3536 6364 3964 3764 3037 6536 3937  4656cd9d7d07e697
+000005c0: 6537 3236 3839 3663 6539 662f 6661 6c63  e726896ce9f/falc
+000005d0: 6f6e 5f6c 6967 6874 2e73 7667 222f 3e3c  on_light.svg"/><
+000005e0: 2f61 3e20 3c62 723e 0a3c 6120 6872 6566  /a> <br>.<a href
+000005f0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000600: 2e63 6f6d 2f4f 4b55 4131 2f61 6765 6e74  .com/OKUA1/agent
+00000610: 5f64 696e 676f 223e 3c69 6d67 2073 7263  _dingo"><img src
+00000620: 3d22 6874 7470 733a 2f2f 6769 7374 2e67  ="https://gist.g
+00000630: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000640: 2e63 6f6d 2f4f 4b55 4131 2f36 3236 3461  .com/OKUA1/6264a
+00000650: 3935 6138 6162 6432 3235 6337 3434 3131  95a8abd225c74411
+00000660: 6132 6237 3037 6230 3234 322f 7261 772f  a2b707b0242/raw/
+00000670: 3162 3233 3161 6162 3731 3866 6361 6236  1b231aab718fcab6
+00000680: 3234 6661 6133 3364 3963 3130 6430 6565  24faa33d9c10d0ee
+00000690: 6531 3763 6131 3630 2f64 696e 676f 5f6c  e17ca160/dingo_l
+000006a0: 6967 6874 2e73 7667 222f 3e3c 2f61 3e0a  ight.svg"/></a>.
+000006b0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
+000006c0: 6e20 f09f 939a 0a0a 2323 2320 436f 6e66  n ......### Conf
+000006d0: 6967 7572 696e 6720 4f70 656e 4149 2041  iguring OpenAI A
+000006e0: 5049 204b 6579 0a0a 4174 2074 6865 206d  PI Key..At the m
+000006f0: 6f6d 656e 7420 7468 6520 6d61 6a6f 7269  oment the majori
+00000700: 7479 206f 6620 7468 6520 5363 696b 6974  ty of the Scikit
+00000710: 2d4c 4c4d 2065 7374 696d 6174 6f72 7320  -LLM estimators 
+00000720: 6172 6520 6f6e 6c79 2063 6f6d 7061 7469  are only compati
+00000730: 626c 6520 7769 7468 2073 6f6d 6520 6f66  ble with some of
+00000740: 2074 6865 204f 7065 6e41 4920 6d6f 6465   the OpenAI mode
+00000750: 6c73 2e20 4865 6e63 652c 2061 2075 7365  ls. Hence, a use
+00000760: 722d 7072 6f76 6964 6564 204f 7065 6e41  r-provided OpenA
+00000770: 4920 4150 4920 6b65 7920 6973 2072 6571  I API key is req
+00000780: 7569 7265 642e 0a0a 6060 6070 7974 686f  uired...```pytho
+00000790: 6e0a 6672 6f6d 2073 6b6c 6c6d 2e63 6f6e  n.from skllm.con
+000007a0: 6669 6720 696d 706f 7274 2053 4b4c 4c4d  fig import SKLLM
+000007b0: 436f 6e66 6967 0a0a 534b 4c4c 4d43 6f6e  Config..SKLLMCon
+000007c0: 6669 672e 7365 745f 6f70 656e 6169 5f6b  fig.set_openai_k
+000007d0: 6579 2822 3c59 4f55 525f 4b45 593e 2229  ey("<YOUR_KEY>")
+000007e0: 0a53 4b4c 4c4d 436f 6e66 6967 2e73 6574  .SKLLMConfig.set
+000007f0: 5f6f 7065 6e61 695f 6f72 6728 223c 594f  _openai_org("<YO
+00000800: 5552 5f4f 5247 414e 4953 4154 494f 4e3e  UR_ORGANISATION>
+00000810: 2229 0a60 6060 0a0a 2a2a 496d 706f 7274  ").```..**Import
+00000820: 616e 7420 6e6f 7469 6365 3a2a 2a0a 0a2d  ant notice:**..-
+00000830: 2049 6620 796f 7520 6861 7665 2061 2066   If you have a f
+00000840: 7265 6520 7472 6961 6c20 4f70 656e 4149  ree trial OpenAI
+00000850: 2061 6363 6f75 6e74 2c20 7468 6520 5b72   account, the [r
+00000860: 6174 6520 6c69 6d69 7473 5d28 6874 7470  ate limits](http
+00000870: 733a 2f2f 706c 6174 666f 726d 2e6f 7065  s://platform.ope
+00000880: 6e61 692e 636f 6d2f 646f 6373 2f67 7569  nai.com/docs/gui
+00000890: 6465 732f 7261 7465 2d6c 696d 6974 732f  des/rate-limits/
+000008a0: 6f76 6572 7669 6577 2920 6172 6520 6e6f  overview) are no
+000008b0: 7420 7375 6666 6963 6965 6e74 2028 7370  t sufficient (sp
+000008c0: 6563 6966 6963 616c 6c79 2033 2072 6571  ecifically 3 req
+000008d0: 7565 7374 7320 7065 7220 6d69 6e75 7465  uests per minute
+000008e0: 292e 2050 6c65 6173 6520 7377 6974 6368  ). Please switch
+000008f0: 2074 6f20 7468 6520 2270 6179 2061 7320   to the "pay as 
+00000900: 796f 7520 676f 2220 706c 616e 2066 6972  you go" plan fir
+00000910: 7374 2e0a 2d20 5768 656e 2063 616c 6c69  st..- When calli
+00000920: 6e67 2060 534b 4c4c 4d43 6f6e 6669 672e  ng `SKLLMConfig.
+00000930: 7365 745f 6f70 656e 6169 5f6f 7267 602c  set_openai_org`,
+00000940: 2079 6f75 2068 6176 6520 746f 2070 726f   you have to pro
+00000950: 7669 6465 2079 6f75 7220 6f72 6761 6e69  vide your organi
+00000960: 7a61 7469 6f6e 2049 4420 616e 6420 2a2a  zation ID and **
+00000970: 4e4f 542a 2a20 7468 6520 6e61 6d65 2e20  NOT** the name. 
+00000980: 596f 7520 6361 6e20 6669 6e64 2079 6f75  You can find you
+00000990: 7220 4944 205b 6865 7265 5d28 6874 7470  r ID [here](http
+000009a0: 733a 2f2f 706c 6174 666f 726d 2e6f 7065  s://platform.ope
+000009b0: 6e61 692e 636f 6d2f 6163 636f 756e 742f  nai.com/account/
+000009c0: 6f72 672d 7365 7474 696e 6773 292e 0a0a  org-settings)...
+000009d0: 2323 2320 5573 696e 6720 417a 7572 6520  ### Using Azure 
+000009e0: 4f70 656e 4149 0a0a 6060 6070 7974 686f  OpenAI..```pytho
+000009f0: 6e0a 6672 6f6d 2073 6b6c 6c6d 2e63 6f6e  n.from skllm.con
+00000a00: 6669 6720 696d 706f 7274 2053 4b4c 4c4d  fig import SKLLM
+00000a10: 436f 6e66 6967 0a0a 534b 4c4c 4d43 6f6e  Config..SKLLMCon
+00000a20: 6669 672e 7365 745f 6f70 656e 6169 5f6b  fig.set_openai_k
+00000a30: 6579 2822 3c59 4f55 525f 4b45 593e 2229  ey("<YOUR_KEY>")
+00000a40: 2023 7573 6520 617a 7572 6520 6b65 7920   #use azure key 
+00000a50: 696e 7374 6561 640a 534b 4c4c 4d43 6f6e  instead.SKLLMCon
+00000a60: 6669 672e 7365 745f 617a 7572 655f 6170  fig.set_azure_ap
+00000a70: 695f 6261 7365 2822 3c41 5049 5f42 4153  i_base("<API_BAS
+00000a80: 453e 2229 0a0a 2320 7374 6172 7420 7769  E>")..# start wi
+00000a90: 7468 2022 617a 7572 653a 3a22 2070 7265  th "azure::" pre
+00000aa0: 6669 7820 7768 656e 2073 6574 7469 6e67  fix when setting
+00000ab0: 2074 6865 206d 6f64 656c 206e 616d 650a   the model name.
+00000ac0: 6d6f 6465 6c5f 6e61 6d65 203d 2022 617a  model_name = "az
+00000ad0: 7572 653a 3a3c 6d6f 6465 6c5f 6e61 6d65  ure::<model_name
+00000ae0: 3e22 0a23 2065 2e67 2e20 5a65 726f 5368  >".# e.g. ZeroSh
+00000af0: 6f74 4750 5443 6c61 7373 6966 6965 7228  otGPTClassifier(
+00000b00: 6f70 656e 6169 5f6d 6f64 656c 3d22 617a  openai_model="az
+00000b10: 7572 653a 3a67 7074 2d33 2e35 2d74 7572  ure::gpt-3.5-tur
+00000b20: 626f 2229 0a60 6060 0a0a 4e6f 7465 3a20  bo").```..Note: 
+00000b30: 417a 7572 6520 4f70 656e 4149 2069 7320  Azure OpenAI is 
+00000b40: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00000b50: 2074 6865 2070 7265 7072 6f63 6573 736f   the preprocesso
+00000b60: 7273 2061 7420 7468 6520 6d6f 6d65 6e74  rs at the moment
+00000b70: 2e0a 0a23 2323 2055 7369 6e67 2047 5054  ...### Using GPT
+00000b80: 3441 4c4c 0a0a 496e 2061 6464 6974 696f  4ALL..In additio
+00000b90: 6e20 746f 204f 7065 6e41 492c 2073 6f6d  n to OpenAI, som
+00000ba0: 6520 6f66 2074 6865 206d 6f64 656c 7320  e of the models 
+00000bb0: 6361 6e20 7573 6520 5b67 7074 3461 6c6c  can use [gpt4all
+00000bc0: 5d28 6874 7470 733a 2f2f 6770 7434 616c  ](https://gpt4al
+00000bd0: 6c2e 696f 2f69 6e64 6578 2e68 746d 6c29  l.io/index.html)
+00000be0: 2061 7320 6120 6261 636b 656e 642e 0a0a   as a backend...
+00000bf0: 2a2a 5468 6973 2066 6561 7475 7265 2069  **This feature i
+00000c00: 7320 636f 6e73 6964 6572 6564 2068 6967  s considered hig
+00000c10: 6c79 2065 7870 6572 696d 656e 7461 6c21  ly experimental!
+00000c20: 2a2a 0a0a 496e 206f 7264 6572 2074 6f20  **..In order to 
+00000c30: 7573 6520 6770 7434 616c 6c2c 2079 6f75  use gpt4all, you
+00000c40: 206e 6565 6420 746f 2069 6e73 7461 6c6c   need to install
+00000c50: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00000c60: 6e67 2073 7562 6d6f 6475 6c65 3a0a 0a60  ng submodule:..`
+00000c70: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00000c80: 6c6c 2022 7363 696b 6974 2d6c 6c6d 5b67  ll "scikit-llm[g
+00000c90: 7074 3461 6c6c 5d22 0a60 6060 0a0a 496e  pt4all]".```..In
+00000ca0: 206f 7264 6572 2074 6f20 7377 6974 6368   order to switch
+00000cb0: 2066 726f 6d20 4f70 656e 4149 2074 6f20   from OpenAI to 
+00000cc0: 4750 5434 414c 4c20 6d6f 6465 6c2c 2073  GPT4ALL model, s
+00000cd0: 696d 706c 7920 7072 6f76 6964 6520 6120  imply provide a 
+00000ce0: 7374 7269 6e67 206f 6620 7468 6520 666f  string of the fo
+00000cf0: 726d 6174 2060 6770 7434 616c 6c3a 3a3c  rmat `gpt4all::<
+00000d00: 6d6f 6465 6c5f 6e61 6d65 3e60 2061 7320  model_name>` as 
+00000d10: 616e 2061 7267 756d 656e 742e 2057 6869  an argument. Whi
+00000d20: 6c65 2074 6865 206d 6f64 656c 2072 756e  le the model run
+00000d30: 7320 636f 6d70 6c65 7465 6c79 206c 6f63  s completely loc
+00000d40: 616c 6c79 2c20 7468 6520 6573 7469 6d61  ally, the estima
+00000d50: 746f 7220 7374 696c 6c20 7472 6561 7473  tor still treats
+00000d60: 2069 7420 6173 2061 6e20 4f70 656e 4149   it as an OpenAI
+00000d70: 2065 6e64 706f 696e 7420 616e 6420 7769   endpoint and wi
+00000d80: 6c6c 2074 7279 2074 6f20 6368 6563 6b20  ll try to check 
+00000d90: 7468 6174 2074 6865 2041 5049 206b 6579  that the API key
+00000da0: 2069 7320 7072 6573 656e 742e 2059 6f75   is present. You
+00000db0: 2063 616e 2070 726f 7669 6465 2061 6e79   can provide any
+00000dc0: 2073 7472 696e 6720 6173 2061 206b 6579   string as a key
+00000dd0: 2e0a 0a60 6060 7079 7468 6f6e 0a53 4b4c  ...```python.SKL
+00000de0: 4c4d 436f 6e66 6967 2e73 6574 5f6f 7065  LMConfig.set_ope
+00000df0: 6e61 695f 6b65 7928 2261 6e79 2073 7472  nai_key("any str
+00000e00: 696e 6722 290a 534b 4c4c 4d43 6f6e 6669  ing").SKLLMConfi
+00000e10: 672e 7365 745f 6f70 656e 6169 5f6f 7267  g.set_openai_org
+00000e20: 2822 616e 7920 7374 7269 6e67 2229 0a0a  ("any string")..
+00000e30: 5a65 726f 5368 6f74 4750 5443 6c61 7373  ZeroShotGPTClass
+00000e40: 6966 6965 7228 6f70 656e 6169 5f6d 6f64  ifier(openai_mod
+00000e50: 656c 3d22 6770 7434 616c 6c3a 3a67 676d  el="gpt4all::ggm
+00000e60: 6c2d 6770 7434 616c 6c2d 6a2d 7631 2e33  l-gpt4all-j-v1.3
+00000e70: 2d67 726f 6f76 7922 290a 6060 600a 0a57  -groovy").```..W
+00000e80: 6865 6e20 7275 6e6e 696e 6720 666f 7220  hen running for 
+00000e90: 7468 6520 6669 7273 7420 7469 6d65 2c20  the first time, 
+00000ea0: 7468 6520 6d6f 6465 6c20 6669 6c65 2077  the model file w
+00000eb0: 696c 6c20 6265 2064 6f77 6e6c 6f61 6465  ill be downloade
+00000ec0: 6420 6175 746f 6d61 7469 616c 6c79 2e0a  d automatially..
+00000ed0: 0a57 6865 6e20 7573 696e 6720 6770 7434  .When using gpt4
+00000ee0: 616c 6c20 706c 6561 7365 206b 6565 7020  all please keep 
+00000ef0: 7468 6520 666f 6c6c 6f77 696e 6720 696e  the following in
+00000f00: 206d 696e 643a 0a0a 312e 204e 6f74 2061   mind:..1. Not a
+00000f10: 6c6c 2067 7074 3461 6c6c 206d 6f64 656c  ll gpt4all model
+00000f20: 7320 6172 6520 636f 6d6d 6572 6369 616c  s are commercial
+00000f30: 6c79 206c 6963 656e 7361 626c 652c 2070  ly licensable, p
+00000f40: 6c65 6173 6520 636f 6e73 756c 7420 6770  lease consult gp
+00000f50: 7434 616c 6c20 7765 6273 6974 6520 666f  t4all website fo
+00000f60: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
+00000f70: 322e 2054 6865 2061 6363 7572 6163 7920  2. The accuracy 
+00000f80: 6f66 2074 6865 206d 6f64 656c 7320 6d61  of the models ma
+00000f90: 7920 6265 206d 7563 6820 6c6f 7765 7220  y be much lower 
+00000fa0: 636f 6d70 6172 6564 2074 6f20 6f6e 6573  compared to ones
+00000fb0: 2070 726f 7669 6465 6420 6279 204f 7065   provided by Ope
+00000fc0: 6e41 4920 2865 7370 6563 6961 6c6c 7920  nAI (especially 
+00000fd0: 6770 742d 3429 2e0a 332e 204e 6f74 2061  gpt-4)..3. Not a
+00000fe0: 6c6c 206f 6620 7468 6520 6176 6169 6c61  ll of the availa
+00000ff0: 626c 6520 6d6f 6465 6c73 2077 6572 6520  ble models were 
+00001000: 7465 7374 6564 2c20 736f 6d65 206d 6179  tested, some may
+00001010: 206e 6f74 2077 6f72 6b20 7769 7468 2073   not work with s
+00001020: 6369 6b69 742d 6c6c 6d20 6174 2061 6c6c  cikit-llm at all
+00001030: 2e0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
+00001040: 206d 6f64 656c 7320 6279 2061 206e 6f6e   models by a non
+00001050: 2d73 7461 6e64 6172 6420 6261 636b 656e  -standard backen
+00001060: 640a 0a41 7420 7468 6520 6d6f 6d65 6e74  d..At the moment
+00001070: 206f 6e6c 7920 7468 6520 666f 6c6c 6f77   only the follow
+00001080: 696e 6720 6573 7469 6d61 746f 7273 2073  ing estimators s
+00001090: 7570 706f 7274 206e 6f6e 2d73 7461 6e64  upport non-stand
+000010a0: 6172 6420 6261 636b 656e 6473 2028 6770  ard backends (gp
+000010b0: 7434 616c 6c2c 2061 7a75 7265 293a 0a0a  t4all, azure):..
+000010c0: 2d20 605a 6572 6f53 686f 7447 5054 436c  - `ZeroShotGPTCl
+000010d0: 6173 7369 6669 6572 600a 2d20 604d 756c  assifier`.- `Mul
+000010e0: 7469 4c61 6265 6c5a 6572 6f53 686f 7447  tiLabelZeroShotG
+000010f0: 5054 436c 6173 7369 6669 6572 600a 2d20  PTClassifier`.- 
+00001100: 6046 6577 5368 6f74 4750 5443 6c61 7373  `FewShotGPTClass
+00001110: 6966 6965 7260 0a0a 2323 2320 5a65 726f  ifier`..### Zero
+00001120: 2d53 686f 7420 5465 7874 2043 6c61 7373  -Shot Text Class
+00001130: 6966 6963 6174 696f 6e0a 0a4f 6e65 206f  ification..One o
+00001140: 6620 7468 6520 706f 7765 7266 756c 2043  f the powerful C
+00001150: 6861 7447 5054 2066 6561 7475 7265 7320  hatGPT features 
+00001160: 6973 2074 6865 2061 6269 6c69 7479 2074  is the ability t
+00001170: 6f20 7065 7266 6f72 6d20 7465 7874 2063  o perform text c
+00001180: 6c61 7373 6966 6963 6174 696f 6e20 7769  lassification wi
+00001190: 7468 6f75 7420 6265 696e 6720 7265 2d74  thout being re-t
+000011a0: 7261 696e 6564 2e20 466f 7220 7468 6174  rained. For that
+000011b0: 2c20 7468 6520 6f6e 6c79 2072 6571 7569  , the only requi
+000011c0: 7265 6d65 6e74 2069 7320 7468 6174 2074  rement is that t
+000011d0: 6865 206c 6162 656c 7320 6d75 7374 2062  he labels must b
+000011e0: 6520 6465 7363 7269 7074 6976 652e 0a0a  e descriptive...
+000011f0: 5765 2070 726f 7669 6465 2061 2063 6c61  We provide a cla
+00001200: 7373 2060 5a65 726f 5368 6f74 4750 5443  ss `ZeroShotGPTC
+00001210: 6c61 7373 6966 6965 7260 2074 6861 7420  lassifier` that 
+00001220: 616c 6c6f 7773 2074 6f20 6372 6561 7465  allows to create
+00001230: 2073 7563 6820 6120 6d6f 6465 6c20 6173   such a model as
+00001240: 2061 2072 6567 756c 6172 2073 6369 6b69   a regular sciki
+00001250: 742d 6c65 6172 6e20 636c 6173 7369 6669  t-learn classifi
+00001260: 6572 2e0a 0a45 7861 6d70 6c65 2031 3a20  er...Example 1: 
+00001270: 5472 6169 6e69 6e67 2061 7320 6120 7265  Training as a re
+00001280: 6775 6c61 7220 636c 6173 7369 6669 6572  gular classifier
+00001290: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000012a0: 2073 6b6c 6c6d 2069 6d70 6f72 7420 5a65   skllm import Ze
+000012b0: 726f 5368 6f74 4750 5443 6c61 7373 6966  roShotGPTClassif
+000012c0: 6965 720a 6672 6f6d 2073 6b6c 6c6d 2e64  ier.from skllm.d
+000012d0: 6174 6173 6574 7320 696d 706f 7274 2067  atasets import g
+000012e0: 6574 5f63 6c61 7373 6966 6963 6174 696f  et_classificatio
+000012f0: 6e5f 6461 7461 7365 740a 0a23 2064 656d  n_dataset..# dem
+00001300: 6f20 7365 6e74 696d 656e 7420 616e 616c  o sentiment anal
+00001310: 7973 6973 2064 6174 6173 6574 0a23 206c  ysis dataset.# l
+00001320: 6162 656c 733a 2070 6f73 6974 6976 652c  abels: positive,
+00001330: 206e 6567 6174 6976 652c 206e 6575 7472   negative, neutr
+00001340: 616c 0a58 2c20 7920 3d20 6765 745f 636c  al.X, y = get_cl
+00001350: 6173 7369 6669 6361 7469 6f6e 5f64 6174  assification_dat
+00001360: 6173 6574 2829 0a0a 636c 6620 3d20 5a65  aset()..clf = Ze
+00001370: 726f 5368 6f74 4750 5443 6c61 7373 6966  roShotGPTClassif
+00001380: 6965 7228 6f70 656e 6169 5f6d 6f64 656c  ier(openai_model
+00001390: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+000013a0: 290a 636c 662e 6669 7428 582c 2079 290a  ).clf.fit(X, y).
+000013b0: 6c61 6265 6c73 203d 2063 6c66 2e70 7265  labels = clf.pre
+000013c0: 6469 6374 2858 290a 6060 600a 0a53 6369  dict(X).```..Sci
+000013d0: 6b69 742d 4c4c 4d20 7769 6c6c 2061 7574  kit-LLM will aut
+000013e0: 6f6d 6174 6963 616c 6c79 2071 7565 7279  omatically query
+000013f0: 2074 6865 204f 7065 6e41 4920 4150 4920   the OpenAI API 
+00001400: 616e 6420 7472 616e 7366 6f72 6d20 7468  and transform th
+00001410: 6520 7265 7370 6f6e 7365 2069 6e74 6f20  e response into 
+00001420: 6120 7265 6775 6c61 7220 6c69 7374 206f  a regular list o
+00001430: 6620 6c61 6265 6c73 2e0a 0a41 6464 6974  f labels...Addit
+00001440: 696f 6e61 6c6c 792c 2053 6369 6b69 742d  ionally, Scikit-
+00001450: 4c4c 4d20 7769 6c6c 2065 6e73 7572 6520  LLM will ensure 
+00001460: 7468 6174 2074 6865 206f 6274 6169 6e65  that the obtaine
+00001470: 6420 7265 7370 6f6e 7365 2063 6f6e 7461  d response conta
+00001480: 696e 7320 6120 7661 6c69 6420 6c61 6265  ins a valid labe
+00001490: 6c2e 2049 6620 7468 6973 2069 7320 6e6f  l. If this is no
+000014a0: 7420 7468 6520 6361 7365 2c20 6120 6c61  t the case, a la
+000014b0: 6265 6c20 7769 6c6c 2062 6520 7365 6c65  bel will be sele
+000014c0: 6374 6564 2072 616e 646f 6d6c 7920 286c  cted randomly (l
+000014d0: 6162 656c 2070 726f 6261 6269 6c69 7469  abel probabiliti
+000014e0: 6573 2061 7265 2070 726f 706f 7274 696f  es are proportio
+000014f0: 6e61 6c20 746f 206c 6162 656c 206f 6363  nal to label occ
+00001500: 7572 7265 6e63 6573 2069 6e20 7468 6520  urrences in the 
+00001510: 7472 6169 6e69 6e67 2073 6574 292e 0a0a  training set)...
+00001520: 4578 616d 706c 6520 323a 2054 7261 696e  Example 2: Train
+00001530: 696e 6720 7769 7468 6f75 7420 6c61 6265  ing without labe
+00001540: 6c65 6420 6461 7461 0a0a 5369 6e63 6520  led data..Since 
+00001550: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
+00001560: 6120 6973 206e 6f74 2073 7472 6963 746c  a is not strictl
+00001570: 7920 7265 7175 6972 6564 2c20 6974 2063  y required, it c
+00001580: 616e 2062 6520 6675 6c6c 7920 6f6d 6d69  an be fully ommi
+00001590: 7465 642e 2054 6865 206f 6e6c 7920 7468  ted. The only th
+000015a0: 696e 6720 7468 6174 2068 6173 2074 6f20  ing that has to 
+000015b0: 6265 2070 726f 7669 6465 6420 6973 2074  be provided is t
+000015c0: 6865 206c 6973 7420 6f66 2063 616e 6469  he list of candi
+000015d0: 6461 7465 206c 6162 656c 732e 0a0a 6060  date labels...``
+000015e0: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+000015f0: 6c6d 2069 6d70 6f72 7420 5a65 726f 5368  lm import ZeroSh
+00001600: 6f74 4750 5443 6c61 7373 6966 6965 720a  otGPTClassifier.
+00001610: 6672 6f6d 2073 6b6c 6c6d 2e64 6174 6173  from skllm.datas
+00001620: 6574 7320 696d 706f 7274 2067 6574 5f63  ets import get_c
+00001630: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
+00001640: 7461 7365 740a 0a58 2c20 5f20 3d20 6765  taset..X, _ = ge
+00001650: 745f 636c 6173 7369 6669 6361 7469 6f6e  t_classification
+00001660: 5f64 6174 6173 6574 2829 0a0a 636c 6620  _dataset()..clf 
+00001670: 3d20 5a65 726f 5368 6f74 4750 5443 6c61  = ZeroShotGPTCla
+00001680: 7373 6966 6965 7228 290a 636c 662e 6669  ssifier().clf.fi
+00001690: 7428 4e6f 6e65 2c20 5b22 706f 7369 7469  t(None, ["positi
+000016a0: 7665 222c 2022 6e65 6761 7469 7665 222c  ve", "negative",
+000016b0: 2022 6e65 7574 7261 6c22 5d29 0a6c 6162   "neutral"]).lab
+000016c0: 656c 7320 3d20 636c 662e 7072 6564 6963  els = clf.predic
+000016d0: 7428 5829 0a60 6060 0a0a 2a2a 4e6f 7465  t(X).```..**Note
+000016e0: 3a2a 2a20 756e 6c69 6b65 2069 6e20 6120  :** unlike in a 
+000016f0: 7479 7069 6361 6c20 7375 7065 7276 6973  typical supervis
+00001700: 6564 2073 6574 7469 6e67 2c20 7468 6520  ed setting, the 
+00001710: 7065 7266 6f72 6d61 6e63 6520 6f66 2061  performance of a
+00001720: 207a 6572 6f2d 7368 6f74 2063 6c61 7373   zero-shot class
+00001730: 6966 6965 7220 6772 6561 746c 7920 6465  ifier greatly de
+00001740: 7065 6e64 7320 6f6e 2068 6f77 2074 6865  pends on how the
+00001750: 206c 6162 656c 2069 7473 656c 6620 6973   label itself is
+00001760: 2073 7472 7563 7475 7265 642e 2049 7420   structured. It 
+00001770: 6861 7320 746f 2062 6520 6578 7072 6573  has to be expres
+00001780: 7365 6420 696e 206e 6174 7572 616c 206c  sed in natural l
+00001790: 616e 6775 6167 652c 2062 6520 6465 7363  anguage, be desc
+000017a0: 7269 7074 6976 6520 616e 6420 7365 6c66  riptive and self
+000017b0: 2d65 7870 6c61 6e61 746f 7279 2e20 466f  -explanatory. Fo
+000017c0: 7220 6578 616d 706c 652c 2069 6e20 7468  r example, in th
+000017d0: 6520 7072 6576 696f 7573 2073 656d 616e  e previous seman
+000017e0: 7469 6320 636c 6173 7369 6669 6361 7469  tic classificati
+000017f0: 6f6e 2074 6173 6b2c 2069 7420 636f 756c  on task, it coul
+00001800: 6420 6265 2062 656e 6566 6963 6961 6c20  d be beneficial 
+00001810: 746f 2074 7261 6e73 666f 726d 2061 206c  to transform a l
+00001820: 6162 656c 2066 726f 6d20 6022 3c73 656d  abel from `"<sem
+00001830: 616e 7469 6373 3e22 6020 746f 2060 2274  antics>"` to `"t
+00001840: 6865 2073 656d 616e 7469 6373 206f 6620  he semantics of 
+00001850: 7468 6520 7072 6f76 6964 6564 2074 6578  the provided tex
+00001860: 7420 6973 203c 7365 6d61 6e74 6963 733e  t is <semantics>
+00001870: 2260 2e0a 0a23 2323 204d 756c 7469 2d4c  "`...### Multi-L
+00001880: 6162 656c 205a 6572 6f2d 5368 6f74 2054  abel Zero-Shot T
+00001890: 6578 7420 436c 6173 7369 6669 6361 7469  ext Classificati
+000018a0: 6f6e 0a0a 5769 7468 2061 2063 6c61 7373  on..With a class
+000018b0: 2060 4d75 6c74 694c 6162 656c 5a65 726f   `MultiLabelZero
+000018c0: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+000018d0: 7260 2069 7420 6973 2070 6f73 7369 626c  r` it is possibl
+000018e0: 6520 746f 2070 6572 666f 726d 2074 6865  e to perform the
+000018f0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
+00001900: 696e 206d 756c 7469 2d6c 6162 656c 2073  in multi-label s
+00001910: 6574 7469 6e67 2c20 7768 6963 6820 6d65  etting, which me
+00001920: 616e 7320 7468 6174 2065 6163 6820 7361  ans that each sa
+00001930: 6d70 6c65 206d 6967 6874 2062 6520 6173  mple might be as
+00001940: 7369 676e 6564 2074 6f20 6f6e 6520 6f72  signed to one or
+00001950: 2073 6576 6572 616c 2064 6973 7469 6e63   several distinc
+00001960: 7420 636c 6173 7365 732e 0a0a 4578 616d  t classes...Exam
+00001970: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00001980: 6672 6f6d 2073 6b6c 6c6d 2069 6d70 6f72  from skllm impor
+00001990: 7420 4d75 6c74 694c 6162 656c 5a65 726f  t MultiLabelZero
+000019a0: 5368 6f74 4750 5443 6c61 7373 6966 6965  ShotGPTClassifie
+000019b0: 720a 6672 6f6d 2073 6b6c 6c6d 2e64 6174  r.from skllm.dat
+000019c0: 6173 6574 7320 696d 706f 7274 2067 6574  asets import get
+000019d0: 5f6d 756c 7469 6c61 6265 6c5f 636c 6173  _multilabel_clas
+000019e0: 7369 6669 6361 7469 6f6e 5f64 6174 6173  sification_datas
+000019f0: 6574 0a0a 582c 2079 203d 2067 6574 5f6d  et..X, y = get_m
+00001a00: 756c 7469 6c61 6265 6c5f 636c 6173 7369  ultilabel_classi
+00001a10: 6669 6361 7469 6f6e 5f64 6174 6173 6574  fication_dataset
+00001a20: 2829 0a0a 636c 6620 3d20 4d75 6c74 694c  ()..clf = MultiL
+00001a30: 6162 656c 5a65 726f 5368 6f74 4750 5443  abelZeroShotGPTC
+00001a40: 6c61 7373 6966 6965 7228 6d61 785f 6c61  lassifier(max_la
+00001a50: 6265 6c73 3d33 290a 636c 662e 6669 7428  bels=3).clf.fit(
+00001a60: 582c 2079 290a 6c61 6265 6c73 203d 2063  X, y).labels = c
+00001a70: 6c66 2e70 7265 6469 6374 2858 290a 6060  lf.predict(X).``
+00001a80: 600a 0a53 696d 696c 6172 6c79 2074 6f20  `..Similarly to 
+00001a90: 7468 6520 605a 6572 6f53 686f 7447 5054  the `ZeroShotGPT
+00001aa0: 436c 6173 7369 6669 6572 6020 6974 2069  Classifier` it i
+00001ab0: 7320 7375 6666 6963 6965 6e74 2069 6620  s sufficient if 
+00001ac0: 6f6e 6c79 2063 616e 6469 6461 7465 206c  only candidate l
+00001ad0: 6162 656c 7320 6172 6520 7072 6f76 6964  abels are provid
+00001ae0: 6564 2e20 486f 7765 7665 722c 2074 6869  ed. However, thi
+00001af0: 7320 7469 6d65 2074 6865 2063 6c61 7373  s time the class
+00001b00: 6966 6965 7220 6578 7065 6374 7320 6079  ifier expects `y
+00001b10: 6020 6f66 2061 2074 7970 6520 604c 6973  ` of a type `Lis
+00001b20: 745b 4c69 7374 5b73 7472 5d5d 602e 0a0a  t[List[str]]`...
+00001b30: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
+00001b40: 6b6c 6c6d 2069 6d70 6f72 7420 4d75 6c74  kllm import Mult
+00001b50: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
+00001b60: 5443 6c61 7373 6966 6965 720a 6672 6f6d  TClassifier.from
+00001b70: 2073 6b6c 6c6d 2e64 6174 6173 6574 7320   skllm.datasets 
+00001b80: 696d 706f 7274 2067 6574 5f6d 756c 7469  import get_multi
+00001b90: 6c61 6265 6c5f 636c 6173 7369 6669 6361  label_classifica
+00001ba0: 7469 6f6e 5f64 6174 6173 6574 0a0a 582c  tion_dataset..X,
+00001bb0: 205f 203d 2067 6574 5f6d 756c 7469 6c61   _ = get_multila
+00001bc0: 6265 6c5f 636c 6173 7369 6669 6361 7469  bel_classificati
+00001bd0: 6f6e 5f64 6174 6173 6574 2829 0a63 616e  on_dataset().can
+00001be0: 6469 6461 7465 5f6c 6162 656c 7320 3d20  didate_labels = 
+00001bf0: 5b0a 2020 2020 2251 7561 6c69 7479 222c  [.    "Quality",
+00001c00: 0a20 2020 2022 5072 6963 6522 2c0a 2020  .    "Price",.  
+00001c10: 2020 2244 656c 6976 6572 7922 2c0a 2020    "Delivery",.  
+00001c20: 2020 2253 6572 7669 6365 222c 0a20 2020    "Service",.   
+00001c30: 2022 5072 6f64 7563 7420 5661 7269 6574   "Product Variet
+00001c40: 7922 2c0a 2020 2020 2243 7573 746f 6d65  y",.    "Custome
+00001c50: 7220 5375 7070 6f72 7422 2c0a 2020 2020  r Support",.    
+00001c60: 2250 6163 6b61 6769 6e67 222c 0a20 2020  "Packaging",.   
+00001c70: 2022 5573 6572 2045 7870 6572 6965 6e63   "User Experienc
+00001c80: 6522 2c0a 2020 2020 2252 6574 7572 6e20  e",.    "Return 
+00001c90: 506f 6c69 6379 222c 0a20 2020 2022 5072  Policy",.    "Pr
+00001ca0: 6f64 7563 7420 496e 666f 726d 6174 696f  oduct Informatio
+00001cb0: 6e22 2c0a 5d0a 636c 6620 3d20 4d75 6c74  n",.].clf = Mult
+00001cc0: 694c 6162 656c 5a65 726f 5368 6f74 4750  iLabelZeroShotGP
+00001cd0: 5443 6c61 7373 6966 6965 7228 6d61 785f  TClassifier(max_
+00001ce0: 6c61 6265 6c73 3d33 290a 636c 662e 6669  labels=3).clf.fi
+00001cf0: 7428 4e6f 6e65 2c20 5b63 616e 6469 6461  t(None, [candida
+00001d00: 7465 5f6c 6162 656c 735d 290a 6c61 6265  te_labels]).labe
+00001d10: 6c73 203d 2063 6c66 2e70 7265 6469 6374  ls = clf.predict
+00001d20: 2858 290a 6060 600a 0a23 2323 2046 6577  (X).```..### Few
+00001d30: 2d53 686f 7420 5465 7874 2043 6c61 7373  -Shot Text Class
+00001d40: 6966 6963 6174 696f 6e0a 0a57 6974 6820  ification..With 
+00001d50: 6046 6577 5368 6f74 4750 5443 6c61 7373  `FewShotGPTClass
+00001d60: 6966 6965 7260 2069 7420 6973 2070 6f73  ifier` it is pos
+00001d70: 7369 626c 6520 746f 2070 6572 666f 726d  sible to perform
+00001d80: 2061 2066 6577 2d73 686f 7420 636c 6173   a few-shot clas
+00001d90: 7369 6669 6361 7469 6f6e 2c20 7768 6963  sification, whic
+00001da0: 6820 6d65 616e 7320 7468 6174 2074 6865  h means that the
+00001db0: 2074 7261 696e 696e 6720 7361 6d70 6c65   training sample
+00001dc0: 7320 7769 6c6c 2062 6520 6164 6465 6420  s will be added 
+00001dd0: 746f 2070 726f 6d70 7420 616e 6420 7061  to prompt and pa
+00001de0: 7373 6564 2074 6f20 7468 6520 6d6f 6465  ssed to the mode
+00001df0: 6c2e 0a0a 6060 6070 7974 686f 6e0a 6672  l...```python.fr
+00001e00: 6f6d 2073 6b6c 6c6d 2069 6d70 6f72 7420  om skllm import 
+00001e10: 4665 7753 686f 7447 5054 436c 6173 7369  FewShotGPTClassi
+00001e20: 6669 6572 0a66 726f 6d20 736b 6c6c 6d2e  fier.from skllm.
+00001e30: 6461 7461 7365 7473 2069 6d70 6f72 7420  datasets import 
+00001e40: 6765 745f 636c 6173 7369 6669 6361 7469  get_classificati
+00001e50: 6f6e 5f64 6174 6173 6574 0a0a 582c 2079  on_dataset..X, y
+00001e60: 203d 2067 6574 5f63 6c61 7373 6966 6963   = get_classific
+00001e70: 6174 696f 6e5f 6461 7461 7365 7428 290a  ation_dataset().
+00001e80: 0a63 6c66 203d 2046 6577 5368 6f74 4750  .clf = FewShotGP
+00001e90: 5443 6c61 7373 6966 6965 7228 6f70 656e  TClassifier(open
+00001ea0: 6169 5f6d 6f64 656c 3d22 6770 742d 332e  ai_model="gpt-3.
+00001eb0: 352d 7475 7262 6f22 290a 636c 662e 6669  5-turbo").clf.fi
+00001ec0: 7428 582c 2079 290a 6c61 6265 6c73 203d  t(X, y).labels =
+00001ed0: 2063 6c66 2e70 7265 6469 6374 2858 290a   clf.predict(X).
+00001ee0: 6060 600a 0a57 6869 6c65 2074 6865 2061  ```..While the a
+00001ef0: 7069 2072 656d 6169 6e73 2074 6865 2073  pi remains the s
+00001f00: 616d 6520 6173 2066 6f72 2074 6865 207a  ame as for the z
+00001f10: 6572 6f20 7368 6f74 2063 6c61 7373 6966  ero shot classif
+00001f20: 6965 722c 2074 6865 7265 2061 7265 2061  ier, there are a
+00001f30: 2066 6577 2074 6869 6e67 7320 746f 2074   few things to t
+00001f40: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
+00001f50: 3a0a 0a2d 2074 6865 2022 7472 6169 6e69  :..- the "traini
+00001f60: 6e67 2220 7265 7175 6972 6573 2073 6f6d  ng" requires som
+00001f70: 6520 6c61 6265 6c6c 6564 2074 7261 696e  e labelled train
+00001f80: 696e 6720 6461 7461 3b0a 2d20 7468 6520  ing data;.- the 
+00001f90: 7472 6169 6e69 6e67 2073 6574 2073 686f  training set sho
+00001fa0: 756c 6420 6265 2073 6d61 6c6c 2065 6e6f  uld be small eno
+00001fb0: 7567 6820 746f 2066 6974 2069 6e74 6f20  ugh to fit into 
+00001fc0: 6120 7369 6e67 6c65 2070 726f 6d70 7420  a single prompt 
+00001fd0: 2877 6520 7265 636f 6d6d 656e 6420 7570  (we recommend up
+00001fe0: 2074 6f20 3130 2073 616d 706c 6573 2070   to 10 samples p
+00001ff0: 6572 206c 6162 656c 293b 0a2d 2062 6563  er label);.- bec
+00002000: 6175 7365 206f 6620 7468 6520 7369 676e  ause of the sign
+00002010: 6966 6963 616e 746c 7920 6c61 7267 6572  ificantly larger
+00002020: 2070 726f 6d70 742c 2074 6865 2069 6e66   prompt, the inf
+00002030: 6572 656e 6365 2074 616b 6573 206c 6f6e  erence takes lon
+00002040: 6765 7220 616e 6420 636f 6e73 756d 6573  ger and consumes
+00002050: 2068 6967 6865 7220 616d 6f75 6e74 206f   higher amount o
+00002060: 6620 746f 6b65 6e73 2e0a 0a4e 6f74 653a  f tokens...Note:
+00002070: 2061 7320 7468 6520 6d6f 6465 6c20 6973   as the model is
+00002080: 206e 6f74 2062 6569 6e67 2072 652d 7472   not being re-tr
+00002090: 6169 6e65 642c 2062 7574 2075 7365 7320  ained, but uses 
+000020a0: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
+000020b0: 6120 6475 7269 6e67 2069 6e66 6572 656e  a during inferen
+000020c0: 6365 2c20 6f6e 6520 636f 756c 6420 7361  ce, one could sa
+000020d0: 7920 7468 6174 2074 6869 7320 6973 2073  y that this is s
+000020e0: 7469 6c6c 2061 2028 6469 6666 6572 656e  till a (differen
+000020f0: 7429 207a 6572 6f2d 7368 6f74 2061 7070  t) zero-shot app
+00002100: 726f 6163 682e 0a0a 2323 2320 4479 6e61  roach...### Dyna
+00002110: 6d69 6320 4665 772d 5368 6f74 2054 6578  mic Few-Shot Tex
+00002120: 7420 436c 6173 7369 6669 6361 7469 6f6e  t Classification
+00002130: 0a0a 6044 796e 616d 6963 4665 7753 686f  ..`DynamicFewSho
+00002140: 7447 5054 436c 6173 7369 6669 6572 6020  tGPTClassifier` 
+00002150: 6479 6e61 6d69 6361 6c6c 7920 7365 6c65  dynamically sele
+00002160: 6374 7320 4e20 7361 6d70 6c65 7320 7065  cts N samples pe
+00002170: 7220 636c 6173 7320 746f 2069 6e63 6c75  r class to inclu
+00002180: 6465 2069 6e20 7468 6520 7072 6f6d 7074  de in the prompt
+00002190: 2e20 5468 6973 2061 6c6c 6f77 7320 7468  . This allows th
+000021a0: 6520 6665 772d 7368 6f74 2063 6c61 7373  e few-shot class
+000021b0: 6966 6965 7220 746f 2073 6361 6c65 2074  ifier to scale t
+000021c0: 6f20 6461 7461 7365 7473 2074 6861 7420  o datasets that 
+000021d0: 6172 6520 746f 6f20 6c61 7267 6520 666f  are too large fo
+000021e0: 7220 7468 6520 7374 616e 6461 7264 2063  r the standard c
+000021f0: 6f6e 7465 7874 2077 696e 646f 7720 6f66  ontext window of
+00002200: 204c 4c4d 732e 0a0a 2a48 6f77 2064 6f65   LLMs...*How doe
+00002210: 7320 6974 2077 6f72 6b3f 2a0a 0a44 7572  s it work?*..Dur
+00002220: 696e 6720 6669 7474 696e 672c 2074 6865  ing fitting, the
+00002230: 2077 686f 6c65 2064 6174 6173 6574 2069   whole dataset i
+00002240: 7320 7061 7274 6974 696f 6e65 6420 6279  s partitioned by
+00002250: 2063 6c61 7373 2c20 7665 6374 6f72 697a   class, vectoriz
+00002260: 6564 2c20 616e 6420 7374 6f72 6564 2e0a  ed, and stored..
+00002270: 0a44 7572 696e 6720 696e 6665 7265 6e63  .During inferenc
+00002280: 652c 2074 6865 205b 616e 6e6f 795d 2868  e, the [annoy](h
+00002290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000022a0: 6d2f 7370 6f74 6966 792f 616e 6e6f 7929  m/spotify/annoy)
+000022b0: 206c 6962 7261 7279 2069 7320 7573 6564   library is used
+000022c0: 2066 6f72 2066 6173 7420 6e65 6967 6862   for fast neighb
+000022d0: 6f72 206c 6f6f 6b75 702c 2077 6869 6368  or lookup, which
+000022e0: 2061 6c6c 6f77 7320 696e 636c 7564 696e   allows includin
+000022f0: 6720 6f6e 6c79 2074 6865 206d 6f73 7420  g only the most 
+00002300: 7369 6d69 6c61 7220 6578 616d 706c 6573  similar examples
+00002310: 2069 6e20 7468 6520 7072 6f6d 7074 2e0a   in the prompt..
+00002320: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00002330: 736b 6c6c 6d20 696d 706f 7274 2044 796e  skllm import Dyn
+00002340: 616d 6963 4665 7753 686f 7447 5054 436c  amicFewShotGPTCl
+00002350: 6173 7369 6669 6572 0a66 726f 6d20 736b  assifier.from sk
+00002360: 6c6c 6d2e 6461 7461 7365 7473 2069 6d70  llm.datasets imp
+00002370: 6f72 7420 6765 745f 636c 6173 7369 6669  ort get_classifi
+00002380: 6361 7469 6f6e 5f64 6174 6173 6574 0a0a  cation_dataset..
+00002390: 582c 2079 203d 2067 6574 5f63 6c61 7373  X, y = get_class
+000023a0: 6966 6963 6174 696f 6e5f 6461 7461 7365  ification_datase
+000023b0: 7428 290a 0a63 6c66 203d 2044 796e 616d  t()..clf = Dynam
+000023c0: 6963 4665 7753 686f 7447 5054 436c 6173  icFewShotGPTClas
+000023d0: 7369 6669 6572 286e 5f65 7861 6d70 6c65  sifier(n_example
+000023e0: 733d 3329 0a63 6c66 2e66 6974 2858 2c20  s=3).clf.fit(X, 
+000023f0: 7929 0a6c 6162 656c 7320 3d20 636c 662e  y).labels = clf.
+00002400: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
+00002410: 2323 2320 5465 7874 2043 6c61 7373 6966  ### Text Classif
+00002420: 6963 6174 696f 6e20 7769 7468 2047 6f6f  ication with Goo
+00002430: 676c 6520 5061 4c4d 2032 0a0a 4174 2074  gle PaLM 2..At t
+00002440: 6865 206d 6f6d 656e 7420 3320 5061 4c4d  he moment 3 PaLM
+00002450: 2062 6173 6564 206d 6f64 656c 7320 6172   based models ar
+00002460: 6520 6176 6169 6c61 626c 6520 696e 2074  e available in t
+00002470: 6573 7420 6d6f 6465 3a0a 2d20 605a 6572  est mode:.- `Zer
+00002480: 6f53 686f 7450 614c 4d43 6c61 7373 6966  oShotPaLMClassif
+00002490: 6965 7260 202d 207a 6572 6f2d 7368 6f74  ier` - zero-shot
+000024a0: 2074 6578 7420 636c 6173 7369 6669 6361   text classifica
+000024b0: 7469 6f6e 2077 6974 6820 5061 4c4d 2032  tion with PaLM 2
+000024c0: 3b0a 2d20 6050 614c 4d43 6c61 7373 6966  ;.- `PaLMClassif
+000024d0: 6965 7260 202d 2066 696e 652d 7475 6e61  ier` - fine-tuna
+000024e0: 626c 6520 7465 7874 2063 6c61 7373 6966  ble text classif
+000024f0: 6965 7220 7769 7468 2050 614c 4d20 323b  ier with PaLM 2;
+00002500: 0a2d 2060 5061 4c4d 6020 2d20 6669 6e65  .- `PaLM` - fine
+00002510: 2d74 756e 6162 6c65 2065 7374 696d 6174  -tunable estimat
+00002520: 6f72 2074 6861 7420 6361 6e20 6265 2074  or that can be t
+00002530: 7261 696e 6564 206f 6e20 6172 6269 7472  rained on arbitr
+00002540: 6172 7920 7465 7874 2069 6e70 7574 2d6f  ary text input-o
+00002550: 7574 7075 7420 7061 6972 732e 0a0a 4578  utput pairs...Ex
+00002560: 616d 706c 653a 200a 0a60 6060 7079 7468  ample: ..```pyth
+00002570: 6f6e 0a66 726f 6d20 736b 6c6c 6d2e 6d6f  on.from skllm.mo
+00002580: 6465 6c73 2e70 616c 6d20 696d 706f 7274  dels.palm import
+00002590: 2050 614c 4d43 6c61 7373 6966 6965 720a   PaLMClassifier.
+000025a0: 6672 6f6d 2073 6b6c 6c6d 2e64 6174 6173  from skllm.datas
+000025b0: 6574 7320 696d 706f 7274 2067 6574 5f63  ets import get_c
+000025c0: 6c61 7373 6966 6963 6174 696f 6e5f 6461  lassification_da
+000025d0: 7461 7365 740a 0a58 2c20 7920 3d20 6765  taset..X, y = ge
+000025e0: 745f 636c 6173 7369 6669 6361 7469 6f6e  t_classification
+000025f0: 5f64 6174 6173 6574 2829 0a0a 636c 6620  _dataset()..clf 
+00002600: 3d20 5061 4c4d 436c 6173 7369 6669 6572  = PaLMClassifier
+00002610: 286e 5f75 7064 6174 655f 7374 6570 733d  (n_update_steps=
+00002620: 3130 3029 0a63 6c66 2e66 6974 2858 2c20  100).clf.fit(X, 
+00002630: 7929 0a6c 6162 656c 7320 3d20 636c 662e  y).labels = clf.
+00002640: 7072 6564 6963 7428 5829 0a60 6060 0a0a  predict(X).```..
+00002650: 4120 6d6f 7265 2064 6574 6169 6c65 6420  A more detailed 
+00002660: 646f 6375 6d65 6e74 6174 696f 6e20 7769  documentation wi
+00002670: 6c6c 2066 6f6c 6c6f 7720 736f 6f6e 2e20  ll follow soon. 
+00002680: 466f 7220 6e6f 772c 2070 6c65 6173 6520  For now, please 
+00002690: 7265 6665 7220 746f 206f 7572 205b 6f66  refer to our [of
+000026a0: 6669 6369 616c 2067 7569 6465 206f 6e20  ficial guide on 
+000026b0: 4d65 6469 756d 5d28 6874 7470 733a 2f2f  Medium](https://
+000026c0: 6d65 6469 756d 2e63 6f6d 2f40 6972 796e  medium.com/@iryn
+000026d0: 6132 3330 3532 3029 2e0a 0a23 2323 2054  a230520)...### T
+000026e0: 6578 7420 5665 6374 6f72 697a 6174 696f  ext Vectorizatio
+000026f0: 6e0a 0a41 7320 616e 2061 6c74 6572 6e61  n..As an alterna
+00002700: 7469 7665 2074 6f20 7573 696e 6720 4750  tive to using GP
+00002710: 5420 6173 2061 2063 6c61 7373 6966 6965  T as a classifie
+00002720: 722c 2069 7420 6361 6e20 6265 2075 7365  r, it can be use
+00002730: 6420 736f 6c65 6c79 2066 6f72 2064 6174  d solely for dat
+00002740: 6120 7072 6570 726f 6365 7373 696e 672e  a preprocessing.
+00002750: 2060 4750 5456 6563 746f 7269 7a65 7260   `GPTVectorizer`
+00002760: 2061 6c6c 6f77 7320 746f 2065 6d62 6564   allows to embed
+00002770: 2061 2063 6875 6e6b 206f 6620 7465 7874   a chunk of text
+00002780: 206f 6620 6172 6269 7472 6172 7920 6c65   of arbitrary le
+00002790: 6e67 7468 2074 6f20 6120 6669 7865 642d  ngth to a fixed-
+000027a0: 6469 6d65 6e73 696f 6e61 6c20 7665 6374  dimensional vect
+000027b0: 6f72 2c20 7468 6174 2063 616e 2062 6520  or, that can be 
+000027c0: 7573 6564 2077 6974 6820 7669 7274 7561  used with virtua
+000027d0: 6c6c 7920 616e 7920 636c 6173 7369 6669  lly any classifi
+000027e0: 6361 7469 6f6e 206f 7220 7265 6772 6573  cation or regres
+000027f0: 7369 6f6e 206d 6f64 656c 2e0a 0a45 7861  sion model...Exa
+00002800: 6d70 6c65 2031 3a20 456d 6265 6464 696e  mple 1: Embeddin
+00002810: 6720 7468 6520 7465 7874 0a0a 6060 6070  g the text..```p
+00002820: 7974 686f 6e0a 6672 6f6d 2073 6b6c 6c6d  ython.from skllm
+00002830: 2e70 7265 7072 6f63 6573 7369 6e67 2069  .preprocessing i
+00002840: 6d70 6f72 7420 4750 5456 6563 746f 7269  mport GPTVectori
+00002850: 7a65 720a 0a6d 6f64 656c 203d 2047 5054  zer..model = GPT
+00002860: 5665 6374 6f72 697a 6572 2829 0a76 6563  Vectorizer().vec
+00002870: 746f 7273 203d 206d 6f64 656c 2e66 6974  tors = model.fit
+00002880: 5f74 7261 6e73 666f 726d 2858 290a 6060  _transform(X).``
+00002890: 600a 0a45 7861 6d70 6c65 2032 3a20 436f  `..Example 2: Co
+000028a0: 6d62 696e 696e 6720 7468 6520 5665 6374  mbining the Vect
+000028b0: 6f72 697a 6572 2077 6974 6820 7468 6520  orizer with the 
+000028c0: 5847 426f 6f73 7420 436c 6173 7369 6669  XGBoost Classifi
+000028d0: 6572 2069 6e20 6120 536b 6c65 6172 6e20  er in a Sklearn 
+000028e0: 5069 7065 6c69 6e65 0a0a 6060 6070 7974  Pipeline..```pyt
+000028f0: 686f 6e0a 6672 6f6d 2073 6b6c 6561 726e  hon.from sklearn
+00002900: 2e70 6970 656c 696e 6520 696d 706f 7274  .pipeline import
+00002910: 2050 6970 656c 696e 650a 6672 6f6d 2073   Pipeline.from s
+00002920: 6b6c 6561 726e 2e70 7265 7072 6f63 6573  klearn.preproces
+00002930: 7369 6e67 2069 6d70 6f72 7420 4c61 6265  sing import Labe
+00002940: 6c45 6e63 6f64 6572 0a66 726f 6d20 7867  lEncoder.from xg
+00002950: 626f 6f73 7420 696d 706f 7274 2058 4742  boost import XGB
+00002960: 436c 6173 7369 6669 6572 0a0a 6c65 203d  Classifier..le =
+00002970: 204c 6162 656c 456e 636f 6465 7228 290a   LabelEncoder().
+00002980: 795f 7472 6169 6e5f 656e 636f 6465 6420  y_train_encoded 
+00002990: 3d20 6c65 2e66 6974 5f74 7261 6e73 666f  = le.fit_transfo
+000029a0: 726d 2879 5f74 7261 696e 290a 795f 7465  rm(y_train).y_te
+000029b0: 7374 5f65 6e63 6f64 6564 203d 206c 652e  st_encoded = le.
+000029c0: 7472 616e 7366 6f72 6d28 795f 7465 7374  transform(y_test
+000029d0: 290a 0a73 7465 7073 203d 205b 2822 4750  )..steps = [("GP
+000029e0: 5422 2c20 4750 5456 6563 746f 7269 7a65  T", GPTVectorize
+000029f0: 7228 2929 2c20 2822 436c 6622 2c20 5847  r()), ("Clf", XG
+00002a00: 4243 6c61 7373 6966 6965 7228 2929 5d0a  BClassifier())].
+00002a10: 636c 6620 3d20 5069 7065 6c69 6e65 2873  clf = Pipeline(s
+00002a20: 7465 7073 290a 636c 662e 6669 7428 585f  teps).clf.fit(X_
+00002a30: 7472 6169 6e2c 2079 5f74 7261 696e 5f65  train, y_train_e
+00002a40: 6e63 6f64 6564 290a 7968 203d 2063 6c66  ncoded).yh = clf
+00002a50: 2e70 7265 6469 6374 2858 5f74 6573 7429  .predict(X_test)
+00002a60: 0a60 6060 0a0a 2323 2320 5465 7874 2053  .```..### Text S
+00002a70: 756d 6d61 7269 7a61 7469 6f6e 0a0a 4750  ummarization..GP
+00002a80: 5420 6578 6365 6c73 2061 7420 7065 7266  T excels at perf
+00002a90: 6f72 6d69 6e67 2073 756d 6d61 7269 7a61  orming summariza
+00002aa0: 7469 6f6e 2074 6173 6b73 2e20 5468 6572  tion tasks. Ther
+00002ab0: 6566 6f72 652c 2077 6520 7072 6f76 6964  efore, we provid
+00002ac0: 6520 6047 5054 5375 6d6d 6172 697a 6572  e `GPTSummarizer
+00002ad0: 6020 7468 6174 2063 616e 2062 6520 7573  ` that can be us
+00002ae0: 6564 2062 6f74 6820 6173 2073 7461 6e64  ed both as stand
+00002af0: 2d61 6c6f 6e65 2065 7374 696d 6174 6f72  -alone estimator
+00002b00: 2c20 6f72 2061 7320 6120 7072 6570 726f  , or as a prepro
+00002b10: 6365 7373 6f72 2028 696e 2074 6869 7320  cessor (in this 
+00002b20: 6361 7365 2077 6520 6361 6e20 6d61 6b65  case we can make
+00002b30: 2061 6e20 616e 616c 6f67 7920 7769 7468   an analogy with
+00002b40: 2061 2064 696d 656e 7369 6f6e 616c 6974   a dimensionalit
+00002b50: 7920 7265 6475 6374 696f 6e20 7072 6570  y reduction prep
+00002b60: 726f 6365 7373 6f72 292e 0a0a 4578 616d  rocessor)...Exam
+00002b70: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00002b80: 6672 6f6d 2073 6b6c 6c6d 2e70 7265 7072  from skllm.prepr
+00002b90: 6f63 6573 7369 6e67 2069 6d70 6f72 7420  ocessing import 
+00002ba0: 4750 5453 756d 6d61 7269 7a65 720a 6672  GPTSummarizer.fr
+00002bb0: 6f6d 2073 6b6c 6c6d 2e64 6174 6173 6574  om skllm.dataset
+00002bc0: 7320 696d 706f 7274 2067 6574 5f73 756d  s import get_sum
+00002bd0: 6d61 7269 7a61 7469 6f6e 5f64 6174 6173  marization_datas
+00002be0: 6574 0a0a 5820 3d20 6765 745f 7375 6d6d  et..X = get_summ
+00002bf0: 6172 697a 6174 696f 6e5f 6461 7461 7365  arization_datase
+00002c00: 7428 290a 7320 3d20 4750 5453 756d 6d61  t().s = GPTSumma
+00002c10: 7269 7a65 7228 6f70 656e 6169 5f6d 6f64  rizer(openai_mod
+00002c20: 656c 3d22 6770 742d 332e 352d 7475 7262  el="gpt-3.5-turb
+00002c30: 6f22 2c20 6d61 785f 776f 7264 733d 3135  o", max_words=15
+00002c40: 290a 7375 6d6d 6172 6965 7320 3d20 732e  ).summaries = s.
+00002c50: 6669 745f 7472 616e 7366 6f72 6d28 5829  fit_transform(X)
+00002c60: 0a60 6060 0a0a 506c 6561 7365 2062 6520  .```..Please be 
+00002c70: 6177 6172 6520 7468 6174 2074 6865 2060  aware that the `
+00002c80: 6d61 785f 776f 7264 7360 2068 7970 6572  max_words` hyper
+00002c90: 7061 7261 6d65 7465 7220 7365 7473 2061  parameter sets a
+00002ca0: 2073 6f66 7420 6c69 6d69 742c 2077 6869   soft limit, whi
+00002cb0: 6368 2069 7320 6e6f 7420 7374 7269 6374  ch is not strict
+00002cc0: 6c79 2065 6e66 6f72 6365 6420 6f75 7473  ly enforced outs
+00002cd0: 6964 6520 6f66 2074 6865 2070 726f 6d70  ide of the promp
+00002ce0: 742e 2054 6865 7265 666f 7265 2c20 696e  t. Therefore, in
+00002cf0: 2073 6f6d 6520 6361 7365 732c 2074 6865   some cases, the
+00002d00: 2061 6374 7561 6c20 6e75 6d62 6572 206f   actual number o
+00002d10: 6620 776f 7264 7320 6d69 6768 7420 6265  f words might be
+00002d20: 2073 6c69 6768 746c 7920 6869 6768 6572   slightly higher
+00002d30: 2e0a 0a49 7420 6973 2070 6f73 7369 626c  ...It is possibl
+00002d40: 6520 746f 2067 656e 6572 6174 6520 6120  e to generate a 
+00002d50: 7375 6d6d 6172 792c 2065 6d70 6861 7369  summary, emphasi
+00002d60: 7a69 6e67 2061 2073 7065 6369 6669 6320  zing a specific 
+00002d70: 636f 6e63 6570 742c 2062 7920 7072 6f76  concept, by prov
+00002d80: 6964 696e 6720 616e 206f 7074 696f 6e61  iding an optiona
+00002d90: 6c20 7061 7261 6d65 7465 7220 6066 6f63  l parameter `foc
+00002da0: 7573 603a 0a0a 6060 6070 7974 686f 6e0a  us`:..```python.
+00002db0: 7320 3d20 4750 5453 756d 6d61 7269 7a65  s = GPTSummarize
+00002dc0: 7228 6f70 656e 6169 5f6d 6f64 656c 3d22  r(openai_model="
+00002dd0: 6770 742d 332e 352d 7475 7262 6f22 2c20  gpt-3.5-turbo", 
+00002de0: 6d61 785f 776f 7264 733d 3135 2c20 666f  max_words=15, fo
+00002df0: 6375 733d 2261 7070 6c65 7322 290a 6060  cus="apples").``
+00002e00: 600a 0a23 2323 2054 6578 7420 5472 616e  `..### Text Tran
+00002e10: 736c 6174 696f 6e0a 0a47 5054 206d 6f64  slation..GPT mod
+00002e20: 656c 7320 6861 7665 2064 656d 6f6e 7374  els have demonst
+00002e30: 7261 7465 6420 7468 6569 7220 6566 6665  rated their effe
+00002e40: 6374 6976 656e 6573 7320 696e 2074 7261  ctiveness in tra
+00002e50: 6e73 6c61 7469 6f6e 2074 6173 6b73 2062  nslation tasks b
+00002e60: 7920 6765 6e65 7261 7469 6e67 2061 6363  y generating acc
+00002e70: 7572 6174 6520 7472 616e 736c 6174 696f  urate translatio
+00002e80: 6e73 2061 6372 6f73 7320 7661 7269 6f75  ns across variou
+00002e90: 7320 6c61 6e67 7561 6765 732e 2054 6875  s languages. Thu
+00002ea0: 732c 2077 6520 6164 6465 6420 6047 5054  s, we added `GPT
+00002eb0: 5472 616e 736c 6174 6f72 6020 7468 6174  Translator` that
+00002ec0: 2061 6c6c 6f77 7320 7472 616e 736c 6174   allows translat
+00002ed0: 696e 6720 616e 2061 7262 6974 7261 7479  ing an arbitraty
+00002ee0: 2074 6578 7420 696e 746f 2061 206c 616e   text into a lan
+00002ef0: 6775 6167 6520 6f66 2069 6e74 6572 6573  guage of interes
+00002f00: 742e 0a0a 4578 616d 706c 653a 0a0a 6060  t...Example:..``
+00002f10: 6070 7974 686f 6e0a 6672 6f6d 2073 6b6c  `python.from skl
+00002f20: 6c6d 2e70 7265 7072 6f63 6573 7369 6e67  lm.preprocessing
+00002f30: 2069 6d70 6f72 7420 4750 5454 7261 6e73   import GPTTrans
+00002f40: 6c61 746f 720a 6672 6f6d 2073 6b6c 6c6d  lator.from skllm
+00002f50: 2e64 6174 6173 6574 7320 696d 706f 7274  .datasets import
+00002f60: 2067 6574 5f74 7261 6e73 6c61 7469 6f6e   get_translation
+00002f70: 5f64 6174 6173 6574 0a0a 5820 3d20 6765  _dataset..X = ge
+00002f80: 745f 7472 616e 736c 6174 696f 6e5f 6461  t_translation_da
+00002f90: 7461 7365 7428 290a 7420 3d20 4750 5454  taset().t = GPTT
+00002fa0: 7261 6e73 6c61 746f 7228 6f70 656e 6169  ranslator(openai
+00002fb0: 5f6d 6f64 656c 3d22 6770 742d 332e 352d  _model="gpt-3.5-
+00002fc0: 7475 7262 6f22 2c20 6f75 7470 7574 5f6c  turbo", output_l
+00002fd0: 616e 6775 6167 653d 2245 6e67 6c69 7368  anguage="English
+00002fe0: 2229 0a74 7261 6e73 6c61 7465 645f 7465  ").translated_te
+00002ff0: 7874 203d 2074 2e66 6974 5f74 7261 6e73  xt = t.fit_trans
+00003000: 666f 726d 2858 290a 6060 600a 0a         form(X).```..
```

### Comparing `scikit-llm-0.2.0/scikit_llm.egg-info/SOURCES.txt` & `scikit-llm-0.3.0/scikit_llm.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,27 @@
 skllm/gpt4all_client.py
 skllm/utils.py
 skllm/datasets/__init__.py
 skllm/datasets/multi_class.py
 skllm/datasets/multi_label.py
 skllm/datasets/summarization.py
 skllm/datasets/translation.py
+skllm/google/completions.py
+skllm/google/tuning.py
 skllm/memory/__init__.py
 skllm/memory/_annoy.py
 skllm/memory/base.py
-skllm/models/gpt_dyn_few_shot_clf.py
-skllm/models/gpt_few_shot_clf.py
-skllm/models/gpt_zero_shot_clf.py
+skllm/models/_base.py
+skllm/models/gpt/__init__.py
+skllm/models/gpt/gpt_dyn_few_shot_clf.py
+skllm/models/gpt/gpt_few_shot_clf.py
+skllm/models/gpt/gpt_zero_shot_clf.py
+skllm/models/palm/__init__.py
+skllm/models/palm/palm_clf.py
+skllm/models/palm/palm_est.py
 skllm/openai/base_gpt.py
 skllm/openai/chatgpt.py
 skllm/openai/credentials.py
 skllm/openai/embeddings.py
 skllm/openai/mixin.py
 skllm/preprocessing/__init__.py
 skllm/preprocessing/gpt_summarizer.py
```

### Comparing `scikit-llm-0.2.0/skllm/completions.py` & `scikit-llm-0.3.0/skllm/completions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from skllm.gpt4all_client import get_chat_completion as _g4a_get_chat_completion
 from skllm.openai.chatgpt import get_chat_completion as _oai_get_chat_completion
 
 
 def get_chat_completion(
-    messages: dict, openai_key: str=None, openai_org: str=None, model: str="gpt-3.5-turbo", max_retries: int=3
+    messages: dict,
+    openai_key: str = None,
+    openai_org: str = None,
+    model: str = "gpt-3.5-turbo",
+    max_retries: int = 3,
 ):
-    """
-    Gets a chat completion from the OpenAI API.
-    """
+    """Gets a chat completion from the OpenAI API."""
     if model.startswith("gpt4all::"):
         return _g4a_get_chat_completion(messages, model[9:])
     else:
+        api = "azure" if model.startswith("azure::") else "openai"
+        if api == "azure":
+            model = model[7:]
         return _oai_get_chat_completion(
-            messages, openai_key, openai_org, model, max_retries
+            messages, openai_key, openai_org, model, max_retries, api=api
         )
```

### Comparing `scikit-llm-0.2.0/skllm/datasets/multi_class.py` & `scikit-llm-0.3.0/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/datasets/multi_label.py` & `scikit-llm-0.3.0/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/datasets/summarization.py` & `scikit-llm-0.3.0/skllm/datasets/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/datasets/translation.py` & `scikit-llm-0.3.0/skllm/datasets/translation.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/gpt4all_client.py` & `scikit-llm-0.3.0/skllm/gpt4all_client.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/memory/_annoy.py` & `scikit-llm-0.3.0/skllm/memory/_annoy.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/memory/base.py` & `scikit-llm-0.3.0/skllm/memory/base.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/models/gpt_dyn_few_shot_clf.py` & `scikit-llm-0.3.0/skllm/models/gpt/gpt_dyn_few_shot_clf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
-from skllm import FewShotGPTClassifier
 from skllm.memory import AnnoyMemoryIndex
-from skllm.models.gpt_few_shot_clf import _TRAINING_SAMPLE_PROMPT_TEMPLATE
+from skllm.models._base import _BaseZeroShotGPTClassifier
 from skllm.preprocessing import GPTVectorizer
 from skllm.prompts.builders import build_few_shot_prompt_slc
 from skllm.utils import to_numpy
 
+_TRAINING_SAMPLE_PROMPT_TEMPLATE = """
+Sample input:
+```{x}```
 
-class DynamicFewShotGPTClassifier(FewShotGPTClassifier):
+Sample target: {label}
+"""
+
+
+class DynamicFewShotGPTClassifier(_BaseZeroShotGPTClassifier):
     """Dynamic few-shot single-label classifier.
 
     Parameters
     ----------
     n_examples : int, optional
         number of examples per class, by default 3
     openai_key : Optional[str] , default : None
```

### Comparing `scikit-llm-0.2.0/skllm/models/gpt_few_shot_clf.py` & `scikit-llm-0.3.0/skllm/models/gpt/gpt_few_shot_clf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
 
-from skllm.models.gpt_zero_shot_clf import (
-    ZeroShotGPTClassifier as _ZeroShotGPTClassifier,
-)
+from skllm.models._base import _BaseZeroShotGPTClassifier
 from skllm.prompts.builders import build_few_shot_prompt_slc
 from skllm.utils import to_numpy as _to_numpy
 
 _TRAINING_SAMPLE_PROMPT_TEMPLATE = """
 Sample input:
 ```{x}```
 
 Sample target: {label}
 """
 
 
-class FewShotGPTClassifier(_ZeroShotGPTClassifier):
+class FewShotGPTClassifier(_BaseZeroShotGPTClassifier):
     """Few-shot single-label classifier."""
 
     def fit(
         self,
         X: Union[np.ndarray, pd.Series, List[str]],
         y: Union[np.ndarray, pd.Series, List[str]],
     ):
```

### Comparing `scikit-llm-0.2.0/skllm/openai/base_gpt.py` & `scikit-llm-0.3.0/skllm/openai/base_gpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,98 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional, Union
+from typing import Any
 
 import numpy as np
 import pandas as pd
 from numpy import ndarray
 from sklearn.base import BaseEstimator as _BaseEstimator
 from sklearn.base import TransformerMixin as _TransformerMixin
 from tqdm import tqdm
 
 from skllm.openai.chatgpt import construct_message, get_chat_completion
 from skllm.openai.mixin import OpenAIMixin as _OAIMixin
 from skllm.utils import to_numpy as _to_numpy
 
 
-class BaseZeroShotGPTTransformer(_BaseEstimator, _TransformerMixin, _OAIMixin): 
-    
+class BaseZeroShotGPTTransformer(_BaseEstimator, _TransformerMixin, _OAIMixin):
     system_msg = "You are an scikit-learn transformer."
     default_output = "Output is unavailable"
 
     def _get_chat_completion(self, X):
-        """
-        Gets the chat completion for the given input using open ai API.
+        """Gets the chat completion for the given input using open ai API.
 
         Parameters
         ----------
         X : str
             Input string
-        
+
         Returns
         -------
         str
-        
         """
         prompt = self._get_prompt(X)
         msgs = []
         msgs.append(construct_message("system", self.system_msg))
         msgs.append(construct_message("user", prompt))
         completion = get_chat_completion(
             msgs, self._get_openai_key(), self._get_openai_org(), self.openai_model
         )
         try:
             return completion.choices[0].message["content"]
         except Exception as e:
             print(f"Skipping a sample due to the following error: {str(e)}")
             return self.default_output
-            
-    def fit(self, X: Any = None, y: Any = None, **kwargs: Any) -> BaseZeroShotGPTTransformer:
-        """
-        Fits the model to the data.
+
+    def fit(
+        self, X: Any = None, y: Any = None, **kwargs: Any
+    ) -> BaseZeroShotGPTTransformer:
+        """Fits the model to the data.
 
         Parameters
         ----------
         X : Any, optional
         y : Any, optional
         kwargs : dict, optional
 
         Returns
         -------
         self : BaseZeroShotGPTTransformer
         """
-
         return self
 
-    def transform(self, X: Optional[Union[np.ndarray, pd.Series, List[str]]], **kwargs: Any) -> ndarray:
-        """
-        Converts a list of strings using the open ai API and a predefined prompt.
+    def transform(
+        self, X: np.ndarray | pd.Series | list[str], **kwargs: Any
+    ) -> ndarray:
+        """Converts a list of strings using the open ai API and a predefined
+        prompt.
 
         Parameters
         ----------
         X : Union[np.ndarray, pd.Series, List[str]]
 
         Returns
         -------
         ndarray
         """
         X = _to_numpy(X)
         transformed = []
         for i in tqdm(range(len(X))):
-            transformed.append(
-                self._get_chat_completion(X[i])
-            )
-        transformed = np.asarray(transformed, dtype = object)
+            transformed.append(self._get_chat_completion(X[i]))
+        transformed = np.asarray(transformed, dtype=object)
         return transformed
 
-    def fit_transform(self, X: Optional[Union[np.ndarray, pd.Series, List[str]]], y=None, **fit_params) -> ndarray:
-        """
-        Fits and transforms a list of strings using the transform method.
-        This is modelled to function as the sklearn fit_transform method
+    def fit_transform(
+        self, X: np.ndarray | pd.Series | list[str], y=None, **fit_params
+    ) -> ndarray:
+        """Fits and transforms a list of strings using the transform method.
+        This is modelled to function as the sklearn fit_transform method.
 
         Parameters
         ----------
         X : np.ndarray, pd.Series, or list
 
         Returns
         -------
-        ndarray       
+        ndarray
         """
-        return self.fit(X, y).transform(X)
+        return self.fit(X, y).transform(X)
```

### Comparing `scikit-llm-0.2.0/skllm/openai/embeddings.py` & `scikit-llm-0.3.0/skllm/openai/embeddings.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/openai/mixin.py` & `scikit-llm-0.3.0/skllm/openai/mixin.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/preprocessing/gpt_vectorizer.py` & `scikit-llm-0.3.0/skllm/preprocessing/gpt_vectorizer.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/skllm/prompts/builders.py` & `scikit-llm-0.3.0/skllm/prompts/builders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 from skllm.prompts.templates import (
     FEW_SHOT_CLF_PROMPT_TEMPLATE,
+    FOCUSED_SUMMARY_PROMPT_TEMPLATE,
     SUMMARY_PROMPT_TEMPLATE,
     TRANSLATION_PROMPT_TEMPLATE,
     ZERO_SHOT_CLF_PROMPT_TEMPLATE,
     ZERO_SHOT_MLCLF_PROMPT_TEMPLATE,
 )
 
 # TODO add validators
@@ -105,14 +106,41 @@
     -------
     str
         prepared prompt
     """
     return template.format(x=x, max_words=max_words)
 
 
+def build_focused_summary_prompt(
+    x: str,
+    max_words: Union[int, str],
+    focus: Union[int, str],
+    template: str = FOCUSED_SUMMARY_PROMPT_TEMPLATE,
+) -> str:
+    """Builds a prompt for focused text summarization.
+
+    Parameters
+    ----------
+    x : str
+        sample to summarize
+    max_words : Union[int,str]
+        maximum number of words to use in the summary
+    focus : Union[int,str]
+        the topic(s) to focus on
+    template : str
+        prompt template to use, must contain placeholders for all variables, by default FOCUSED_SUMMARY_PROMPT_TEMPLATE
+
+    Returns
+    -------
+    str
+        prepared prompt
+    """
+    return template.format(x=x, max_words=max_words, focus=focus)
+
+
 def build_translation_prompt(
     x: str, output_language: str, template: str = TRANSLATION_PROMPT_TEMPLATE
 ) -> str:
     """Builds a prompt for text translation.
 
     Parameters
     ----------
```

### Comparing `scikit-llm-0.2.0/skllm/prompts/templates.py` & `scikit-llm-0.3.0/skllm/prompts/templates.py`

 * *Files 23% similar despite different names*

```diff
@@ -57,21 +57,33 @@
 Your task is to generate a summary of the text sample.
 Summarize the text sample provided below, delimited by triple backticks, in at most {max_words} words.
 
 Text sample: ```{x}```
 Summarized text:
 """
 
-TRANSLATION_PROMPT_TEMPLATE = """
-You will be provided with an arbitrary text sample, delimited by triple backticks.
-Your task is to translate this text to {output_language} language and output the translated text.
+FOCUSED_SUMMARY_PROMPT_TEMPLATE = """
+As an input you will receive:
+1. A focus parameter delimited with square brackets.
+2. A single text sample delimited with triple backticks.
 
 Perform the following actions:
-1. Determine the language of the text sample.
-2. If the language is not {output_language}, translate the text sample to {output_language} language.
-3. Output the translated text.
-If the text sample provided is not in a recognizable language, output "No translation available".
-Do not output any additional information except the translated text.
+1. Determine whether there is something in the text that matches focus. Do not output anything.
+2. Summarise the text in at most {max_words} words.
+3. If possible, make the summarisation focused on the concept provided in the focus parameter. Otherwise, provide a general summarisation. Do not state that general summary is provided.
+4. Do not output anything except of the summary. Do not output any text that was not present in the original text.
+5. If no focused summary possible, or the mentioned concept is not present in the text, output "Mentioned concept is not present in the text." and the general summary. Do not state that general summary is provided.
+
+Focus: [{focus}]
 
 Text sample: ```{x}```
-Translated text:
+
+Summarized text:
+"""
+
+TRANSLATION_PROMPT_TEMPLATE = """
+If the original text, delimited by triple backticks, is already in {output_language} language, output the original text.
+Otherwise, translate the original text, delimited by triple backticks, to {output_language} language, and output the translated text only. Do not output any additional information except the translated text.
+
+Original text: ```{x}```
+Output:
 """
```

### Comparing `scikit-llm-0.2.0/skllm/utils.py` & `scikit-llm-0.3.0/skllm/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,72 @@
+import json
+from typing import Any
+
 import numpy as np
 import pandas as pd
 
-from typing import Any
 
 def to_numpy(X: Any) -> np.ndarray:
-    """
-    Converts a pandas Series or list to a numpy array.
+    """Converts a pandas Series or list to a numpy array.
 
     Parameters
     ----------
     X : Any
         The data to convert to a numpy array.
-    
+
     Returns
     -------
     X : np.ndarray
     """
     if isinstance(X, pd.Series):
         X = X.to_numpy().astype(object)
     elif isinstance(X, list):
         X = np.asarray(X, dtype=object)
     if isinstance(X, np.ndarray) and len(X.shape) > 1:
         X = np.squeeze(X)
     return X
 
 
 def find_json_in_string(string: str) -> str:
-    """
-    Finds the JSON object in a string.
-    
+    """Finds the JSON object in a string.
+
     Parameters
     ----------
     string : str
         The string to search for a JSON object.
-    
+
     Returns
     -------
     json_string : str
     """
-
     start = string.find("{")
     end = string.rfind("}")
     if start != -1 and end != -1:
         json_string = string[start : end + 1]
     else:
         json_string = "{}"
     return json_string
+
+
+def extract_json_key(json_: str, key: str):
+    """Extracts JSON key from a string.
+
+    json_ : str
+        The JSON string to extract the key from.
+    key : str
+        The key to extract.
+    """
+    original_json = json_
+    for i in range(2):
+        try:
+            json_ = original_json.replace("\n", "")
+            if i == 1:
+                json_ = json_.replace("'", '"')
+            json_ = find_json_in_string(json_)
+            as_json = json.loads(json_)
+            if key not in as_json.keys():
+                raise KeyError("The required key was not found")
+            return as_json[key]
+        except Exception:
+            if i == 0:
+                continue
+            return None
```

### Comparing `scikit-llm-0.2.0/tests/test_chatgpt.py` & `scikit-llm-0.3.0/tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/tests/test_gpt_few_shot_clf.py` & `scikit-llm-0.3.0/tests/test_gpt_few_shot_clf.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.2.0/tests/test_gpt_zero_shot_clf.py` & `scikit-llm-0.3.0/tests/test_gpt_zero_shot_clf.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,25 @@
         y = np.array(["class1", "class2", "class1"])
         clf.fit(X, y)
 
         self.assertEqual(set(clf.classes_), set(["class1", "class2"]))
         self.assertEqual(clf.probabilities_, [2 / 3, 1 / 3])
         return clf
 
-    @patch(
-        "skllm.models.gpt_zero_shot_clf.get_chat_completion", return_value=MagicMock()
-    )
+    @patch("skllm.models._base.get_chat_completion", return_value=MagicMock())
     def test_fit_predict(self, mock_get_chat_completion):
         clf = self.get_mock_clf_model()
         mock_get_chat_completion.return_value.choices[0].message = {
             "content": json.dumps({"label": "class1"})
         }
         predictions = clf.predict(["text1", "text2", "text3"])
 
         self.assertEqual(predictions, ["class1", "class1", "class1"])
 
-    @patch(
-        "skllm.models.gpt_zero_shot_clf.get_chat_completion", return_value=MagicMock()
-    )
+    @patch("skllm.models._base.get_chat_completion", return_value=MagicMock())
     def test_fit_predict_unknown_label_set_default(self, mock_get_chat_completion):
         clf = self.get_mock_clf_model()
 
         # Random choice
         mock_get_chat_completion.return_value.choices[0].message = {
             "content": json.dumps({"label": "new_class"})
         }
@@ -81,29 +77,25 @@
         ]  # Adjusted y to ensure [0.5, 0.5] probability
         clf.fit(X, y)
 
         self.assertEqual(set(clf.classes_), set(["class1", "class2"]))
         self.assertEqual(clf.probabilities_, [0.5, 0.5])
         return clf
 
-    @patch(
-        "skllm.models.gpt_zero_shot_clf.get_chat_completion", return_value=MagicMock()
-    )
+    @patch("skllm.models._base.get_chat_completion", return_value=MagicMock())
     def test_fit_predict(self, mock_get_chat_completion):
         clf = self.get_mock_clf_model()
         mock_get_chat_completion.return_value = _get_ret(["class1", "class2"])
         predictions = clf.predict(["text1", "text2", "text3"])
         self.assertEqual(
             predictions,
             [["class1", "class2"], ["class1", "class2"], ["class1", "class2"]],
         )
 
-    @patch(
-        "skllm.models.gpt_zero_shot_clf.get_chat_completion", return_value=MagicMock()
-    )
+    @patch("skllm.models._base.get_chat_completion", return_value=MagicMock())
     def test_fit_predict_unknown_label_set_default(self, mock_get_chat_completion):
         clf = self.get_mock_clf_model()
         mock_get_chat_completion.return_value.choices[0].message = {
             "content": json.dumps({"label": "new_class"})
         }
 
         clf.probabilities_ = [0.0, 1.0]
```

