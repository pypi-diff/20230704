# Comparing `tmp/kuki-0.2.0.tar.gz` & `tmp/kuki-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.2.0.tar", last modified: Tue Jun 27 13:17:13 2023, max compression
+gzip compressed data, was "kuki-0.3.0.tar", last modified: Tue Jul  4 16:06:49 2023, max compression
```

## Comparing `kuki-0.2.0.tar` & `kuki-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/
--rw-r--r--   0 jshinonome  (1000) users      (100)    11357 2023-06-15 05:01:08.000000 kuki-0.2.0/LICENSE
--rw-r--r--   0 jshinonome  (1000) users      (100)    12993 2023-06-27 13:17:13.765620 kuki-0.2.0/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) users      (100)     1412 2023-06-27 13:15:32.000000 kuki-0.2.0/README.md
-drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki/
--rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     1176 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     4844 2023-06-27 08:58:19.000000 kuki-0.2.0/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     3088 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/krun.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     3371 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     3313 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/package_util.py
--rw-r--r--   0 jshinonome  (1000) users      (100)      279 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/profile_util.py
-drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki/q/
--rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 12:26:24.000000 kuki-0.2.0/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     3262 2023-06-27 13:09:13.000000 kuki-0.2.0/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) users      (100)     6359 2023-06-27 11:09:55.000000 kuki-0.2.0/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/q/krun.q
--rw-r--r--   0 jshinonome  (1000) users      (100)     1958 2023-06-27 10:44:52.000000 kuki-0.2.0/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) users      (100)     2177 2023-06-20 14:00:10.000000 kuki-0.2.0/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) users      (100)      878 2023-06-27 09:49:09.000000 kuki-0.2.0/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) users      (100)    13261 2023-06-15 05:01:08.000000 kuki-0.2.0/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     2141 2023-06-27 11:04:34.000000 kuki-0.2.0/kuki/util.py
--rw-r--r--   0 jshinonome  (1000) users      (100)       22 2023-06-27 13:10:22.000000 kuki-0.2.0/kuki/version.py
-drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) users      (100)    12993 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) users      (100)      573 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) users      (100)        1 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) users      (100)       84 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) users      (100)        1 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) users      (100)       17 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) users      (100)       10 2023-06-27 13:17:13.000000 kuki-0.2.0/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) users      (100)      486 2023-06-27 13:17:13.765620 kuki-0.2.0/setup.cfg
--rw-r--r--   0 jshinonome  (1000) users      (100)      315 2023-06-15 11:42:17.000000 kuki-0.2.0/setup.py
-drwxr-xr-x   0 jshinonome  (1000) users      (100)        0 2023-06-27 13:17:13.765620 kuki-0.2.0/test/
--rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) users      (100)        0 2023-06-15 05:01:08.000000 kuki-0.2.0/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) users      (100)     1605 2023-06-15 12:34:54.000000 kuki-0.2.0/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) users      (100)    14435 2023-06-15 05:01:08.000000 kuki-0.2.0/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.3.0/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13802 2023-07-04 16:06:49.922429 kuki-0.3.0/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2221 2023-07-03 15:40:17.000000 kuki-0.3.0/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.920429 kuki-0.3.0/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.3.0/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.3.0/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1563 2023-07-04 15:42:52.000000 kuki-0.3.0/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1521 2023-07-04 15:42:58.000000 kuki-0.3.0/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3371 2023-06-09 16:35:49.000000 kuki-0.3.0/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3313 2023-05-13 05:48:24.000000 kuki-0.3.0/kuki/package_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      279 2023-06-09 16:35:43.000000 kuki-0.3.0/kuki/profile_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.3.0/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     6406 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      175 2023-07-04 15:27:24.000000 kuki-0.3.0/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1853 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2177 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      878 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13261 2023-06-09 16:35:40.000000 kuki-0.3.0/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3619 2023-07-04 15:58:02.000000 kuki-0.3.0/kuki/util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-07-04 16:05:26.000000 kuki-0.3.0/kuki/version.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.921429 kuki-0.3.0/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13802 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      573 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      486 2023-07-04 16:06:49.922429 kuki-0.3.0/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.3.0/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.3.0/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.3.0/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1399 2023-07-03 12:47:22.000000 kuki-0.3.0/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14435 2023-05-20 06:46:07.000000 kuki-0.3.0/test/test_kuki.py
```

### Comparing `kuki-0.2.0/LICENSE` & `kuki-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/PKG-INFO` & `kuki-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.2.0
+Version: 0.3.0
 Summary: kdb+/q package manager
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: kdb,q
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -75,31 +75,60 @@
 
 ### Command: kest
 
 K tEST CLI
 
 #### Define Test
 
-- `.kest.Test`
+- `.kest.Test[description;function]`
 
 #### Setup and Teardown
 
-- `.kest.BeforeAll`
-- `.kest.AfterAll`
-- `.kest.BeforeEach`
-- `.kest.AfterEach`
+- `.kest.BeforeAll function`
+- `.kest.AfterAll function`
+- `.kest.BeforeEach function`
+- `.kest.AfterEach function`
 
 #### Using Matchers
 
-- `.kest.ToThrow`
-- `.kest.Match`
-- `.kest.MatchTable`
-- `.kest.MatchDict`
+- `.kest.ToThrow[functionCall;errorMsg]`
+- `.kest.Match[expect;actual]`
+- `.kest.MatchTable[expect;actual]`
+- `.kest.MatchDict[expect;actual]`
 
