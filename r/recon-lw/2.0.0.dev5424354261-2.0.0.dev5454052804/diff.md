# Comparing `tmp/recon_lw-2.0.0.dev5424354261.tar.gz` & `tmp/recon_lw-2.0.0.dev5454052804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5424354261.tar", last modified: Fri Jun 30 15:10:10 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5454052804.tar", last modified: Tue Jul  4 11:16:22 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5424354261.tar` & `recon_lw-2.0.0.dev5454052804.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-30 15:09:51.000000 recon_lw-2.0.0.dev5424354261/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34667 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-04 11:16:03.000000 recon_lw-2.0.0.dev5454052804/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34732 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,16 +779,18 @@
 
 def display_l3(order_book):
     header = ["bid_price", "bid_qty", "bid_order_id",
               "ask_price", "ask_qty", "ask_order_id"]
     result = [header]
     bid_prices = list(order_book["bid"])
     bid_prices.sort()
-    bid_items = [[p, q, o_id] for p in bid_prices for o_id,q in order_book["bid"][p].items()]
-    ask_items = [[p, q, o_id] for p in bid_prices for o_id,q in order_book["ask"][p].items()]
+    ask_prices = list(order_book["ask"])
+    ask_prices.sort()
+    bid_items = [[p, q, o_id] for p in bid_prices for o_id, q in order_book["bid"][p].items()]
+    ask_items = [[p, q, o_id] for p in ask_prices for o_id, q in order_book["ask"][p].items()]
     levels = max(len(bid_items), len(ask_items))
     for i in range(levels):
         line = []
         if i < len(bid_items):
             line.extend(bid_items[i])
         else:
             line.extend([None]*3)
```

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/setup.py` & `recon_lw-2.0.0.dev5454052804/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5424354261/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5454052804/test/test_recon_ob.py`

 * *Files identical despite different names*

