# Comparing `tmp/energat-1.0.5.tar.gz` & `tmp/energat-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energat-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "energat-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `energat-1.0.5.tar` & `energat-1.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      345 2023-07-03 18:26:15.346384 energat-1.0.5/.github/pull_request_template.md
--rw-r--r--   0        0        0      543 2023-07-03 19:23:07.674738 energat-1.0.5/.github/workflows/test_basics.yaml
--rw-r--r--   0        0        0     1920 2023-07-01 18:23:31.475457 energat-1.0.5/.gitignore
--rw-r--r--   0        0        0       71 2023-07-01 20:01:33.302859 energat-1.0.5/.isort.cfg
--rw-r--r--   0        0        0      223 2023-07-01 20:02:11.370908 energat-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-07-01 19:08:55.042734 energat-1.0.5/.pypirc
--rw-r--r--   0        0        0     1053 2023-07-03 19:26:58.291023 energat-1.0.5/LICENSE
--rw-r--r--   0        0        0     6595 2023-07-03 21:55:47.073783 energat-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-18 21:31:14.236597 energat-1.0.5/bin/.gitkeep
--rwxr-xr-x   0        0        0 27608440 2023-06-18 21:31:14.416597 energat-1.0.5/bin/scaphandre
--rwxr-xr-x   0        0        0    31256 2023-06-18 21:31:14.416597 energat-1.0.5/bin/uarch_rapl
--rw-r--r--   0        0        0      510 2023-07-03 17:45:46.807280 energat-1.0.5/configs/default.py
--rw-r--r--   0        0        0        0 2023-06-18 21:31:14.416597 energat-1.0.5/data/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-18 21:31:14.416597 energat-1.0.5/data/results/.gitkeep
--rw-r--r--   0        0        0       99 2023-07-03 21:54:49.641713 energat-1.0.5/energat/__init__.py
--rw-r--r--   0        0        0     1349 2023-07-03 21:54:20.893679 energat-1.0.5/energat/__main__.py
--rw-r--r--   0        0        0      709 2023-07-01 19:40:10.701142 energat-1.0.5/energat/basepower.py
--rw-r--r--   0        0        0     5418 2023-07-03 18:43:17.815697 energat-1.0.5/energat/common.py
--rw-r--r--   0        0        0     1764 2023-07-01 19:46:06.941616 energat-1.0.5/energat/target.py
--rw-r--r--   0        0        0    34235 2023-07-03 18:32:23.106857 energat-1.0.5/energat/tracer.py
--rw-r--r--   0        0        0     1221 2023-07-03 21:43:32.436896 energat-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      188 2023-07-01 19:14:08.299151 energat-1.0.5/requirements.txt
--rw-r--r--   0        0        0      101 2023-07-01 19:32:17.696554 energat-1.0.5/requirements_dev.txt
--rw-r--r--   0        0        0     5435 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/cachestat
--rwxr-xr-x   0        0        0      214 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/check_versions.sh
--rwxr-xr-x   0        0        0      106 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/clear_cache.sh
--rw-r--r--   0        0        0    14980 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/energy/firefox_rapl.cpp
--rw-r--r--   0        0        0       71 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/energy/get_proc_numa_mem.sh
--rw-r--r--   0        0        0       48 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/energy/get_total_numa_mem.sh
--rw-r--r--   0        0        0    28996 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/energy/mozilla_rapl.cpp
--rw-r--r--   0        0        0    25905 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/energy/uarch_rapl.c
--rwxr-xr-x   0        0        0       29 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/gpustat.sh
--rw-r--r--   0        0        0     1028 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/jnb/jnb.cfg
--rwxr-xr-x   0        0        0    22365 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/jnb/start_jnb.sh
--rwxr-xr-x   0        0        0       45 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/scratch/refresh_all.sh
--rwxr-xr-x   0        0        0      139 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/scratch/to_newest_within.sh
--rwxr-xr-x   0        0        0     2011 2023-07-01 21:05:15.971999 energat-1.0.5/scripts/setup/init_cloudlab.sh
--rwxr-xr-x   0        0        0      392 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/setup/init_euler.sh
--rwxr-xr-x   0        0        0     1026 2023-07-01 21:05:08.863989 energat-1.0.5/scripts/setup/init_system.sh
--rwxr-xr-x   0        0        0      736 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/turbo_boost.sh
--rwxr-xr-x   0        0        0       75 2023-06-18 21:31:14.420597 energat-1.0.5/scripts/turnoff_smt.sh
--rw-r--r--   0        0        0       25 2023-07-01 19:40:10.657142 energat-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-01 19:40:10.673142 energat-1.0.5/tests/test_common.py
--rw-r--r--   0        0        0      543 2023-07-01 19:40:10.685142 energat-1.0.5/tests/test_tracer.py
--rw-r--r--   0        0        0     7585 1970-01-01 00:00:00.000000 energat-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      345 2023-07-03 18:26:15.346384 energat-1.0.6/.github/pull_request_template.md
+-rw-r--r--   0        0        0      543 2023-07-03 19:23:07.674738 energat-1.0.6/.github/workflows/test_basics.yaml
+-rw-r--r--   0        0        0     1920 2023-07-01 18:23:31.475457 energat-1.0.6/.gitignore
+-rw-r--r--   0        0        0       71 2023-07-01 20:01:33.302859 energat-1.0.6/.isort.cfg
+-rw-r--r--   0        0        0      223 2023-07-01 20:02:11.370908 energat-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-07-01 19:08:55.042734 energat-1.0.6/.pypirc
+-rw-r--r--   0        0        0     1053 2023-07-03 19:26:58.291023 energat-1.0.6/LICENSE
+-rw-r--r--   0        0        0     6595 2023-07-03 22:06:23.654559 energat-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 21:31:14.236597 energat-1.0.6/bin/.gitkeep
+-rwxr-xr-x   0        0        0 27608440 2023-06-18 21:31:14.416597 energat-1.0.6/bin/scaphandre
+-rwxr-xr-x   0        0        0    31256 2023-06-18 21:31:14.416597 energat-1.0.6/bin/uarch_rapl
+-rw-r--r--   0        0        0      510 2023-07-03 17:45:46.807280 energat-1.0.6/configs/default.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:31:14.416597 energat-1.0.6/data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-18 21:31:14.416597 energat-1.0.6/data/results/.gitkeep
+-rw-r--r--   0        0        0       99 2023-07-03 22:05:28.330492 energat-1.0.6/energat/__init__.py
+-rw-r--r--   0        0        0     1350 2023-07-03 22:00:27.722126 energat-1.0.6/energat/__main__.py
+-rw-r--r--   0        0        0      709 2023-07-01 19:40:10.701142 energat-1.0.6/energat/basepower.py
+-rw-r--r--   0        0        0     5418 2023-07-03 18:43:17.815697 energat-1.0.6/energat/common.py
+-rw-r--r--   0        0        0     1764 2023-07-01 19:46:06.941616 energat-1.0.6/energat/target.py
+-rw-r--r--   0        0        0    34235 2023-07-03 18:32:23.106857 energat-1.0.6/energat/tracer.py
+-rw-r--r--   0        0        0     1221 2023-07-03 21:43:32.436896 energat-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-07-01 19:14:08.299151 energat-1.0.6/requirements.txt
+-rw-r--r--   0        0        0      101 2023-07-01 19:32:17.696554 energat-1.0.6/requirements_dev.txt
+-rw-r--r--   0        0        0     5435 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/cachestat
+-rwxr-xr-x   0        0        0      214 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/check_versions.sh
+-rwxr-xr-x   0        0        0      106 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/clear_cache.sh
+-rw-r--r--   0        0        0    14980 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/energy/firefox_rapl.cpp
+-rw-r--r--   0        0        0       71 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/energy/get_proc_numa_mem.sh
+-rw-r--r--   0        0        0       48 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/energy/get_total_numa_mem.sh
+-rw-r--r--   0        0        0    28996 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/energy/mozilla_rapl.cpp
+-rw-r--r--   0        0        0    25905 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/energy/uarch_rapl.c
+-rwxr-xr-x   0        0        0       29 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/gpustat.sh
+-rw-r--r--   0        0        0     1028 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/jnb/jnb.cfg
+-rwxr-xr-x   0        0        0    22365 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/jnb/start_jnb.sh
+-rwxr-xr-x   0        0        0       45 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/scratch/refresh_all.sh
+-rwxr-xr-x   0        0        0      139 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/scratch/to_newest_within.sh
+-rwxr-xr-x   0        0        0     2011 2023-07-01 21:05:15.971999 energat-1.0.6/scripts/setup/init_cloudlab.sh
+-rwxr-xr-x   0        0        0      392 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/setup/init_euler.sh
+-rwxr-xr-x   0        0        0     1026 2023-07-01 21:05:08.863989 energat-1.0.6/scripts/setup/init_system.sh
+-rwxr-xr-x   0        0        0      736 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/turbo_boost.sh
+-rwxr-xr-x   0        0        0       75 2023-06-18 21:31:14.420597 energat-1.0.6/scripts/turnoff_smt.sh
+-rw-r--r--   0        0        0       25 2023-07-01 19:40:10.657142 energat-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-01 19:40:10.673142 energat-1.0.6/tests/test_common.py
+-rw-r--r--   0        0        0      543 2023-07-01 19:40:10.685142 energat-1.0.6/tests/test_tracer.py
+-rw-r--r--   0        0        0     7585 1970-01-01 00:00:00.000000 energat-1.0.6/PKG-INFO
```

### Comparing `energat-1.0.5/.github/workflows/test_basics.yaml` & `energat-1.0.6/.github/workflows/test_basics.yaml`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/.gitignore` & `energat-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/LICENSE` & `energat-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/README.md` & `energat-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # EnergAt 🔋🎯
 
-![version](https://img.shields.io/badge/version-1.0.5-blue) 
+![version](https://img.shields.io/badge/version-1.0.6-blue) 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/hongyuhe/energat/graphs/commit-activity) 
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) 
 [![build](https://github.com/HongyuHe/energat/actions/workflows/test_basics.yaml/badge.svg)](https://github.com/HongyuHe/energat/actions/workflows/test_basics.yaml)
 [![PyPI version](https://badge.fury.io/py/energat.svg)](https://badge.fury.io/py/energat)
 
 EnergAt is a prototype implementation of the thread-level, NUMA-aware energy attribution model for multi-tenancy, as proposed in our [paper](https://hongyu.nl/papers/2023_hotcarbon_energat.pdf). It offers precise tracking of the energy consumption of your software application, even when it is running alongside other jobs from different users.
```

