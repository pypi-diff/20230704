# Comparing `tmp/huhangkai-1.4.8.tar.gz` & `tmp/huhangkai-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\huhangkai-1.4.8.tar", last modified: Mon Jul  3 16:38:23 2023, max compression
+gzip compressed data, was "huhangkai-1.4.9.tar", last modified: Tue Jul  4 10:17:20 2023, max compression
```

## Comparing `huhangkai-1.4.8.tar` & `huhangkai-1.4.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/
--rw-rw-rw-   0        0        0      158 2023-07-03 16:38:23.000000 huhangkai-1.4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/
--rw-rw-rw-   0        0        0      933 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      803 2023-07-03 16:30:27.000000 huhangkai-1.4.8/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/init_project.py
--rw-rw-rw-   0        0        0      276 2023-07-03 16:38:21.000000 huhangkai-1.4.8/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3252 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     1348 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0     1548 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2609 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    13338 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    23691 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-03 16:12:55.000000 huhangkai-1.4.8/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      158 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 16:38:23.000000 huhangkai-1.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.747933 huhangkai-1.4.9/
+-rw-rw-rw-   0        0        0      228 2023-07-04 10:17:20.747933 huhangkai-1.4.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.711059 huhangkai-1.4.9/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.718014 huhangkai-1.4.9/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      803 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-04 10:17:20.000000 huhangkai-1.4.9/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29301 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.720008 huhangkai-1.4.9/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.738992 huhangkai-1.4.9/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-04 02:56:42.000000 huhangkai-1.4.9/commen/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     4328 2023-07-04 07:35:21.000000 huhangkai-1.4.9/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     5298 2023-07-04 10:01:19.000000 huhangkai-1.4.9/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0     1548 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2621 2023-07-04 02:41:44.000000 huhangkai-1.4.9/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    16359 2023-07-04 10:17:06.000000 huhangkai-1.4.9/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    23691 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-04 01:23:37.000000 huhangkai-1.4.9/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:17:20.745939 huhangkai-1.4.9/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-04 10:17:20.000000 huhangkai-1.4.9/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-07-04 10:17:20.000000 huhangkai-1.4.9/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:17:20.000000 huhangkai-1.4.9/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-04 10:17:20.000000 huhangkai-1.4.9/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-04 10:17:20.000000 huhangkai-1.4.9/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 10:17:20.748965 huhangkai-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhangkai-1.4.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `huhangkai-1.4.8/commen/__init__.py` & `huhangkai-1.4.9/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/case_project/base_project.py` & `huhangkai-1.4.9/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/case_project/setup_set.py` & `huhangkai-1.4.9/commen/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/init_project.py` & `huhangkai-1.4.9/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/par_do.py` & `huhangkai-1.4.9/commen/testcase/apache/beam_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,8 +54,65 @@
     yield beam.utils.windowed_value.WindowedValue(
         value='* finish_bundle: 🌱🌳🌍',
         timestamp=0,
         windows=[self.window],
     )
 
   def teardown(self):
-    print('teardown')
+    print('teardown')
+
+
+class AverageFn(beam.CombineFn):
+  def create_accumulator(self):
+    sum = 0.0
+    count = 0
+    accumulator = sum, count
+    return accumulator
+
+  def add_input(self, accumulator, input):
+    sum, count = accumulator
+    return sum + input, count + 1
+
+  def merge_accumulators(self, accumulators):
+    sums, counts = zip(*accumulators)
+    return sum(sums), sum(counts)
+
+  def extract_output(self, accumulator):
+    sum, count = accumulator
+    if count == 0:
+      return float('NaN')
+    return sum / count
+
+
+class AverageFn2(beam.CombineFn):
+  def create_accumulator(self):
+    return {}
+
+  def add_input(self, accumulator, input):
+    # accumulator == {}
+    # input == '🥕'
+    if input not in accumulator:
+      accumulator[input] = 0  # {'🥕': 0}
+    accumulator[input] += 1  # {'🥕': 1}
+    return accumulator
+
+  def merge_accumulators(self, accumulators):
+    # accumulators == [
+    #     {'🥕': 1, '🍅': 1},
+    #     {'🥕': 1, '🍅': 1, '🍆': 1},
+    # ]
+    merged = {}
+    for accum in accumulators:
+      for item, count in accum.items():
+        if item not in merged:
+          merged[item] = 0
+        merged[item] += count
+    # merged == {'🥕': 2, '🍅': 2, '🍆': 1}
+    return merged
+
+  def extract_output(self, accumulator):
+    # accumulator == {'🥕': 2, '🍅': 2, '🍆': 1}
+    total = sum(accumulator.values())  # 5
+    percentages = {item: count / total for item, count in accumulator.items()}
+    # percentages == {'🥕': 0.4, '🍅': 0.4, '🍆': 0.2}
+    return percentages
+
```

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_fiter.py` & `huhangkai-1.4.9/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.4.9/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_map.py` & `huhangkai-1.4.9/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_par_do.py` & `huhangkai-1.4.9/commen/testcase/apache/test_par_do.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import random
 from commen.testcase.apache.data import *
 from commen.unit_apache_beam import ApacheFun
