# Comparing `tmp/pwasopt-0.0.6.tar.gz` & `tmp/pwasopt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.6.tar", last modified: Mon Jul  3 15:16:01 2023, max compression
+gzip compressed data, was "pwasopt-0.0.7.tar", last modified: Mon Jul  3 22:46:27 2023, max compression
```

## Comparing `pwasopt-0.0.6.tar` & `pwasopt-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.220931 pwasopt-0.0.6/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    17840 2023-07-03 15:16:01.218196 pwasopt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    17111 2023-07-03 15:12:57.000000 pwasopt-0.0.6/README.md
--rw-rw-rw-   0        0        0      932 2023-07-03 15:14:32.000000 pwasopt-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 15:16:01.220931 pwasopt-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.102627 pwasopt-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.184053 pwasopt-0.0.6/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.6/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.6/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.6/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.6/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.6/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21959 2023-07-03 15:10:09.000000 pwasopt-0.0.6/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22300 2023-07-03 15:10:09.000000 pwasopt-0.0.6/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.6/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.6/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.6/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.6/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.211094 pwasopt-0.0.6/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0    17840 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 22:46:27.097653 pwasopt-0.0.7/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    17840 2023-07-03 22:46:27.097653 pwasopt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    17111 2023-07-03 15:12:57.000000 pwasopt-0.0.7/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-03 22:45:34.000000 pwasopt-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 22:46:27.097653 pwasopt-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 22:46:27.044252 pwasopt-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 22:46:27.082012 pwasopt-0.0.7/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.7/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.7/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.7/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.7/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.7/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21959 2023-07-03 15:10:09.000000 pwasopt-0.0.7/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22300 2023-07-03 15:10:09.000000 pwasopt-0.0.7/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.7/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.7/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12424 2023-07-03 22:44:29.000000 pwasopt-0.0.7/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.7/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-03 22:46:27.097653 pwasopt-0.0.7/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0    17840 2023-07-03 22:46:27.000000 pwasopt-0.0.7/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-03 22:46:27.000000 pwasopt-0.0.7/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 22:46:27.000000 pwasopt-0.0.7/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-03 22:46:27.000000 pwasopt-0.0.7/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 22:46:27.000000 pwasopt-0.0.7/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.6/LICENSE` & `pwasopt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/PKG-INFO` & `pwasopt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.6
+Version: 0.0.7
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pwasopt-0.0.6/README.md` & `pwasopt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/pyproject.toml` & `pwasopt-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.6/src/pwasopt/acquisition.py` & `pwasopt-0.0.7/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.7/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.7/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.7/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/main_pwas.py` & `pwasopt-0.0.7/src/pwasopt/main_pwas.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.7/src/pwasopt/main_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/pref_fun.py` & `pwasopt-0.0.7/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.7/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt/prob_setup.py` & `pwasopt-0.0.7/src/pwasopt/prob_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         self.delta_E = delta_E
         self.nc = nc
         self.nint = nint
         self.nci = nc + nint
         self.nd = nd
         self.X_d = X_d
-        self.sum_X_d = sum(X_d)
+        self.sum_X_d = round(sum(X_d))
         self.nvars = self.nci + nd
         self.nvars_encoded = self.nci + self.sum_X_d
 
         if np.isinf(lb).any() or np.isinf(ub).any():
             errstr_inf = "Please specify non-infinity upper and lower bounds"
             print(errstr_inf)
             sys.exit(1)
```

### Comparing `pwasopt-0.0.6/src/pwasopt/sample.py` & `pwasopt-0.0.7/src/pwasopt/sample.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.6/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.7/src/pwasopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.6
+Version: 0.0.7
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

