# Comparing `tmp/llm_agents-0.0.1-py3-none-any.whl.zip` & `tmp/llm_agents-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 5839 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      484 b- defN 23-Jul-04 19:33 llm_agents/__init__.py
 -rw-r--r--  2.0 unx     3755 b- defN 23-Jul-04 19:33 llm_agents/agent.py
 -rw-r--r--  2.0 unx      702 b- defN 23-Jul-04 19:33 llm_agents/llm.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-04 19:44 llm_agents-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3277 b- defN 23-Jul-04 19:44 llm_agents-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 19:44 llm_agents-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-04 19:44 llm_agents-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-Jul-04 19:44 llm_agents-0.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-04 19:44 llm_agents-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3277 b- defN 23-Jul-04 19:44 llm_agents-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 19:44 llm_agents-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-04 19:44 llm_agents-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jul-04 19:44 llm_agents-0.0.2.dist-info/RECORD
 8 files, 10018 bytes uncompressed, 4745 bytes compressed:  52.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: llm_agents/agent.py
 Comment: 
 
 Filename: llm_agents/llm.py
 Comment: 
 
-Filename: llm_agents-0.0.1.dist-info/LICENSE
+Filename: llm_agents-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: llm_agents-0.0.1.dist-info/METADATA
+Filename: llm_agents-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: llm_agents-0.0.1.dist-info/WHEEL
+Filename: llm_agents-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: llm_agents-0.0.1.dist-info/top_level.txt
+Filename: llm_agents-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_agents-0.0.1.dist-info/RECORD
+Filename: llm_agents-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `llm_agents-0.0.1.dist-info/LICENSE` & `llm_agents-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `llm_agents-0.0.1.dist-info/METADATA` & `llm_agents-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-agents
-Version: 0.0.1
+Version: 0.0.2
 Summary: llm_agents
 Home-page: https://github.com/mpaepper/llm_agents
 Author: Marc Päpper
 Author-email: mpaepper <mpaepper@gmx.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: llm-agents Version: 0.0.1 Summary: llm_agents Home-
+Metadata-Version: 2.1 Name: llm-agents Version: 0.0.2 Summary: llm_agents Home-
 page: https://github.com/mpaepper/llm_agents Author: Marc PÃ¤pper Author-email:
 mpaepper
 gmx.de> Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: google-search-results (>=2.4.2) Requires-Dist: openai
 (>=0.27.0) Requires-Dist: pydantic (>=1.10.5) Requires-Dist: requests
```

## Comparing `llm_agents-0.0.1.dist-info/RECORD` & `llm_agents-0.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 llm_agents/__init__.py,sha256=iQZWrMFhJowDrH0EaHPwnmC60VL6mr9ZVSh1P0NKGh4,484
 llm_agents/agent.py,sha256=aMDz5Mt_JkWY9KxSD1jMHDu-UwlPFlQCKgSn-K9pxys,3755
 llm_agents/llm.py,sha256=DfwPmdK8fGgYsiXSQYNcFPe0dqC8hRn-aoYnbiaZPC4,702
-llm_agents-0.0.1.dist-info/LICENSE,sha256=blPOzDwffgLgZKoUJYl9pSSkAVLL1tIRZhRYsehqagA,1069
-llm_agents-0.0.1.dist-info/METADATA,sha256=eDw0qIXA26WTDYSW22arnLoLJQPoDQcuwsD4yoRdo1E,3277
-llm_agents-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-llm_agents-0.0.1.dist-info/top_level.txt,sha256=wH_SBC-XosfIHLaeT96zREd7Z0XhTr8FYQONtZhqLvs,11
-llm_agents-0.0.1.dist-info/RECORD,,
+llm_agents-0.0.2.dist-info/LICENSE,sha256=blPOzDwffgLgZKoUJYl9pSSkAVLL1tIRZhRYsehqagA,1069
+llm_agents-0.0.2.dist-info/METADATA,sha256=ZV4KzvVwjEFahAqupx57-pj6gSSw-Z92uIRIWRSafTw,3277
+llm_agents-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+llm_agents-0.0.2.dist-info/top_level.txt,sha256=wH_SBC-XosfIHLaeT96zREd7Z0XhTr8FYQONtZhqLvs,11
+llm_agents-0.0.2.dist-info/RECORD,,
```

