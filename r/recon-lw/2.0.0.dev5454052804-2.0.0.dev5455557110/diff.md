# Comparing `tmp/recon_lw-2.0.0.dev5454052804.tar.gz` & `tmp/recon_lw-2.0.0.dev5455557110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5454052804.tar", last modified: Tue Jul  4 11:16:22 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5455557110.tar", last modified: Tue Jul  4 13:59:03 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5454052804.tar` & `recon_lw-2.0.0.dev5455557110.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-04 11:16:03.000000 recon_lw-2.0.0.dev5454052804/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34732 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:16:22.000000 recon_lw-2.0.0.dev5454052804/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-04 11:15:39.000000 recon_lw-2.0.0.dev5454052804/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-04 13:58:32.000000 recon_lw-2.0.0.dev5455557110/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13589 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34732 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3998 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/recon_lw.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,18 @@
 
         file_name = output_path + "/" + s + "_OUT.pickle"
         print("Saving ", file_name, " ", datetime.now())
         messages_session_out_to_save.build_cache(file_name)
 
 
 def protocol(m):
+    if "body" not in m:
+        #simplified message
+        return m["protocol"]
+    
     if len(m["body"]) == 0:
         return "error"
     if "protocol" not in m["body"]["metadata"]:
         return "not_defined"
     return m["body"]["metadata"]["protocol"]
```

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
     reverse = -1 if side == "bid" else 1
     if new_price is None:  # deleted level
         return book[side+"_real_n_orders"] == 0
     elif book[side+"_price"] is None:  # added level to empty book
         return new_real_n_orders == 0
     if book[side+"_price"] == new_price:  # top level update
         return new_real_n_orders == book[side+"_real_n_orders"] and book[side+"_real_qty"] == new_real_qty
-    if (reverse * book[side+"_price"]) < (reverse * new_price):  # price is better - new level is added
+    if (reverse * book[side+"_price"]) > (reverse * new_price):  # price is better - new level is added
         return new_real_n_orders == 0
     else:  # price is worse old level is deleted
         return book[side+"_real_n_orders"] == 0
 
 
 def ob_top_update(ask_price: float, ask_real_qty: int, ask_impl_qty: int, ask_real_n_orders: int, ask_impl_n_orders: int,
                   bid_price: float, bid_real_qty: int, bid_impl_qty: int, bid_real_n_orders: int, bid_impl_n_orders: int,
```

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 recon_lw/StateSequenceGenerator.py
 recon_lw/TimeCacheMatcher.py
 recon_lw/__init__.py
 recon_lw/recon_lw.py
 recon_lw/recon_ob.py
 recon_lw/recon_ob_cross_stream.py
 recon_lw/recon_ob_stats.py
+recon_lw/recon_oe_ob.py
 recon_lw.egg-info/PKG-INFO
 recon_lw.egg-info/SOURCES.txt
 recon_lw.egg-info/dependency_links.txt
 recon_lw.egg-info/requires.txt
 recon_lw.egg-info/top_level.txt
 test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5454052804/setup.py` & `recon_lw-2.0.0.dev5455557110/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5454052804/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5455557110/test/test_recon_ob.py`

 * *Files identical despite different names*

