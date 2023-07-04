# Comparing `tmp/mly_pipeline-0.5.1.tar.gz` & `tmp/mly_pipeline-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.5.1.tar", last modified: Tue Jun 13 11:00:08 2023, max compression
+gzip compressed data, was "mly_pipeline-0.5.2.tar", last modified: Tue Jul  4 14:07:20 2023, max compression
```

## Comparing `mly_pipeline-0.5.1.tar` & `mly_pipeline-0.5.2.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.428854 mly_pipeline-0.5.1/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      101 2023-05-16 13:28:31.000000 mly_pipeline-0.5.1/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.1/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.1/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-06-13 11:00:08.428854 mly_pipeline-0.5.1/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.1/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.350854 mly_pipeline-0.5.1/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.1/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.341853 mly_pipeline-0.5.1/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.363854 mly_pipeline-0.5.1/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.1/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.1/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.1/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.1/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.1/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.380854 mly_pipeline-0.5.1/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.382854 mly_pipeline-0.5.1/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.1/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.386854 mly_pipeline-0.5.1/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.405854 mly_pipeline-0.5.1/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.1/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.1/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.1/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.1/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.1/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.1/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.1/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.411854 mly_pipeline-0.5.1/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.1/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.1/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.1/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.1/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.1/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.419854 mly_pipeline-0.5.1/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.1/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28609 2023-06-13 09:15:28.000000 mly_pipeline-0.5.1/mly_pipeline/continuous_FAR.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26878 2023-06-07 12:32:57.000000 mly_pipeline-0.5.1/mly_pipeline/initialization.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.1/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    23213 2023-06-12 14:37:57.000000 mly_pipeline-0.5.1/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5825 2023-06-06 08:44:31.000000 mly_pipeline-0.5.1/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20433 2023-06-08 11:04:49.000000 mly_pipeline-0.5.1/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    18492 2023-06-13 09:02:17.000000 mly_pipeline-0.5.1/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    48952 2023-06-12 15:53:57.000000 mly_pipeline-0.5.1/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.427854 mly_pipeline-0.5.1/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.1/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-05-16 13:28:31.000000 mly_pipeline-0.5.1/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-06-13 11:00:08.425854 mly_pipeline-0.5.1/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2594 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-06-13 11:00:08.000000 mly_pipeline-0.5.1/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-06-13 10:59:24.000000 mly_pipeline-0.5.1/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-06-13 11:00:08.428854 mly_pipeline-0.5.1/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.584667 mly_pipeline-0.5.2/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      123 2023-06-27 09:51:40.000000 mly_pipeline-0.5.2/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.5.2/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.5.2/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-04 14:07:20.584667 mly_pipeline-0.5.2/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.5.2/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.059661 mly_pipeline-0.5.2/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.051661 mly_pipeline-0.5.2/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.285664 mly_pipeline-0.5.2/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.5.2/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2074627 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6321 2023-05-18 11:06:49.000000 mly_pipeline-0.5.2/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9106 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    61091 2023-06-13 10:37:26.000000 mly_pipeline-0.5.2/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    74931 2023-05-18 14:02:37.000000 mly_pipeline-0.5.2/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.382665 mly_pipeline-0.5.2/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.406665 mly_pipeline-0.5.2/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.5.2/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.419665 mly_pipeline-0.5.2/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.510666 mly_pipeline-0.5.2/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15228 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9827 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1141 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      421 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.5.2/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3127 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8175 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8623 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1577 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.5.2/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27464 2023-06-13 10:37:27.000000 mly_pipeline-0.5.2/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3430 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21370 2023-06-13 10:58:46.000000 mly_pipeline-0.5.2/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27034 2023-05-18 14:02:37.000000 mly_pipeline-0.5.2/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.532666 mly_pipeline-0.5.2/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5973 2023-05-18 14:08:16.000000 mly_pipeline-0.5.2/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.5.2/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2134 2023-06-13 10:58:33.000000 mly_pipeline-0.5.2/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14941 2023-05-30 13:25:04.000000 mly_pipeline-0.5.2/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13940 2023-05-18 14:02:00.000000 mly_pipeline-0.5.2/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.566666 mly_pipeline-0.5.2/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.5.2/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    28059 2023-06-28 14:28:41.000000 mly_pipeline-0.5.2/mly_pipeline/continuous_FAR.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    17355 2023-06-27 11:02:28.000000 mly_pipeline-0.5.2/mly_pipeline/continuous_FAR_test.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    31499 2023-06-29 14:15:00.000000 mly_pipeline-0.5.2/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.5.2/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    33496 2023-06-30 13:55:36.000000 mly_pipeline-0.5.2/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5825 2023-06-06 08:44:31.000000 mly_pipeline-0.5.2/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    21032 2023-06-15 11:06:35.000000 mly_pipeline-0.5.2/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16742 2023-06-30 11:44:45.000000 mly_pipeline-0.5.2/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    49651 2023-06-30 11:52:05.000000 mly_pipeline-0.5.2/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.582666 mly_pipeline-0.5.2/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.5.2/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-07-04 13:10:16.000000 mly_pipeline-0.5.2/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:07:20.579666 mly_pipeline-0.5.2/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6681 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2630 2023-07-04 14:07:20.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-07-04 14:07:19.000000 mly_pipeline-0.5.2/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      762 2023-07-04 12:43:13.000000 mly_pipeline-0.5.2/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-07-04 14:07:20.585667 mly_pipeline-0.5.2/setup.cfg
```

### Comparing `mly_pipeline-0.5.1/.gitlab-ci.yml` & `mly_pipeline-0.5.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/LICENSE` & `mly_pipeline-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/PKG-INFO` & `mly_pipeline-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.5.1
+Version: 0.5.2
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.1/README.md` & `mly_pipeline-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/Makefile` & `mly_pipeline-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.5.2/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/index.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.5.2/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/Getting Started.html` & `mly_pipeline-0.5.2/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/GettingStarted.html` & `mly_pipeline-0.5.2/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/How to use.html` & `mly_pipeline-0.5.2/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/HowToUse.html` & `mly_pipeline-0.5.2/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/Installation.html` & `mly_pipeline-0.5.2/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_modules/index.html` & `mly_pipeline-0.5.2/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_modules/io.html` & `mly_pipeline-0.5.2/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.5.2/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.5.2/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.5.2/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.5.2/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.5.2/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.5.2/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/basic.css` & `mly_pipeline-0.5.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.5.2/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.5.2/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/doctools.js` & `mly_pipeline-0.5.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.5.2/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/jquery.js` & `mly_pipeline-0.5.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/language_data.js` & `mly_pipeline-0.5.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/pygments.css` & `mly_pipeline-0.5.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.5.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.5.2/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/underscore.js` & `mly_pipeline-0.5.2/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/_static/websupport.js` & `mly_pipeline-0.5.2/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/genindex.html` & `mly_pipeline-0.5.2/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/gettingstarted.html` & `mly_pipeline-0.5.2/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/howtouse.html` & `mly_pipeline-0.5.2/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/index.html` & `mly_pipeline-0.5.2/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/installation.html` & `mly_pipeline-0.5.2/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/objects.inv` & `mly_pipeline-0.5.2/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/py-modindex.html` & `mly_pipeline-0.5.2/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/runningasearch.html` & `mly_pipeline-0.5.2/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/search.html` & `mly_pipeline-0.5.2/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/searchindex.js` & `mly_pipeline-0.5.2/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/build/html/settingupasearch.html` & `mly_pipeline-0.5.2/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/source/conf.py` & `mly_pipeline-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/source/index.rst` & `mly_pipeline-0.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/source/installation.rst` & `mly_pipeline-0.5.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/source/runningasearch.rst` & `mly_pipeline-0.5.2/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/docs/source/settingupasearch.rst` & `mly_pipeline-0.5.2/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline/__init__.py` & `mly_pipeline-0.5.2/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline/continuous_FAR.py` & `mly_pipeline-0.5.2/mly_pipeline/continuous_FAR.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,44 @@
 #!/usr/bin/env python
 
-import os, json
+import os, sys, json, time, argparse, subprocess
+
+# Scipy and numpy env parameters that limit the threads
+os.environ["MKL_NUM_THREADS"] = "1"
+os.environ["NUMEXPR_NUM_THREADS"] = "1"
+os.environ["OMP_NUM_THREADS"] = "1"
+
+
+import logging
+from logging import handlers
+
 import shutil
-import time
 import pickle
-import logging
-from datetime import datetime
 
+from datetime import datetime
 from pathlib import Path
 from pycondor import Job, Dagman
+from multiprocessing import Process , Queue , Pool
 
 import numpy as np
 import pandas as pd
-import multiprocessing
-from multiprocessing import Process , Queue , Pool
-import subprocess
-
-
-
-
-with open('config.json') as json_file:
-    config = json.load(json_file)
-
-if config['far_config']['visible_gpu_devices']=="local":
-    try:
-        cuda_visible_devices = os.environ["CUDA_VISIBLE_DEVICES"] 
-    except KeyError:
-        cuda_visible_devices = '0'
-else:
-    cuda_visible_devices = config['far_config']["visible_gpu_devices"]
-
-print("cuda_visible_devices ", cuda_visible_devices, ",type: ", type(cuda_visible_devices))
-
-os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
 # Input creation
-import sys, os, argparse
-sys.path.append(config['mlyPipelineSource']+"/mly/")
     
 from mly.tools import dirlist
 from mly.datatools import DataSet, DataPod
 # Data assemble
 from mly.offlinefar import assembleDataSet
 
 
 arguments = ["mode",
             "dataSet",
             "batchNumber"
 
 ]
-
 #Construct argument parser:
 parser = argparse.ArgumentParser()
 #[parser.add_argument(f"--{argument}") for argument in arguments]
 
 parser.add_argument('--mode')
 
 parser.add_argument('--dataSet', type=str, default=None)
@@ -65,28 +50,44 @@
 
 # Store arguments in dictionary:
 kwdict = {}
 for argument in arguments:
     kwdict[argument] = getattr(args, argument)
 
 