-from commen.testcase.apache.par_do import SplitWords, AnalyzeElement, DoFnMethods
+from commen.testcase.apache.beam_class import SplitWords, AnalyzeElement, DoFnMethods
 
 
 class TestParDo:
     # 有简单 DoFn 的 ParDo
-    def test_pardo_001(self):
+    def test_par_do_001(self):
         ApacheFun(data_list_str2, data_type=data_type).par_do(SplitWords(',')).print()
 
     # 带有时间戳和窗口信息的 ParDo
-    def test_pardo_002(self):
+    def test_par_do_002(self):
         af = ApacheFun([':)'])
         af.map(lambda elem: af.window.TimestampedValue(elem, 1584675660))
         af.window_info(af.window.FixedWindows(30))
         af.par_do(AnalyzeElement()).print()
 
     # ParDo 与 DoFn 方法
-    def test_pardo_003(self):
+    def test_par_do_003(self):
         ApacheFun(['🍓', '🥕', '🍆', '🍅', '🥔'], data_type=data_type).par_do(DoFnMethods()).print()
 
     # 使用函数进行分区
-    def test_pardo_004(self):
+    def test_par_do_004(self):
         durations = ['annual', 'biennial', 'perennial']
 
         def by_duration(plant, num_partitions):
             return durations.index(plant['duration']) if plant['duration'] in durations else len(durations)
 
         out = ApacheFun(data_list_dict, data_type=data_type).partition(by_duration, 4)
         # out.print("'{}: {}'.format(x['duration'], x)")
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
         out.run()
 
     # 使用 lambda 函数进行分区
-    def test_pardo_005(self):
+    def test_par_do_005(self):
         durations = ['annual', 'biennial', 'perennial']
         out = ApacheFun(data_list_dict, data_type=data_type).partition(
             lambda plant, num_partitions:
             durations.index(plant['duration']) if plant['duration'] in durations else len(durations), 4)
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
         out.run()
 
     # 具有多个参数的分区
-    def test_pardo_006(self):
+    def test_par_do_006(self):
 
         def split_dataset(plant, num_partitions, ratio):
             assert num_partitions == len(ratio)
             bucket = random.randint(0, sum(ratio)-1)
             total = 0
             for i, part in enumerate(ratio):
                 total += part
                 if bucket < total:
                     return i
             return len(ratio) - 1
 
         out = ApacheFun(data_list_dict*3).partition(split_dataset, 2, ratio=[10, 20])
         out.value[0].print("'1: {}'.format(x)")
         out.value[1].print("'2: {}'.format(x)")