-### Command: krun
+### Command: ktrl
+
+K conTRoL CLI
+
+#### Init ktrl Profile
+
+`ktrl -init [-global|mongodb] profile_name`
+
+locations for profiles
+
+- mongodb: stored in MongoDB
+- global: `$HOME/kuki/_profile`
+- local: `$PWD/profile`
+
+#### Start Process Using ktrl Profile
+
+`ktrl -profile [-global|mongodb] profile_name`
+
+- with `-mongodb`, ktrl will use profiles in MongoDB
+- with `-global`, ktrl will use profiles in global profile directory
+- without `-global|mongodb`, ktrl will use profiles as following priorities:
+  - local directory
+  - global profile directory
+  - MongoDB
+
+#### Config ktrl
+
+`ktrl -config`
+
+Config ktrl includes MongoDB connection details, configuration file path `$HOME/kuki/_config/ktrlrc.json`
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.2.0/kuki/config_util.py` & `kuki-0.3.0/kuki/config_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki/kuki.py` & `kuki-0.3.0/kuki/kuki.py`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki/package_util.py` & `kuki-0.3.0/kuki/package_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki/q/kest.q` & `kuki-0.3.0/kuki/q/kest.q`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
   if[not .cli.args`debug;
     exit not all exec `passed=status from .kest.testResults;
   ];
  };
 
 / -debug option
 .cli.Boolean[`debug;0b;"debug mode"];
+.cli.Boolean[`init;0b;"initialize kest.json"];
 .cli.Symbol[`testRoot;`:test;"directory that kest use to search for test files in"];
 .cli.Symbol[`testOutputFile;`;"write test results to a file"];
 .cli.String[`testPattern;"*";"run only tests with a name that matches the pattern"];
 .cli.Symbol[`testFile;`;"run specific test file"];
 .cli.SetName["K tEST CLI"];
 .cli.Parse[];
```

### Comparing `kuki-0.2.0/kuki/q/kuki.q` & `kuki-0.3.0/kuki/q/kuki.q`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,8 @@
   $[module like "./*"; .kuki.importLocal[path;module];.kuki.importGlobal[module]]
  };
 
 import {"./log"};
 import {"./cli"};
 import {"./path"};
 
-.cli.Selection[`kScriptType;`krun`kest;"kuki script type"];
-
-.cli.Parse[];
-
-import {"./",string .cli.args`kScriptType};
-
-.cli.AppendIgnores`kScriptType;
+import {"./",first .Q.opt[.z.x][`kScriptType]};
```

### Comparing `kuki-0.2.0/kuki/q/log.q` & `kuki-0.3.0/kuki/q/log.q`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki/q/path.q` & `kuki-0.3.0/kuki/q/path.q`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki/registry_util.py` & `kuki-0.3.0/kuki/registry_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.2.0/kuki.egg-info/PKG-INFO` & `kuki-0.3.0/kuki.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.2.0
+Version: 0.3.0
 Summary: kdb+/q package manager
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: kdb,q
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -75,31 +75,60 @@
 
 ### Command: kest
 
 K tEST CLI
 
 #### Define Test
 
-- `.kest.Test`
+- `.kest.Test[description;function]`
 
 #### Setup and Teardown
 
-- `.kest.BeforeAll`
-- `.kest.AfterAll`
-- `.kest.BeforeEach`
-- `.kest.AfterEach`
+- `.kest.BeforeAll function`
+- `.kest.AfterAll function`
+- `.kest.BeforeEach function`
+- `.kest.AfterEach function`
 
 #### Using Matchers
 
-- `.kest.ToThrow`
-- `.kest.Match`
-- `.kest.MatchTable`
-- `.kest.MatchDict`
+- `.kest.ToThrow[functionCall;errorMsg]`
+- `.kest.Match[expect;actual]`
+- `.kest.MatchTable[expect;actual]`
+- `.kest.MatchDict[expect;actual]`
 
-### Command: krun
+### Command: ktrl
+
+K conTRoL CLI
+
+#### Init ktrl Profile
+
+`ktrl -init [-global|mongodb] profile_name`
+
+locations for profiles
+
+- mongodb: stored in MongoDB
+- global: `$HOME/kuki/_profile`
+- local: `$PWD/profile`
+
+#### Start Process Using ktrl Profile
+
+`ktrl -profile [-global|mongodb] profile_name`
+
+- with `-mongodb`, ktrl will use profiles in MongoDB
+- with `-global`, ktrl will use profiles in global profile directory
+- without `-global|mongodb`, ktrl will use profiles as following priorities:
+  - local directory
+  - global profile directory
+  - MongoDB
+
+#### Config ktrl
+
+`ktrl -config`
+
+Config ktrl includes MongoDB connection details, configuration file path `$HOME/kuki/_config/ktrlrc.json`
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.2.0/kuki.egg-info/SOURCES.txt` & `kuki-0.3.0/kuki.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 kuki/__init__.py
 kuki/config_util.py
 kuki/kest.py
-kuki/krun.py
+kuki/ktrl.py
 kuki/kuki.py
 kuki/package_util.py
 kuki/profile_util.py
 kuki/registry_util.py
 kuki/util.py
 kuki/version.py
 kuki.egg-info/PKG-INFO
@@ -18,15 +18,15 @@
 kuki.egg-info/entry_points.txt
 kuki.egg-info/not-zip-safe
 kuki.egg-info/requires.txt
 kuki.egg-info/top_level.txt
 kuki/q/__init__.py
 kuki/q/cli.q
 kuki/q/kest.q
-kuki/q/krun.q
+kuki/q/ktrl.q
 kuki/q/kuki.q
 kuki/q/log.q
 kuki/q/path.q
 test/__init__.py
 test/conftest.py
 test/test_kest.py
 test/test_kuki.py
```

### Comparing `kuki-0.2.0/test/test_kuki.py` & `kuki-0.3.0/test/test_kuki.py`

 * *Files identical despite different names*

