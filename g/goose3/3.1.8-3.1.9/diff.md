# Comparing `tmp/goose3-3.1.8.tar.gz` & `tmp/goose3-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goose3-3.1.8.tar", last modified: Mon Feb 22 14:09:59 2021, max compression
+gzip compressed data, was "goose3-3.1.9.tar", last modified: Tue Apr 27 11:09:46 2021, max compression
```

## Comparing `goose3-3.1.8.tar` & `goose3-3.1.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.117663 goose3-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)       37 2021-02-22 14:09:43.000000 goose3-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    12996 2021-02-22 14:09:59.117663 goose3-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9846 2021-02-22 14:09:43.000000 goose3-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.113664 goose3-3.1.8/goose3/
--rw-r--r--   0 runner    (1001) docker     (116)     5764 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8582 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/article.py
--rw-r--r--   0 runner    (1001) docker     (116)    10739 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (116)    23040 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    11592 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/crawler.py
--rw-r--r--   0 runner    (1001) docker     (116)       62 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.117663 goose3-3.1.8/goose3/extractors/
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2390 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/authors.py
--rw-r--r--   0 runner    (1001) docker     (116)    14339 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/content.py
--rw-r--r--   0 runner    (1001) docker     (116)    15313 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/images.py
--rw-r--r--   0 runner    (1001) docker     (116)     1220 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/links.py
--rw-r--r--   0 runner    (1001) docker     (116)     4822 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/metas.py
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/opengraph.py
--rw-r--r--   0 runner    (1001) docker     (116)     8762 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/publishdate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2089 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     1634 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/tags.py
--rw-r--r--   0 runner    (1001) docker     (116)     4098 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/title.py
--rw-r--r--   0 runner    (1001) docker     (116)     1462 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/tweets.py
--rw-r--r--   0 runner    (1001) docker     (116)     4654 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/extractors/videos.py
--rw-r--r--   0 runner    (1001) docker     (116)     3808 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     2209 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/network.py
--rw-r--r--   0 runner    (1001) docker     (116)     5494 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/outputformatters.py
--rw-r--r--   0 runner    (1001) docker     (116)     7273 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.113664 goose3-3.1.8/goose3/resources/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.117663 goose3-3.1.8/goose3/resources/images/
--rw-r--r--   0 runner    (1001) docker     (116)      232 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/images/known-image-css.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.117663 goose3-3.1.8/goose3/resources/text/
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-ar.txt
--rw-r--r--   0 runner    (1001) docker     (116)      484 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-da.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5967 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-de.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3585 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-en.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2185 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-es.txt
--rw-r--r--   0 runner    (1001) docker     (116)      464 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-fi.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-fr.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2337 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-hu.txt
--rw-r--r--   0 runner    (1001) docker     (116)    10499 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-id.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3005 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-it.txt
--rw-r--r--   0 runner    (1001) docker     (116)      459 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-ko.txt
--rw-r--r--   0 runner    (1001) docker     (116)      587 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-nb.txt
--rw-r--r--   0 runner    (1001) docker     (116)      177 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-nl.txt
--rw-r--r--   0 runner    (1001) docker     (116)      513 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-no.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1591 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-pl.txt
--rw-r--r--   0 runner    (1001) docker     (116)      865 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-pt.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4540 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-ru.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3956 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-sv.txt
--rw-r--r--   0 runner    (1001) docker     (116)      604 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/resources/text/stopwords-zh.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6804 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/text.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.117663 goose3-3.1.8/goose3/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     3397 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5209 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     5016 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (116)      970 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     2260 2021-02-22 14:09:43.000000 goose3-3.1.8/goose3/video.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 14:09:59.113664 goose3-3.1.8/goose3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    12996 2021-02-22 14:09:58.000000 goose3-3.1.8/goose3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1695 2021-02-22 14:09:59.000000 goose3-3.1.8/goose3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-22 14:09:58.000000 goose3-3.1.8/goose3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-22 14:09:58.000000 goose3-3.1.8/goose3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       73 2021-02-22 14:09:58.000000 goose3-3.1.8/goose3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-02-22 14:09:58.000000 goose3-3.1.8/goose3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-02-22 14:09:59.117663 goose3-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2936 2021-02-22 14:09:43.000000 goose3-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.752830 goose3-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-04-27 11:09:28.000000 goose3-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12996 2021-04-27 11:09:46.752830 goose3-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9846 2021-04-27 11:09:28.000000 goose3-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.748830 goose3-3.1.9/goose3/
+-rw-r--r--   0 runner    (1001) docker     (121)     5764 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8582 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/article.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10739 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23040 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11592 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.748830 goose3-3.1.9/goose3/extractors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/authors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14339 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15313 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4822 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/metas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/opengraph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8762 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/publishdate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4205 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/title.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/tweets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4654 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/extractors/videos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5494 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/outputformatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7273 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.744830 goose3-3.1.9/goose3/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.748830 goose3-3.1.9/goose3/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/images/known-image-css.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.752830 goose3-3.1.9/goose3/resources/text/
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-ar.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-da.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5967 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-de.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-en.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2185 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-es.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-fi.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-fr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-hu.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10499 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-id.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3005 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-it.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-ko.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-nb.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-nl.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-no.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-pt.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4540 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-ru.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3956 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-sv.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/resources/text/stopwords-zh.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6816 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.752830 goose3-3.1.9/goose3/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3397 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5209 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5016 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-04-27 11:09:28.000000 goose3-3.1.9/goose3/video.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-27 11:09:46.748830 goose3-3.1.9/goose3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12996 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-27 11:09:46.000000 goose3-3.1.9/goose3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-04-27 11:09:46.752830 goose3-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2936 2021-04-27 11:09:28.000000 goose3-3.1.9/setup.py
```

### Comparing `goose3-3.1.8/PKG-INFO` & `goose3-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: goose3
-Version: 3.1.8
+Version: 3.1.9
 Summary: Html Content / Article Extractor, web scrapping for Python3
 Home-page: https://github.com/goose3/goose3
 Maintainer: Mahmoud Lababidi
 Maintainer-email: lababidi+py@gmail.com
 License: Apache
 Description: Goose3 - Article Extractor
         ===============================================