+with open('config.json') as json_file:
+    config = json.load(json_file)
+
 mode = kwdict['mode']
 masterDirectory = config['masterDirectory']
 detectors = config['detectors'] #to get from config
 dataSet = kwdict['dataSet']
 
 batches =  config['far_config']['batches']
 batchNumber = kwdict['batchNumber']
 
 lags = config['far_config']['lags']
 selectedGPUs = config['far_config']['selectedGPUs']
 batch_size = config['far_config']['batch_size']
 parallelGenerations = config["far_config"]["parallelGenerations"]
 
 
+
+if config['far_config']['visible_gpu_devices']=="local":
+    try:
+        cuda_visible_devices = os.environ["CUDA_VISIBLE_DEVICES"] 
+    except KeyError:
+        print("No visible GPU devices detected, setting index to 0.")
+        cuda_visible_devices = '0'
+else:
+    cuda_visible_devices = config['far_config']["visible_gpu_devices"]
+
+
+
+
 # # # Initialising logging
 
 # create logger
 logger = logging.getLogger("logger_for_manager")
 logger.setLevel(logging.DEBUG)
 
 
@@ -100,40 +101,34 @@
 # add formatter to ch
 ch.setFormatter(formatter)
 
 # add ch to logger
 logger.addHandler(ch)
 
 