-        out.run()
+        out.run()
```

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_regex.py` & `huhangkai-1.4.9/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_time.py` & `huhangkai-1.4.9/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/testcase/apache/test_to_string.py` & `huhangkai-1.4.9/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_apache_beam.py` & `huhangkai-1.4.9/commen/unit_apache_beam.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 
 
 class ApacheFun:
     window = window
 
     def __init__(self, data=None, name="", out=None, data_type=1):
         """data_type: 1 管道， 2 数据"""
+
         self.pipeline = beam.Pipeline()
         self.data = data
         self.out = out
         self.value = None
         self.name = name or str(uuid.uuid4())[-12:]
         self.data_type = data_type
         self._i = 0
         self._tmp_value = None
+        self._group_by = None
+        self._group_by_old = None
+        self._aggregate_field = []
         if data:
             self.create()
 
     def __str__(self):
         return self.value
 
     def _name(self):
         self._i += 1
-        return str(self.name) + str(self._i)
+        return str(self.name) + "_" + str(self._i)
 
     def run(self):
         """执行"""
         self.pipeline.run()
 
     def print(self, fmt=None):
         """打印"""
@@ -213,14 +217,24 @@
                 elif type == "bj":
                     plant[key] = datetime.datetime.fromtimestamp(timestamp.micros / 1e6).strftime("%Y-%m-%d %H:%M:%S")
                 elif type == "rfc":
                     plant[key] = timestamp.to_rfc3339()
                 elif type == "proto":
                     plant[key] = timestamp.to_proto()
                 yield plant
+
+        def get_key(plant):
+            if key and plant.get(key):
+                return plant[key]
+            else:
+                try:
+                    self._tmp_value
+                except:
+                    return time.time()
+
         if self.data_type == 1:
             self.value = self.out = self.get_out() | self._name() >> beam.Map(
                 lambda plant: self.window.TimestampedValue(plant, plant[key] if key and plant.get(key) else time.time())
             ) | self._name() >> beam.ParDo(GetTimestamp(key=key))
         else:
             def get_plant(plant):
                 micros = plant[key] if key and plant.get(key) else time.time()
@@ -290,11 +304,69 @@
                 elif self.type == 3:
                     total = sum(accumulator.values())  # 10
                     percentages = {item: ("%.1f%%" % (count / total * 100)) for item, count in accumulator.items()}
                     return percentages
         self.value = self.out = self.combine_globally(PercentagesFn(key, type)).value
         return self
 
+    def combine_per_key(self, fn, *args, **kwargs):
+        """组合集合中每个键的所有元素"""
+        self.value = self.out = self.get_out() | self._name() >> beam.CombinePerKey(fn, *args, **kwargs)
+        return self
+
+    def combine_values(self, fn, *args, **kwargs):
+        """在键控元素集合中组合可迭代的值"""
+        self.value = self.out = self.get_out() | self._name() >> beam.CombineValues(fn, *args, **kwargs)
+        return self
+
+    def count_globally(self):
+        """计算每个聚合中的元素个数"""
+        self.value = self.out = self.get_out() | self._name() >> beam.combiners.Count.Globally()
+        return self
+
+    def count_per_key(self):
+        """计算键值的 PCollection 中每个唯一键的元素"""
+        self.value = self.out = self.get_out() | self._name() >> beam.combiners.Count.PerKey()
+        return self
+
+    def count_per_element(self):
+        """计算PCollection中唯一的元素"""
+        self.value = self.out = self.get_out() | self._name() >> beam.combiners.Count.PerElement()
+        return self
+
+    def distinct(self):
+        """生成一个包含输入集合的不同元素的集合"""
+        self.value = self.out = self.get_out() | self._name() >> beam.Distinct()
+        return self
+
+    def group_by_key(self):
+        """获取元素的键值集合，并生成一个集合，其中每个元素由一个键和与该键关联的所有值组成"""
+        self.value = self.out = self.get_out() | self._name() >> beam.GroupByKey()
+        return self
+
+    def group_by(self, *fields, **kwargs):
+        self._group_by = beam.GroupBy(*fields, **kwargs)
+        self._group_by_old = self.get_out()
+        self.value = self.out = self._group_by_old | self._name() >> self._group_by
+        return self
+
+    def aggregate_field(self, field, combine_fn, dest):
+        self._aggregate_field.append((field, combine_fn, dest))
+        _group_by = self._group_by if self._group_by else beam.GroupBy()
+        self._group_by_old = self._group_by_old if self._group_by_old else self.get_out()
+        for i in self._aggregate_field:
+            _group_by = _group_by.aggregate_field(*i)
+        self.value = self.out = self._group_by_old | self._name() >> _group_by
+        return self
+
+    def group_into_batches(self, batch_size):
+        self.value = self.out = self.get_out() | self._name() >> beam.GroupIntoBatches(batch_size)
+        return self
+
+    def latest_globally(self):
+        self.value = self.out = self.get_out() | self._name() >> beam.combiners.Latest.Globally()
+        return self
+
 
 if __name__ == '__main__':
-    from study.data.data import *
+    from commen.testcase.apache.data import *
     ApacheFun(data_list_tuple).create().print()
```

### Comparing `huhangkai-1.4.8/commen/unit_dict.py` & `huhangkai-1.4.9/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_encryption.py` & `huhangkai-1.4.9/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_fun.py` & `huhangkai-1.4.9/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_logger.py` & `huhangkai-1.4.9/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_request.py` & `huhangkai-1.4.9/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/unit_tasks.py` & `huhangkai-1.4.9/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/commen/常用命令.py` & `huhangkai-1.4.9/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.8/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.4.9/huhangkai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+setup.py
 commen/__init__.py
 commen/init_project.py
 commen/setup_run.py
 commen/unit_apache_beam.py
 commen/unit_dict.py
 commen/unit_encryption.py
 commen/unit_fun.py
@@ -11,16 +12,16 @@
 commen/常用命令.py
 commen/case_project/__init__.py
 commen/case_project/base_project.py
 commen/case_project/setup_set.py
 commen/case_project/version.py
 commen/testcase/__init__.py
 commen/testcase/apache/__init__.py
+commen/testcase/apache/beam_class.py
 commen/testcase/apache/data.py
-commen/testcase/apache/par_do.py
 commen/testcase/apache/test_cogroupbykey.py
 commen/testcase/apache/test_fiter.py
 commen/testcase/apache/test_flatmap.py
 commen/testcase/apache/test_map.py
 commen/testcase/apache/test_par_do.py
 commen/testcase/apache/test_regex.py
 commen/testcase/apache/test_time.py
```