### Comparing `energat-1.0.5/bin/scaphandre` & `energat-1.0.6/bin/scaphandre`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/bin/uarch_rapl` & `energat-1.0.6/bin/uarch_rapl`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/energat/__main__.py` & `energat-1.0.6/energat/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             )
         except:
             logger.error("System check failed!")
             return 1
         logger.info("System check passed!")
         return 0
 
-    if FLAGS.basefile:
+    if FLAGS.basepower:
         EnergyTracer(pid).estimate_baseline_power(save=True)
         return 0
 
     name = FLAGS.name if FLAGS.name else f"target-{FLAGS.pid}"
     if FLAGS.pid > 0:
         tracer = EnergyTracer(FLAGS.pid, attach=True, project=name)
         try:
```

### Comparing `energat-1.0.5/energat/basepower.py` & `energat-1.0.6/energat/basepower.py`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/energat/common.py` & `energat-1.0.6/energat/common.py`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/energat/target.py` & `energat-1.0.6/energat/target.py`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/energat/tracer.py` & `energat-1.0.6/energat/tracer.py`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/pyproject.toml` & `energat-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/cachestat` & `energat-1.0.6/scripts/cachestat`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/energy/firefox_rapl.cpp` & `energat-1.0.6/scripts/energy/firefox_rapl.cpp`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/energy/mozilla_rapl.cpp` & `energat-1.0.6/scripts/energy/mozilla_rapl.cpp`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/energy/uarch_rapl.c` & `energat-1.0.6/scripts/energy/uarch_rapl.c`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/jnb/jnb.cfg` & `energat-1.0.6/scripts/jnb/jnb.cfg`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/jnb/start_jnb.sh` & `energat-1.0.6/scripts/jnb/start_jnb.sh`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/setup/init_cloudlab.sh` & `energat-1.0.6/scripts/setup/init_cloudlab.sh`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/setup/init_system.sh` & `energat-1.0.6/scripts/setup/init_system.sh`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/scripts/turbo_boost.sh` & `energat-1.0.6/scripts/turbo_boost.sh`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/tests/test_tracer.py` & `energat-1.0.6/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `energat-1.0.5/PKG-INFO` & `energat-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energat
-Version: 1.0.5
+Version: 1.0.6
 Summary: EnergAt: A software energy attribution tool.
 Author-email: Hongyu Hè <honghe@inf.ethz.ch>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Power (UPS)
@@ -26,15 +26,15 @@
 Requires-Dist: flake8 ; extra == "test"
 Project-URL: Paper, https://hongyu.nl/papers/2023_hotcarbon_energat.pdf
 Project-URL: Source, https://github.com/HongyuHe/energat
 Provides-Extra: test
 
 # EnergAt 🔋🎯
 
-![version](https://img.shields.io/badge/version-1.0.5-blue) 
+![version](https://img.shields.io/badge/version-1.0.6-blue) 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/hongyuhe/energat/graphs/commit-activity) 
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) 
 [![build](https://github.com/HongyuHe/energat/actions/workflows/test_basics.yaml/badge.svg)](https://github.com/HongyuHe/energat/actions/workflows/test_basics.yaml)
 [![PyPI version](https://badge.fury.io/py/energat.svg)](https://badge.fury.io/py/energat)
 
 EnergAt is a prototype implementation of the thread-level, NUMA-aware energy attribution model for multi-tenancy, as proposed in our [paper](https://hongyu.nl/papers/2023_hotcarbon_energat.pdf). It offers precise tracking of the energy consumption of your software application, even when it is running alongside other jobs from different users.
```