-logger.debug(f"PROCESSES hermes imports: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
 
 if mode == 'inference':
 
     import tensorflow as tf
     from tensorflow.keras.models import load_model
     from tensorflow.config import threading
 
     threading.set_inter_op_parallelism_threads(1)
     threading.set_intra_op_parallelism_threads(1)
-    try:
-        # our hermes imports
-        from hermes import quiver as qv
-        from hermes.aeriel.client import InferenceClient
-        from hermes.aeriel.serve import serve
-    except Exception as e:
-        print(f"Exception for importing hermes from environment: {e}")
-        sys.path.append("/home/$USER/hermes/hermes")
-        from hermes import quiver as qv
-        from hermes.aeriel.client import InferenceClient
-        from hermes.aeriel.serve import serve
-    logger.debug(f"PROCESSES after hermes imports: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+    from hermes import quiver as qv
+    from hermes.aeriel.client import InferenceClient
+    from hermes.aeriel.serve import serve
 
 
 
+    logger.debug(f"PROCESSES hermes imports: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+
 
 def dataToQueue(dataSet_Q, dataSetName_Q): # Depricated until Hermes issue solved
 
     already_used=[]
     while (1):
 
         fileList = dirlist(config["falseAlarmRates"]+"/temp/")
@@ -531,24 +526,28 @@
 
 
 
     # now serve a local Triton instance on GPU 0 using Singularity
 
     openingclientT0 = time.time()
     with serve(repo_path, image="hermes/tritonserver:22.12"
-             , gpus=selectedGPUs, log_file="./server.log",server_args=["--allow-gpu-metrics false --grpc-port 8003 --http-thread-count 1 --model-load-thread-count 1 --grpc-infer-allocation-pool-size 1"]) as instance:
+             , gpus=selectedGPUs, log_file="./server.log",server_args=["--allow-gpu-metrics false --grpc-port 8003 --http-thread-count 1 --model-load-thread-count 1"]) as instance:
         
+        threading.set_inter_op_parallelism_threads(1)
+        threading.set_intra_op_parallelism_threads(1)
         logger.debug(f"PROCESSES at the start of server: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+        
 
-        instance.wait()
-
+        instance.wait(endpoint="localhost:8003")
+        threading.set_inter_op_parallelism_threads(1)
+        threading.set_intra_op_parallelism_threads(1)
         logger.debug(f"PROCESSES after instance waiting: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
         client = InferenceClient(
-            "localhost:8001",
+            "localhost:8003",
             model_name="ensemble",
             model_version=1,
             batch_size=batch_size,
         )
         # monitor = ServerMonitor(
         #     model_name="ensemble",
         #     ips="localhost",
@@ -632,27 +631,24 @@
                         stop = start + 1 * batch_size
                         c_start = i * 1 * batch_size
                         c_stop = c_start + 1 * batch_size
 
                         kernel = {'strain' : strainList[ start : stop ]
                                     ,'correlation' : correlationList[ c_start : c_stop ]}
                         
-                        logger.debug(f"PROCESSES with serve before client.infer: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
                         client.infer(kernel, request_id=i)
-                        logger.debug(f"PROCESSES with serve before client.infer: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
                         # sleep to roughly maintain our inference rate
                         time.sleep(0.9 / batches_per_second)
 
                         if i < 5:
                             response_ = client.get()
                             trials = 1
                             while response_ is None and trials<5000:
                                 response_ = client.get()
-                                logger.debug(f"PROCESSES client.get {i}: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
                                 time.sleep(1e-2)
                                 trials+=1
                                 if trials>=5000: raise(Exception("Trials exceeded 5000."))
 
                             response, _, __ = response_
                             logger.debug(f"{i} response type {type(response)} ,with shape {response.shape} and {trials} trials")
@@ -680,17 +676,21 @@
                     result=np.hstack((np.expand_dims(results,axis=1),np.array(gpsTimes)[:len(results)]))
                     logger.info(f"Size of the result {len(result)}")
                     #print(result)
 
                     name = '_'.join(out_name[:-4].split('_')[:2])+'_'+str(len(result))
 
                     if 'V' not in detectors:
-                        temp_detectors = detectors+'V'
+                        if isinstance(detectors,str):
+                            temp_detectors = detectors+'V'
+                        else:
+                            temp_detectors = detectors + ['V']
                     else:
                         temp_detectors = detectors
+
                     result_pd = pd.DataFrame(result ,columns = ['score']+list('GPS'+str(det) for det in temp_detectors))
                     logger.info(f"len before restriction: {len(result_pd)}")
                     result_pd = result_pd[result_pd['score'] >= config['far_config']['restriction'] ]
                     logger.info(f"len after restriction: {len(result_pd)}")
 
                     with open(config["falseAlarmRates"]+"/"+name+'.pkl', 'wb') as output:
                         pickle.dump(result_pd, output, 4)
@@ -721,15 +721,15 @@
         subGeneration(dataSet      
                   , batchNumber         
                   , batches     
                   , masterDirectory
                   , lags)
     
     elif mode == 'inference':
-        print(batch_size)
+
         inference()   
 
 
         # dataSet_Q = Queue()
         # dataSetName_Q = Queue()
         # print(batch_size)
         # t1 = Process(target = dataToQueue, args = (dataSet_Q, dataSetName_Q))
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/initialization.py` & `mly_pipeline-0.5.2/mly_pipeline/initialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,25 @@
                  ,"triggerplot_directory"
                  ,"masterDirectory"
                  ,"bufferDirectory"
                  ,"falseAlarmRates"
                  ,"efficiencies"
                  ,"detectors"
                  ,"reset"
-                 ,"part"]
+                 ,"far"]
 
     
     #Construct argument parser:
     parser = argparse.ArgumentParser()
 
-    parser.add_argument('-search_mode', '--search_mode', type=str
+    parser.add_argument('-s', '--search_mode', type=str
                         , default = "DEFAULT_OFFLINE"
                         , help = "For automatically setting the pipeline for different uses"
                         , required = False)
-    
+
     parser.add_argument('-p', '--path', type=str
                         , default = "./mlyPipelineOrigin"
                         , help = "The path and name of the"
                         +" directory to be used by mlyPipeline."
                         , required = False)
 
     parser.add_argument('-o', '--output_directory', type=str
@@ -89,31 +89,33 @@
     
     parser.add_argument('-R', '--reset', type=bool
                         , default = False
                         , help = "If true it will ovewright the target path"
                         + " with a clean new filesystem."
                         , required = False)
 
-    parser.add_argument('-part', '--part', type=int
-                        , default = 0
-                        , help = "Used to separate the different offline channels"
-                        +" of the burst pipeline benchmark"
+    parser.add_argument('-far', '--far', type=bool
+                        , default = True
+                        , help = "If true it will include the FAR scripts used for background estimation. This is only for OFFLINE searches"
                         , required = False)
+
+
+
+
     
     # Pass arguments:
     args = parser.parse_args()
     
     # Store arguments in dictionary:
     kwargs = {}
     for argument in arguments:
         kwargs[argument] = getattr(args, argument)
 
     return kwargs
-
-    
+   
 def connect_path_relatively_to(path_to_change,path_to_connect):
     common_part = []
     for dir in path_to_change.split('/'):
         if dir in path_to_connect.split('/'):
             common_part.append(dir)
         else:
             break
@@ -162,26 +164,28 @@
             f.write("   done" + "\n\n\n")
         
             # Script that runs the manager script
             f.write("   nohup python -m mly_pipeline.manager &> manager.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
             
             # If the search runs as expected by default, it will also run scripts
             # for generating timelags and running FAR tests.
-            if kwargs['search_mode'] not in ["O3MDC" , 'BENCHMARK_MDC_OFFLINE']:
+            if kwargs['far_config']['far_enabled']:
                 f.write("   nohup python -m mly_pipeline.continuous_FAR --mode generation &> continuous_FAR_generation.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
                 f.write("   nohup python -m mly_pipeline.continuous_FAR --mode inference &> continuous_FAR_inference.out & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
             
             # # # Maintenance of jobs 
             
             # If total_failure becomes 1, the script runs everything from scratch
             f.write("    total_failure=0" + "\n")
             
             # Sometimes the FAR script might stal indefinetly for unknow reasons
             # related to triton package, so if it does we restart it.
-            f.write("    staling_points=0" + "\n")
+            if kwargs['far_config']['far_enabled']:
+
+               f.write("    staling_points=0" + "\n")
             
             # We add the number of timelag files present to see if our rate of 
             # doing FAR inference is efficient. Check the monitor.txt present in
             # the search directory, if there are too many zeros we can increase
             # our timelag production - "lags", always along with "batches". If
             # there are no zeros, we need to decrease the "lags" or inference 
             # does not work properly.
@@ -206,15 +210,16 @@
             f.write("                echo total failure" + "\n")
             f.write("                break" + "\n")
             f.write("            fi" + "\n") 
             f.write("        done" + "\n")
 
             # Specifically for inference script we check seperatelly, if it
             # doesn't look properly we rerun only the inference script. 
-            if kwargs['search_mode'] not in ["O3MDC" , 'BENCHMARK_MDC_OFFLINE']:
+            if kwargs['far_config']['far_enabled']:
+
             
                 # Checking if the number of inference files stays 0 for a long time.
                 # If lag files increase without any new inference files, that means
                 # staling, and we add a staling point. If not we reset it to 0.
                 f.write("        if [ $(ls falseAlarmRates | wc -l) -eq 4 ] && [ $(ls falseAlarmRates/temp | wc -l) -ne 0 ]" + "\n")
                 f.write("        then" + "\n")
                 f.write("            echo stalling points increase to $staling_points" + "\n")   
@@ -252,28 +257,89 @@
                 f.write("   kill $inferenceID" + "\n")
                 f.write("   singularity instance stop --all" + "\n")
 
             f.write("done" + "\n")
         
         # Currently the offline script is very simple (under developement)
         else:
+
+            if kwargs['far_config']['far_enabled']:
+
+                f.write("nohup python -m mly_pipeline.offline_search --mode set_file_system &> set_file_system.out & echo $!>>.jobids.txt" + "\n\n")
+                
+                f.write("sleep 300" + "\n\n")
+
+                f.write("nohup python -m mly_pipeline.continuous_FAR --mode generation &> continuous_FAR_generation.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
+                f.write("nohup python -m mly_pipeline.continuous_FAR --mode inference &> continuous_FAR_inference.out & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
+
+                # Checking if the number of inference files stays 0 for a long time.
+                # If lag files increase without any new inference files, that means
+                # staling, and we add a staling point. If not we reset it to 0.
+                
+                f.write("staling_points=0" + "\n")
+                f.write("# The batches of generation times the dagmans" + "\n")
+                f.write("max_inference_files=$(( $(jq .far_config.batches config.json) * $(ls masterDirectory/*.py | wc -l)  ))" + "\n")
+
+                f.write("premature_ending_points=0" + "\n")
+
+                f.write("# While the number of far files generated is not equal to max inference files" + "\n")
+                f.write("while [ $(($(ls falseAlarmRates | wc -l) - 4)) -lt $max_inference_files ]" + "\n")
+                f.write("do" + "\n")
+                
+                f.write("        echo FAR completion: $(($(ls falseAlarmRates | wc -l) - 4)) / $max_inference_files" + "\n")
+                f.write("        sleep 300" + "\n\n")
+
+                f.write("        if [ $(ls falseAlarmRates | wc -l) -eq 4 ] && [ $(ls falseAlarmRates/temp | wc -l) -ne 0 ]" + "\n")
+                f.write("        then" + "\n")
+                f.write("            echo stalling points increase to $staling_points" + "\n")   
+                f.write("            ((staling_points=staling_points+1))" + "\n")
+                f.write("        else" + "\n")
+                f.write("            staling_points=0" + "\n")
+                f.write("        fi" + "\n\n")
+
+                # In case inference script gets killed or we have at least 5 minutes
+                # of staling, we restart inference script. Although, we keep the 
+                # corresponding unix time it got killed in the name of the  output
+                # file.
+                f.write("        if ! ps $inferenceID > /dev/null || [ $staling_points -gt 5 ]"+ "\n")
+                f.write("        then" + "\n")
+                f.write("            singularity instance stop --all" + "\n")
+                f.write("            nohup python -m mly_pipeline.continuous_FAR --mode inference >"
+                                    +" continuous_FAR_inference.out 2>&1"
+                                    +" & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
+                f.write("        fi" + "\n\n")                        
+                        
+                f.write("        if [ $(condor_q -autoformat RequestMemory | wc -l) -eq 0 ] && [ $(($(ls falseAlarmRates | wc -l) - 4)) -ne 0 ] " + "\n")
+                f.write("        then    " + "\n")
+                f.write("            ((premature_ending_points=premature_ending_points+1))" + "\n")
+                f.write("            echo premature ending points increased: $premature_ending_points / 3" + "\n")
+                f.write("        fi" + "\n\n")
+
+                f.write("        if [ $premature_ending_points -ge 3 ]" + "\n")
+                f.write("        then " + "\n")
+                f.write("            break" + "\n")
+                f.write("        fi" + "\n\n")
+
+                f.write("done" + "\n")
+
+                f.write("kill $inferenceID $generationID" + "\n")
+                f.write("singularity instance stop --all" + "\n")
+
+                f.write("python -c \"from mly_pipeline.manager import manage_FAR_inefernce_files; manage_FAR_inefernce_files()\" "+ "\n")
+                f.write("# Need to add a manager of FAR files at the beggining of offline search"+ "\n")
+            
+            # If FAR is already calculated we only need this to run
             f.write("nohup python -m mly_pipeline.offline_search &> search.out & echo $!>>.jobids.txt" + "\n\n")
 
 
 
 def main():
     
     kwargs = _parser()
 
-    pwd = os.getcwd()
-
-    mlyPipelineSourceString = connect_path_relatively_to(  os.path.abspath('/'.join(sys.argv[0].split('/')[:-1]))
-                                                            ,pwd )
-
-
     if kwargs['path'][-1]=="/" : kwargs['path'] = kwargs['path'][:-1]
     
     
     if os.path.isdir(kwargs['path']) and kwargs['reset'] == True:
                 
         
         print(kwargs['path']," is going to be reset")
@@ -301,20 +367,17 @@
         
     else:
         raise ValueError("Wrong input for file", os.path.isfile(kwargs['path'])
                          , kwargs['reset'] == True)
         
     print(f"Search mode selected: {kwargs['search_mode']}")
 
-    frames_dict = dict(DEFAULT_ONLINE = {'H':""
-                                 ,'L':""
-                                 ,'V':""}
-                        ,DEFAULT_OFFLINE = {'H':""
-                                 ,'L':""
-                                 ,'V':""}
+    frames_dict = dict(   DEFAULT_ONLINE = {'H':"" ,'L':"" ,'V':""}
+
+                        ,DEFAULT_OFFLINE = {'H':"" ,'L':"" ,'V':""}
 
                         , O4_ONLINE = {'H':"/dev/shm/kafka/H1/"
                                       ,'L':"/dev/shm/kafka/L1/"
                                       ,'V':"/dev/shm/kafka/V1/"}
 
                         , O3MDC = {'H':"/dev/shm/kafka/H1_O3ReplayMDC/"
                                   ,'L':"/dev/shm/kafka/L1_O3ReplayMDC/"
@@ -325,38 +388,51 @@
                                      ,'V':"/dev/shm/kafka/V1_O3ReplayMDC/"}
 
                         , BENCHMARK_MDC_OFFLINE = {'H':"/scratch/florent.robinet/BurstBenchmark/"
                                               ,'L':"/scratch/florent.robinet/BurstBenchmark/"
                                               ,'V':"/scratch/florent.robinet/BurstBenchmark/"}
                     )
 
-    channels_dict = dict( DEFAULT_ONLINE = {'H':""
-                                 ,'L':""
-                                 ,'V':""}
-                        ,DEFAULT_OFFLINE = {'H':""
-                                 ,'L':""
-                                 ,'V':""}
+    channels_dict = dict( DEFAULT_ONLINE = {'H':"" ,'L':"" ,'V':""}
+    
+                        ,DEFAULT_OFFLINE = {'H':"" ,'L':"" ,'V':""}
 
                         , O4_ONLINE = {'H':"H1:GDS-CALIB_STRAIN_CLEAN"
                                       ,'L':"L1:GDS-CALIB_STRAIN_CLEAN"
                                       ,'V':"V1:Hrec_hoft_16384Hz_Gated"}
 
                         , O3MDC = {'H':"H1:GDS-CALIB_STRAIN_INJ1_O3Replay"
                                   ,'L':"L1:GDS-CALIB_STRAIN_INJ1_O3Replay"
                                   ,'V':"V1:Hrec_hoft_16384Hz_INJ1_O3Replay"}
 
                         , O3REPLAY = {'H':"H1:GDS-CALIB_STRAIN_O3Replay"
                                      ,'L':"L1:GDS-CALIB_STRAIN_O3Replay"
                                      ,'V':"V1:Hrec_hoft_16384Hz_INJ1_O3Replay"}
 
                         , BENCHMARK_MDC_OFFLINE = {'H':"H1:STRAIN_BURST_0"
-                                              ,'L':"L1:STRAIN_BURST_0"
-                                              ,'V':"V1:STRAIN_BURST_0"}
+                                                  ,'L':"L1:STRAIN_BURST_0"
+                                                  ,'V':"V1:STRAIN_BURST_0"}
                                 )
     
+    state_vector_channel_dict = dict( 
+                          DEFAULT_ONLINE = {'H':"" ,'L':"" ,'V':""}
+    
+                        , DEFAULT_OFFLINE = None
+
+                        , O4_ONLINE = {'H':'H1:GDS-CALIB_STATE_VECTOR'
+                                      ,'L':'L1:GDS-CALIB_STATE_VECTOR'
+                                      ,'V':'V1:DQ_ANALYSIS_STATE_VECTOR'}
+
+                        , O3MDC = None
+
+                        , O3REPLAY = None
+
+                        , BENCHMARK_MDC_OFFLINE = None
+                                )
+
     if kwargs['search_mode'] == "BENCHMARK_MDC_OFFLINE":
         segment_list_default = "/home/vasileios.skliris/public_html/benchmark_segments.txt"
     else:
         segment_list_default = []
 
 
     # # # # # # # CONFIG FILE # # # # # # #
@@ -373,16 +449,14 @@
     triggerplot_directory = kwargs["triggerplot_directory"],
     masterDirectory = kwargs["masterDirectory"],
     bufferDirectory = kwargs["bufferDirectory"],
     falseAlarmRates = kwargs["falseAlarmRates"],
     efficiencies = kwargs["efficiencies"],
     log = "log",
     
-    # local mlyPipeline installation path
-    mlyPipelineSource = mlyPipelineSourceString,
         
     # User name
     
     user_name = os.environ['HOME'].split("/")[-1],
 
 
     accounting_group_user = os.environ['HOME'].split("/")[-1],
@@ -409,15 +483,16 @@
     
     # Frame file prefixes to use
     frames_directory= frames_dict[kwargs['search_mode']],
     
     # The channels to use, INJ is the MDC and NOISE is O3-replay
     channels = channels_dict[kwargs['search_mode']],
 
-
+    # The channels used for the state vector in online searches
+    state_vector_channels= state_vector_channel_dict[kwargs['search_mode']],
 
     segment_list = segment_list_default,
 
     max_continuous_segment = 10000,
     # # # Fetching data related parameters 
 
     # The number of search script running. (The number of scripts must be more than 
@@ -438,16 +513,18 @@
     start_lag=92,
         
     # If search time is left behind by that amount of seconds it skips ahead.
     gps_reset_time=32,
         
     # FAR file that is used to calculate FAR. It is used only at
     # the beggining of the search, until there is enough background estimation.
-    farfile=("/home/vasileios.skliris/mly-hermes/outputs/FARfile"),
-
+    
+    farfile= ("/home/vasileios.skliris/mly-hermes/outputs/FARfile" if kwargs['far'] 
+              else kwargs["falseAlarmRates"]+"/FARfile" ),
+    
     # # # Models 
         
     # Model1 path, conincidence model.
     model1_path=("/home/mly/models/model1_32V_No5.h5"), 
         
     # Model2 path, coherence model.
     model2_path=("/home/mly/models/model2_32V_No6.h5"),  
@@ -478,15 +555,19 @@
                                              ,'wnb_03_train_pod'
                                              ,'cusp_00'] if "OFFLINE" not in kwargs['search_mode'] else []
                       ,injectionHRSS = "1e-22,1e-21,1e-22"
                       ,injectionSNR =  "0,50,5"
                       ,testSize = "100"
                       ,howOften = 3600),
 
-    far_config = dict( batch_size=1024
+    far_config = dict( 
+                    # Enabling or not the calculation of FAR.
+                    far_enabled = True if kwargs['far'] else False
+                    # Number of timelags used.
+                    ,batch_size=1024
                     # It is used only at the beggining of a search until a FAR is estimated.
                     ,threshold = 2.3148e-05 if "OFFLINE" in kwargs['search_mode'] else 1/3600
                     # The score from which we keep FAR statistics.
                     ,restriction = 0.0001
                     # The maximum lag to be used. Determines the DataSet size of the saved instances.
                     ,max_lag = 3600
                     # The amount of lags to use for each file. Depends on the capasity to produce them.
@@ -507,25 +588,25 @@
     
     # The group size of the files that used to save the outputs    
     maxDataFrameSize = 3600,
     
     # The destination of the triggers, None means testing mode with FAKEIDs.
     trigger_destination = "playground" if kwargs['search_mode'] in ["O3MDC"] else None,
 
-    part = kwargs['part'] if kwargs['search_mode']=="OFFLINE" else None
     
 
     )
 
 
     os.system("mkdir " + configuration['path'] +"/"+ configuration['output_directory'])
     os.system("mkdir " + configuration['path'] +"/"+ configuration['trigger_directory'])
     os.system("mkdir " + configuration['path'] +"/"+ configuration['triggerplot_directory'])
+    os.system("mkdir " + configuration['path'] +"/"+ configuration['log'])
 
-    if "OFFLINE" not in kwargs['search_mode']:
+    if not ("OFFLINE" in kwargs['search_mode'] and not kwargs['far']):
 
         os.system("mkdir " + configuration['path'] +"/"+ configuration['masterDirectory'])
         os.system("mkdir " + configuration['path'] +"/"+ configuration['masterDirectory'] 
                 +"/temp")
 
         for det in configuration['detectors']:
             os.system("mkdir " + configuration['path'] +"/"+ configuration['masterDirectory'] 
@@ -549,15 +630,15 @@
 
         
         
         os.system("mkdir " + configuration['path'] +"/"+ configuration['efficiencies'])
         os.system("mkdir " + configuration['path'] +"/"+ configuration['efficiencies'] 
                 +"/history")
         
-        os.system("mkdir " + configuration['path'] +"/"+ configuration['log'])
+
 
 
 
     # Saving config file to json format
     with open(configuration['path'] +"/"+"config.json", "w") as config_json:
         json.dump(configuration, config_json,indent=4)
         config_json.close()
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.5.2/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline/manager.py` & `mly_pipeline-0.5.2/mly_pipeline/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+
+import os
+# Scipy and numpy env parameters that limit the threads
+os.environ["MKL_NUM_THREADS"] = "1"
+os.environ["NUMEXPR_NUM_THREADS"] = "1"
+os.environ["OMP_NUM_THREADS"] = "1"
+
 import json
 import pickle
 import argparse
 import sys ,time
-import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from lal import gpstime
-from gwpy.time import from_gps, to_gps
 import os
 import logging
 import subprocess
 
 
 from mly.tools import dirlist
 from mly.datatools import *
 from .search_functions import *
 
+
+
 # # # Initialising logging
 
 # create logger
 logger = logging.getLogger("logger_for_manager")
 logger.setLevel(logging.DEBUG)
 
 
@@ -34,16 +39,14 @@
 # add formatter to ch
 ch.setFormatter(formatter)
 
 # add ch to logger
 logger.addHandler(ch)
 
 
-
-
 # # # Managing arguments
 # 
 # List of arguments to pass:
 arguments = [
 
     "restriction",
     "timeUnit"
@@ -51,351 +54,560 @@
 
 #Construct argument parser:
 parser = argparse.ArgumentParser()
 
 parser.add_argument('--restriction')
 parser.add_argument('--timeUnit')
 
- 
+
 # Pass arguments
 args = parser.parse_args()
 
 # Store arguments in dictionary:
 kwdict = {}
 for argument in arguments:
     kwdict[argument] = getattr(args, argument)
-
     
 with open('config.json') as json_file:
     config = json.load(json_file)
     
 config={ **kwdict , **config}
-    
-# # # Argument checks
 
-config = checkOutputDirectoryArguments(config)
 
-# The size in which we group the outputs
-if config['maxDataFrameSize']==None: 
-    config['maxDataFrameSize']=3600
+def main(config):
 
-maxDataFrameSize = int(config['maxDataFrameSize'])
+    config = checkOutputDirectoryArguments(config)
 
-if config['restriction']==None: 
-    config['restriction']=0.0
-restriction=float(config['restriction'])
-    
-# This is the time scale to use for the plots
-timeUnitDict={1:'s', 60:'m', 3600:'h', 24*3600:'days',30*24*3600:'months', 365*24*3600:'years'}
+    # The size in which we group the outputs
+    if config['maxDataFrameSize']==None: 
+        config['maxDataFrameSize']=3600
 
-if config['timeUnit']==None: 
-    config['timeUnit']=3600
-else:
-    config['timeUnit']=int(config['timeUnit'])
-    
+    maxDataFrameSize = int(config['maxDataFrameSize'])
 
-sys.stdout.flush()
 
+    # This is the time scale to use for the plots
+    timeUnitDict={1:'s', 60:'m', 3600:'h', 24*3600:'days',30*24*3600:'months', 365*24*3600:'years'}
+
+    if config['timeUnit']==None: 
+        config['timeUnit']=3600
+    else:
+        config['timeUnit']=int(config['timeUnit'])
+        
+
+    sys.stdout.flush()
 
-while (1):
-    logger.debug(f"PROCESSES before output management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
-    loopT0=time.time()
-    
-    output_directory = config['output_directory']
-    
-    frameSizeCheck=0
-    fileList = dirlist(output_directory)
-    dFramesList  = []
-    jsonList = []
-    # Listing the files in the directory
-    # Separating the json from pkl
-    for file in fileList:
-
-        if ".json" in file:
-            jsonList.append(file)
-        elif ".pkl" in file:
-            dFramesList.append(file)
-
-    # if there are no new outputs we skip that step
-    if len(jsonList)!=0: 
-
-        # We expect that every time the manager runs, there is a tempFrame
-        # file that might have events but it is not of the size we group
-        # them (maxDataFrameSize). 
-        try:
-
-            with open(output_directory+'tempFrame.pkl','rb') as obj:
-                tempFrame = pickle.load(obj)
-        # The first time manager is running this file is created instead.
-        except Exception as e:
-            tempFrame = pd.DataFrame(columns = ['gpstime','far','ifos'
-                                                ,'coincidence','coherency'
-                                                ,'combined','trigger'])
-            logger.info(f"Creating tempfile for the first time.")
-
-        # The size of the frame
-        initialTempFrameSize=len(tempFrame)
-
-        # A check value to make sure we add all the json files.
-        frameSizeCheck = len(jsonList) + initialTempFrameSize
-        print("firstcheck",frameSizeCheck, len(tempFrame))
 
-        # Adding all the events in json format to the tempFrame
-        for file in jsonList:
+    while (1):
+        logger.debug(f"PROCESSES before output management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        loopT0=time.time()
+        
+        output_directory = config['output_directory']
+        
+        frameSizeCheck=0
+        fileList = dirlist(output_directory)
+        dFramesList  = []
+        jsonList = []
+        # Listing the files in the directory
+        # Separating the json from pkl
+        for file in fileList:
+
+            if ".json" in file:
+                jsonList.append(file)
+            elif ".pkl" in file:
+                dFramesList.append(file)
+
+        # if there are no new outputs we skip that step
+        if len(jsonList)!=0: 
+
+            # We expect that every time the manager runs, there is a tempFrame
+            # file that might have events but it is not of the size we group
+            # them (maxDataFrameSize). 
             try:
-                with open(output_directory+file,"r") as jf:
-                    p=json.load(jf)
-                    jf.close()
+
+                with open(output_directory+'tempFrame.pkl','rb') as obj:
+                    tempFrame = pickle.load(obj)
+            # The first time manager is running this file is created instead.
             except Exception as e:
-                logger.warning(f"Exception in loading json file {file}, {e}")
-                continue
+                tempFrame = pd.DataFrame(columns = ['gpstime','far','ifos'
+                                                    ,'coincidence','coherency'
+                                                    ,'combined','trigger'])
+                logger.info(f"Creating tempfile for the first time.")
 
+            # The size of the frame
+            initialTempFrameSize=len(tempFrame)
 
+            # A check value to make sure we add all the json files.
+            frameSizeCheck = len(jsonList) + initialTempFrameSize
 
-        # Reformating the score parameters to the desired format.
-            for k in list(p['scores'].keys()):
-                p[k]=p['scores'][k]
-            # Making a list of ifos to avoid line breaking into two
-            p['ifos'] = [p['ifos']]
+            # Adding all the events in json format to the tempFrame
+            for file in jsonList:
+                try:
+                    with open(output_directory+file,"r") as jf:
+                        p=json.load(jf)
+                        jf.close()
+                except Exception as e:
+                    logger.warning(f"Exception in loading json file {file}, {e}")
+                    continue
 
-            if file[0]=='N':
-                p['trigger']=False
-            elif file[0]=='T':
-                p['trigger']=True
-            else:
-                p['trigger']=False
 
 
-            del(p['scores'])  
-            print('jsontopd',pd.DataFrame.from_dict(p))
-            tempFrame=pd.concat([tempFrame, pd.DataFrame.from_dict(p)]
-                                ,ignore_index=True)
-
-        # Reseting index and sorting by GPS time
-        tempFrame=tempFrame.sort_values(by="gpstime").reset_index(drop=True)
-        # Rearanging the columns
-        tempFrame = tempFrame[['gpstime','far','ifos','coincidence','coherency'
-                            ,'combined','trigger']]
-        print(tempFrame.head(4))
-        # Chopping the tempFrame to chuncs of maxDataFrameSize outputs
-        # IMPORTANT: We don't separate them by hour, we just collect 
-        # maxDataFrameSize of them together
-        while len(tempFrame) > maxDataFrameSize:
-
-            print("secondcheck",frameSizeCheck, len(tempFrame))
-
-            # Creating a newframe to include the maxDataFrameSize instances
-            newFrame=tempFrame[:maxDataFrameSize]
-            with open(output_directory+str(newFrame['gpstime'][0])+"-"
+            # Reformating the score parameters to the desired format.
+                for k in list(p['scores'].keys()):
+                    p[k]=p['scores'][k]
+                # Making a list of ifos to avoid line breaking into two
+                p['ifos'] = [p['ifos']]
+
+                if file[0]=='N':
+                    p['trigger']=False
+                elif file[0]=='T':
+                    p['trigger']=True
+                else:
+                    p['trigger']=False
+
+
+                del(p['scores'])  
+                tempFrame=pd.concat([tempFrame, pd.DataFrame.from_dict(p)]
+                                    ,ignore_index=True)
+
+            # Reseting index and sorting by GPS time
+            tempFrame=tempFrame.sort_values(by="gpstime").reset_index(drop=True)
+            # Rearanging the columns
+            tempFrame = tempFrame[['gpstime','far','ifos','coincidence','coherency'
+                                ,'combined','trigger']]
+            # Chopping the tempFrame to chuncs of maxDataFrameSize outputs
+            # IMPORTANT: We don't separate them by hour, we just collect 
+            # maxDataFrameSize of them together
+            while len(tempFrame) > maxDataFrameSize:
+
+                # Creating a newframe to include the maxDataFrameSize instances
+                newFrame=tempFrame[:maxDataFrameSize]
+                with open(output_directory+str(newFrame['gpstime'][0])+"-"
+                        +str(newFrame['gpstime'][maxDataFrameSize-1])
+                        +"_"+str(maxDataFrameSize)+'.pkl', 'wb') as output:
+                    pickle.dump(newFrame, output, 4)
+
+                logger.info("Saving group of outputs: ", output_directory+str(newFrame['gpstime'][0])+"-"
                     +str(newFrame['gpstime'][maxDataFrameSize-1])
-                    +"_"+str(maxDataFrameSize)+'.pkl', 'wb') as output:
-                pickle.dump(newFrame, output, 4)
+                    +"-"+str(maxDataFrameSize)+'.pkl')
 
-            logger.info("Saving group of outputs: ", output_directory+str(newFrame['gpstime'][0])+"-"
-                +str(newFrame['gpstime'][maxDataFrameSize-1])
-                +"-"+str(maxDataFrameSize)+'.pkl')
-
-            # Removing the newframe from tempFrame
-            tempFrame=tempFrame[maxDataFrameSize:].reset_index(drop=True)
-
-            frameSizeCheck-=maxDataFrameSize
-
-        # What is left in tempFrame, overights the tempFrame.pkl
-        with open(output_directory+'tempFrame.pkl', 'wb') as output:
-            pickle.dump(tempFrame, output, 4)
-            logger.info(f"Saving the incomplete group of outputs: {output_directory}tempFrame.pkl")
+                # Removing the newframe from tempFrame
+                tempFrame=tempFrame[maxDataFrameSize:].reset_index(drop=True)
 
-        
-        # We remove all json files already included in a dataFrame
-        for file in jsonList:
-            os.system("rm "+output_directory+file )
+                frameSizeCheck-=maxDataFrameSize
 
+            # What is left in tempFrame, overights the tempFrame.pkl
+            with open(output_directory+'tempFrame.pkl', 'wb') as output:
+                pickle.dump(tempFrame, output, 4)
+                logger.info(f"Saving the incomplete group of outputs: {output_directory}tempFrame.pkl")
 
-        # # Plotting all available events in a zero-lagged score rate
-        # # (Might remove in the future, used to see consistency)
-        # testNumber=0
-        # dFramesList  = []
-        # scores=[]
-        # # Listing the files in the directory
-        # # Separating the json from pkl
-        # fileList = dirlist(output_directory)
-        # for file in fileList:
-        #     if ".pkl" in file : dFramesList.append(file)
+            
+            # We remove all json files already included in a dataFrame
+            for file in jsonList:
+                os.system("rm "+output_directory+file )
 
-        # for file in dFramesList:
 
-        #     with open(output_directory+file,'rb') as obj:
-        #         frame_ = pickle.load(obj)
+            # # Plotting all available events in a zero-lagged score rate
+            # # (Might remove in the future, used to see consistency)
+            # testNumber=0
+            # dFramesList  = []
+            # scores=[]
+            # # Listing the files in the directory
+            # # Separating the json from pkl
+            # fileList = dirlist(output_directory)
+            # for file in fileList:
+            #     if ".pkl" in file : dFramesList.append(file)
 
-        #     testNumber+=len(frame_)
+            # for file in dFramesList:
 
-        #     scores+=list(frame_[frame_['combined']>=restriction]['combined'])
+            #     with open(output_directory+file,'rb') as obj:
+            #         frame_ = pickle.load(obj)
 
+            #     testNumber+=len(frame_)
 
-        # s=np.sort(scores)[::-1]
+            #     scores+=list(frame_[frame_['combined']>=restriction]['combined'])
 
 
-        # fig,ax1=plt.subplots(figsize=(6,6))
+            # s=np.sort(scores)[::-1]
 
-        # ax1.loglog(s,np.arange(len(s))+1,label='O3a '+config['detectors']+' backround')
-        # ax1.set_title(config['detectors']+"-FAR up to : "+str(from_gps(gpstime.gps_time_now()))+", total time: "+"{:.2f}".format(testNumber/config['timeUnit'])+timeUnitDict[config['timeUnit']])
 
+            # fig,ax1=plt.subplots(figsize=(6,6))
 
-        # #ax1.set_yticks(np.array([1e0,1e1,119,1e3,1e4,1e5,1e6]))
-        # #ax1.set_yticklabels(np.array(['10 years','1 year','1 month','3.6 days','8.64 hours', '51.84 min' ,'5.18 min']))
+            # ax1.loglog(s,np.arange(len(s))+1,label='O3a '+config['detectors']+' backround')
+            # ax1.set_title(config['detectors']+"-FAR up to : "+str(from_gps(gpstime.gps_time_now()))+", total time: "+"{:.2f}".format(testNumber/config['timeUnit'])+timeUnitDict[config['timeUnit']])
 
-        # ax1.set_ylim(1,)
-        # if restriction>0: ax1.set_xlim(restriction,1)
-        # ax1.set_xlabel("Scores")
-        # ax1.set_ylabel("FAR")
-        # plt.savefig('./'+config['detectors']+"_far.png")
-        # plt.close('all')
 
-        
-    logger.debug(f"PROCESSES before FAR management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+            # #ax1.set_yticks(np.array([1e0,1e1,119,1e3,1e4,1e5,1e6]))
+            # #ax1.set_yticklabels(np.array(['10 years','1 year','1 month','3.6 days','8.64 hours', '51.84 min' ,'5.18 min']))
 
-    # # # FileSystem for FAR management
-    #
-    # Listing all files saved in the temp file (files to be managed)
-    detectors= list( det for det in config['detectors'])
-    
-    t0=time.time()
+            # ax1.set_ylim(1,)
+            # if restriction>0: ax1.set_xlim(restriction,1)
+            # ax1.set_xlabel("Scores")
+            # ax1.set_ylabel("FAR")
+            # plt.savefig('./'+config['detectors']+"_far.png")
+            # plt.close('all')
 
-    numberOfFiles={}
-    fileNumbers={}
-    dataSetDict={}
-    
-    # For each detector we count how many files have been saved in all
-    # detectors and we sort them.
-    for det in detectors:
-        numberOfFiles[det] = len(dirlist(config['masterDirectory']+'/temp/'+det))
-        fileNumbers[det] = sorted(list(file.split('_')[0] for file in dirlist(
-            config['masterDirectory']+'/temp/'+det)))
-        dataSetDict[det] = []
-
-    # If there are no files we skip this step
-    if len(fileNumbers[detectors[0]])==0:
-        logger.info(f"Empty temp directory")
-        #time.sleep(60)
-          
-    # If the files included in temp are less than maxDataFrameSize, we skip
-    # this step.
-    elif (int(float(fileNumbers[detectors[0]][-1]))
-         -int(float(fileNumbers[detectors[0]][0]))) < maxDataFrameSize:
-        logger.info(f"Not enough data \
-                    {maxDataFrameSize - (int(float(fileNumbers[detectors[0]][-1])) -  int(float(fileNumbers[detectors[0]][0])))}\
-                     to run the FAR test yet")
-        
-    # If the files included in temp are enough we group them
-    elif (int(float(fileNumbers[detectors[0]][-1]))
-          -int(float(fileNumbers[detectors[0]][0]))) >= maxDataFrameSize:
-        
-        c=0
-        
-        # We keep track of the files used to delete them later
-        filesToDelete=[]
-        
-        # Checking that all detectors have the same number of files
-        logger.debug(f"Number of files for each detector: {list(len(fileNumbers[det]) for det in detectors)}")
+            
+        logger.debug(f"PROCESSES before FAR management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        # # # FileSystem for FAR management
+        #
+        # Listing all files saved in the temp file (files to be managed)
+        detectors= list( det for det in config['detectors'])
         
-        lastFileNumber=None
-        # print("group size check: ",len(fileNumbers[detectors[0]][:int(maxDataFrameSize)]))
+        t0=time.time()
+
+        numberOfFiles={}
+        fileNumbers={}
+        dataSetDict={}
         
-        for filenumber in fileNumbers[detectors[0]][:int(maxDataFrameSize)]:
+        # For each detector we count how many files have been saved in all
+        # detectors and we sort them.
+        for det in detectors:
+            numberOfFiles[det] = len(dirlist(config['masterDirectory']+'/temp/'+det))
+            fileNumbers[det] = sorted(list(file.split('_')[0] for file in dirlist(
+                config['masterDirectory']+'/temp/'+det)))
+            dataSetDict[det] = []
+
+        # If there are no files we skip this step
+        if len(fileNumbers[detectors[0]])==0:
+            logger.info(f"Empty temp directory")
+            #time.sleep(60)
+            
+        # If the files included in temp are less than maxDataFrameSize, we skip
+        # this step.
+        elif (int(float(fileNumbers[detectors[0]][-1]))
+            -int(float(fileNumbers[detectors[0]][0]))) < maxDataFrameSize:
+            logger.info(f"Not enough data \
+                        {maxDataFrameSize - (int(float(fileNumbers[detectors[0]][-1])) -  int(float(fileNumbers[detectors[0]][0])))}\
+                        to run the FAR test yet")
+            
+        # If the files included in temp are enough we group them
+        elif (int(float(fileNumbers[detectors[0]][-1]))
+            -int(float(fileNumbers[detectors[0]][0]))) >= maxDataFrameSize:
+            
+            c=0
+            
+            # We keep track of the files used to delete them later
+            filesToDelete=[]
+            
+            # Checking that all detectors have the same number of files
+            logger.debug(f"Number of files for each detector: {list(len(fileNumbers[det]) for det in detectors)}")
+            
+            lastFileNumber=None
+            # print("group size check: ",len(fileNumbers[detectors[0]][:int(maxDataFrameSize)]))
+            
+            for filenumber in fileNumbers[detectors[0]][:int(maxDataFrameSize)]:
 
-            # For each file we in first detector we check that it exists in the
-            # other detectors too. 
-            if all( list( os.path.isfile(config['masterDirectory']
-                                         +'/temp/'+det+'/'+fileNumbers[detectors[0]][c]
-                                         +'_1.pkl') for det in detectors)):
-                
-                for det in detectors:
-                    dataSetDict[det].append(
-                        DataPod.load(config['masterDirectory']
-                                     +'/temp/'+det+'/'+str(filenumber)+'_1.pkl'))
+                # For each file we in first detector we check that it exists in the
+                # other detectors too. 
+                if all( list( os.path.isfile(config['masterDirectory']
+                                            +'/temp/'+det+'/'+fileNumbers[detectors[0]][c]
+                                            +'_1.pkl') for det in detectors)):
+                    
+                    for det in detectors:
+                        dataSetDict[det].append(
+                            DataPod.load(config['masterDirectory']
+                                        +'/temp/'+det+'/'+str(filenumber)+'_1.pkl'))
+                        
+                    lastFileNumber=int(float(filenumber))
+                    filesToDelete.append(str(filenumber)+'_1.pkl')
+                    
                     
-                lastFileNumber=int(float(filenumber))
-                filesToDelete.append(str(filenumber)+'_1.pkl')
                 
+                # Othewise we delete it and it can't be used
+                else:
+                    filesToDelete.append(str(filenumber)+'_1.pkl')
                 
+                c+=1
+
+            # We use those two for name creation
+            first = str(int(float(fileNumbers[detectors[0]][0])))
+            last = str(lastFileNumber)
+            # print('first,last: ',first,last)
             
-            # Othewise we delete it and it can't be used
-            else:
-                filesToDelete.append(str(filenumber)+'_1.pkl')
-            
-            c+=1
+            # Saving the instances in dataSets
+            for det in detectors:
+                _set = DataSet(dataSetDict[det])
+                name = first+'-'+last+'_'+str(len(_set))
+                _set.save(config['masterDirectory']+'/' + det + '/' + name)
+
+                # # Deleting files that already passed.
+                for file in filesToDelete:
+                    try:
+                        os.system("rm "+config['masterDirectory']+'/temp/'+det+'/'+file)
+                    except Exception as e:
+                        pass
 
-        # We use those two for name creation
-        first = str(int(float(fileNumbers[detectors[0]][0])))
-        last = str(lastFileNumber)
-        # print('first,last: ',first,last)
+        logger.debug(f"PROCESSES before efficiency and buffers management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        # # # Efficiency test buffer management
+        #
         
-        # Saving the instances in dataSets
-        for det in detectors:
-            _set = DataSet(dataSetDict[det])
-            name = first+'-'+last+'_'+str(len(_set))
-            _set.save(config['masterDirectory']+'/' + det + '/' + name)
+        if os.path.isdir(config['efficiencies']):
+            
+            # How many inferences to wait to run the test, roughly how often in seconds
 
-            # # Deleting files that already passed.
-            for file in filesToDelete:
-                try:
-                    os.system("rm "+config['masterDirectory']+'/temp/'+det+'/'+file)
-                except Exception as e:
-                    pass
+            efficiencyTestBuffer = config["eff_config"]["howOften"]
 
-    logger.debug(f"PROCESSES before efficiency and buffers management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+            # We load all the buffer pods that live in temp
+            buffer_set = []
+            pod_list = sorted(dirlist(config['bufferDirectory']+"/temp"))
+            
+            num_pods = len(pod_list)
+            
+            # If number of the buffer pods are more than maxDataFrameSize, we 
+            # putting them in a dataSet to be used.
+            logger.info(f"Buffer size accumulated: {num_pods}/{efficiencyTestBuffer} .Start efficiency test: {num_pods >= efficiencyTestBuffer}")
+            # I there are enough buffer pods we can save them to be used in an efficiency test.
+            if num_pods >= efficiencyTestBuffer:
+                
+                for each_pod in pod_list[:efficiencyTestBuffer]:
+                    pod = DataPod.load(config['bufferDirectory']+"/temp/"+each_pod) 
+                    buffer_set.append(pod)
+
+                buffer_dataset = DataSet(buffer_set)
+                buffer_dataset.save(config['bufferDirectory']+"/BUFFER_SET")
+
+                logger.info(f"Saving {config['bufferDirectory']}/BUFFER_SET")
+                # Removing all the ones we used after we made sure the set is saved.   
+                for each_pod in pod_list[:efficiencyTestBuffer]:
 
-    # # # Efficiency test buffer management
-    #
-    
-    if os.path.isdir(config['efficiencies']):
-        
-        # How many inferences to wait to run the test, roughly how often in seconds
+                    os.system("rm "+config['bufferDirectory']+"/temp/"+each_pod)
+                    
+                # Running the efficiencies script only if the previous has finished.
+                if len(dirlist(config['efficiencies'])) <= 2:
+                    os.system("nohup python "+config["mlyPipelineSource"]+"/make_eff_estimation.py --mode condor > efficiencyTest.out &")
+                    logger.info(f"Efficiency test initiated")
 
-        efficiencyTestBuffer = config["eff_config"]["howOften"]
 
-        # We load all the buffer pods that live in temp
-        buffer_set = []
-        pod_list = sorted(dirlist(config['bufferDirectory']+"/temp"))
-        
-        num_pods = len(pod_list)
-        
-        # If number of the buffer pods are more than maxDataFrameSize, we 
-        # putting them in a dataSet to be used.
-        logger.info(f"Buffer size accumulated: {num_pods}/{efficiencyTestBuffer} .Start efficiency test: {num_pods >= efficiencyTestBuffer}")
-        # I there are enough buffer pods we can save them to be used in an efficiency test.
-        if num_pods >= efficiencyTestBuffer:
-            
-            for each_pod in pod_list[:efficiencyTestBuffer]:
-                pod = DataPod.load(config['bufferDirectory']+"/temp/"+each_pod) 
-                buffer_set.append(pod)
-
-            buffer_dataset = DataSet(buffer_set)
-            buffer_dataset.save(config['bufferDirectory']+"/BUFFER_SET")
-
-            logger.info(f"Saving {config['bufferDirectory']}/BUFFER_SET")
-            # Removing all the ones we used after we made sure the set is saved.   
-            for each_pod in pod_list[:efficiencyTestBuffer]:
+        logger.debug(f"PROCESSES before fartest management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
+
+        # # # FAR test management 
+        #
 
-                os.system("rm "+config['bufferDirectory']+"/temp/"+each_pod)
+        manage_FAR_inefernce_files(config)
+
+        # # The list of all temporary inference files
+        # if os.path.isdir(config['falseAlarmRates']):
+            
+        #     inference_temp_files = dirlist(config['falseAlarmRates'])
+
+        #     for directory in ['hourly', 'condor', 'FARfile','temp']:
+        #         if directory in inference_temp_files: inference_temp_files.remove(directory)
+
+
+        #     # The list of all the files in hourly (grouped by hour/DAG of generation)
+        #     hourly_files = dirlist(config['falseAlarmRates']+"/hourly")
+
+        #     # The list of all condor dagman directories
+        #     condor_files =  dirlist(config['falseAlarmRates']+"/condor")
+
+        #     # The group names (start-end gps) in inference_temp_files
+        #     inference_temp_files_groups = list(file.split("_")[0] for file in inference_temp_files)
+        #     inference_temp_files_groups = list(dict.fromkeys(inference_temp_files_groups))
+
+        #     # The group names inside hourly
+        #     hourly_files_groups = list(file.split("_")[0] for file in hourly_files)
+
+        #     # The group names of condor directories
+        #     condor_groups= list(file.split("_")[0] for file in condor_files)
+
+        #     logger.debug(f"HOURLY GROUPS: {len(hourly_files_groups)}")
+        #     logger.debug(f"TEMP GROUPS: {len(inference_temp_files_groups)}")
+
+        #     # First we will go through the files that already have a group inside hourly
+        #     # We will add them in their corresponding hourly group file and remove them 
+        #     # from inference_temp_files
+
+        #     for hgroup, hfile_name in zip(hourly_files_groups, hourly_files):
+
+        #         if hgroup in inference_temp_files_groups:
+
+        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
+        #                 hfile = pickle.load(obj)
+                    
+        #             hfile_size = int(hfile_name.split("_")[-1][:-4])
+
+        #             to_remove_from_inference_temp_files = []
+
+        #             for file_name in inference_temp_files:
+                        
+        #                 if hgroup in file_name:
+
+        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
+        #                         file = pickle.load(obj)
+
+        #                     file = file[file['score'] >= restriction]
+
+        #                     hfile = pd.concat([hfile, file], ignore_index=True)
+                            
+        #                     # Adding the size of the file to the hourly file
+        #                     hfile_size += int(file_name.split("_")[-1][:-4])
+
+        #                     #TEMPORARY
+        #                     os.system("rm "+config['falseAlarmRates']+"/"+file_name)
+        #                     to_remove_from_inference_temp_files.append(file_name)
+
+        #             new_hfile_name = "_".join(hfile_name.split("_")[:-1])+"_"+str(hfile_size)
+        #             with open(config['falseAlarmRates']+"/hourly/"+new_hfile_name+'.pkl', 'wb') as output:
+        #                 pickle.dump(hfile, output, 4)
+
+        #             os.system("rm "+config['falseAlarmRates']+"/hourly/"+hfile_name)
+
+        #             for file_name in to_remove_from_inference_temp_files:
+        #                 inference_temp_files.remove(file_name)
+
+        #     # Now we can create new hourly files for the new groups that appeared
+        #     # First we reset the inference_temp_files. There will be no already existing froup
+        #     # for those files
+
+        #     # Reseting temp_file_groups 
+        #     inference_temp_files_groups = list(file.split("_")[0] for file in inference_temp_files)
+        #     inference_temp_files_groups = list(dict.fromkeys(inference_temp_files_groups))
+
+        #     # A check to make sure all files left do not belong in an existing group.
+        #     check = all( [ all([hgroup not in file for file in inference_temp_files]) for hgroup in hourly_files_groups] )
+        #     logger.debug(f"All groups left are new: {check}")
+
+
+        #     for tgroup in inference_temp_files_groups:
+
+        #         to_remove_from_inference_temp_files = []
+
+        #         for file_name in inference_temp_files:
+
+        #             if tgroup in file_name:
+
+        #                 if len(to_remove_from_inference_temp_files)==0:
+
+        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
+        #                         new_hfile = pickle.load(obj)
+
+        #                     new_hfile_size = int(file_name.split("_")[-1][:-4])
+
+        #                     to_remove_from_inference_temp_files.append(file_name)
+                        
+        #                 else:
+
+        #                     with open(config['falseAlarmRates']+"/"+file_name,'rb') as obj:
+        #                         file = pickle.load(obj)
+
+        #                     new_hfile = pd.concat([new_hfile, file], ignore_index=True)
+
+        #                     new_hfile_size += int(file_name.split("_")[-1][:-4])
+
+        #                     to_remove_from_inference_temp_files.append(file_name)
+
+        #         new_hfile_name = tgroup+"_"+str(new_hfile_size)
+        #         with open(config['falseAlarmRates']+"/hourly/"+new_hfile_name+'.pkl', 'wb') as output:
+        #             pickle.dump(new_hfile, output, 4)
+
+        #         logger.info(f"Informing / Saving FAR file : {config['falseAlarmRates']}/hourly/{new_hfile_name}.pkl")
+
+        #         for file_name in to_remove_from_inference_temp_files:
+        #             inference_temp_files.remove(file_name)
+
+        #             #TEMPORARY
+        #             os.system("rm "+config['falseAlarmRates']+"/"+file_name)
+
+        #     logger.debug(f"This should be zero, inference_temp_files: {len(inference_temp_files)}")
+
+
+        #     hourly_files = dirlist(config['falseAlarmRates']+"/hourly") 
+
+        #     for i, hfile_name in enumerate(hourly_files):
+
+        #         if i==0: 
+        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
+        #                 farfile = pickle.load(obj)
+
+        #             farfile_size = int(hfile_name.split("_")[-1][:-4])
+        #         else:
+                    
+        #             with open(config['falseAlarmRates']+"/hourly/"+hfile_name,'rb') as obj:
+        #                 farfile_part = pickle.load(obj)
+
+        #             farfile = pd.concat([farfile, farfile_part], ignore_index=True)
+
+        #             farfile_size += int(hfile_name.split("_")[-1][:-4])
+
+        #     # Deleting the old FARfile before creating the new one (they have the size of tests on their name).
+        #     farfile_to_delete = None
+        #     old_far_files = dirlist(config['falseAlarmRates']+"/FARfile")
+        #     for file in old_far_files:
+        #         if 'FARfile_interpolation' not in file:
+        #             farfile_to_delete = file
+        #             logger.info(f"FARfile to be replaced: {farfile_to_delete}")
+        #             break 
+
+        #     if len(hourly_files)!=0:
+        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_"+str(farfile_size)+".pkl", 'wb') as output:
+        #             pickle.dump(farfile, output, 4)
+
+        #             logger.info(f"New FARfile saved: {config['falseAlarmRates']}/FARfile/FARfile_{farfile_size}.pkl")
+
+        #         far_interpolation_output = far_interpolation(farfile, farfile_size, inverse = False)
+        #         far_interpolation_output_inverse = far_interpolation(farfile, farfile_size, inverse = True)
+
+        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation.pkl", 'wb') as output:
+        #             pickle.dump( far_interpolation_output , output, 4)
+        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_reserve.pkl", 'wb') as output:
+        #             pickle.dump( far_interpolation_output , output, 4)
+                    
+        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_inverse.pkl", 'wb') as output:
+        #             pickle.dump(far_interpolation_output_inverse , output, 4)
+        #         with open(config['falseAlarmRates']+"/FARfile/FARfile_interpolation_inverse_reserve.pkl", 'wb') as output:
+        #             pickle.dump(far_interpolation_output_inverse , output, 4)
                 
-            # Running the efficiencies script only if the previous has finished.
-            if len(dirlist(config['efficiencies'])) <= 2:
-                os.system("nohup python "+config["mlyPipelineSource"]+"/make_eff_estimation.py --mode condor > efficiencyTest.out &")
-                logger.info(f"Efficiency test initiated")
+        #         logger.info(f"New FARfile interpolations saced")
+
+        #         if (farfile_to_delete is not None 
+        #                 and farfile_to_delete!="FARfile_"+str(farfile_size)+".pkl"):
+        #             os.system("rm "+config['falseAlarmRates']+"/FARfile/"+farfile_to_delete)
+                
+        #     # Overwriting config farfile when enough files
+        #     if len(hourly_files)!=0 and (farfile_size) >= 1*365*24*3600 and (config['path']+"/"+config['falseAlarmRates'] not in config['farfile']):
+
+        #         with open('config.json') as json_file:
+        #             _config = json.load(json_file)
+        #             _config['farfile'] = config['falseAlarmRates']+"/FARfile"
+        #         with open("config.json", "w") as config_json:
+        #             json.dump(_config, config_json,indent=4)
+        #             config_json.close()
 
+        #         logger.info(f"FARFILE UPDATED FROM THE TEMPORARY TO THE SEARCH LOCAL!")
+        #         raise SystemError("This is just an interuption to load the new FAR sourse.")
+
+
+        # Timing
+        logger.info(f"Manager loop time:{time.time()-loopT0}, waiting 5 minutes ... ")
+        sys.stdout.flush()
+
+        time.sleep(5*60)
+        
 
-    logger.debug(f"PROCESSES before fartest management: {subprocess.check_output(['pgrep','-c', '-w','-u',config['user_name']]) }")
 
+
+
+def manage_FAR_inefernce_files(config = None):
+
+    if config is None:
+        with open('config.json') as json_file:
+            config = json.load(json_file)
     # # # FAR test management 
     #
 
     # The list of all temporary inference files
     if os.path.isdir(config['falseAlarmRates']):
+        if config['restriction']==None: 
+            config['restriction']=0.0
+        
+        restriction=float(config['restriction'])
         
         inference_temp_files = dirlist(config['falseAlarmRates'])
 
         for directory in ['hourly', 'condor', 'FARfile','temp']:
             if directory in inference_temp_files: inference_temp_files.remove(directory)
 
 
@@ -576,23 +788,16 @@
                 _config['farfile'] = config['falseAlarmRates']+"/FARfile"
             with open("config.json", "w") as config_json:
                 json.dump(_config, config_json,indent=4)
                 config_json.close()
 
             logger.info(f"FARFILE UPDATED FROM THE TEMPORARY TO THE SEARCH LOCAL!")
             raise SystemError("This is just an interuption to load the new FAR sourse.")
-        # # Deleting old condor directories 
-        # c = 0
-        # for cgroup, cdir in zip(condor_groups, condor_files):
-        #     if ((c < len(hourly_files_groups) - config['far_config']['parallelGenerations'])
-        #                 and (cgroup in hourly_files_groups)
-        #                 and (cgroup not in inference_temp_files_groups)):
 
-        #         os.system("rm -r "+config['falseAlarmRates']+"/condor/"+cdir)
-        #     c+=1
 
-    # Timing
-    logger.info(f"Manager loop time:{time.time()-loopT0}, waiting 5 minutes ... ")
-    sys.stdout.flush()
 
-    time.sleep(5*60)
+if __name__ == "__main__":
+        
+    main(config)
     
+
+
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.5.2/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline/offline_search.py` & `mly_pipeline-0.5.2/mly_pipeline/offline_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 import pickle
 import json
 from tensorflow.keras.models import load_model
 import pandas as pd
 
 import gwdatafind
 
-# Sourcing the submodule of mly in a very unpythonic way 
-sys.path.append("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
-
-
 from mly.datatools import DataPod
 from mly.validators import Validator
+from mly.createFileSystem import createFileSysem
 from mly.null_energy_map import *
 from .search_functions import *
 
 from mly.null_energy_map import *
 from ligo.skymap.io import fits
 
 import matplotlib.pyplot as plt
@@ -478,14 +475,32 @@
 
 
         print(config['output_directory']+file_name_prefix + ' saved')
         print("Size of file and interval ",frameSizeCheck, segment_size)
 
         print("Analysis complete ",str(1+i),"/",len(file_name_prefix))
 
+    elif kwargs['mode']=='set_file_system':
+
+        createFileSysem(duration=config['duration']
+                         ,fs=config['fs']
+                         ,detectors=detectors
+                         ,dates = segment_list
+                         ,windowSize = 16
+                         ,backgroundType='real'
+                         ,masterDirectory=config['masterDirectory']
+                         ,frames=config['frames_directory'] 
+                         ,channels=config['channels']
+                         ,accounting_group_user = config['accounting_group_user']
+                         ,accounting_group = config['accounting_group']
+        )
+
+
+
+
 if __name__ == "__main__":
 
     # # # Managing arguments
     # 
     # List of arguments to pass:
     arguments = ['mode','i']
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/search.py` & `mly_pipeline-0.5.2/mly_pipeline/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 import os, json, time
 
 # Scipy and numpy env parameters that limit the threads
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
 
-# with open('config.json') as json_file:
-#     config = json.load(json_file)
-
-# logging_level = config['logging_level']
-
-# # # # Initialising logging
-
-# create logger
-
 import logging
 from logging import handlers
 import subprocess
 
 
 logger = logging.getLogger("logger_for_search")
 logger.setLevel(logging.DEBUG)
@@ -34,67 +25,32 @@
 
 # add formatter to ch
 ch.setFormatter(formatter)
 
 # add ch to logger
 logger.addHandler(ch)
 
-logger.debug(f"PROCESSES after  logger: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris'])}")
-from ast import literal_eval as make_tuple
-time.sleep(1)
-logger.debug(f"PROCESSES after  ast: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-
-time.sleep(1)
-
-#from lal import gpstime
-logger.debug(f"PROCESSES after  llllllllal: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-time.sleep(1)
-
-from scipy import signal
-logger.debug(f"PROCESSES after  scipy.signal: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-time.sleep(1)
 
-from scipy.interpolate import interp1d
-logger.debug(f"PROCESSES after  scipy: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-time.sleep(1)
-
-from gwpy.time import to_gps, from_gps
-logger.debug(f"PROCESSES after  gwpy.time: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-time.sleep(1)
-
-from gwpy.timeseries import TimeSeries
-logger.debug(f"PROCESSES after  gwpy: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-time.sleep(1)
-
-
-from math import ceil
-from os import path
-import matplotlib.pyplot as plt
 import numpy as np
 import argparse
-import os
-import time
 import sys
 import pickle
-import json
 
-logger.debug(f"PROCESSES after  json: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
+from lal import gpstime
 
 from tensorflow.keras.models import load_model
 from tensorflow.config import threading
-logger.debug(f"PROCESSES after  tensorflow: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
 
 threading.set_inter_op_parallelism_threads(1)
 threading.set_intra_op_parallelism_threads(1)
 
-logger.debug(f"PROCESSES after  restricting threading: {subprocess.check_output(['pgrep','-c', '-w','-u','vasileios.skliris']) }")
-
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.null_energy_map import *
+
 from .search_functions import *
 
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/search_functions.py` & `mly_pipeline-0.5.2/mly_pipeline/search_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import json, pickle, sys, time, os, argparse
 
 import numpy             as np
 import matplotlib.pyplot as plt
 
 from os                import path
 from math              import ceil
-from gwpy.timeseries   import TimeSeries
+from gwpy.timeseries   import TimeSeries, StateVector, TimeSeriesDict
 from gwpy.segments     import SegmentList, Segment
 from gwpy.time         import to_gps, from_gps, tconvert
 from scipy.interpolate import interp1d
 from scipy             import signal
 from lal               import gpstime
 from dqsegdb2.query    import query_segments
 
 from ast               import literal_eval as make_tuple
 
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.plugins import *
 
+
+# Scipy and numpy env parameters that limit the threads
+os.environ["MKL_NUM_THREADS"] = "1"
+os.environ["NUMEXPR_NUM_THREADS"] = "1"
+os.environ["OMP_NUM_THREADS"] = "1"
+
 def checkDetectorArguments(config):
     
     """Injests command line arguments dictionary and outputs runtime config
         dictionary with error checked detector parameters.
         
        Parameters
        ----------
@@ -633,15 +639,15 @@
         config['prefix'] = prefix_name_list[0]
         return config
     else:
         raise ValueError("Prefix names are not consistent in frames")
 
 
     
-def readFrameFile(frames, channel, start_gps = None, end_gps = None, wait = 0.5, timeout = 10, count=0):
+def readFrameFile(frames, channel, state_vector_channel , start_gps = None, end_gps = None, wait = 0.5, timeout = 10, count=0):
     
     """A wrapper function for TimeSeries.read from gwpy. It reads the channels
     from the frames provided. If the reading fails for any reason it 
     waits <wait> time and tries again, up to <timeout> times.
     
     Parameters
     ----------
@@ -672,25 +678,43 @@
         If data are fetched sucessfully it returns a gwpy TimeSeries
         
     None: 
         If data are not fetched after <timeout> attemts
 
     """
 
+    channels = [channel, state_vector_channel]
+
     try:
-        data = TimeSeries.read(frames, channel, start = start_gps, end = end_gps)
-        return data
+        
+        try:
+            data = TimeSeriesDict.read(frames, channels, start = start_gps, end = end_gps)
+
+        except Exception as ex:
+
+            raise(ex)
+        
+        
+
+        state_vector_status = StateVector(data[state_vector_channel]).boolean[:,0:2].value.all()
+
+        if state_vector_status:
+            return data[channel]
+
+        else:
+            raise Exception(f"State vector is {state_vector_status}")
+
         
     except Exception as e:
 
         time.sleep(wait)
         count += 1;
         
         if count < timeout:
-            return readFrameFile(frames, channel, start_gps, end_gps 
+            return readFrameFile(frames, channel, state_vector_channel, start_gps, end_gps 
                                     , wait = wait, timeout=timeout, count = count)
             
         else:
             print(e)
             print("Could not find frames.")
             
         return None
@@ -1007,18 +1031,20 @@
 
         #Combine path to frame file with prefix variable for readability:
         prefix = config['frames_directory'][detector_initial] + detector_initial+"-"+detector_initial+"1_"+config['prefix']
 
         #Generate names of fram files to be read:
         frames = [f"{prefix}{gps_time + i}-1.gwf" for i in range(config["required_buffer"] + 1)]
 
+        
         #Search for frame files, return None if not found
         strain = readFrameFile(
             frames, 
             config["channels"][detector_initial],
+            config["state_vector_channels"][detector_initial],
             wait = config["wait"],
             timeout = int((config["num_scripts"]*1.5)/config["wait"]) # Using up to 1.5 times the time available in one loop of time. 
         )
 
         if strain != None:
             #Resample all strain data:
             strain = strain.resample(config["fs"]).value[int(config["fs"]*0.5):-int(config["fs"]*0.5)]
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.5.2/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.5.2/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.5.1/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.5.2/mly_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.5.1
+Version: 0.5.2
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.5.1/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.5.2/mly_pipeline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/runningasearch.rst
 docs/source/settingupasearch.rst
 mly_pipeline/__init__.py
 mly_pipeline/continuous_FAR.py
+mly_pipeline/continuous_FAR_test.py
 mly_pipeline/initialization.py
 mly_pipeline/make_eff_estimation.py
 mly_pipeline/manager.py
 mly_pipeline/mly_to_grace.py
 mly_pipeline/offline_search.py
 mly_pipeline/search.py
 mly_pipeline/search_functions.py
```

### Comparing `mly_pipeline-0.5.1/pyproject.toml` & `mly_pipeline-0.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
```

