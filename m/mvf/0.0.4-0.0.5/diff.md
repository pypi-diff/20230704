# Comparing `tmp/mvf-0.0.4.tar.gz` & `tmp/mvf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.4.tar", last modified: Fri Jun 30 16:22:11 2023, max compression
+gzip compressed data, was "mvf-0.0.5.tar", last modified: Tue Jul  4 09:27:42 2023, max compression
```

## Comparing `mvf-0.0.4.tar` & `mvf-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-30 16:22:07.000000 mvf-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-30 16:22:11.451746 mvf-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-30 16:22:07.000000 mvf-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.444746 mvf-0.0.4/mvf/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.446746 mvf-0.0.4/mvf/cli/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.446746 mvf-0.0.4/mvf/dag/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/dag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11252 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/dag/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.447746 mvf-0.0.4/mvf/integration/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.448746 mvf-0.0.4/mvf/integration/config/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/validate_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/mvf_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.449746 mvf-0.0.4/mvf/integration/process/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/mvf/process/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3619 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/validate_model_r.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.445746 mvf-0.0.4/mvf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1077 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 16:22:11.451746 mvf-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-30 16:22:07.000000 mvf-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/test/
--rw-rw-rw-   0 root         (0) root         (0)     6632 2023-06-30 16:22:07.000000 mvf-0.0.4/test/test_build_dag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.276385 mvf-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-04 09:27:38.000000 mvf-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-04 09:27:42.276385 mvf-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-07-04 09:27:38.000000 mvf-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.268385 mvf-0.0.5/mvf/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.270385 mvf-0.0.5/mvf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.270385 mvf-0.0.5/mvf/dag/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/dag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11636 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/dag/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.271385 mvf-0.0.5/mvf/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.272385 mvf-0.0.5/mvf/integration/config/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/config/validate_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/mvf_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.274385 mvf-0.0.5/mvf/integration/process/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/integration/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.275385 mvf-0.0.5/mvf/process/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-04 09:27:38.000000 mvf-0.0.5/mvf/process/validate_model_r.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 09:27:42.269385 mvf-0.0.5/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-04 09:27:42.000000 mvf-0.0.5/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 09:27:42.276385 mvf-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-04 09:27:38.000000 mvf-0.0.5/setup.py
```

### Comparing `mvf-0.0.4/LICENSE` & `mvf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/PKG-INFO` & `mvf-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.4/README.md` & `mvf-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/cli/cli.py` & `mvf-0.0.5/mvf/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/dag/builder.py` & `mvf-0.0.5/mvf/dag/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,18 @@
         validate = self.__build_validate()
         # model tasks
         for model in self.config['models']:
             # get model params
             name = model['name']
             lang = model['lang']
             val_step = model['validation_step']
+            return_quantiles = model.get('return_quantiles', False)
             # build up model tasks
             fit_model = self.__build_fit_model(name, lang)
-            predict_model = self.__build_predict_model(name, lang)
+            predict_model = self.__build_predict_model(name, lang, return_quantiles=return_quantiles)
             if val_step:
                 validate_model = self.__build_validate_model(name, lang)
                 # set upstream
                 fit_model >> validate_model
             # set upstream
             split_data >> fit_model
             split_data >> predict_model
@@ -223,28 +224,29 @@
             fit_model.on_finish = on_finish.fit_model.fit_model_py
         else:
             fit_model.on_render = on_render.fit_model.fit_model_r
             fit_model.on_finish = on_finish.fit_model.fit_model_r
         return fit_model
 
 
-    def __build_predict_model(self, name, lang):
+    def __build_predict_model(self, name, lang, return_quantiles=False):
         task_name = name + '_predict'
         # source
-        if lang == 'Python':
-            source = process.predict_model.predict_py
-        else:
-            source = process.predict_model.predict_r
+        source = process.predict_model.predict_model
         # params
         params = {
+            'split_type': self.config['data']['split'],
             'model_name': name,
+            'lang': lang,
         }
         if self.config['data']['split'] == 'k_fold':
-            params['split_type'] = self.config['data']['split']
             params['n_folds'] = self.config['data']['n_folds']
+        if 'output' in self.config:
+            if 'quantile_intervals' in self.config['output'] and return_quantiles:
+                params['quantile_intervals'] = self.config['output']['quantile_intervals']
         # define task
         predict_model = PythonCallable(
             source=source,
             product={
                 'predictions': File(
                     os.path.join(
                         self.output_dir,
@@ -253,16 +255,19 @@
                     ),
                 ),
             },
             dag=self.dag,
             name=task_name,
             params=params
         )
