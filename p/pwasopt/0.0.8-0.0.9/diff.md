# Comparing `tmp/pwasopt-0.0.8.tar.gz` & `tmp/pwasopt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.8.tar", last modified: Mon Jul  3 22:52:10 2023, max compression
+gzip compressed data, was "pwasopt-0.0.9.tar", last modified: Mon Jul  3 23:04:34 2023, max compression
```

## Comparing `pwasopt-0.0.8.tar` & `pwasopt-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 22:52:10.048953 pwasopt-0.0.8/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    17840 2023-07-03 22:52:10.048953 pwasopt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    17111 2023-07-03 15:12:57.000000 pwasopt-0.0.8/README.md
--rw-rw-rw-   0        0        0      932 2023-07-03 22:51:43.000000 pwasopt-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 22:52:10.048953 pwasopt-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 22:52:09.995529 pwasopt-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 22:52:10.033318 pwasopt-0.0.8/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.8/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.8/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.8/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.8/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.8/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21959 2023-07-03 15:10:09.000000 pwasopt-0.0.8/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22300 2023-07-03 15:10:09.000000 pwasopt-0.0.8/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.8/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.8/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12438 2023-07-03 22:50:28.000000 pwasopt-0.0.8/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.8/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-03 22:52:10.033318 pwasopt-0.0.8/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0    17840 2023-07-03 22:52:09.000000 pwasopt-0.0.8/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-03 22:52:09.000000 pwasopt-0.0.8/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 22:52:09.000000 pwasopt-0.0.8/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-03 22:52:09.000000 pwasopt-0.0.8/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 22:52:09.000000 pwasopt-0.0.8/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 23:04:34.364026 pwasopt-0.0.9/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    17840 2023-07-03 23:04:34.364026 pwasopt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    17111 2023-07-03 15:12:57.000000 pwasopt-0.0.9/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-03 23:04:15.000000 pwasopt-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 23:04:34.379653 pwasopt-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 23:04:34.317141 pwasopt-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 23:04:34.348401 pwasopt-0.0.9/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.9/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.9/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.9/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.9/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.9/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21959 2023-07-03 15:10:09.000000 pwasopt-0.0.9/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22300 2023-07-03 15:10:09.000000 pwasopt-0.0.9/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.9/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.9/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12478 2023-07-03 23:02:33.000000 pwasopt-0.0.9/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.9/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-03 23:04:34.364026 pwasopt-0.0.9/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0    17840 2023-07-03 23:04:34.000000 pwasopt-0.0.9/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-03 23:04:34.000000 pwasopt-0.0.9/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 23:04:34.000000 pwasopt-0.0.9/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-03 23:04:34.000000 pwasopt-0.0.9/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 23:04:34.000000 pwasopt-0.0.9/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.8/LICENSE` & `pwasopt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/PKG-INFO` & `pwasopt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.8
+Version: 0.0.9
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pwasopt-0.0.8/README.md` & `pwasopt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/pyproject.toml` & `pwasopt-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.8/src/pwasopt/acquisition.py` & `pwasopt-0.0.9/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.9/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.9/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.9/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/main_pwas.py` & `pwasopt-0.0.9/src/pwasopt/main_pwas.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.9/src/pwasopt/main_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/pref_fun.py` & `pwasopt-0.0.9/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.9/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt/prob_setup.py` & `pwasopt-0.0.9/src/pwasopt/prob_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         self.delta_E = delta_E
         self.nc = nc
         self.nint = nint
         self.nci = nc + nint
         self.nd = nd
         self.X_d = X_d
-        self.sum_X_d = round(sum(X_d))
+        self.sum_X_d = int(round(sum(X_d)))
         self.nvars = self.nci + nd
         self.nvars_encoded = self.nci + self.sum_X_d
 
         if np.isinf(lb).any() or np.isinf(ub).any():
             errstr_inf = "Please specify non-infinity upper and lower bounds"
             print(errstr_inf)
             sys.exit(1)
@@ -207,49 +207,49 @@
 
             self.lb_nvars[:self.nci] = lb_shrink[:self.nci]
             self.ub_nvars[:self.nci] = ub_shrink[:self.nci]
 
         if nint >0:
             int_interval = np.round(self.ub_original[self.nc:self.nci] - self.lb_original[self.nc:self.nci] + 1)
             self.int_prod = np.prod(int_interval)
-            int_sum = round(np.sum(int_interval))
+            int_sum = int(round(np.sum(int_interval)))
             self.int_interval = int_interval
         else:
             self.int_prod = 0
             self.int_interval = []
 
         if nint >0 and self.int_prod < maxevals:
             self.int_encoded = True
             # if number of possible combinations of integer variables exceed the number of max evaluations, one-hot encode integer variables
             if isLin_eqConstrained:
                 Aeq_int_encode = np.zeros((Aeq.shape[0],nc+int_sum+self.sum_X_d))
                 Aeq_int_encode[:,:nc] = self.Aeq[:,:nc]
                 Aeq_int_encode[:,nc+int_sum:] = self.Aeq[:,self.nci:]
                 for i in range(nint):
-                    Aeq_int_encode[:, nc + round(np.sum(int_interval[:i])):nc + round(np.sum(int_interval[:i + 1]))] = \
+                    Aeq_int_encode[:, nc + int(round(np.sum(int_interval[:i]))):nc + int(round(np.sum(int_interval[:i + 1])))] = \
                         self.Aeq[:,nc+i].dot(np.arange(self.lb[nc+i],self.ub[nc+i]+1))
 
                 self.Aeq = Aeq_int_encode
 
             if isLin_ineqConstrained:
                 Aineq_int_encode = np.zeros((Aineq.shape[0], nc + int_sum + self.sum_X_d))
                 Aineq_int_encode[:, :nc] = self.Aineq[:, :nc]
                 Aineq_int_encode[:, nc + int_sum:] = self.Aineq[:, self.nci:]
                 for i in range(nint):
-                    Aineq_int_encode[:, nc + round(np.sum(int_interval[:i])):nc + round(np.sum(int_interval[:i + 1]))] = \
+                    Aineq_int_encode[:, nc + int(round(np.sum(int_interval[:i]))):nc + int(round(np.sum(int_interval[:i + 1])))] = \
                         self.Aineq[:,nc+i].reshape((-1,1)).dot(np.arange(self.lb_original[nc + i], self.ub_original[nc + i] + 1).reshape((1,-1)))
 
                 self.Aineq = Aineq_int_encode
 
             self.nint_encoded = int_sum
             self.nci_encoded = self.nc + self.nint_encoded
             self.nvars_encoded = self.nci_encoded + self.sum_X_d
 
-            lb_int_encoded = np.zeros(round(self.nvars_encoded))
-            ub_int_encoded = np.ones(round(self.nvars_encoded))
+            lb_int_encoded = np.zeros(int(round(self.nvars_encoded)))
+            ub_int_encoded = np.ones(int(round(self.nvars_encoded)))
             lb_int_encoded[:self.nc] = self.lb[:self.nc]
             ub_int_encoded[:self.nc] = self.ub[:self.nc]
             self.lb = lb_int_encoded
             self.ub = ub_int_encoded
         else:
             self.int_encoded = False
             self.nint_encoded = nint
```

### Comparing `pwasopt-0.0.8/src/pwasopt/sample.py` & `pwasopt-0.0.9/src/pwasopt/sample.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.8/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.9/src/pwasopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.8
+Version: 0.0.9
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

