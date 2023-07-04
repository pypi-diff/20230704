# Comparing `tmp/git-pr-linear-merge-1.1.0.tar.gz` & `tmp/git-pr-linear-merge-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-pr-linear-merge-1.1.0.tar", last modified: Mon Jun 13 00:40:26 2022, max compression
+gzip compressed data, was "git-pr-linear-merge-1.1.1.tar", last modified: Tue Jul  4 18:07:56 2023, max compression
```

## Comparing `git-pr-linear-merge-1.1.0.tar` & `git-pr-linear-merge-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 waldo      (501) staff       (20)        0 2022-06-13 00:40:26.709311 git-pr-linear-merge-1.1.0/
--rw-r--r--   0 waldo      (501) staff       (20)     1072 2021-04-15 00:56:23.000000 git-pr-linear-merge-1.1.0/LICENSE
--rw-r--r--   0 waldo      (501) staff       (20)     5486 2022-06-13 00:40:26.709384 git-pr-linear-merge-1.1.0/PKG-INFO
--rw-r--r--   0 waldo      (501) staff       (20)     4552 2022-06-13 00:39:04.000000 git-pr-linear-merge-1.1.0/README.md
--rw-r--r--   0 waldo      (501) staff       (20)      103 2021-04-23 16:08:01.000000 git-pr-linear-merge-1.1.0/pyproject.toml
--rw-r--r--   0 waldo      (501) staff       (20)     1234 2022-06-13 00:40:26.709693 git-pr-linear-merge-1.1.0/setup.cfg
-drwxr-xr-x   0 waldo      (501) staff       (20)        0 2022-06-13 00:40:26.707427 git-pr-linear-merge-1.1.0/src/
-drwxr-xr-x   0 waldo      (501) staff       (20)        0 2022-06-13 00:40:26.708548 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/
--rw-r--r--   0 waldo      (501) staff       (20)        0 2021-08-21 17:30:56.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/__init__.py
--rw-r--r--   0 waldo      (501) staff       (20)     2165 2021-04-23 16:08:01.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/auth.py
--rw-r--r--   0 waldo      (501) staff       (20)      965 2021-08-23 15:06:02.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/cfg.py
--rw-r--r--   0 waldo      (501) staff       (20)     1035 2021-05-01 03:27:36.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/logger.py
--rw-r--r--   0 waldo      (501) staff       (20)    18039 2022-06-13 00:18:54.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/main.py
-drwxr-xr-x   0 waldo      (501) staff       (20)        0 2022-06-13 00:40:26.709220 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/
--rw-r--r--   0 waldo      (501) staff       (20)     5486 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/PKG-INFO
--rw-r--r--   0 waldo      (501) staff       (20)      491 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/SOURCES.txt
--rw-r--r--   0 waldo      (501) staff       (20)        1 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/dependency_links.txt
--rw-r--r--   0 waldo      (501) staff       (20)       56 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/entry_points.txt
--rw-r--r--   0 waldo      (501) staff       (20)       84 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/requires.txt
--rw-r--r--   0 waldo      (501) staff       (20)       20 2022-06-13 00:40:26.000000 git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/top_level.txt
+drwxr-xr-x   0 waldo      (501) staff       (20)        0 2023-07-04 18:07:56.995665 git-pr-linear-merge-1.1.1/
+-rw-r--r--   0 waldo      (501) staff       (20)     1072 2021-04-15 00:56:23.000000 git-pr-linear-merge-1.1.1/LICENSE
+-rw-r--r--   0 waldo      (501) staff       (20)     5486 2023-07-04 18:07:56.995728 git-pr-linear-merge-1.1.1/PKG-INFO
+-rw-r--r--   0 waldo      (501) staff       (20)     4552 2022-06-13 00:39:04.000000 git-pr-linear-merge-1.1.1/README.md
+-rw-r--r--   0 waldo      (501) staff       (20)      103 2021-04-23 16:08:01.000000 git-pr-linear-merge-1.1.1/pyproject.toml
+-rw-r--r--   0 waldo      (501) staff       (20)     1234 2023-07-04 18:07:56.996004 git-pr-linear-merge-1.1.1/setup.cfg
+drwxr-xr-x   0 waldo      (501) staff       (20)        0 2023-07-04 18:07:56.993159 git-pr-linear-merge-1.1.1/src/
+drwxr-xr-x   0 waldo      (501) staff       (20)        0 2023-07-04 18:07:56.994679 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/
+-rw-r--r--   0 waldo      (501) staff       (20)        0 2021-08-21 17:30:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/__init__.py
+-rw-r--r--   0 waldo      (501) staff       (20)     2165 2021-04-23 16:08:01.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/auth.py
+-rw-r--r--   0 waldo      (501) staff       (20)      965 2021-08-23 15:06:02.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/cfg.py
+-rw-r--r--   0 waldo      (501) staff       (20)     1035 2021-05-01 03:27:36.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/logger.py
+-rw-r--r--   0 waldo      (501) staff       (20)    18039 2022-06-13 00:18:54.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/main.py
+drwxr-xr-x   0 waldo      (501) staff       (20)        0 2023-07-04 18:07:56.995580 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/
+-rw-r--r--   0 waldo      (501) staff       (20)     5486 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/PKG-INFO
+-rw-r--r--   0 waldo      (501) staff       (20)      491 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/SOURCES.txt
+-rw-r--r--   0 waldo      (501) staff       (20)        1 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/dependency_links.txt
+-rw-r--r--   0 waldo      (501) staff       (20)       56 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/entry_points.txt
+-rw-r--r--   0 waldo      (501) staff       (20)       84 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/requires.txt
+-rw-r--r--   0 waldo      (501) staff       (20)       20 2023-07-04 18:07:56.000000 git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/top_level.txt
```

### Comparing `git-pr-linear-merge-1.1.0/LICENSE` & `git-pr-linear-merge-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/PKG-INFO` & `git-pr-linear-merge-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pr-linear-merge
-Version: 1.1.0
+Version: 1.1.1
 Summary: A command line utility to list and merge GitHub pull requests while maintaining linear history
 Home-page: https://github.com/waldobronchart/git-pr-linear-merge
 Author: Waldo Bronchart
 Author-email: wbronchart@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/waldobronchart/git-pr-linear-merge
 Project-URL: Bug Tracker, https://github.com/waldobronchart/git-pr-linear-merge/issues