```

### Comparing `goose3-3.1.8/README.rst` & `goose3-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/__init__.py` & `goose3-3.1.9/goose3/__init__.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/article.py` & `goose3-3.1.9/goose3/article.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/cleaners.py` & `goose3-3.1.9/goose3/cleaners.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/configuration.py` & `goose3-3.1.9/goose3/configuration.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/crawler.py` & `goose3-3.1.9/goose3/crawler.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/__init__.py` & `goose3-3.1.9/goose3/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/authors.py` & `goose3-3.1.9/goose3/extractors/authors.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/content.py` & `goose3-3.1.9/goose3/extractors/content.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/images.py` & `goose3-3.1.9/goose3/extractors/images.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/links.py` & `goose3-3.1.9/goose3/extractors/links.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/metas.py` & `goose3-3.1.9/goose3/extractors/metas.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/opengraph.py` & `goose3-3.1.9/goose3/extractors/opengraph.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/publishdate.py` & `goose3-3.1.9/goose3/extractors/publishdate.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/schema.py` & `goose3-3.1.9/goose3/extractors/schema.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/tags.py` & `goose3-3.1.9/goose3/extractors/tags.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/title.py` & `goose3-3.1.9/goose3/extractors/title.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,30 +31,34 @@
 class TitleExtractor(BaseExtractor):
 
     def clean_title(self, title):
         """Clean title with the use of og:site_name
         in this case try to get rid of site name
         and use TITLE_SPLITTERS to reformat title
         """
-        # check if we have the site name in opengraph data
-        if "site_name" in list(self.article.opengraph.keys()) and self.article.opengraph['site_name'] != title:
-            site_name = self.article.opengraph['site_name']
-            # remove the site name from title
-            title = title.replace(site_name, '').strip()
-        elif (self.article.schema and "publisher" in self.article.schema and
-              "name" in self.article.schema["publisher"]):
-            site_name = self.article.schema["publisher"]["name"]
-            # remove the site name from title
-            title = title.replace(site_name, '').strip()
 
         # try to remove the domain from url
         if self.article.domain:
             pattern = re.compile(self.article.domain, re.IGNORECASE)
             title = pattern.sub("", title).strip()
 
