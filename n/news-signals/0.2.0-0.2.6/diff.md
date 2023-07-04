# Comparing `tmp/news-signals-0.2.0.tar.gz` & `tmp/news-signals-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.2.0.tar", last modified: Sun May 21 22:29:08 2023, max compression
+gzip compressed data, was "news-signals-0.2.6.tar", last modified: Tue Jul  4 07:51:31 2023, max compression
```

## Comparing `news-signals-0.2.0.tar` & `news-signals-0.2.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.288320 news-signals-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-21 22:28:54.000000 news-signals-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 22:28:54.000000 news-signals-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-21 22:29:08.288320 news-signals-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-21 22:28:54.000000 news-signals-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 22:28:54.000000 news-signals-0.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.280320 news-signals-0.2.0/news_signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    38558 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_aql_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_dataset_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_exogenous_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_newsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_representative_story.py
--rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_signals_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/wikidata_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-21 22:28:54.000000 news-signals-0.2.0/news_signals/yfinance_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.280320 news-signals-0.2.0/news_signals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 22:29:08.000000 news-signals-0.2.0/news_signals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.276320 news-signals-0.2.0/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.284320 news-signals-0.2.0/resources/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/elon_musk_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100.small.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:29:08.288320 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/politics_china_australia_timeseries.json
--rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/sample_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-05-21 22:28:54.000000 news-signals-0.2.0/resources/test/tesla_stories.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 22:29:08.288320 news-signals-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-21 22:28:54.000000 news-signals-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.108557 news-signals-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 07:51:19.000000 news-signals-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 07:51:19.000000 news-signals-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 07:51:31.108557 news-signals-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-04 07:51:19.000000 news-signals-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 07:51:19.000000 news-signals-0.2.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/news_signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_aql_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_dataset_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_exogenous_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_newsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_representative_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_signals_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/wikidata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-04 07:51:19.000000 news-signals-0.2.6/news_signals/yfinance_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/news_signals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 07:51:31.000000 news-signals-0.2.6/news_signals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.100557 news-signals-0.2.6/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.104557 news-signals-0.2.6/resources/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28512 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/elon_musk_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100.small.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:51:31.108557 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110293 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   113236 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    90390 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131955 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   123388 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109117 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91683 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)    94002 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100871 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.static_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)   135305 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    28298 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/politics_china_australia_timeseries.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235658 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/sample_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218541 2023-07-04 07:51:19.000000 news-signals-0.2.6/resources/test/tesla_stories.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 07:51:31.108557 news-signals-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-04 07:51:19.000000 news-signals-0.2.6/setup.py
```

### Comparing `news-signals-0.2.0/LICENSE` & `news-signals-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/PKG-INFO` & `news-signals-0.2.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: news-signals
-Version: 0.2.0
-Summary: A library for working with text and timeseries data.
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # News Signals
 
 ### Example Colab Notebooks
 
 These notebooks let you try out `news-signals` without installing anything!
 
 - [Find Emerging Categories in a Newsfeed](https://drive.google.com/file/d/1NVBdCfKL3qdSIGITcLsewGETTqn-V9j6/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=oJa-xWusaCQ)       
@@ -65,14 +58,33 @@
 git clone https://github.com/AYLIEN/news-signals-datasets.git
 cd news-signals-datasets
 pip install -r requirements.txt
 pip install -e . # install in editable mode
 make test   # run tests
 ```
 
+## Setting up Aylien NewsAPI credentials
+
+The news-signals library looks for environment variables called 
+`'NEWSAPI_APP_ID'` and `'NEWSAPI_APP_KEY'` - these are used to authenticate to the NewsAPI. 
+
+One way to set these variables up for local development is to 
+Put your Aylien NewsAPI credentials in a file called `~/.aylienconfig`
+`.aylienconfig`
+```
+app-id=<your-app-id>
+app-key=<your-app-key>
+```
+
+Then put the following in your `.bashrc` or similar shell config file:
+```
+export NEWSAPI_APP_ID=$(cat ~/.aylienconfig | grep "app-id" | cut -d'=' -f2)
+export NEWSAPI_APP_KEY=$(cat ~/.aylienconfig| grep "app-key" | cut -d'=' -f2)
+```
+
 ## Generating a new Dataset
 
 Generate a new signals dataset as follows:
 
 ```shell
 make create-dataset DATASET_CONFIG=resources/dataset-config-example.json
 ```
```

### Comparing `news-signals-0.2.0/README.md` & `news-signals-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: news-signals
+Version: 0.2.6
+Summary: A library for working with text and timeseries data.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # News Signals
 
 ### Example Colab Notebooks
 
 These notebooks let you try out `news-signals` without installing anything!
 
 - [Find Emerging Categories in a Newsfeed](https://drive.google.com/file/d/1NVBdCfKL3qdSIGITcLsewGETTqn-V9j6/view?usp=share_link) - [Video](https://www.youtube.com/watch?v=oJa-xWusaCQ)       
@@ -58,14 +65,33 @@
 git clone https://github.com/AYLIEN/news-signals-datasets.git
 cd news-signals-datasets
 pip install -r requirements.txt
 pip install -e . # install in editable mode
 make test   # run tests
 ```
 
+## Setting up Aylien NewsAPI credentials
+
+The news-signals library looks for environment variables called 
+`'NEWSAPI_APP_ID'` and `'NEWSAPI_APP_KEY'` - these are used to authenticate to the NewsAPI. 
+
+One way to set these variables up for local development is to 
+Put your Aylien NewsAPI credentials in a file called `~/.aylienconfig`
+`.aylienconfig`
+```
+app-id=<your-app-id>
+app-key=<your-app-key>
+```
+
+Then put the following in your `.bashrc` or similar shell config file:
+```
+export NEWSAPI_APP_ID=$(cat ~/.aylienconfig | grep "app-id" | cut -d'=' -f2)
+export NEWSAPI_APP_KEY=$(cat ~/.aylienconfig| grep "app-key" | cut -d'=' -f2)
+```
+
 ## Generating a new Dataset
 
 Generate a new signals dataset as follows:
 
 ```shell
 make create-dataset DATASET_CONFIG=resources/dataset-config-example.json
 ```
```

### Comparing `news-signals-0.2.0/news_signals/anomaly_detection.py` & `news-signals-0.2.6/news_signals/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/aql_builder.py` & `news-signals-0.2.6/news_signals/aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/data.py` & `news-signals-0.2.6/news_signals/data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/dataset_transformations.py` & `news-signals-0.2.6/news_signals/dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/exogenous_signals.py` & `news-signals-0.2.6/news_signals/exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/newsapi.py` & `news-signals-0.2.6/news_signals/newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/plotting.py` & `news-signals-0.2.6/news_signals/plotting.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/representative_story.py` & `news-signals-0.2.6/news_signals/representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/signals.py` & `news-signals-0.2.6/news_signals/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -970,15 +970,15 @@
         # make their indexes match, then assert that everything is ok
         for c in realized_components:
             ts_df = c.timeseries_df
             ts_df['normalized_index'] = ts_df.index.floor(freq=freq)
             ts_df.set_index('normalized_index', drop=True, inplace=True)
         assert all(len(c) == len(realized_components[0]) for c in realized_components)
         return pd.concat(
-            [s.timeseries_df for s in realized_components],
+            [s.timeseries_df[s.ts_column] for s in realized_components],
             axis=1
         )
 
     def infer_index_args(self):
         reference_index = self.components[0].timeseries_df.index
         freq = pd.infer_freq(reference_index)
         start = reference_index.min()
```

### Comparing `news-signals-0.2.0/news_signals/signals_dataset.py` & `news-signals-0.2.6/news_signals/signals_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from copy import deepcopy
 
 import appdirs
 import arrow
 import gdown
 import pandas as pd
 import tqdm
+from google.cloud import storage
 
 import news_signals.signals as signals
 import news_signals.newsapi as newsapi
 from news_signals.data import aylien_ts_to_df, arrow_to_aylien_date
 from news_signals.aql_builder import params_to_aql
 from news_signals.log import create_logger
 
@@ -52,44 +53,58 @@
         self.signals = signals
 
     def update(self):
         raise NotImplementedError
         
     @classmethod
     def load(cls, dataset_path, cache_dir=None):       
-
-        # handle downloading from url
-        if type(dataset_path) is str and dataset_path.startswith('https://drive.google.com'):
+        # handle downloading from urls
+        if type(dataset_path) is str \
+            and (dataset_path.startswith('https://drive.google.com') or dataset_path.startswith('gs://')):
             basename = base64.b64encode(dataset_path.encode()).decode()
             if cache_dir is None:
                 cache_dir = cls.DEFAULT_CACHE_DIR
 
             local_dataset_dir = cache_dir / basename
             if not local_dataset_dir.exists():
-                if 'folders' in dataset_path:
-                    local_dataset_dir = Path(cache_dir) / basename
-                    local_dataset_dir.mkdir(parents=True, exist_ok=True)
-                    logger.info(f'Downloading dataset from {dataset_path} to {local_dataset_dir}.')
-                    status = gdown.download_folder(
-                        url=dataset_path,
-                        output=str(local_dataset_dir),
-                        remaining_ok=True
-                    )
-                    dataset_path = local_dataset_dir
-                else:
+                if dataset_path.startswith('https://drive.google.com'):
+                    # folder vs file download from gdrive
+                    if 'folders' in dataset_path:
+                        local_dataset_dir = Path(cache_dir) / basename
+                        local_dataset_dir.mkdir(parents=True, exist_ok=True)
+                        logger.info(f'Downloading dataset from {dataset_path} to {local_dataset_dir}.')
+                        status = gdown.download_folder(
+                            url=dataset_path,
+                            output=str(local_dataset_dir),
+                            remaining_ok=True
+                        )
+                        dataset_path = local_dataset_dir
+                    else:
+                        local_dataset_path = Path(str(local_dataset_dir) + '.tar.gz')
+                        logger.info(f'Downloading dataset from {dataset_path} to {local_dataset_path}.')
+                        status = gdown.download(url=dataset_path, output=str(local_dataset_path))
+                        assert status is not None, 'Download as file failed.'
+                        dataset_path = local_dataset_path
+                elif dataset_path.startswith('gs://'):
+                    assert dataset_path.endswith('.tar.gz'), \
+                        'Datasets stored in GCS currently must be in .tar.gz format'
                     local_dataset_path = Path(str(local_dataset_dir) + '.tar.gz')
-                    logger.info(f'Downloading dataset from {dataset_path} to {local_dataset_path}.')
-                    status = gdown.download(url=dataset_path, output=str(local_dataset_path))
-                    assert status is not None, 'Download as file failed.'
+                    gcs_client = storage.Client()
+                    bucket_name, blob_name = dataset_path.replace("gs://", "").split("/", 1)
+                    bucket = gcs_client.bucket(bucket_name)
+                    blob = bucket.blob(blob_name)
+                    ds_cache_dir = Path(os.path.dirname(local_dataset_path))
+                    ds_cache_dir.mkdir(parents=True, exist_ok=True)
+                    blob.download_to_filename(str(local_dataset_path))
+                    print(f'GCS blob {blob_name} downloaded to {local_dataset_path}.')
                     dataset_path = local_dataset_path
             else:
                 logger.info(f'Using cached dataset at {local_dataset_dir}.') 
                 dataset_path = local_dataset_dir
 
-
         # handle decompressing tar.gz
         dataset_path = Path(dataset_path)
         if str(dataset_path).endswith('.tar.gz') or dataset_path.with_suffix('.tar.gz').exists():
             # add .tar.gz suffix if dataset_path doesn't already have it
             if not str(dataset_path).endswith('.tar.gz'):
                 dataset_path = dataset_path.with_suffix('.tar.gz')
 
@@ -116,42 +131,58 @@
         else:
             metadata = None
         return cls(
             signals=dataset_signals,
             metadata=metadata
         )
 
-    def save(self, dataset_path, compress=True, overwrite=False):
+    def save(self, dataset_path, compress=True, overwrite=False, gcs_bucket_name=None):
+        if gcs_bucket_name is not None:
+            assert compress, 'Datasets uploaded to GCS must be compressed.'
         dataset_path = Path(dataset_path)
         if (overwrite and dataset_path.exists()) and not dataset_path.is_dir():
             dataset_path.unlink()
         dataset_path.mkdir(parents=True, exist_ok=overwrite)
         for signal in self.signals.values():
             signal.save(dataset_path)
         write_json(
             self.metadata,
             dataset_path / 'metadata.json'
         )
         if compress:
             shutil.make_archive(
-                base_name=dataset_path,
-                format='gztar',
+                base_name=str(dataset_path),
                 root_dir=dataset_path.parent,
-                base_dir=dataset_path.name
+                base_dir=dataset_path.name,
+                format='gztar'
             )
             if dataset_path.exists():
                 shutil.rmtree(dataset_path)
             logger.info(f'Saved compressed dataset to {dataset_path}.tar.gz')
+            if gcs_bucket_name is not None:
+                self.upload_to_gcs(
+                    bucket_name=gcs_bucket_name,
+                    source_file_name=f'{dataset_path}.tar.gz',
+                    destination_blob_name=f'{dataset_path.name}.tar.gz'
+                )
             return f'{dataset_path}.tar.gz'
         else:
             logger.info(
                 f'Saved {len(self.signals)} signals in dataset to {dataset_path}.'
             )
             return dataset_path
     
+    @staticmethod
+    def upload_to_gcs(bucket_name, source_file_name, destination_blob_name):
+        gcs_client = storage.Client()
+        bucket = gcs_client.get_bucket(bucket_name)
+        blob = bucket.blob(destination_blob_name)
+        blob.upload_from_filename(source_file_name)
+        logger.info(f"File {source_file_name} uploaded to gs://{bucket_name}/{destination_blob_name}.")
+    
     def aggregate_signal(self, name=None):
         if name is None:
             name = self.metadata['name']
         return signals.AggregateSignal(
             name=name,
             components=list(self.signals.values())
         )
@@ -405,14 +436,15 @@
         [f.name.startswith(signal.id) for f in dataset_output_dir.iterdir()]
     )
 
 
 def generate_dataset(
     input: Union[List[signals.Signal], Path],
     output_dataset_dir: Path,
+    gcs_bucket: str,
     start: datetime,
     end: datetime,
     id_field: str = "",
     name_field: str = "",
     stories_per_day: int = 20,
     overwrite: bool = False,
     delete_tmp_files: bool = False,
@@ -456,14 +488,16 @@
         try:
             post_process_story = globals()[post_process_story]
         except:
             raise NotImplementedError(
                 f"Unknown function for processing stories: {post_process_story}"
             )
 
+    # Note this function creates queries from signals, but it
+    # does not use the __call__ method implemented on Signal objects.
     for signal in tqdm.tqdm(signals_):
         if signal_exists(signal, output_dataset_dir):
             logger.info("signal exists already, skipping to next")
             continue
 
         stories_path = (
             output_dataset_dir / f"buckets_{signal.id}.jsonl"
@@ -506,9 +540,13 @@
         if delete_tmp_files:
             ts_path.unlink()
             stories_path.unlink()
 
     dataset = SignalsDataset.load(output_dataset_dir)
     if compress:
         shutil.rmtree(output_dataset_dir)
-        dataset.save(output_dataset_dir, compress=compress)
+        dataset.save(
+            output_dataset_dir,
+            compress=compress,
+            gcs_bucket_name=gcs_bucket
+        )
     return dataset
```

### Comparing `news-signals-0.2.0/news_signals/summarization.py` & `news-signals-0.2.6/news_signals/summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_anomaly_detection.py` & `news-signals-0.2.6/news_signals/test_anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_aql_builder.py` & `news-signals-0.2.6/news_signals/test_aql_builder.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_data.py` & `news-signals-0.2.6/news_signals/test_data.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_dataset_transformations.py` & `news-signals-0.2.6/news_signals/test_dataset_transformations.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_exogenous_signals.py` & `news-signals-0.2.6/news_signals/test_exogenous_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_newsapi.py` & `news-signals-0.2.6/news_signals/test_newsapi.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_representative_story.py` & `news-signals-0.2.6/news_signals/test_representative_story.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_signals.py` & `news-signals-0.2.6/news_signals/test_signals.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/test_signals_dataset.py` & `news-signals-0.2.6/news_signals/test_signals_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import base64
 from pathlib import Path
 
 import arrow
 import pandas as pd
 
-from news_signals.data import aylien_ts_to_df, datetime_to_aylien_str
+from news_signals.data import datetime_to_aylien_str
 from news_signals.log import create_logger
 from news_signals import signals, test_signals
 from news_signals import signals_dataset
 from news_signals.signals_dataset import SignalsDataset
 
 
 logger = create_logger(__name__)
@@ -130,14 +130,47 @@
                 len(tick) == len(self.stories_endpoint.sample_stories)
                 for tick in signal.feeds_df['stories']
             )
 
             assert signal.params is not None
             assert signal.name is not None
             assert signal.id is not None              
+ 
+    def test_signals_dataset_from_initialized_signals(self):
+        # test that we can create a dataset from signals initialized
+        # elsewhere
+        start = datetime.datetime(2023, 3, 1)
+        end = datetime.datetime(2023, 5, 20)
+        name = 'biz-crime-usa-constrained'
+        params = {
+            'categories': ['ay.biz.crime'],
+            'source.locations.country[]': 'US',
+            'language': 'en'
+        }
+        signal = signals.AylienSignal(
+            name=name,
+            params=params
+        )
+  
+        signals_dataset.generate_dataset(
+            input=[signal],
+            output_dataset_dir=Path(self.output_dataset_dir),
+            start=start,
+            end=end,
+            stories_per_day=50,
+            delete_tmp_files=True,
+            stories_endpoint=self.stories_endpoint,
+            ts_endpoint=self.ts_endpoint,
+            compress=False
+        )
+        dataset = signals_dataset.SignalsDataset.load(self.output_dataset_dir)
+        assert list(dataset.signals.values())[0].name == name
+        difference = end - start
+        days = difference.days + 1  # to include the start date
+        assert len(list(dataset.signals.values())[0]) == days
 
     def test_signal_exists(self):
         self.generate_sample_dataset()
         signals_ = signals.Signal.load(self.output_dataset_dir)
         for s in signals_:            
             assert signals_dataset.signal_exists(s, self.output_dataset_dir)
 
@@ -188,28 +221,89 @@
         tmp_dir = Path('/tmp/test_signals_dataset')
         d1.save(tmp_dir, compress=False)
         d2 = SignalsDataset.load(tmp_dir)
         for k in d1:
             assert d1[k].name == d2[k].name
         assert json.dumps(d1.metadata) == json.dumps(d2.metadata)
         shutil.rmtree(tmp_dir)
+
+    def test_save_to_gcs(self):
+        d1 = SignalsDataset(self.aylien_signals())
+        tmp_dir = Path('/tmp/test_signals_dataset')
+        fake_gcs_bucket = 'fake-path'
+        
+        class upload_from_filename:
+            @classmethod
+            def set_args(cls, args):
+                cls.args = args
+            def __call__(self, *args):
+                self.set_args(args)
+
+        class MockGCStorage:
+            def Client(self):
+                class get_bucket:
+                    def __init__(self, bucket_name):
+                        self.bucket_name = bucket_name
+                    def blob(self, path):
+                        self.path = path
+                        self.upload_from_filename = upload_from_filename()
+                        return self
+                self.get_bucket = get_bucket 
+                return self
+        
+        mock_storage = MockGCStorage()
+        signals_dataset.storage = mock_storage
+        save_path = d1.save(tmp_dir, compress=True, gcs_bucket_name=fake_gcs_bucket)
+        assert upload_from_filename.args[0] == save_path
     
     def test_load_from_url(self):
         cache_dir = Path('/tmp/test_signals_dataset')
         cache_dir.mkdir(parents=True)
         fake_gdrive_path = 'https://drive.google.com/fake-path'
         basename = base64.b64encode(fake_gdrive_path.encode()).decode()
 
         d1 = SignalsDataset(self.aylien_signals())
         _ = d1.save(cache_dir / basename, compress=False)
         # assert that the loader thinks the dataset already exists
         d2 = SignalsDataset.load(fake_gdrive_path, cache_dir=cache_dir)
         assert len(d1) == len(d2)
         shutil.rmtree(cache_dir)
+
+        # test loading from GCS urls
+        cache_dir.mkdir(parents=True)
+        fake_gcs_path = 'gs://fake-path'
+        # this should break because GCS bucket download requires tar.gz
+        with self.assertRaises(AssertionError):
+            _ = SignalsDataset.load(fake_gcs_path, cache_dir=cache_dir)
+        shutil.rmtree(cache_dir)
+
+        class download_to_filename:
+            args = None
+            def __call__(self, *args):
+                self.args = args
+
+        class MockGCStorage:
+            def Client(self):
+                class bucket:
+                    def __init__(self, bucket_name):
+                        self.bucket_name = bucket_name
+                    def blob(self, path):
+                        self.path = path
+                        self.download_to_filename = download_to_filename()
+                        return self
+                self.bucket = bucket 
+                return self
         
+        signals_dataset.storage = MockGCStorage()
+        fake_gcs_path = 'gs://fake-path/dataset.tar.gz'
+        basename = base64.b64encode(fake_gcs_path.encode()).decode()
+        with self.assertRaises(FileNotFoundError):
+            _ = SignalsDataset.load(fake_gcs_path, cache_dir=cache_dir)
+            assert download_to_filename.args[0] == cache_dir / basename + '.tar.gz'
+
     def test_plot_dataset(self):
         dataset = SignalsDataset(self.aylien_signals())
         savedir = Path('/tmp/test_plot_dataset')
         dataset.plot(savedir=savedir)
         assert os.path.exists(savedir / f'{dataset.metadata["name"]}.png')
         shutil.rmtree(savedir)
```

### Comparing `news-signals-0.2.0/news_signals/test_summarization.py` & `news-signals-0.2.6/news_signals/test_summarization.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/users.py` & `news-signals-0.2.6/news_signals/users.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/wikidata_utils.py` & `news-signals-0.2.6/news_signals/wikidata_utils.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals/yfinance_timeseries.py` & `news-signals-0.2.6/news_signals/yfinance_timeseries.py`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/news_signals.egg-info/PKG-INFO` & `news-signals-0.2.6/news_signals.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-signals
-Version: 0.2.0
+Version: 0.2.6
 Summary: A library for working with text and timeseries data.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # News Signals
 
 ### Example Colab Notebooks
@@ -65,14 +65,33 @@
 git clone https://github.com/AYLIEN/news-signals-datasets.git
 cd news-signals-datasets
 pip install -r requirements.txt
 pip install -e . # install in editable mode
 make test   # run tests
 ```
 
+## Setting up Aylien NewsAPI credentials
+
+The news-signals library looks for environment variables called 
+`'NEWSAPI_APP_ID'` and `'NEWSAPI_APP_KEY'` - these are used to authenticate to the NewsAPI. 
+
+One way to set these variables up for local development is to 
+Put your Aylien NewsAPI credentials in a file called `~/.aylienconfig`
+`.aylienconfig`
+```
+app-id=<your-app-id>
+app-key=<your-app-key>
+```
+
+Then put the following in your `.bashrc` or similar shell config file:
+```
+export NEWSAPI_APP_ID=$(cat ~/.aylienconfig | grep "app-id" | cut -d'=' -f2)
+export NEWSAPI_APP_KEY=$(cat ~/.aylienconfig| grep "app-key" | cut -d'=' -f2)
+```
+
 ## Generating a new Dataset
 
 Generate a new signals dataset as follows:
 
 ```shell
 make create-dataset DATASET_CONFIG=resources/dataset-config-example.json
 ```
```

### Comparing `news-signals-0.2.0/news_signals.egg-info/SOURCES.txt` & `news-signals-0.2.6/news_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/elon_musk_timeseries.json` & `news-signals-0.2.6/resources/test/elon_musk_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDI0NDU0IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDU1MzkwIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMDkyNTcxIiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTQ2MyIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMTU1NjY4IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExMzgzNjY5IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNDc3MiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTEwOTg2NSIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNTQ1MDc2IiwgIm1ldGFkYXRhIjoge319.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet` & `news-signals-0.2.6/resources/test/nasdaq100_sample_dataset/eyJuYW1lIjogIlExNzA4MTYxMiIsICJtZXRhZGF0YSI6IHt9fQ==.stories_df.parquet`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/politics_china_australia_timeseries.json` & `news-signals-0.2.6/resources/test/politics_china_australia_timeseries.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/sample_stories.json` & `news-signals-0.2.6/resources/test/sample_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/resources/test/tesla_stories.json` & `news-signals-0.2.6/resources/test/tesla_stories.json`

 * *Files identical despite different names*

### Comparing `news-signals-0.2.0/setup.py` & `news-signals-0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # If you add a new dependency, make sure to make the version range as wide as possible.
 # TODO: we need to decide on the best way to install particular spacy models
 # and other data files that are not python modules.
 INSTALL_REQUIRES = [
     "appdirs>=1.4.4",
     "arrow>=1.1.1",
     "gdown>=4.6.4",
+    "google-cloud-storage>=2.10.0",
     "matplotlib>=3.5.3",
     "networkx<=2.7",
     "pandas>=1.4.1",
     "pyarrow>=11.0.0",
     "ratelimit>=2.2.1",
     "requests>=2.28.1",
     "scikit-learn>=1.1.0",
```