```

### Comparing `git-pr-linear-merge-1.1.0/README.md` & `git-pr-linear-merge-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/setup.cfg` & `git-pr-linear-merge-1.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git-pr-linear-merge
-version = 1.1.0
+version = 1.1.1
 author = Waldo Bronchart
 author_email = wbronchart@gmail.com
 description = A command line utility to list and merge GitHub pull requests while maintaining linear history
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/waldobronchart/git-pr-linear-merge
 project_urls = 
@@ -23,18 +23,18 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	GitPython==3.1.14
+	GitPython==3.1.30
 	PyGithub==1.54.1
 	tabulate==0.8.9
-	requests==2.25.1
+	requests==2.31.0
 	colorama==0.4.4
 
 [options.entry_points]
 console_scripts = 
 	git-pr=git_pr_linear_merge.main:run
 
 [options.packages.find]
```

### Comparing `git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/auth.py` & `git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/auth.py`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/cfg.py` & `git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/cfg.py`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/logger.py` & `git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/logger.py`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/src/git_pr_linear_merge/main.py` & `git-pr-linear-merge-1.1.1/src/git_pr_linear_merge/main.py`

 * *Files identical despite different names*

### Comparing `git-pr-linear-merge-1.1.0/src/git_pr_linear_merge.egg-info/PKG-INFO` & `git-pr-linear-merge-1.1.1/src/git_pr_linear_merge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pr-linear-merge
-Version: 1.1.0
+Version: 1.1.1
 Summary: A command line utility to list and merge GitHub pull requests while maintaining linear history
 Home-page: https://github.com/waldobronchart/git-pr-linear-merge
 Author: Waldo Bronchart
 Author-email: wbronchart@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/waldobronchart/git-pr-linear-merge
 Project-URL: Bug Tracker, https://github.com/waldobronchart/git-pr-linear-merge/issues
```

