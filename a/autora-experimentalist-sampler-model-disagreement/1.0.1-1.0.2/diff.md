# Comparing `tmp/autora-experimentalist-sampler-model-disagreement-1.0.1.tar.gz` & `tmp/autora-experimentalist-sampler-model-disagreement-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-model-disagreement-1.0.1.tar", last modified: Wed May 31 18:18:22 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-model-disagreement-1.0.2.tar", last modified: Mon Jul  3 22:18:58 2023, max compression
```

## Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1.tar` & `autora-experimentalist-sampler-model-disagreement-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   154072 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/test_model_disagreement_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.138788 autora-experimentalist-sampler-model-disagreement-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.122788 autora-experimentalist-sampler-model-disagreement-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.130788 autora-experimentalist-sampler-model-disagreement-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-03 22:18:58.138788 autora-experimentalist-sampler-model-disagreement-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.130788 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   130647 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.130788 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.130788 autora-experimentalist-sampler-model-disagreement-1.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:18:58.138788 autora-experimentalist-sampler-model-disagreement-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.126788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.122788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.122788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.122788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.130788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/experimentalist/sampler/model_disagreement/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/experimentalist/sampler/model_disagreement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.134788 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-03 22:18:58.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-03 22:18:58.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:18:58.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 22:18:58.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 22:18:58.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:58.138788 autora-experimentalist-sampler-model-disagreement-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 22:18:45.000000 autora-experimentalist-sampler-model-disagreement-1.0.2/tests/test_model_disagreement_sampler.py
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-model-disagreement-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/.gitignore` & `autora-experimentalist-sampler-model-disagreement-1.0.2/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -63,7 +63,10 @@
 
 # Material for MkDocs
 site/
 docs/reference/
 
 # Jupyter Notebook load data
 .ipynb_checkpoints
+
+# IDE Files
+/.idea/
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/.pre-commit-config.yaml` & `autora-experimentalist-sampler-model-disagreement-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-model-disagreement
-Version: 1.0.1
+Version: 1.0.2
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -19,15 +19,15 @@
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -36,9 +36,9 @@
 #Theorists
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
-X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
+X_new = model_disagreement_sample(X, [bms_theorist, darts_theorist], n)
 ```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/README.md` & `autora-experimentalist-sampler-model-disagreement-1.0.2/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# AutoRA Model Disagreement Sampler
+# Model Disagreement Sampler
 
 The model disagreement sampler identifies experimental conditions $\vec{x}' \in X'$ with respect to
 a pairwise distance metric between theorist models, $P_{M_{i}}(\hat{y}, \vec{x}')$:
 
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -23,9 +23,9 @@
 #Theorists
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
-X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
+X_new = model_disagreement_sample(X, [bms_theorist, darts_theorist], n)
 ```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/docs/index.md` & `autora-experimentalist-sampler-model-disagreement-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Model Disagreement Sampler
+# AutoRA Model Disagreement Sampler
 
 The model disagreement sampler identifies experimental conditions $\vec{x}' \in X'$ with respect to
 a pairwise distance metric between theorist models, $P_{M_{i}}(\hat{y}, \vec{x}')$:
 
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -23,9 +23,9 @@
 #Theorists
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
-X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
-```
+X_new = model_disagreement_sample(X, [bms_theorist, darts_theorist], n)
+```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/base.yml` & `autora-experimentalist-sampler-model-disagreement-1.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/pyproject.toml` & `autora-experimentalist-sampler-model-disagreement-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
-    "autora-core",
+    "autora-core>=3.1.0",
     "scikit-learn",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/__init__.py` & `autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora/experimentalist/sampler/model_disagreement/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import itertools
 from typing import Iterable, List
 import numpy as np
 
-def model_disagreement_sampler(X: np.array, models: List, num_samples: int = 1):
+from autora.utils.deprecation import deprecated_alias
+
+def model_disagreement_sample(condition_pool: np.array, models: List, num_samples: int = 1):
     """
     A sampler that returns selected samples for independent variables
     for which the models disagree the most in terms of their predictions.
 
     Args:
         X: pool of IV conditions to evaluate in terms of model disagreement
         models: List of Scikit-learn (regression or classification) models to compare
         num_samples: number of samples to select
 
     Returns: Sampled pool
     """
 
-    if isinstance(X, Iterable):
-        X = np.array(list(X))
+    if isinstance(condition_pool, Iterable):
+        condition_pool = np.array(list(condition_pool))
 
-    X_predict = np.array(X)
+    X_predict = np.array(condition_pool)
     if len(X_predict.shape) == 1:
         X_predict = X_predict.reshape(-1, 1)
 
     model_disagreement = list()
 
     # collect diagreements for each model pair
     for model_a, model_b in itertools.combinations(models, 2):
@@ -57,8 +59,10 @@
 
     # sum up all model disagreements
     summed_disagreement = np.sum(model_disagreement, axis=0)
 
     # sort the summed disagreements and select the top n
     idx = (-summed_disagreement).argsort()[:num_samples]
 
-    return X[idx]
+    return X[idx]
+
+model_disagreement_sampler = deprecated_alias(model_disagreement_sample, "model_disagreement_sampler")
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-model-disagreement
-Version: 1.0.1
+Version: 1.0.2
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -19,15 +19,15 @@
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -36,9 +36,9 @@
 #Theorists
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
-X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
+X_new = model_disagreement_sample(X, [bms_theorist, darts_theorist], n)
 ```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-model-disagreement-1.0.2/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/tests/README.md` & `autora-experimentalist-sampler-model-disagreement-1.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.1/tests/test_model_disagreement_sampler.py` & `autora-experimentalist-sampler-model-disagreement-1.0.2/tests/test_model_disagreement_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sample
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 def test_output_dimensions():
     #Meta-Setup
     X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
@@ -13,11 +13,11 @@
     bms_theorist = BMSRegressor()
     darts_theorist = DARTSRegressor()
     
     bms_theorist.fit(X,y)
     darts_theorist.fit(X,y)
 
     #Sampler
-    X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
+    X_new = model_disagreement_sample(X, [bms_theorist, darts_theorist], n)
 
     # Check that the sampler returns n experiment conditions
-    assert X_new.shape == (n, X.shape[1])
+    assert X_new.shape == (n, X.shape[1])
```

