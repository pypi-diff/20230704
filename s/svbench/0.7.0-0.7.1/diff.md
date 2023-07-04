# Comparing `tmp/svbench-0.7.0.tar.gz` & `tmp/svbench-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svbench-0.7.0.tar", last modified: Fri May 26 13:39:58 2023, max compression
+gzip compressed data, was "svbench-0.7.1.tar", last modified: Tue Jul  4 13:57:27 2023, max compression
```

## Comparing `svbench-0.7.0.tar` & `svbench-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.912095 svbench-0.7.0/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.0/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.0/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-05-26 13:39:58.911707 svbench-0.7.0/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.0/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-05-26 13:39:58.912196 svbench-0.7.0/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-05-26 11:53:14.000000 svbench-0.7.0/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.898792 svbench-0.7.0/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.0/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.0/svbench/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     1158 2023-05-26 13:39:20.000000 svbench-0.7.0/svbench/cli.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    69040 2023-05-26 12:20:45.000000 svbench-0.7.0/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.0/svbench/loaders.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.911378 svbench-0.7.0/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.0/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.0/svbench/quant_tools.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.910923 svbench-0.7.0/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/entry_points.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/top_level.txt
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.998912 svbench-0.7.1/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.1/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.1/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-04 13:57:26.998572 svbench-0.7.1/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.1/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-07-04 13:57:26.999004 svbench-0.7.1/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-07-04 13:52:52.000000 svbench-0.7.1/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.986272 svbench-0.7.1/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.1/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.1/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1158 2023-05-26 13:39:20.000000 svbench-0.7.1/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    69121 2023-07-04 13:56:22.000000 svbench-0.7.1/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.1/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.998266 svbench-0.7.1/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.1/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.1/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-07-04 13:57:26.997865 svbench-0.7.1/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-07-04 13:57:26.000000 svbench-0.7.1/svbench.egg-info/top_level.txt
```

### Comparing `svbench-0.7.0/LICENSE.md` & `svbench-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `svbench-0.7.0/README.rst` & `svbench-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `svbench-0.7.0/svbench/.DS_Store` & `svbench-0.7.1/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.7.0/svbench/cli.py` & `svbench-0.7.1/svbench/cli.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.0/svbench/io_tools.py` & `svbench-0.7.1/svbench/io_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1770,20 +1770,21 @@
         for idx in range(len(s_ranges) - 1):
             size_brackets.append("[{}, {})".format(s_ranges[idx], s_ranges[idx + 1]))
 
         size_brackets.append("All ranges")
         s = np.append(s, [s.sum()])
         s2, _ = np.histogram(ref_bedpe["svlen"], ref_size_bins)
         s2 = np.append(s2, [s2.sum()])
-        sens = s / s2
 
-        s_fp, _ = np.histogram([i for i, j in zip(dat["svlen"], dat["TP"]) if i == i and not j], ref_size_bins)
-        s_fp = np.append(s_fp, [s_fp.sum()])
-        prec = s / (s + s_fp)
-        f1 = 2 * ((prec * sens) / (prec + sens))
+        with np.errstate(divide='ignore', invalid='ignore'):
+            sens = s / s2
+            s_fp, _ = np.histogram([i for i, j in zip(dat["svlen"], dat["TP"]) if i == i and not j], ref_size_bins)
+            s_fp = np.append(s_fp, [s_fp.sum()])
+            prec = s / (s + s_fp)
+            f1 = 2 * ((prec * sens) / (prec + sens))
 
         # Duplicated are currently filtered before this step
         # s_dtp, _ = np.histogram([i for i, j in zip(dat["svlen"], dat["DTP"]) if i == i and j], ref_size_bins)
         # s_dtp = np.append(s_dtp, [s_dtp.sum()])
 
         s_fn, _ = np.histogram([ref_data.breaks_df["svlen"].loc[i] for i in missing_ref_indexes], ref_size_bins)
         s_fn = np.append(s_fn, [s_fn.sum()])
```

### Comparing `svbench-0.7.0/svbench/loaders.py` & `svbench-0.7.1/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.7.0/svbench/quant_tools.py` & `svbench-0.7.1/svbench/quant_tools.py`

 * *Files identical despite different names*

