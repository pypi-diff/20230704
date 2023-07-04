# Comparing `tmp/GRLP-1.7.0.tar.gz` & `tmp/GRLP-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GRLP-1.7.0.tar", last modified: Fri Aug  5 22:12:41 2022, max compression
+gzip compressed data, was "GRLP-1.8.0.tar", last modified: Tue Jul  4 14:55:56 2023, max compression
```

## Comparing `GRLP-1.7.0.tar` & `GRLP-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-08-05 22:12:41.782563 GRLP-1.7.0/
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-08-05 22:12:41.782563 GRLP-1.7.0/GRLP.egg-info/
--rw-r--r--   0 awickert  (1000) awickert  (1000)     4331 2022-08-05 22:12:41.000000 GRLP-1.7.0/GRLP.egg-info/PKG-INFO
--rw-r--r--   0 awickert  (1000) awickert  (1000)      237 2022-08-05 22:12:41.000000 GRLP-1.7.0/GRLP.egg-info/SOURCES.txt
--rw-r--r--   0 awickert  (1000) awickert  (1000)        1 2022-08-05 22:12:41.000000 GRLP-1.7.0/GRLP.egg-info/dependency_links.txt
--rw-r--r--   0 awickert  (1000) awickert  (1000)       23 2022-08-05 22:12:41.000000 GRLP-1.7.0/GRLP.egg-info/requires.txt
--rw-r--r--   0 awickert  (1000) awickert  (1000)        5 2022-08-05 22:12:41.000000 GRLP-1.7.0/GRLP.egg-info/top_level.txt
--rw-r--r--   0 awickert  (1000) awickert  (1000)    35147 2020-07-14 17:59:23.000000 GRLP-1.7.0/LICENSE
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     4331 2022-08-05 22:12:41.786563 GRLP-1.7.0/PKG-INFO
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     3043 2022-08-05 16:07:12.000000 GRLP-1.7.0/README.md
-drwxrwxr-x   0 awickert  (1000) awickert  (1000)        0 2022-08-05 22:12:41.782563 GRLP-1.7.0/grlp/
--rw-rw-r--   0 awickert  (1000) awickert  (1000)      291 2021-11-30 09:06:46.000000 GRLP-1.7.0/grlp/__init__.py
--rw-rw-r--   0 awickert  (1000) awickert  (1000)    11421 2021-11-30 09:06:46.000000 GRLP-1.7.0/grlp/build_synthetic_network.py
--rw-rw-r--   0 awickert  (1000) awickert  (1000)    41438 2022-08-05 16:01:25.000000 GRLP-1.7.0/grlp/grlp.py
--rw-r--r--   0 awickert  (1000) awickert  (1000)      132 2022-08-05 22:12:41.786563 GRLP-1.7.0/setup.cfg
--rw-rw-r--   0 awickert  (1000) awickert  (1000)     1055 2022-08-05 16:14:06.000000 GRLP-1.7.0/setup.py
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-04 14:55:56.728456 GRLP-1.8.0/
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-04 14:55:56.728456 GRLP-1.8.0/GRLP.egg-info/
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     3817 2023-07-04 14:55:56.000000 GRLP-1.8.0/GRLP.egg-info/PKG-INFO
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      237 2023-07-04 14:55:56.000000 GRLP-1.8.0/GRLP.egg-info/SOURCES.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)        1 2023-07-04 14:55:56.000000 GRLP-1.8.0/GRLP.egg-info/dependency_links.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)       23 2023-07-04 14:55:56.000000 GRLP-1.8.0/GRLP.egg-info/requires.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)        5 2023-07-04 14:55:56.000000 GRLP-1.8.0/GRLP.egg-info/top_level.txt
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)    35147 2023-07-04 13:26:27.000000 GRLP-1.8.0/LICENSE
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     3817 2023-07-04 14:55:56.728456 GRLP-1.8.0/PKG-INFO
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     3054 2023-07-04 13:26:27.000000 GRLP-1.8.0/README.md
+drwxrwxr-x   0 awickert  (1001) awickert  (1001)        0 2023-07-04 14:55:56.728456 GRLP-1.8.0/grlp/
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      291 2023-07-04 13:26:27.000000 GRLP-1.8.0/grlp/__init__.py
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)    20619 2023-07-04 13:26:27.000000 GRLP-1.8.0/grlp/build_synthetic_network.py
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)    45639 2023-07-04 13:26:27.000000 GRLP-1.8.0/grlp/grlp.py
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)      132 2023-07-04 14:55:56.728456 GRLP-1.8.0/setup.cfg
+-rw-rw-r--   0 awickert  (1001) awickert  (1001)     1055 2023-07-04 13:26:27.000000 GRLP-1.8.0/setup.py
```

### Comparing `GRLP-1.7.0/LICENSE` & `GRLP-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GRLP-1.7.0/README.md` & `GRLP-1.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![DOI](https://zenodo.org/badge/159710833.svg)](https://zenodo.org/badge/latestdoi/159710833)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6968526.svg)](https://doi.org/10.5281/zenodo.6968526)
 
 # gravel-river-long-profile
 Long-profile evolution of gravel-bed rivers
 
 `grlp.py` is module that contains the equations and solvers. `run_grlp.py` interfaces with these to, well, run a model based off of `grlp.py`. Comments inside `run_grlp.py` should help you learn how to write your own models. Please contact Andy Wickert for questions or assistance.
```

### Comparing `GRLP-1.7.0/grlp/grlp.py` & `GRLP-1.8.0/grlp/grlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -969,28 +969,123 @@
         self.max_topological_length = False
         for i in self.sources:
             self.topological_length = -1
             _step_down(i)
             self.max_topological_length = max(self.max_topological_length, self.topological_length)
         del self.topological_length
 
+        # organise segments into streams
+        self.streams_by_order = {}
+        for order in np.unique(self.segment_orders):
+            self.streams_by_order[order+1] = []
+        for seg in self.list_of_LongProfile_objects:
+            up_IDs = self.find_upstream_IDs(seg.ID)
+            down_IDs = self.find_downstream_IDs(seg.ID)
+            if not self.streams_by_order[self.segment_orders[seg.ID]+1]:
+                self.streams_by_order[self.segment_orders[seg.ID]+1].append([seg.ID])
+            else:
+                for i,stream in enumerate(self.streams_by_order[self.segment_orders[seg.ID]+1]):
+                    if any(ID in stream for ID in up_IDs) or any(ID in stream for ID in down_IDs):
+                        self.streams_by_order[self.segment_orders[seg.ID]+1][i].append(seg.ID)
+                if not seg.ID in np.hstack(self.streams_by_order[self.segment_orders[seg.ID]+1]):
+                    self.streams_by_order[self.segment_orders[seg.ID]+1].append([seg.ID])
+
         # count number of streams in each order
-        self.order_counts = np.zeros(max(self.segment_orders)+1)
-        lengths = np.zeros(len(self.order_counts))
-        for i,seg in enumerate(self.list_of_LongProfile_objects):
-            up_os = self.segment_orders[seg.upstream_segment_IDs]
-            if self.segment_orders[i] not in up_os:
-                self.order_counts[self.segment_orders[i]] += 1
-            lengths[self.segment_orders[i]] += seg.x.max() - seg.x.min()
-        self.order_lengths = lengths / self.order_counts
+        self.order_counts = {}
+        for order in self.streams_by_order.keys():
+            self.order_counts[order] = len(self.streams_by_order[order])
+            
+        # bifurcation ratio
+        self.orders = list(self.order_counts.keys())
+        fit = np.polyfit(
+            self.orders,
+            np.log10([self.order_counts[o] for o in self.orders]),
+            1)
+        self.bifurcation_ratio = 10.**(-fit[0])
+        self.bifurcation_scale = 10.**(fit[1] -fit[0])
+        
+        # compute stream lengths
+        self.stream_lengths = {}
+        self.order_lengths = {}
+        for o in self.orders:
+            self.stream_lengths[o] = []
+            for stream in self.streams_by_order[o]:
+                l = 0.
+                for segID in stream:
+                    l += (
+                        self.list_of_LongProfile_objects[segID].x.max() -
+                        self.list_of_LongProfile_objects[segID].x.min()
+                        )
+                self.stream_lengths[o].append(l)
+            self.order_lengths[o] = np.mean([l for l in self.stream_lengths[o]])
+        
+        # compute length ratio
+        fit = np.polyfit(
+            self.orders,
+            np.log10([self.order_lengths[o] for o in self.orders]),
+            1)
+        self.length_ratio = 10.**(fit[0])
+        self.length_scale = 10.**(fit[0] + fit[1])    
 
-        # compute bifurcation ratios
-        self.bifurcation_ratios = np.full(len(self.order_counts), np.nan)
-        for i in range(len(self.order_counts)-1):
-            self.bifurcation_ratios[i] = (self.order_counts[i] / 
-                                          self.order_counts[i+1])
+        # compute stream discharges
+        self.stream_discharges = {}
+        self.order_discharges = {}
+        for o in self.orders:
+            self.stream_discharges[o] = []
+            for stream in self.streams_by_order[o]:
+                self.stream_discharges[o] = [
+                    self.list_of_LongProfile_objects[segID].Q.mean()
+                    for segID in stream
+                    ]
+            self.order_discharges[o] = np.mean([q for q in self.stream_discharges[o]])
+            
+        # compute discharge ratio
+        fit = np.polyfit(
+            self.orders,
+            np.log10([self.order_discharges[o] for o in self.orders]),
+            1)
+        self.discharge_ratio = 10.**fit[0]
+        self.discharge_scale = 10.**(fit[0] + fit[1])    
 
-        # compute length ratios
-        self.length_ratios = np.full(len(self.order_counts), np.nan)
-        for i in range(1,len(self.order_counts)):
-            self.length_ratios[i] = (self.order_lengths[i] / 
-                                     self.order_lengths[i-1])
+        # # count number of streams in each order
+        # self.order_counts = np.zeros(max(self.segment_orders)+1)
+        # lengths = np.zeros(len(self.order_counts))
+        # discharges = np.zeros(len(self.order_counts))
+        # for i,seg in enumerate(self.list_of_LongProfile_objects):
+        #     up_os = self.segment_orders[seg.upstream_segment_IDs]
+        #     if self.segment_orders[i] not in up_os:
+        #         self.order_counts[self.segment_orders[i]] += 1
+        #     lengths[self.segment_orders[i]] += seg.x.max() - seg.x.min()
+        #     discharges[self.segment_orders[i]] += seg.Q.mean()
+        # self.order_lengths = lengths / self.order_counts / 1.e3
+        # self.order_discharges = discharges / self.order_counts
+        # 
+        # # compute bifurcation ratios directly and estimate with log-fit
+        # self.bifurcation_ratios = np.full(len(self.order_counts), np.nan)
+        # for i in range(len(self.order_counts)-1):
+        #     self.bifurcation_ratios[i] = (self.order_counts[i] / 
+        #                                   self.order_counts[i+1])
+        # fit = np.polyfit(
+        #     np.arange(1,len(self.order_counts)+1,1),
+        #     np.log10(self.order_counts),
+        #     1)
+        # self.bifurcation_ratio = 10.**(-fit[0])
+        # self.bifurcation_intercept = fit[1]
+        # 
+        # # compute length ratios
+        # self.length_ratios = np.full(len(self.order_counts), np.nan)
+        # for i in range(1,len(self.order_counts)):
+        #     self.length_ratios[i] = (self.order_lengths[i] / 
+        #                              self.order_lengths[i-1])
+        # fit = np.polyfit(
+        #     np.arange(1,len(self.order_lengths)+1,1),
+        #     np.log10(self.order_lengths),
+        #     1)
+        # self.length_ratio = 10.**(fit[0])
+        # self.length_intercept = fit[1]
+        # 
+        # # compute discharge ratios
+        # fit = np.polyfit(
+        #     np.arange(1,len(self.order_discharges)+1,1),
+        #     np.log10(self.order_discharges),
+        #     1)
+        # self.discharge_ratio = 10.**(fit[0])
```

### Comparing `GRLP-1.7.0/setup.py` & `GRLP-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GRLP",
-    version="1.7.0",
+    version="1.8.0",
     author="Andrew D. Wickert",
     author_email="awickert@umn.edu",
     description="Evolves gravel-bed river long profiles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awickert/GRLP",
     install_requires=[
```

