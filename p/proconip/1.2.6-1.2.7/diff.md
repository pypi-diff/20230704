# Comparing `tmp/proconip-1.2.6.tar.gz` & `tmp/proconip-1.2.7.tar.gz`

## Comparing `proconip-1.2.6.tar` & `proconip-1.2.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.6/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.6/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.6/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.6/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.6/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.6/src/proconip/__init__.py
--rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 proconip-1.2.6/src/proconip/api.py
--rw-r--r--   0        0        0    23560 2020-02-02 00:00:00.000000 proconip-1.2.6/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.6/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.6/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.6/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.6/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.6/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.6/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.7/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.7/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.7/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.7/src/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.7/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.7/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.7/src/proconip/__init__.py
+-rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 proconip-1.2.7/src/proconip/api.py
+-rw-r--r--   0        0        0    23582 2020-02-02 00:00:00.000000 proconip-1.2.7/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.7/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.7/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.7/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.7/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.7/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.7/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.7/PKG-INFO
```

### Comparing `proconip-1.2.6/CODE_OF_CONDUCT.md` & `proconip-1.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/CONTRIBUTING.md` & `proconip-1.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/.github/workflows/pylint.yml` & `proconip-1.2.7/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/.github/workflows/python-publish.yml` & `proconip-1.2.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/.github/workflows/unittest.yml` & `proconip-1.2.7/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/src/proconip/api.py` & `proconip-1.2.7/src/proconip/api.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/src/proconip/definitions.py` & `proconip-1.2.7/src/proconip/definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         self._column = column
 
         self._name = name
         self._unit = unit
         self._offset = offset
         self._gain = gain
         self._raw_value = value
-        self._value = (value - offset) * gain
+        self._value = self._offset + (self._gain * self._raw_value)
 
         if column == 0:
             self._category = CATEGORY_TIME
             self._category_id = 0
             self._display_value = f"{int(self._value / 256):02d}:{(int(self._value) % 256):02d}"
         elif 1 <= column <= 5:
             self._category = CATEGORY_ANALOG
```

### Comparing `proconip-1.2.6/tests/helper.py` & `proconip-1.2.7/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/tests/test_definitions.py` & `proconip-1.2.7/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/.gitignore` & `proconip-1.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/LICENSE` & `proconip-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/README.md` & `proconip-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.6/pyproject.toml` & `proconip-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.6/PKG-INFO` & `proconip-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.6
+Version: 1.2.7
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

