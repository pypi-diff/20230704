# Comparing `tmp/audioscrape-0.0.4.tar.gz` & `tmp/audioscrape-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/audioscrape-0.0.4.tar", last modified: Mon Dec  5 08:12:19 2016, max compression
+gzip compressed data, was "audioscrape-0.2.0.tar", last modified: Tue Jul  4 00:07:35 2023, max compression
```

## Comparing `audioscrape-0.0.4.tar` & `audioscrape-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2016-12-05 08:12:19.000000 audioscrape-0.0.4/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape/
--rw-r--r--   0 travis    (1000) travis    (1000)       83 2016-12-05 08:10:35.000000 audioscrape-0.0.4/audioscrape/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1775 2016-12-05 08:10:35.000000 audioscrape-0.0.4/audioscrape/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3200 2016-12-05 08:10:35.000000 audioscrape-0.0.4/audioscrape/soundcloud.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1615 2016-12-05 08:10:35.000000 audioscrape-0.0.4/audioscrape/youtube.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)      707 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      358 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       59 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       45 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       12 2016-12-05 08:12:19.000000 audioscrape-0.0.4/audioscrape.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     1078 2016-12-05 08:10:35.000000 audioscrape-0.0.4/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)       33 2016-12-05 08:10:35.000000 audioscrape-0.0.4/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     1745 2016-12-05 08:12:12.000000 audioscrape-0.0.4/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)       84 2016-12-05 08:12:19.000000 audioscrape-0.0.4/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1124 2016-12-05 08:10:35.000000 audioscrape-0.0.4/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      707 2016-12-05 08:12:19.000000 audioscrape-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.679726 audioscrape-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 00:07:21.000000 audioscrape-0.2.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.667725 audioscrape-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.667725 audioscrape-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-04 00:07:21.000000 audioscrape-0.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 00:07:21.000000 audioscrape-0.2.0/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 00:07:21.000000 audioscrape-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 00:07:21.000000 audioscrape-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 00:07:21.000000 audioscrape-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-04 00:07:35.679726 audioscrape-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 00:07:21.000000 audioscrape-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.675726 audioscrape-0.2.0/audioscrape/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/freesound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4126810 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/yamnet.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-04 00:07:21.000000 audioscrape-0.2.0/audioscrape/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.675726 audioscrape-0.2.0/audioscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 00:07:35.000000 audioscrape-0.2.0/audioscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 00:07:21.000000 audioscrape-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:07:35.679726 audioscrape-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:07:35.679726 audioscrape-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   320991 2023-07-04 00:07:21.000000 audioscrape-0.2.0/tests/example.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-04 00:07:21.000000 audioscrape-0.2.0/tests/test_audioscrape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-04 00:07:21.000000 audioscrape-0.2.0/tests/test_classify.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `audioscrape-0.0.4/audioscrape/__main__.py` & `audioscrape-0.2.0/audioscrape/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,44 @@
-# coding=utf-8
 """Download audio."""
 import argparse
+import logging
 import sys
 
 from . import soundcloud, youtube
 
+logger = logging.getLogger(__name__)
 
-def download(query, include=None, exclude=None, quiet=False, overwrite=False):
+
+def download(query, include, exclude, quiet, verbose, overwrite, limit):
     """Scrape various websites for audio."""
-    youtube.scrape(query, include, exclude, quiet, overwrite)
-    soundcloud.scrape(query, include, exclude, quiet, overwrite)
+    youtube.scrape(query, include, exclude, quiet, verbose, overwrite, limit)
+    soundcloud.scrape(query, include, exclude, quiet, verbose, overwrite, limit)
 
 
-def main(args=None):
+def cli(args=None):
     """CLI for scraping audio."""
-    if args is None:
-        args = sys.argv[1:]
 
-    # Parse program arguments.
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        'query', default="Cerulean Crayons", nargs='?', help="search terms")
-    parser.add_argument(
-        '-i',
-        '--include',
-        default=[],
-        action='append',
-        help="only download audio with this tag (this flag can be used multiple times)"
-    )
-    parser.add_argument(
-        '-e',
-        '--exclude',
-        default=[],
-        action='append',
-        help="ignore results with this tag (this flag can be used multiple times)"
-    )
-    parser.add_argument(
-        '-q',
-        '--quiet',
-        default=False,
-        action='store_true',
-        help="hide progress reporting")
-    parser.add_argument(
-        '-o',
-        '--overwrite',
-        default=False,
-        action='store_true',
-        help="overwrite existing files")
+    parser.add_argument("query", default="Cerulean Crayons", nargs="?", help="search terms")
+    parser.add_argument("-i", "--include", default=[], action="append", help="only download audio with this tag")
+    parser.add_argument("-e", "--exclude", default=[], action="append", help="ignore results with this tag")
+    parser.add_argument("-q", "--quiet", default=False, action="store_true", help="hide progress reporting")
+    parser.add_argument("-v", "--verbose", default=False, action="store_true", help="display debug information")
+    parser.add_argument("-o", "--overwrite", default=False, action="store_true", help="overwrite existing files")
+    parser.add_argument("-l", "--limit", default=10, type=int, help="limit number of downloads")
     args = parser.parse_args()
 
-    # Search YouTube and download audio from videos.
-    if not args.quiet:
-        print('Downloading audio from "{}" videos tagged {} and not {}.'.
-              format(args.query, args.include, args.exclude))
-    download(args.query, args.include, args.exclude, args.quiet,
-             args.overwrite)
-    if not args.quiet:
-        print("Finished downloading audio.")
+    logging.basicConfig(format="[%(name)s] %(message)s")
+    if args.verbose:
+        logger.setLevel(logging.DEBUG)
+    elif args.quiet:
+        logger.setLevel(logging.ERROR)
+    else:
+        logger.setLevel(logging.INFO)
+
+    logger.info(f'Downloading audio from "{args.query}" videos tagged {args.include} and not {args.exclude}.')
+    download(args.query, args.include, args.exclude, args.quiet, args.verbose, args.overwrite, args.limit)
+    logger.info("Finished downloading audio.")
 
 
 if __name__ == "__main__":
-    main()
+    cli(sys.argv[1:])
```

### Comparing `audioscrape-0.0.4/LICENSE` & `audioscrape-0.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2016 Carl Thomé
+Copyright (c) 2023 Carl Thomé
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

