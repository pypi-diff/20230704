# Comparing `tmp/merge_segments-0.6.0.tar.gz` & `tmp/merge_segments-0.6.1.tar.gz`

## Comparing `merge_segments-0.6.0.tar` & `merge_segments-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,22 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 merge_segments-0.6.0/icon/.gitignore
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 merge_segments-0.6.0/icon/icon.svg
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme_extras/old_merge_macro_docs/readme.md
--rw-r--r--   0        0        0    31610 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme_extras/old_merge_macro_docs/sample data illustration.svg
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme_extras/old_merge_macro_docs/test_data_file.csv
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme_extras/old_merge_macro_docs/test_locations_file.csv
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme_extras/old_merge_macro_docs/test_result_file.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 merge_segments-0.6.0/src/merge_segments/__init__.py
--rw-r--r--   0        0        0    19214 2020-02-02 00:00:00.000000 merge_segments-0.6.0/src/merge_segments/merge.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_Sum.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_doc_example.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_graceful_missing_mismatched_columns.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_graceful_overlapping_columns_error.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_keep_longest_value.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_merge_on_one_key.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_min_max_argmin_argmax.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_proportional_sum.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_wrong_argument_type.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/test_zero_length.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests/testing.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests_manual/generate_test_charts.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 merge_segments-0.6.0/tests_manual/test_plots/.gitignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 merge_segments-0.6.0/.gitignore
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 merge_segments-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 merge_segments-0.6.0/readme.md
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 merge_segments-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 merge_segments-0.6.1/icon/.gitignore
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 merge_segments-0.6.1/icon/icon.svg
+-rw-r--r--   0        0        0    31610 2020-02-02 00:00:00.000000 merge_segments-0.6.1/readme_extras/old_merge_macro_docs/sample data illustration.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 merge_segments-0.6.1/src/merge_segments/__init__.py
+-rw-r--r--   0        0        0    19214 2020-02-02 00:00:00.000000 merge_segments-0.6.1/src/merge_segments/merge.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_Sum.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_doc_example.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_graceful_missing_mismatched_columns.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_graceful_overlapping_columns_error.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_keep_longest_value.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_merge_on_one_key.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_min_max_argmin_argmax.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_proportional_sum.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_wrong_argument_type.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/test_zero_length.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests/testing.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests_manual/generate_test_charts.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 merge_segments-0.6.1/tests_manual/test_plots/.gitignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 merge_segments-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 merge_segments-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    20890 2020-02-02 00:00:00.000000 merge_segments-0.6.1/readme.md
+-rw-r--r--   0        0        0    21102 2020-02-02 00:00:00.000000 merge_segments-0.6.1/PKG-INFO
```

### Comparing `merge_segments-0.6.0/icon/icon.svg` & `merge_segments-0.6.1/icon/icon.svg`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/readme_extras/old_merge_macro_docs/sample data illustration.svg` & `merge_segments-0.6.1/readme_extras/old_merge_macro_docs/sample data illustration.svg`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/src/merge_segments/merge.py` & `merge_segments-0.6.1/src/merge_segments/merge.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_Sum.py` & `merge_segments-0.6.1/tests/test_Sum.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_doc_example.py` & `merge_segments-0.6.1/tests/test_doc_example.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_graceful_missing_mismatched_columns.py` & `merge_segments-0.6.1/tests/test_graceful_missing_mismatched_columns.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_graceful_overlapping_columns_error.py` & `merge_segments-0.6.1/tests/test_graceful_overlapping_columns_error.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_keep_longest_value.py` & `merge_segments-0.6.1/tests/test_keep_longest_value.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_merge_on_one_key.py` & `merge_segments-0.6.1/tests/test_merge_on_one_key.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_min_max_argmin_argmax.py` & `merge_segments-0.6.1/tests/test_min_max_argmin_argmax.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_proportional_sum.py` & `merge_segments-0.6.1/tests/test_proportional_sum.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_wrong_argument_type.py` & `merge_segments-0.6.1/tests/test_wrong_argument_type.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/test_zero_length.py` & `merge_segments-0.6.1/tests/test_zero_length.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests/testing.py` & `merge_segments-0.6.1/tests/testing.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/tests_manual/generate_test_charts.py` & `merge_segments-0.6.1/tests_manual/generate_test_charts.py`

 * *Files identical despite different names*

### Comparing `merge_segments-0.6.0/pyproject.toml` & `merge_segments-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "merge_segments"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   {name="Nicholas Archer"},
 ]
 description = "A tool for merging data onto a road network segmentation"
 readme = "readme.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `merge_segments-0.6.0/readme.md` & `merge_segments-0.6.1/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 # `merge_segments`<!-- omit in toc -->
 
 [![Publish to PyPi](https://github.com/thehappycheese/merge-segments/actions/workflows/publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/thehappycheese/merge-segments/actions/workflows/publish_to_pypi.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/merge_segments.svg)](https://pypi.org/project/wideprint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/merge_segments.svg)](https://pypi.org/project/wideprint)
 
 - [1. Introduction](#1-introduction)
-  - [1.1. Dependencies](#11-dependencies)
 - [2. Install, Upgrade, Uninstall](#2-install-upgrade-uninstall)
 - [3. Module `merge`](#3-module-merge)
   - [3.1. Function `merge.on_slk_intervals()`](#31-function-mergeon_slk_intervals)
   - [3.2. Class `merge.Action`](#32-class-mergeaction)
   - [3.3. Class `merge.Aggregation`](#33-class-mergeaggregation)
-    - [3.3.1. Notes about `Aggregation.KeepLongest()`](#331-notes-about-aggregationkeeplongest)
+    - [3.3.1. Notes about `KeepLongest()`](#331-notes-about-keeplongest)
+    - [3.3.2. Notes about `LengthWeightedPercentile(...)`](#332-notes-about-lengthweightedpercentile)
   - [3.4. Practical Example of Merge](#34-practical-example-of-merge)
 - [4. Notes](#4-notes)
   - [4.1. Correctness, Robustness, Test Coverage and Performance](#41-correctness-robustness-test-coverage-and-performance)
 
 ## 1. Introduction
 
 `merge_segments` is a python package which reproduces an old excell process.
 
 The purpose is to combine two data tables which have a linear segment index ("from" and "to" columns); ie where each row in the input tables represents some linear portion of an entity; for example a road segment from 5km to 10km.
 
 There is an ongoing effort to accelerate and parallelise the merge function
 under a new repo called
 [megamerge](https://github.com/thehappycheese/megamerge)
 
-### 1.1. Dependencies
-
-This package depends on Pandas (tested with version 1.3.1) and is most likely to
-work as expected in Python 3.9+.
-
 ## 2. Install, Upgrade, Uninstall
 
 To install:
 
 ```powershell
-pip install "https://github.com/thehappycheese/merge-segments/zipball/main/"
+pip install merge_segments
 ```
 
 To Upgrade:
 
 ```powershell
-pip install --upgrade "https://github.com/thehappycheese/merge-segments/zipball/main"
+pip install --upgrade merge_segments
 ```
 
 To show installed version:
 
 ```powershell
 pip show merge_segments
 ```
@@ -151,27 +146,27 @@
 ### 3.3. Class `merge.Aggregation`
 
 The following merge aggregations are supported:
 
 | Constructor                                                   | Purpose                                                                                                                                                                                                                          |
 | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `merge.Aggregation.First()`                                   | Keep the first non-blank value.                                                                                                                                                                                                  |
-| `merge.Aggregation.KeepLongest()`                             | Keep the longest non-blank value. see notes below                                                                                                                                                                                |
+| `merge.Aggregation.KeepLongest()`                             | Keep the longest non-blank value. ( [see notes below](#331-notes-about-aggregationkeeplongest) )                                                                                                                                                                                |
 | `merge.Aggregation.LengthWeightedAverage()`                   | Compute the length weighted average of non-blank values                                                                                                                                                                          |
 | `merge.Aggregation.Average()`                                 | The average non-blank overlapping value.                                                                                                                                         |
-| `merge.Aggregation.LengthWeightedPercentile(percentile=0.75)` | Compute the length weighted percentile (see description of method below). Value should be between 0.0 and 1.0. 0.75 means 75th percentile.                                                                                       |
+| `merge.Aggregation.LengthWeightedPercentile(percentile=0.75)` | Compute the length weighted percentile ( [see notes below](#332-notes-about-aggregationlengthweightedpercentilepercentile) ). Value should be between 0.0 and 1.0. 0.75 means 75th percentile.                                                                                       |
 | `merge.Aggregation.SumProportionOfData()`                     | The sum of all overlapping `data` segments, where the value of each overlapping segment is multiplied by the length of the overlap divided by the length of the `data` segment. This is the same behaviour as the old VBA macro. |
 | `merge.Aggregation.SumProportionOfTarget()`                   | The sum of all overlapping `data` segments, where the value of each overlapping segment is multiplied by the length of the overlap divided by the length of the `target` segment. This aggregation method is suitable when aggregating columns measured in `Units per Kilometre` or `% of length`. The aggregated value will have the same unit.                                                |
 | `merge.Aggregation.Sum()`                                     | Compute the sum of all data overlapping the target segment.                                                                                                                                                                      |
 | `merge.Aggregation.Min()`                                     | The minimum value in `data` which overlaps the segment in `target`.                                                                                                                                                              |
 | `merge.Aggregation.Max()`                                     | The maximum value in `data` which overlaps the segment in `target`.                                                                                                                                                              |
 | `merge.Aggregation.IndexOfMin()`                              | The row-index in the `data` with the minimum value. After merging the index can be used to fetch things like `"Surface Type"` of `"Oldest Surface"` (ie minimum `"Surface Year"`)                                                |
 | `merge.Aggregation.IndexOfMax()`                              | The row-index in the `data` with the maximum value.                                                                                                                                                                              |
 
-#### 3.3.1. Notes about `Aggregation.KeepLongest()`
+#### 3.3.1. Notes about `KeepLongest()`
 
 `KeepLongest()` works by observing both the segment lengths and segment values
 for data rows matching a particular target segment.
 
 **Note 1:** If all segments are the same length but have different values, then
 the first segment to appear in the data input table will be selected. This
 'select first' behaviour is determined by the internal behaviour of pandas and
@@ -221,14 +216,46 @@
 Notes 2, 3 and 4. Data must be pre-processed if it is expected that issues
 regarding floating point number equality (ie `1.0 == 0.99999999999999999`) will
 cause misbehaviour for the `KeepLongest` aggregation. Internally the `pandas`
 `Series.groupby()` function is used to choose the longest segment by grouping by
 segment values. Actual behaviour will depend on how that function is implemented
 by `pandas` internal code.
 
+#### 3.3.2. Notes about `LengthWeightedPercentile(...)`
+
+A the 'length weighted' version of percentile is a fairly uncommon operation
+that only really makes sense when aggregating values for segments of varying
+lengths;
+
+The procedure is similar to a normal percentile calculation in that it involves
+sorting the values to be merged in ascending order onto a vertical bar chart,
+then sampling the `y` value of the chart at some fraction (percentage) of the
+way along the `x` axis.
+
+The 'length weighted' version provided by this package is very similar, except
+that the 'width' of the bars in the bar chart are increased to match the (slk)
+length of the segments they represent. Values are still sorted by ascending
+order along the `x` axis, not by length of segment. The percentage is then
+measured from the midpoint of the first bar to the midpoint of the last bar, and
+linear interpolation is performed between the midpoint of each bar in between.
+
+```text
+      |                          _○_
+      |                         |   |
+      |                      ▴  |   |   <---- 75th percentile Value
+Value |              _____○_____|   |
+      |        __○__|           |   |
+      |       |     |           |   |
+      |  __○__|     |           |   |
+      | |     |     |           |   |
+           |<-----SLK Length----->|
+           0%                ↑   100%
+                             │
+      75th percentile ───────┘
+```
 
 ### 3.4. Practical Example of Merge
 
 ```python
 import pandas as pd
 import merge_segments.merge as merge
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `merge_segments-0.6.0/PKG-INFO` & `merge_segments-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merge_segments
-Version: 0.6.0
+Version: 0.6.1
 Summary: A tool for merging data onto a road network segmentation
 Project-URL: Homepage, https://github.com/thehappycheese/merge-segments
 Author: Nicholas Archer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,52 +17,47 @@
 # `merge_segments`<!-- omit in toc -->
 
 [![Publish to PyPi](https://github.com/thehappycheese/merge-segments/actions/workflows/publish_to_pypi.yml/badge.svg?branch=main)](https://github.com/thehappycheese/merge-segments/actions/workflows/publish_to_pypi.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/merge_segments.svg)](https://pypi.org/project/wideprint)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/merge_segments.svg)](https://pypi.org/project/wideprint)
 
 - [1. Introduction](#1-introduction)
-  - [1.1. Dependencies](#11-dependencies)
 - [2. Install, Upgrade, Uninstall](#2-install-upgrade-uninstall)
 - [3. Module `merge`](#3-module-merge)
   - [3.1. Function `merge.on_slk_intervals()`](#31-function-mergeon_slk_intervals)
   - [3.2. Class `merge.Action`](#32-class-mergeaction)
   - [3.3. Class `merge.Aggregation`](#33-class-mergeaggregation)
-    - [3.3.1. Notes about `Aggregation.KeepLongest()`](#331-notes-about-aggregationkeeplongest)
+    - [3.3.1. Notes about `KeepLongest()`](#331-notes-about-keeplongest)
+    - [3.3.2. Notes about `LengthWeightedPercentile(...)`](#332-notes-about-lengthweightedpercentile)
   - [3.4. Practical Example of Merge](#34-practical-example-of-merge)
 - [4. Notes](#4-notes)
   - [4.1. Correctness, Robustness, Test Coverage and Performance](#41-correctness-robustness-test-coverage-and-performance)
 
 ## 1. Introduction
 
 `merge_segments` is a python package which reproduces an old excell process.
 
 The purpose is to combine two data tables which have a linear segment index ("from" and "to" columns); ie where each row in the input tables represents some linear portion of an entity; for example a road segment from 5km to 10km.
 
 There is an ongoing effort to accelerate and parallelise the merge function
 under a new repo called
 [megamerge](https://github.com/thehappycheese/megamerge)
 
-### 1.1. Dependencies
-
-This package depends on Pandas (tested with version 1.3.1) and is most likely to
-work as expected in Python 3.9+.
-
 ## 2. Install, Upgrade, Uninstall
 
 To install:
 
 ```powershell
-pip install "https://github.com/thehappycheese/merge-segments/zipball/main/"
+pip install merge_segments
 ```
 
 To Upgrade:
 
 ```powershell
-pip install --upgrade "https://github.com/thehappycheese/merge-segments/zipball/main"
+pip install --upgrade merge_segments
 ```
 
 To show installed version:
 
 ```powershell
 pip show merge_segments
 ```
@@ -167,27 +162,27 @@
 ### 3.3. Class `merge.Aggregation`
 
 The following merge aggregations are supported:
 
 | Constructor                                                   | Purpose                                                                                                                                                                                                                          |
 | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `merge.Aggregation.First()`                                   | Keep the first non-blank value.                                                                                                                                                                                                  |
-| `merge.Aggregation.KeepLongest()`                             | Keep the longest non-blank value. see notes below                                                                                                                                                                                |
+| `merge.Aggregation.KeepLongest()`                             | Keep the longest non-blank value. ( [see notes below](#331-notes-about-aggregationkeeplongest) )                                                                                                                                                                                |
 | `merge.Aggregation.LengthWeightedAverage()`                   | Compute the length weighted average of non-blank values                                                                                                                                                                          |
 | `merge.Aggregation.Average()`                                 | The average non-blank overlapping value.                                                                                                                                         |
-| `merge.Aggregation.LengthWeightedPercentile(percentile=0.75)` | Compute the length weighted percentile (see description of method below). Value should be between 0.0 and 1.0. 0.75 means 75th percentile.                                                                                       |
+| `merge.Aggregation.LengthWeightedPercentile(percentile=0.75)` | Compute the length weighted percentile ( [see notes below](#332-notes-about-aggregationlengthweightedpercentilepercentile) ). Value should be between 0.0 and 1.0. 0.75 means 75th percentile.                                                                                       |
 | `merge.Aggregation.SumProportionOfData()`                     | The sum of all overlapping `data` segments, where the value of each overlapping segment is multiplied by the length of the overlap divided by the length of the `data` segment. This is the same behaviour as the old VBA macro. |
 | `merge.Aggregation.SumProportionOfTarget()`                   | The sum of all overlapping `data` segments, where the value of each overlapping segment is multiplied by the length of the overlap divided by the length of the `target` segment. This aggregation method is suitable when aggregating columns measured in `Units per Kilometre` or `% of length`. The aggregated value will have the same unit.                                                |
 | `merge.Aggregation.Sum()`                                     | Compute the sum of all data overlapping the target segment.                                                                                                                                                                      |
 | `merge.Aggregation.Min()`                                     | The minimum value in `data` which overlaps the segment in `target`.                                                                                                                                                              |
 | `merge.Aggregation.Max()`                                     | The maximum value in `data` which overlaps the segment in `target`.                                                                                                                                                              |
 | `merge.Aggregation.IndexOfMin()`                              | The row-index in the `data` with the minimum value. After merging the index can be used to fetch things like `"Surface Type"` of `"Oldest Surface"` (ie minimum `"Surface Year"`)                                                |
 | `merge.Aggregation.IndexOfMax()`                              | The row-index in the `data` with the maximum value.                                                                                                                                                                              |
 
-#### 3.3.1. Notes about `Aggregation.KeepLongest()`
+#### 3.3.1. Notes about `KeepLongest()`
 
 `KeepLongest()` works by observing both the segment lengths and segment values
 for data rows matching a particular target segment.
 
 **Note 1:** If all segments are the same length but have different values, then
 the first segment to appear in the data input table will be selected. This
 'select first' behaviour is determined by the internal behaviour of pandas and
@@ -237,14 +232,46 @@
 Notes 2, 3 and 4. Data must be pre-processed if it is expected that issues
 regarding floating point number equality (ie `1.0 == 0.99999999999999999`) will
 cause misbehaviour for the `KeepLongest` aggregation. Internally the `pandas`
 `Series.groupby()` function is used to choose the longest segment by grouping by
 segment values. Actual behaviour will depend on how that function is implemented
 by `pandas` internal code.
 
+#### 3.3.2. Notes about `LengthWeightedPercentile(...)`
+
+A the 'length weighted' version of percentile is a fairly uncommon operation
+that only really makes sense when aggregating values for segments of varying
+lengths;
+
+The procedure is similar to a normal percentile calculation in that it involves
+sorting the values to be merged in ascending order onto a vertical bar chart,
+then sampling the `y` value of the chart at some fraction (percentage) of the
+way along the `x` axis.
+
+The 'length weighted' version provided by this package is very similar, except
+that the 'width' of the bars in the bar chart are increased to match the (slk)
+length of the segments they represent. Values are still sorted by ascending
+order along the `x` axis, not by length of segment. The percentage is then
+measured from the midpoint of the first bar to the midpoint of the last bar, and
+linear interpolation is performed between the midpoint of each bar in between.
+
+```text
+      |                          _○_
+      |                         |   |
+      |                      ▴  |   |   <---- 75th percentile Value
+Value |              _____○_____|   |
+      |        __○__|           |   |
+      |       |     |           |   |
+      |  __○__|     |           |   |
+      | |     |     |           |   |
+           |<-----SLK Length----->|
+           0%                ↑   100%
+                             │
+      75th percentile ───────┘
+```
 
 ### 3.4. Practical Example of Merge
 
 ```python
 import pandas as pd
 import merge_segments.merge as merge
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