-        # hooks  
-        predict_model.on_render = on_render.predict_model.predict_model
+        # hooks
+        if lang == 'Python':
+            predict_model.on_render = on_render.predict_model.predict_model_py
+        else:
+            predict_model.on_render = on_render.predict_model.predict_model_r
         predict_model.on_finish = on_finish.predict_model.predict_model
         return predict_model
     
 
     def __build_validate_model(self, name, lang):
         task_name = name + '_validate'
         # source
```

### Comparing `mvf-0.0.4/mvf/integration/config/fit_model.py` & `mvf-0.0.5/mvf/integration/config/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/integration/config/split_data.py` & `mvf-0.0.5/mvf/integration/config/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/integration/process/fit_model.py` & `mvf-0.0.5/mvf/integration/process/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/integration/process/split_data.py` & `mvf-0.0.5/mvf/integration/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/process/fit_model.py` & `mvf-0.0.5/mvf/process/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/process/predict_model.py` & `mvf-0.0.5/mvf/process/predict_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,117 @@
 # imports
 import feather
 import pandas
 
 
-def predict_py(upstream, product, model_name, split_type, n_folds=10):
+def predict_model(upstream, product, lang, model_name, split_type, n_folds=10, quantile_intervals=None):
     # format variable
     upstream = dict(upstream)
 
-    # imports
-    import models
+    # import model class
+    if lang == 'Python':
+        import models
+    elif lang == 'R':
+        import rpy2.robjects as robjects
+        from rpy2.robjects import pandas2ri
+        import rpy2_r6.r6b as r6b
+        r = robjects.r
+        r['source']('models.R')
 
     if split_type == 'train_test':
-        # load data from upstream process
+        # load test data
         X_test = feather.read_dataframe(upstream['split_data']['test_X_data'])
         del upstream['split_data']
 
-        # load model from upstream process
-        model_class = getattr(models, model_name)
-        model = model_class()
-        model.load(next(iter(upstream.values()))['model'])
+        # load model
+        if lang == 'Python':
+            model = load_python_model(
+                models,
+                model_name,
+                next(iter(upstream.values()))['model']
+            )
+        elif lang == 'R':
+            model = load_r_model(
+                r6b,
+                r,
+                model_name,
+                str(next(iter(upstream.values()))['model'])
+            )
+            # convert pandas dataframe to R dataframe
+            pandas2ri.activate()
+            X_test = pandas2ri.py2rpy_pandasdataframe(
+                X_test
+            )
+            pandas2ri.deactivate()
 
         # predict
-        preds = model.predict(X_test)
+        preds = model.predict(X_test, quantile_intervals)
+
+        if lang == 'R':
+        # convert to pandas dataframe
+            pandas2ri.activate()
+            preds = robjects.conversion.rpy2py(preds)
+            pandas2ri.deactivate()
 
         # save data for next process
         feather.write_dataframe(preds, product['predictions'])
     elif split_type == 'k_fold':
+        # allocate memory for predictions
         predictions = []
+        # for each fold
         for i in range(1, n_folds+1):
-            # load data from upstream process
+            # load test data
             X_test = feather.read_dataframe(
-                upstream['split_data'][f'fold_{i}_X_data'])
+                upstream['split_data'][f'fold_{i}_X_data']
+            )
 
-            # load model from upstream process
-            model_class = getattr(models, model_name)
-            model = model_class()
-            model.load(upstream[f'{model_name}_fit'][f'model_{i}'])
+            # load model
+            if lang == 'Python':
+                model = load_python_model(
+                    models,
+                    model_name,
+                    upstream[f'{model_name}_fit'][f'model_{i}']
+                )
+            elif lang == 'R':
+                model = load_r_model(
+                    r6b,
+                    r,
+                    model_name,
+                    str(upstream[f'{model_name}_fit'][f'model_{i}'])
+                )
+                # convert pandas dataframe to R dataframe
+                pandas2ri.activate()
+                X_test = pandas2ri.py2rpy_pandasdataframe(
+                    X_test
+                )
+                pandas2ri.deactivate()
 
             # predict
-            preds = model.predict(X_test)
+            preds = model.predict(X_test, quantile_intervals)
+
+            if lang == 'R':
+            # convert to pandas dataframe
+                pandas2ri.activate()
+                preds = robjects.conversion.rpy2py(preds)
+                pandas2ri.deactivate()
+
+            # append fold predictions to predictions set
             predictions.append(preds)
         # save data for next process
         feather.write_dataframe(
             pandas.concat(predictions),
             product['predictions']
         )
+        
 
+def load_python_model(models, model_name, path):
+    model_class = getattr(models, model_name)
+    model = model_class()
+    model.load(path)
+    return model
 
