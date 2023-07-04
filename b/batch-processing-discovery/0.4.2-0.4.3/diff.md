# Comparing `tmp/batch_processing_discovery-0.4.2.tar.gz` & `tmp/batch_processing_discovery-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_processing_discovery-0.4.2.tar", max compression
+gzip compressed data, was "batch_processing_discovery-0.4.3.tar", max compression
```

## Comparing `batch_processing_discovery-0.4.2.tar` & `batch_processing_discovery-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11349 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/LICENSE
--rw-r--r--   0        0        0     4075 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/README.md
--rw-r--r--   0        0        0      648 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/__init__.py
--rw-r--r--   0        0        0     8792 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/batch_characteristics.py
--rw-r--r--   0        0        0     2264 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/config.py
--rw-r--r--   0        0        0     5618 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/discovery.py
--rw-r--r--   0        0        0     6681 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/features_table.py
--rw-r--r--   0        0        0     4876 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/rules.py
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4075 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/README.md
+-rw-r--r--   0        0        0      648 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/__init__.py
+-rw-r--r--   0        0        0     8792 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/batch_characteristics.py
+-rw-r--r--   0        0        0     2264 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/config.py
+-rw-r--r--   0        0        0     5618 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/discovery.py
+-rw-r--r--   0        0        0     6681 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/features_table.py
+-rw-r--r--   0        0        0     4881 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/rules.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.3/PKG-INFO
```

### Comparing `batch_processing_discovery-0.4.2/LICENSE` & `batch_processing_discovery-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/README.md` & `batch_processing_discovery-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/pyproject.toml` & `batch_processing_discovery-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batch-processing-discovery"
-version = "0.4.2"
+version = "0.4.3"
 description = "Python algorithm to discover, from an event log, activity instances that are executed in a batch."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "batch_processing_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `batch_processing_discovery-0.4.2/src/batch_processing_discovery/batch_characteristics.py` & `batch_processing_discovery-0.4.3/src/batch_processing_discovery/batch_characteristics.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/src/batch_processing_discovery/config.py` & `batch_processing_discovery-0.4.3/src/batch_processing_discovery/config.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/src/batch_processing_discovery/discovery.py` & `batch_processing_discovery-0.4.3/src/batch_processing_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/src/batch_processing_discovery/features_table.py` & `batch_processing_discovery-0.4.3/src/batch_processing_discovery/features_table.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.2/src/batch_processing_discovery/rules.py` & `batch_processing_discovery-0.4.3/src/batch_processing_discovery/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 def _get_rules(
         data: pd.DataFrame,
         outcome: str,
         min_rule_support: float = 0.25,
         max_rules: int = 3
 ) -> dict:
     """
-    Discover the rules that lead to the positive outcome in the observations passed as argument in [data]. In this function, the support
-    is measured only with positive outcome observations, instead of all observations. In this way, a rule with 50% support explains 50% of
-    positive outcome observations, and a rule with 100% explains all of them.
+    Discover the rules that lead to the positive outcome in the observations passed as argument in [data].
+    In this function, the support is measured only with positive outcome observations, instead of all
+    observations. In this way, a rule with 50% support explains 50% of positive outcome observations,
+    and a rule with 100% explains all of them.
 
     :param data:                pd.DataFrame with one observation per row.
     :param outcome              ID of the column with the variable to predict (1 positive, 0 negative).
     :param min_rule_support:    Minimum individual support for the discovered activation rules.
     :param max_rules:           Maximum number of activation rules to extract from a batch.
     :return: a dict with the RIPPER model, its confidence, and its support.
     """
@@ -103,12 +104,12 @@
                     index = indexes[0]
                     operator = "in"
                     value = [condition.val[:index], condition.val[index + 1:]]
                 else:
                     print("Error parsing interval '{}', couldn't find the separating character '-'.".format(condition.val))
                     operator = "null"
                     value = "null"
-            sublist += [{'attribute': condition.feature, 'condition': operator, 'value': value}]
+            sublist += [{'attribute': condition.feature, 'comparison': operator, 'value': value}]
         # Add sublist of rules to complete
         rules += [sublist]
     # Return the rules
     return rules
```

### Comparing `batch_processing_discovery-0.4.2/PKG-INFO` & `batch_processing_discovery-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-processing-discovery
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python algorithm to discover, from an event log, activity instances that are executed in a batch.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