+        site_name = ""
+        # check if we have the site name in opengraph data
+        if "site_name" in list(self.article.opengraph.keys()) and self.article.opengraph['site_name'] != title:
+            site_name = self.article.opengraph['site_name']
+        elif (self.article.schema and "publisher" in self.article.schema and "name" in self.article.schema["publisher"]):
+            site_name = self.article.schema["publisher"]["name"]
+
+
+        # if there is a sperator, speratate and check if site name is present
+        seps = [s for s in TITLE_SPLITTERS if s in title]
+        if seps:
+            # NOTE: Perhaps it should only be removed if, once seperated it is "by itself"
+            title = title.replace(site_name, '').strip()
+
         # split the title in words
         # TechCrunch | my wonderfull article
         # my wonderfull article | TechCrunch
         title_words = title.split()
 
         # check if first letter is in TITLE_SPLITTERS
         # if so remove it
```

### Comparing `goose3-3.1.8/goose3/extractors/tweets.py` & `goose3-3.1.9/goose3/extractors/tweets.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/extractors/videos.py` & `goose3-3.1.9/goose3/extractors/videos.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/image.py` & `goose3-3.1.9/goose3/image.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/network.py` & `goose3-3.1.9/goose3/network.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/outputformatters.py` & `goose3-3.1.9/goose3/outputformatters.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/parsers.py` & `goose3-3.1.9/goose3/parsers.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-ar.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-ar.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-de.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-de.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-en.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-en.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-es.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-es.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-fr.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-fr.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-hu.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-hu.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-id.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-id.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-it.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-it.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-nb.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-nb.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-no.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-no.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-pl.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-pl.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-pt.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-pt.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-ru.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-ru.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-sv.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-sv.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/resources/text/stopwords-zh.txt` & `goose3-3.1.9/goose3/resources/text/stopwords-zh.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/text.py` & `goose3-3.1.9/goose3/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,29 @@
     Code from:
     https://github.com/sigmavirus24/requests-toolbelt/blob/master/requests_toolbelt/utils/deprecated.py
     Return encodings from given content string.
     :param content: string to extract encodings from.
     """
     if isinstance(content, bytes):
         find_charset = re.compile(
-            br'<meta.*?charset=["\']*([a-z0-9\-_]+?) *?["\'>]', flags=re.I
+            br'<meta.*?charset=["\']*([a-zA-Z0-9\-_]+?) *?["\'>]', flags=re.I
         ).findall
 
         find_xml = re.compile(
-            br'^<\?xml.*?encoding=["\']*([a-z0-9\-_]+?) *?["\'>]'
+            br'^<\?xml.*?encoding=["\']*([a-zA-Z0-9\-_]+?) *?["\'>]'
         ).findall
         return [encoding.decode('utf-8') for encoding in
                 find_charset(content) + find_xml(content)]
     else:
         find_charset = re.compile(
-            r'<meta.*?charset=["\']*([a-z0-9\-_]+?) *?["\'>]', flags=re.I
+            r'<meta.*?charset=["\']*([a-zA-Z0-9\-_]+?) *?["\'>]', flags=re.I
         ).findall
 
         find_xml = re.compile(
-            r'^<\?xml.*?encoding=["\']*([a-z0-9\-_]+?) *?["\'>]'
+            r'^<\?xml.*?encoding=["\']*([a-zA-Z0-9\-_]+?) *?["\'>]'
         ).findall
         return find_charset(content) + find_xml(content)
 
 
 def innerTrim(value):
     if isinstance(value, str):
         # remove tab and white space
```

### Comparing `goose3-3.1.8/goose3/utils/__init__.py` & `goose3-3.1.9/goose3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/utils/encoding.py` & `goose3-3.1.9/goose3/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/utils/images.py` & `goose3-3.1.9/goose3/utils/images.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3/version.py` & `goose3-3.1.9/goose3/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-version_info = (3, 1, 8)  # pylint: disable=C0103
+version_info = (3, 1, 9)  # pylint: disable=C0103
 __version__ = ".".join([str(x) for x in version_info])
```

### Comparing `goose3-3.1.8/goose3/video.py` & `goose3-3.1.9/goose3/video.py`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/goose3.egg-info/PKG-INFO` & `goose3-3.1.9/goose3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: goose3
-Version: 3.1.8
+Version: 3.1.9
 Summary: Html Content / Article Extractor, web scrapping for Python3
 Home-page: https://github.com/goose3/goose3
 Maintainer: Mahmoud Lababidi
 Maintainer-email: lababidi+py@gmail.com
 License: Apache
 Description: Goose3 - Article Extractor
         ===============================================
```

### Comparing `goose3-3.1.8/goose3.egg-info/SOURCES.txt` & `goose3-3.1.9/goose3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goose3-3.1.8/setup.py` & `goose3-3.1.9/setup.py`

 * *Files identical despite different names*