-def predict_r(upstream, product, model_name, split_type, n_folds=10):
-    # format variable
-    upstream = dict(upstream)
-
-    # imports
-    import rpy2.robjects as robjects
-    from rpy2.robjects import pandas2ri
-    import rpy2_r6.r6b as r6b
-    r = robjects.r
-    r['source']('models.R')
-
-    if split_type == 'train_test':
-        # load data from upstream process
-        pandas2ri.activate()
-        X_test = pandas2ri.py2rpy_pandasdataframe(
-            feather.read_dataframe(
-                upstream['split_data']['test_X_data']
-            )
-        )
-        pandas2ri.deactivate()
-        del upstream['split_data']
-
-        # load model from upstream process
-        model_class = r6b.R6DynamicClassGenerator(r[model_name])
-        model = model_class.new()
-        model.load(str(next(iter(upstream.values()))['model']))
 
-        # predict
-        preds = model.predict(X_test)
-        # convert to pandas DF
-        pandas2ri.activate()
-        preds = robjects.conversion.rpy2py(preds)
-        pandas2ri.deactivate()
-
-        # save data for next process
-        feather.write_dataframe(preds, product['predictions'])
-    elif split_type == 'k_fold':
-        predictions = []
-        for i in range(1, n_folds+1):
-            # load data from upstream process
-            pandas2ri.activate()
-            X_test = pandas2ri.py2rpy_pandasdataframe(
-                feather.read_dataframe(
-                    upstream['split_data'][f'fold_{i}_X_data']
-                )
-            )
-            pandas2ri.deactivate()
-
-            # load model from upstream process
-            model_class = r6b.R6DynamicClassGenerator(r[model_name])
-            model = model_class.new()
-            model.load(str(upstream[f'{model_name}_fit'][f'model_{i}']))
-
-            # predict
-            preds = model.predict(X_test)
-            # convert to pandas DF
-            pandas2ri.activate()
-            preds = robjects.conversion.rpy2py(preds)
-            pandas2ri.deactivate()
-            predictions.append(preds)
-        # save data for next process
-        feather.write_dataframe(
-            pandas.concat(predictions),
-            product['predictions']
-        )
+def load_r_model(r6b, r, model_name, path):
+    model_class = r6b.R6DynamicClassGenerator(r[model_name])
+    model = model_class.new()
+    model.load(path)
+    return model
```

### Comparing `mvf-0.0.4/mvf/process/split_data.py` & `mvf-0.0.5/mvf/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.4/mvf/process/validate.py` & `mvf-0.0.5/mvf/process/validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 del upstream['split_data']
 
 # load predictions from upstream
 predictions = {}
 for model_name, p in upstream.items():
     predictions[model_name] = feather.read_dataframe(p['predictions'])
 
-# + papermill={"duration": 0.011862, "end_time": "2023-06-22T11:34:46.373683", "exception": false, "start_time": "2023-06-22T11:34:46.361821", "status": "completed"}
 # error
 error_df = pandas.DataFrame()
 # mse
 for model, preds in predictions.items():
-    error_df.loc[model, 'MSE'] = mean_squared_error(ground_truth, preds)
+    mean_preds = preds['predictions']
+    error_df.loc[model, 'MSE'] = mean_squared_error(ground_truth, mean_preds)
 
 error_df
```

### Comparing `mvf-0.0.4/mvf/process/validate_model_r.py` & `mvf-0.0.5/mvf/process/validate_model_r.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 r['source']('models.R')
 
 # + tags=["parameters"]
 upstream = None
 product = None
 model_name = ''
 split_type = ''
+n_folds = 10
 # -
 
 # load model class
 model_class = r6b.R6DynamicClassGenerator(r[model_name])
 
 # run validation
 if split_type == 'train_test':
```

### Comparing `mvf-0.0.4/mvf.egg-info/PKG-INFO` & `mvf-0.0.5/mvf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.4/mvf.egg-info/SOURCES.txt` & `mvf-0.0.5/mvf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,9 +30,8 @@
 mvf/integration/process/validate.py
 mvf/integration/process/validate_model.py
 mvf/process/__init__.py
 mvf/process/fit_model.py
 mvf/process/predict_model.py
 mvf/process/split_data.py
 mvf/process/validate.py
-mvf/process/validate_model_r.py
-test/test_build_dag.py
+mvf/process/validate_model_r.py
```

### Comparing `mvf-0.0.4/setup.py` & `mvf-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         'schema',
         'scikit-learn',
     ],
     extras_require={
         'dev': [
             'coverage',
             'pytest',
+            'testbook',
             'twine',
         ]
     },
     keywords=[
         'python',
         'R',
         'machine learning',
```

