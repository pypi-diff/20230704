# Comparing `tmp/search-me-2.1.tar.gz` & `tmp/search-me-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\search-me-2.1.tar", last modified: Fri Dec 10 20:31:01 2021, max compression
+gzip compressed data, was "search-me-3.0.0.tar", last modified: Tue Jul  4 15:39:55 2023, max compression
```

## Comparing `search-me-2.1.tar` & `search-me-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxrwxrwx   0        0        0        0 2021-12-10 20:31:01.841615 search-me-2.1/
--rw-rw-rw-   0        0        0     7202 2021-12-10 20:31:01.841615 search-me-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4643 2021-12-10 20:30:18.000000 search-me-2.1/README.md
-drwxrwxrwx   0        0        0        0 2021-12-10 20:31:01.831615 search-me-2.1/search_me/
--rw-rw-rw-   0        0        0      205 2021-12-08 21:18:30.000000 search-me-2.1/search_me/__init__.py
--rw-rw-rw-   0        0        0    37819 2021-12-10 20:15:20.000000 search-me-2.1/search_me/api.py
--rw-rw-rw-   0        0        0      738 2021-12-10 19:56:58.000000 search-me-2.1/search_me/tests.py
-drwxrwxrwx   0        0        0        0 2021-12-10 20:31:01.841615 search-me-2.1/search_me.egg-info/
--rw-rw-rw-   0        0        0     7202 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      414 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-12-10 20:31:01.000000 search-me-2.1/search_me.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-10 20:31:01.841615 search-me-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1079 2021-09-24 12:47:44.000000 search-me-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.921924 search-me-3.0.0/
+-rw-rw-rw-   0        0        0     1096 2023-07-04 15:26:23.000000 search-me-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4485 2023-07-04 15:39:55.923925 search-me-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2795 2023-07-04 15:37:06.000000 search-me-3.0.0/README.md
+-rw-rw-rw-   0        0        0     2087 2023-07-04 15:26:23.000000 search-me-3.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.854920 search-me-3.0.0/search_me/
+drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.917924 search-me-3.0.0/search_me/.engines/
+-rw-rw-rw-   0        0        0     1892 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.domains
+-rw-rw-rw-   0        0        0      248 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.formats
+-rw-rw-rw-   0        0        0     1188 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.languages
+-rw-rw-rw-   0        0        0      312 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.params
+-rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.pass
+-rw-rw-rw-   0        0        0      332 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.regex
+-rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.salt
+-rw-rw-rw-   0        0        0      554 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/__init__.py
+-rw-rw-rw-   0        0        0     4198 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/balancers.py
+-rw-rw-rw-   0        0        0    12426 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/engines.py
+-rw-rw-rw-   0        0        0     1932 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/exceptions.py
+-rw-rw-rw-   0        0        0      389 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/models.py
+-rw-rw-rw-   0        0        0     4846 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/storage.py
+-rw-rw-rw-   0        0        0     2510 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.884922 search-me-3.0.0/search_me.egg-info/
+-rw-rw-rw-   0        0        0     4485 2023-07-04 15:39:54.000000 search-me-3.0.0/search_me.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 15:39:54.000000 search-me-3.0.0/search_me.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2895 2023-07-04 15:39:55.927925 search-me-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-04 15:26:23.000000 search-me-3.0.0/setup.py
```

