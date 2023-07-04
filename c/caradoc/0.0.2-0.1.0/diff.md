# Comparing `tmp/caradoc-0.0.2.tar.gz` & `tmp/caradoc-0.1.0.tar.gz`

## Comparing `caradoc-0.0.2.tar` & `caradoc-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 caradoc-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 caradoc-0.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 caradoc-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 caradoc-0.0.2/src/caradoc/__about__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 caradoc-0.0.2/src/caradoc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caradoc-0.0.2/src/caradoc/utils/__init__.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 caradoc-0.0.2/src/caradoc/utils/dataoutput.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 caradoc-0.0.2/src/caradoc/utils/financialyear.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 caradoc-0.0.2/tests/test_dataoutput.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 caradoc-0.0.2/tests/test_financialyear.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 caradoc-0.0.2/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 caradoc-0.0.2/LICENSE
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 caradoc-0.0.2/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 caradoc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 caradoc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 caradoc-0.1.0/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 caradoc-0.1.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 caradoc-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 caradoc-0.1.0/src/caradoc/__about__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 caradoc-0.1.0/src/caradoc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caradoc-0.1.0/src/caradoc/utils/__init__.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 caradoc-0.1.0/src/caradoc/utils/dataoutput.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 caradoc-0.1.0/src/caradoc/utils/financialyear.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 caradoc-0.1.0/tests/test_dataoutput.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 caradoc-0.1.0/tests/test_financialyear.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 caradoc-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 caradoc-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 caradoc-0.1.0/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 caradoc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 caradoc-0.1.0/PKG-INFO
```

### Comparing `caradoc-0.0.2/.github/workflows/linting.yml` & `caradoc-0.1.0/.github/workflows/run-tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-name: linting
+name: Run tests
 
 on: [push, pull_request]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
     - name: Install dependencies
-      run: pip install -e .
-    - name: Lint
-      run: hatch run lint:all
+      run: |
+        pip install -e .
+        pip install hatch
+    - name: Run tests
+      run: hatch run test
```

### Comparing `caradoc-0.0.2/src/caradoc/utils/dataoutput.py` & `caradoc-0.1.0/src/caradoc/utils/dataoutput.py`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/src/caradoc/utils/financialyear.py` & `caradoc-0.1.0/src/caradoc/utils/financialyear.py`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/tests/test_dataoutput.py` & `caradoc-0.1.0/tests/test_dataoutput.py`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/tests/test_financialyear.py` & `caradoc-0.1.0/tests/test_financialyear.py`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/.gitignore` & `caradoc-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/LICENSE` & `caradoc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/README.md` & `caradoc-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# data-analysis
+# Caradoc
 
-Python utilities for doing data analysis
+Python utilities for doing data analysis. Named for [Caradoc Vreichvras](https://en.wikipedia.org/wiki/Caradoc), a knight of the round table.
 
 Currently includes two utilities:
 
 ## `FinancialYear`
 
 Represents a Financial Year, from a string in the format "2020-21".
```

### Comparing `caradoc-0.0.2/pyproject.toml` & `caradoc-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caradoc-0.0.2/PKG-INFO` & `caradoc-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caradoc
-Version: 0.0.2
+Version: 0.1.0
 Summary: A suite of tools to help with data analysis in python.
 Project-URL: Documentation, https://github.com/kanedata/caradoc#readme
 Project-URL: Issues, https://github.com/kanedata/caradoc/issues
 Project-URL: Source, https://github.com/kanedata/caradoc
 Author-email: David Kane <david@dkane.net>
 License-Expression: MIT
 License-File: LICENSE
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: xlsxwriter
 Description-Content-Type: text/markdown
 
-# data-analysis
+# Caradoc
 
-Python utilities for doing data analysis
+Python utilities for doing data analysis. Named for [Caradoc Vreichvras](https://en.wikipedia.org/wiki/Caradoc), a knight of the round table.
 
 Currently includes two utilities:
 
 ## `FinancialYear`
 
 Represents a Financial Year, from a string in the format "2020-21".
```

