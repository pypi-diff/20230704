# Comparing `tmp/labcrawler-1.0.4.tar.gz` & `tmp/labcrawler-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-1.0.4.tar", last modified: Wed May  3 14:49:58 2023, max compression
+gzip compressed data, was "labcrawler-1.0.6.tar", last modified: Tue Jul  4 04:27:39 2023, max compression
```

## Comparing `labcrawler-1.0.4.tar` & `labcrawler-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.519645 labcrawler-1.0.4/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.4/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.4/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)    14373 2023-05-03 14:49:58.518974 labcrawler-1.0.4/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    14091 2023-05-03 14:49:29.000000 labcrawler-1.0.4/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.492976 labcrawler-1.0.4/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.4/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3710 2023-05-03 14:49:24.000000 labcrawler-1.0.4/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5582 2023-05-03 14:49:29.000000 labcrawler-1.0.4/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.4/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-05-03 14:49:24.000000 labcrawler-1.0.4/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.4/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.516083 labcrawler-1.0.4/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.4/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.505751 labcrawler-1.0.4/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    14373 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       80 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-05-03 14:49:58.000000 labcrawler-1.0.4/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      714 2023-05-01 22:16:55.000000 labcrawler-1.0.4/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-05-03 14:49:58.519785 labcrawler-1.0.4/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-03 14:49:58.517933 labcrawler-1.0.4/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.4/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-05-03 14:49:43.000000 labcrawler-1.0.4/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-04 04:26:51.000000 labcrawler-1.0.6/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-04 04:27:30.000000 labcrawler-1.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-04 04:27:30.000000 labcrawler-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15062 2023-07-04 04:27:39.232059 labcrawler-1.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14780 2023-07-04 04:27:30.000000 labcrawler-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.229059 labcrawler-1.0.6/labcrawler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/_legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.231059 labcrawler-1.0.6/labcrawler/analyzers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/analyzers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/analyzers/gitlab_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6271 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.231059 labcrawler-1.0.6/labcrawler/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/gitlab_ci_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/gitlab_repository_files_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab/project_data_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/gitlab_ci_data_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/labcrawler/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/labcrawler.json.template
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-07-04 04:27:30.000000 labcrawler-1.0.6/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.230059 labcrawler-1.0.6/labcrawler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15062 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-04 04:27:39.000000 labcrawler-1.0.6/labcrawler.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-04 04:27:30.000000 labcrawler-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 04:27:39.232059 labcrawler-1.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 04:27:39.232059 labcrawler-1.0.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-04 04:27:30.000000 labcrawler-1.0.6/test/test_gitlab_ci_config.py
```

### Comparing `labcrawler-1.0.4/LICENSE` & `labcrawler-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.4/PKG-INFO` & `labcrawler-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-Metadata-Version: 2.1
-Name: labcrawler
-Version: 1.0.4
-Summary: Analysis tool for GitLab project and CI configurations
-Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 Summary
 -------
 
+*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
+
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
 Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
