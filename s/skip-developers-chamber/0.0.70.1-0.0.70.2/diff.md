# Comparing `tmp/skip-developers-chamber-0.0.70.1.tar.gz` & `tmp/skip-developers-chamber-0.0.70.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-developers-chamber-0.0.70.1.tar", last modified: Thu Jun 29 12:01:41 2023, max compression
+gzip compressed data, was "skip-developers-chamber-0.0.70.2.tar", last modified: Tue Jul  4 13:39:21 2023, max compression
```

## Comparing `skip-developers-chamber-0.0.70.1.tar` & `skip-developers-chamber-0.0.70.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.681050 skip-developers-chamber-0.0.70.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 12:01:41.681050 skip-developers-chamber-0.0.70.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.677049 skip-developers-chamber-0.0.70.1/developers_chamber/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.677049 skip-developers-chamber-0.0.70.1/developers_chamber/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/bin/pydev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.677049 skip-developers-chamber-0.0.70.1/developers_chamber/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/click/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/ecs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/gitlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/jira_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/project_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.677049 skip-developers-chamber-0.0.70.1/developers_chamber/qa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/qa/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/qa/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.677049 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/init_aliasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/sh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/scripts/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/toggle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/developers_chamber/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:01:41.681050 skip-developers-chamber-0.0.70.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 12:01:30.000000 skip-developers-chamber-0.0.70.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:01:41.681050 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 12:01:41.000000 skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bin/pydev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/click/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25338 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/ecs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/gitlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/jira_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/project_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.798667 skip-developers-chamber-0.0.70.2/developers_chamber/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/qa/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/init_aliasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/scripts/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/toggle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/developers_chamber/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-04 13:39:10.000000 skip-developers-chamber-0.0.70.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:39:21.802667 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 13:39:21.000000 skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/top_level.txt
```

### Comparing `skip-developers-chamber-0.0.70.1/LICENSE` & `skip-developers-chamber-0.0.70.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/README.md` & `skip-developers-chamber-0.0.70.2/README.md`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/bin/pydev.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/bitbucket_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/click/options.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/ecs_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/git_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/git_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/gitlab_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/jira_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/jira_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/project_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/project_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/qa/base.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/qa/base.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/qa/checks.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/qa/checks.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/bitbucket.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/docker.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/ecs.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/ecs.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/git.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/git.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/gitlab.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/gitlab.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/init_aliasses.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/init_aliasses.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/jira.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/jira.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/project.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/project.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/qa.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/qa.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/slack.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/slack.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/toggle.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/toggle.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/scripts/version.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/slack_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/slack_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/toggle_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/toggle_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/types.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/types.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/developers_chamber/version_utils.py` & `skip-developers-chamber-0.0.70.2/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-0.0.70.1/setup.py` & `skip-developers-chamber-0.0.70.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from setuptools import find_packages, setup
 
 setup(
     name='skip-developers-chamber',
-    version='0.0.70.1',
+    version='0.0.70.2',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/developers-chamber',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
-        'oauthlib==3.1.0',
-        'gitpython==3.1.30',
-        'click==7.0',
-        'requests>=2.23.0',
-        'python-dotenv==0.14.0',
         'boto3<2',
-        'python-hosts==0.4.6',
-        'isort==5.12.0',
-        'coloredlogs==10.0',
+        'click>=7.0',
         'click-completion==0.5.2',
+        'coloredlogs==10.0',
+        'flake8>=4.0.1',
+        'gitpython==3.1.30',
+        'isort>=5.12.0',
         'jira==2.0.0',
-        'unidecode==1.1.1',
-        'TogglPy==0.1.2',
-        'flake8==4.0.1',
+        'oauthlib==3.1.0',
+        'pip-tools==6.13.0',
+        'python-dotenv==0.14.0',
+        'python-hosts==0.4.6',
+        'requests>=2.23.0',
         'slack-sdk==3.21.3',
+        'TogglPy==0.1.2',
+        'unidecode==1.1.1',
     ],
     entry_points={'console_scripts': [
         'pydev=developers_chamber.bin.pydev:cli',
     ]},
     zip_safe=False,
 )
```

### Comparing `skip-developers-chamber-0.0.70.1/skip_developers_chamber.egg-info/SOURCES.txt` & `skip-developers-chamber-0.0.70.2/skip_developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