@@ -268,7 +260,38 @@
 
 [tap-gitlab on GitHub](https://github.com/MeltanoLabs/tap-gitlab)
 
 [GitLab API docs](https://docs.gitlab.com/ee/api/)
 
 [Pandas DataFrame reference](https://pandas.pydata.org/docs/reference/frame.html)
 
+
+Development
+-----------
+
+1. Make sure you have Python 3.8+ and Pip installed
+2. Make a GitLab account and give it your SSH public key
+3. Follow the steps below (YMMV, from memory, please update if I missed anything)
+
+```
+git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+cd labcrawler
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -r requirements/freeze.txt
+```
+
+Then to run it:
+
+```
+python -m labcrawler init
+```
+
+... and the other commands
+
+Thoughts on adding `tap-github`:
+
+- Add it to `meltano.yml`
+- Set up required env vars in `labcrawler.json`
+- Re-run `init`
+
+
```

### Comparing `labcrawler-1.0.4/README.md` & `labcrawler-1.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+Metadata-Version: 2.1
+Name: labcrawler
+Version: 1.0.6
+Summary: Analysis tool for GitLab project and CI configurations
+Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 Summary
 -------
 
+*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
+
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
 Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
@@ -258,7 +270,38 @@
 
 [tap-gitlab on GitHub](https://github.com/MeltanoLabs/tap-gitlab)
 
 [GitLab API docs](https://docs.gitlab.com/ee/api/)
 
 [Pandas DataFrame reference](https://pandas.pydata.org/docs/reference/frame.html)
 
+
+Development
+-----------
+
+1. Make sure you have Python 3.8+ and Pip installed
+2. Make a GitLab account and give it your SSH public key
+3. Follow the steps below (YMMV, from memory, please update if I missed anything)
+
+```
+git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+cd labcrawler
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -r requirements/freeze.txt
+```
+
+Then to run it:
+
+```
+python -m labcrawler init
+```
+
+... and the other commands
+
+Thoughts on adding `tap-github`:
+
+- Add it to `meltano.yml`
+- Set up required env vars in `labcrawler.json`
+- Re-run `init`
+
+
```

### Comparing `labcrawler-1.0.4/labcrawler/_legacy.py` & `labcrawler-1.0.6/labcrawler/_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from os import environ
 from dataclasses import dataclass
 import logging
 import sys
 from argparse import ArgumentParser
 from pprint import pp
 
-from labcrawler.gitlab_ci_config import GitLabCIConfig
-from labcrawler.gitlab_repository_files_extractor import GitLabRepositoryFilesExtractor
-from labcrawler.project_data_file import ProjectDataFile
+from labcrawler.gitlab.gitlab_ci_config import GitLabCIConfig
+from labcrawler.gitlab.gitlab_repository_files_extractor import GitLabRepositoryFilesExtractor
+from labcrawler.gitlab.project_data_file import ProjectDataFile
 
 if __name__ == '__main__':
 
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     handler = logging.StreamHandler(sys.stdout)
     handler.setLevel(logging.INFO)
```

### Comparing `labcrawler-1.0.4/labcrawler/analysis.py` & `labcrawler-1.0.6/labcrawler/analyzers/gitlab_analyzer.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,79 +3,77 @@
 from sys import argv
 from inspect import get_annotations
 
 from pandas import DataFrame
 from pandas import read_csv
 from tabulate import tabulate
 
-@dataclass
-class DataSet:
-    access_levels:DataFrame = None
-    groups:DataFrame = None
-    projects:DataFrame = None
-    branches:DataFrame = None
-    merge_requests:DataFrame = None
-    project_members:DataFrame = None
-    group_members:DataFrame = None
-    users:DataFrame = None
-    ci_config_committers:DataFrame = None
-    ci_config_paths:DataFrame = None
-
-def datatypes():
-    annotations = get_annotations(DataSet)
-    return  [n for n in annotations if annotations[n] == DataFrame]
+from labcrawler.analyzers import Abstract
 
-DATATYPES = datatypes()
 
-class RawDataSet(DataSet):
+class GitLabAnalyzer:
+    
+    source = 'gitlab'
+
+    datatypes = [
+        'access_levels',
+        'groups',
+        'projects',
+        'branches',
+        'merge_requests',
+        'project_members',
+        'group_members',
+        'users',
+        'ci_config_committers',
+        'ci_config_paths']
 
-    def __init__(self, output_path_str:str):
+    def load_raw_from_csv(self, output_path_str:str):
         output_path = Path(output_path_str).expanduser()
-        for datatype in DATATYPES:
+        self.raw = Abstract()
+        for datatype in self.datatypes:
             path = output_path / f'{datatype}.csv'
             if path.exists():
                 with open(path) as dtfile:
                     dtframe = read_csv(dtfile)
-                    setattr(self, datatype, dtframe)
-
-class AssembledDataSet(DataSet):
+                    setattr(self.raw, datatype, dtframe)
 
-    def __init__(self, raw:RawDataSet):
+    def __init__(self, output_path_str:str):
+        self.load_raw_from_csv(output_path_str)
         self.access_levels = \
                 DataFrame(data = [[0,'No access'], [5,'Minimal access'],
                 [10, 'Guest'], [20, 'Reporter'], [30, 'Developer'], [40, 'Maintainer'],
                 [50, 'Owner']], columns = ['id', 'name']).set_index('id')
-        if isinstance(raw.groups, DataFrame):
-                self.groups = raw.groups.set_index('id')
-        if isinstance(raw.projects, DataFrame):
-                self.projects = raw.projects.set_index('id')
-        if isinstance(raw.users, DataFrame):
-                self.users = raw.users.set_index('id')
-        if isinstance(raw.branches, DataFrame):
-                self.branches = raw.branches.set_index('project_id').\
+        if hasattr(self.raw, 'groups'):
+                self.groups = self.raw.groups.set_index('id')
+        if hasattr(self.raw, 'projects'):
+                self.projects = self.raw.projects.set_index('id')
+        if hasattr(self.raw, 'users'):
+                self.users = self.raw.users.set_index('id')
+        if hasattr(self.raw, 'branches'):
+                self.branches = self.raw.branches.set_index('project_id').\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'))
-        if isinstance(raw.merge_requests, DataFrame):
-                self.merge_requests = raw.merge_requests.set_index('project_id').\
+        if hasattr(self.raw, 'merge_requests'):
+                self.merge_requests = self.raw.merge_requests.set_index('project_id').\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'))
-        if isinstance(raw.project_members, DataFrame):
-                self.project_members = raw.project_members.\
+        if hasattr(self.raw, 'project_members'):
+                self.project_members = self.raw.project_members.\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id').\
                         join(self.users[['username']].add_prefix('user_'), on='user_id').\
                         join(self.access_levels[['name']].add_prefix('access_level_'), on='access_level')
-        if isinstance(raw.group_members, DataFrame):
-                self.group_members = raw.group_members.\
+        if hasattr(self.raw, 'group_members'):
+                self.group_members = self.raw.group_members.\
                         join(self.groups[['path']].add_prefix('group_'), on='group_id').\
                         join(self.access_levels[['name']].add_prefix('access_level_'), on='access_level')
-        if isinstance(raw.ci_config_committers, DataFrame):
-                self.ci_config_committers = raw.ci_config_committers.\
+        if hasattr(self.raw, 'ci_config_committers'):
+                self.ci_config_committers = self.raw.ci_config_committers.\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id' )
-        if isinstance(raw.ci_config_paths, DataFrame):
-                self.ci_config_paths = raw.ci_config_paths.\
+        if hasattr(self.raw, 'ci_config_paths'):
+                self.ci_config_paths = self.raw.ci_config_paths.\
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id', how='right')
         
-        for datatype in DATATYPES:
-            df = getattr(self, datatype)
-            if df is not None:
+        for datatype in self.datatypes:
+            if hasattr(self, datatype):
+                df = getattr(self, datatype)
                 df.index.name = 'id'
 
 def output_neat(dataframe):
         print(tabulate(dataframe, showindex=False, headers=dataframe.columns))
```

### Comparing `labcrawler-1.0.4/labcrawler/cli.py` & `labcrawler-1.0.6/labcrawler/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,56 +14,62 @@
 import sys
 import os
 
 from platformdirs import user_data_dir
 from platformdirs import user_documents_dir
 import pandas
 
-from labcrawler.analysis import RawDataSet
-from labcrawler.analysis import AssembledDataSet
-from labcrawler.analysis import DATATYPES
+from labcrawler.analyzers.gitlab_analyzer import GitLabAnalyzer
 from labcrawler.gitlab_ci_data_loader import GitLabCIDataLoader
-from labcrawler.analysis import output_neat
+from labcrawler.analyzers.gitlab_analyzer import output_neat
 
 APPNAME = "LabCrawler"
 APPAUTHOR = "SteampunkWizard"
 
+SOURCES = ['gitlab']
+
+class Simple:
+    pass
+
 class LabCrawlerCLI:
 
     def __init__(self):
         self.set_logging()
         parser = ArgumentParser()
-        parser.add_argument('command', choices=['init','melt','load','analyze'])
+        parser.add_argument('--workspace')
+        commands = parser.add_subparsers(dest='command')
+        for command in ['melt','load','analyze']:
+            commands.add_parser(command)
+        initparser = commands.add_parser('init')
+        initparser.add_argument('--output')
         namespace = parser.parse_args(argv[1:])
-        getattr(self, namespace.command)()
+        if namespace.workspace:
+            self.workspace = Path(namespace.workspace).expanduser()
+        else:
+            self.workspace = Path(user_data_dir(APPNAME, APPAUTHOR))
+        getattr(self, namespace.command)(namespace)
 
     @staticmethod
     def set_logging():
         logger = logging.getLogger()
         logger.setLevel(logging.INFO)
         handler = logging.StreamHandler(sys.stdout)
         handler.setLevel(logging.INFO)
         formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
     @property
-    def workspace(self):
-        if not hasattr(self, '_workspace'):
-            self._workspace = Path(user_data_dir(APPNAME, APPAUTHOR))
-        return self._workspace
-
-    @property
     def config_path(self):
         return self.workspace / 'labcrawler.json'
 
-    def init(self):
+    def init(self, namespace):
         self.clear_dir("the LabCrawler workspace", self.workspace)
         self.init_meltano()
-        self.init_config()
+        self.init_config(namespace.output)
         self.init_plugins()
         print(f"Remember to edit the config file at\n  {self.config_path}")
 
     @staticmethod
     def clear_dir(prompt:str, dir:Path):
         if dir.exists():
             if dir.is_dir():
@@ -80,21 +86,23 @@
         dir.mkdir(parents=True)
 
     def init_meltano(self):
         print(f"Initializing Meltano... ")
         run(['meltano','init',str(self.workspace)])
         print(f"Initialized Meltano.")
 
-    def init_config(self):
-        # Is this going to work after pipx install?
+    def init_config(self, output):
         templates = Path(__file__).parent / 'templates'
         copy(templates / 'meltano.yml', self.workspace / 'meltano.yml')
         with open(templates / 'labcrawler.json.template') as config_template_file:
             config_template = config_template_file.read()
-        output_dir = Path(user_documents_dir()) / APPNAME
+        if output:
+            output_dir = Path(output).expanduser().absolute()
+        else:
+            output_dir = Path(user_documents_dir()) / APPNAME
         with open(self.config_path, 'w') as config_file:
             config_file.write(config_template.format(output_dir=output_dir))
 
     def init_plugins(self):
         chdir(self.workspace)
         print("Installing Meltano plugins...")
         run(['meltano','install'])
@@ -113,45 +121,53 @@
         if not 'GITLAB_PRIVATE_TOKEN' in environ:         
             secret = getpass("GitLab Private Token: ").strip()
             if len(secret) != 26:
                 raise RuntimeError("GitLab Private Token must contain 26 characters")
             environ['GITLAB_PRIVATE_TOKEN'] = secret
 
 
-    def melt(self):
+    def melt(self, namespace):
         """Load all the data via meltano"""
         if not self.workspace.exists():
             raise RuntimeError("Use the init command first")
         output_dir = self.config['output_dir']
         self.clear_dir("previous output", Path(output_dir))
-        self.grab_token()
-        environ['OUTPUT_DIR'] = output_dir
-        environ['GITLAB_API_URL'] = self.config['api_url']
-        environ['GITLAB_GROUPS'] = ' '.join(self.config['groups'])
         chdir(self.workspace)
-        run(['meltano','run','tap-gitlab','target-csv'])
+        for source in SOURCES:
+            csv_dir = Path(output_dir) / source
+            csv_dir.mkdir()
+            self.grab_token()
+            environ['OUTPUT_DIR'] = str(csv_dir)
+            environ['GITLAB_API_URL'] = self.config['api_url']
+            environ['GITLAB_GROUPS'] = ' '.join(self.config['groups'])
+            run(['meltano','run','tap-gitlab','target-csv'])
         print(f"Output is in {output_dir}")
 
-    def load(self):
+    def load(self, namespace):
         """Load CI includes (and later blames), not covered by meltano"""
         # Cheap and easy cli argument: give me PROJECT_ID to limit scope
         self.grab_token()
         if 'PROJECT_ID' in os.environ:
             loader = GitLabCIDataLoader(self.config, \
                     project_id=os.environ['PROJECT_ID'])
         else:
             loader = GitLabCIDataLoader(self.config)
         loader.load_files()
         loader.load_blames()
 
-    def analyze(self):
-        raw = RawDataSet(self.config['output_dir'])
-        assembled = AssembledDataSet(raw)
-        values = vars(assembled)
-        banner = "Available: raw, neat, pandas\n"
-        banner += "\n".join([f"{len(values[t].index)} {t}" for t in values])
-        banner = f"LabCrawler analysis\n{banner}\nPython {python_version()}"
-        values['raw'] = raw
+    def analyze(self, namespace):
+        banner = "Globals: pandas, neat\n\n"
+        values = {}
         values['neat'] = output_neat
         values['pandas'] = pandas
+        for source in SOURCES:
+            csv_dir = Path(self.config['output_dir']) / source
+            analyzer = GitLabAnalyzer(csv_dir)
+            banner += f"{source}\n"
+            for datatype in analyzer.datatypes:
+                if hasattr(analyzer, datatype):
+                    banner += f"{len(getattr(analyzer, datatype).index):>8} {datatype}\n"
+            banner += "         raw\n"
+            values[source] = analyzer
+        banner = f"\nLabCrawler analysis\n{banner}\nPython {python_version()}  ctrl-d to quit"
         pandas.set_option('display.max_rows', None)
-        interact(local=values, banner=banner)
+        interact(local=values, banner=banner)
```

### Comparing `labcrawler-1.0.4/labcrawler/gitlab_ci_config.py` & `labcrawler-1.0.6/labcrawler/gitlab/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.4/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.6/labcrawler/gitlab_ci_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from os import environ
 from pathlib import Path
 from csv import DictWriter
 import logging
 
-from labcrawler.project_data_file import ProjectDataFile
-from labcrawler.gitlab_repository_files_extractor import \
+from labcrawler.gitlab.project_data_file import ProjectDataFile
+from labcrawler.gitlab.gitlab_repository_files_extractor import \
         GitLabRepositoryFilesExtractor
-from labcrawler.gitlab_ci_config import GitLabCIConfig
+from labcrawler.gitlab.gitlab_ci_config import GitLabCIConfig
 
 
 class GitLabCIDataLoader:
     """Load includes (and later blames) from GitLab CI configs"""
 
     def __init__(self, config:GitLabCIConfig, project_id:int=None):
         self.config = config
@@ -54,14 +54,14 @@
                     branch = project_data['default_branch'], \
                     repo_path = project_data['ci_config_path'] or '.gitlab-ci.yml' )
             committers.extend(project_committers)
         self.write_csv(committers, 'ci_config_committers', \
                 ['project_id','committer_name','committer_email'])
 
     def write_csv(self, rows:list, filename:str, fieldnames:list):
-        path = Path(self.config['output_dir']) / (filename + '.csv')
+        path = Path(self.config['output_dir']) / 'gitlab' / (filename + '.csv')
         with open(path, 'w') as outfile:
             writer = DictWriter(outfile, fieldnames)
             writer.writeheader()
             for row in rows:
                 writer.writerow(row)
             logging.info(f"Wrote {len(rows)} rows to {str(path.absolute())}")
```

### Comparing `labcrawler-1.0.4/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-1.0.6/labcrawler/gitlab/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.4/labcrawler/templates/meltano.yml` & `labcrawler-1.0.6/labcrawler/templates/meltano.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 version: 1
-default_environment: dev
 project_id: 1bef1be2-7cb3-48ef-a68e-0866820daeb7
+default_environment: main
 environments:
-- name: dev
-  config:
-    plugins:
-      extractors:
-      - name: tap-gitlab
-        config:
-          api_url: $GITLAB_API_URL
-          private_token: $GITLAB_PRIVATE_TOKEN
-          groups: $GITLAB_GROUPS
-          ultimate_license: true
-          start_date: '2000-01-01T00:00:00Z'
-        select:
-        - groups.*
-        - projects.*
-        - branches.*
-        - merge_requests.*
-        - pipelines.*
-        - project_members.*
-        - group_members.*
-        - users.*
-- name: staging
-- name: prod
+  - name: main
 plugins:
   extractors:
   - name: tap-gitlab
     variant: meltanolabs
-    pip_url: git+https://github.com/francispotter/tap-gitlab.git
+    pip_url: git+https://github.com/MeltanoLabs/tap-gitlab.git
+    config:
+      api_url: $GITLAB_API_URL
+      private_token: $GITLAB_PRIVATE_TOKEN
+      groups: $GITLAB_GROUPS
+      ultimate_license: true
+      start_date: '2000-01-01T00:00:00Z'
+    select:
+    - groups.*
+    - projects.*
+    - branches.*
+    - merge_requests.*
+    - pipelines.*
+    - project_members.*
+    - group_members.*
+    - users.*
   loaders:
   - name: target-csv
     variant: meltanolabs
     pip_url: git+https://github.com/MeltanoLabs/target-csv.git
     config:
       output_path_prefix: $OUTPUT_DIR/
       file_naming_scheme: '{stream_name}.csv'
```

### Comparing `labcrawler-1.0.4/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.6/labcrawler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.4
+Version: 1.0.6
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Summary
 -------
 
+*NOTE: README not yet updated for the new source approach (i.e. 'gitlab' has its own namespace)*
+
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
 
 Labcrawler will ultimately assume the use of the GitLab "ultimate" paid tier, as it will look for configuration settings such as merge request approvals, which are only available at that level.
 
 Remember, in GitLab, a "group" is like a portfolio or folder containing projects and subgroups. Currently, Labcrawler doesn't actually "crawl" - it only surveys projects that live directly in the designated groups.
@@ -268,7 +270,38 @@
 
 [tap-gitlab on GitHub](https://github.com/MeltanoLabs/tap-gitlab)
 
 [GitLab API docs](https://docs.gitlab.com/ee/api/)
 
 [Pandas DataFrame reference](https://pandas.pydata.org/docs/reference/frame.html)
 
+
+Development
+-----------
+
+1. Make sure you have Python 3.8+ and Pip installed
+2. Make a GitLab account and give it your SSH public key
+3. Follow the steps below (YMMV, from memory, please update if I missed anything)
+
+```
+git clone git@gitlab.com:steampunk-wizard/labcrawler.git
+cd labcrawler
+python3 -m venv .venv
+source .venv/bin/activate
+pip install -r requirements/freeze.txt
+```
+
+Then to run it:
+
+```
+python -m labcrawler init
+```
+
+... and the other commands
+
+Thoughts on adding `tap-github`:
+
+- Add it to `meltano.yml`
+- Set up required env vars in `labcrawler.json`
+- Re-run `init`
+
+
```

### Comparing `labcrawler-1.0.4/pyproject.toml` & `labcrawler-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 labcrawler = "labcrawler"
 
 [project.scripts]
 labcrawler = "labcrawler.cli:LabCrawlerCLI"
 meltano = "meltano.cli:main"
 
 [tool.setuptools.dynamic]
-version = {file = ["version"]}
+version = {file = [".version"]}
```

### Comparing `labcrawler-1.0.4/test/test_gitlab_ci_config.py` & `labcrawler-1.0.6/test/test_gitlab_ci_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from labcrawler.gitlab_ci_config import GitLabCIConfig
+from labcrawler.gitlab.gitlab_ci_config import GitLabCIConfig
 
 
 class TestGitLabCIConfig(TestCase):
 
     def test_nothing(self):
         self.assertEqual(3,3)
```

