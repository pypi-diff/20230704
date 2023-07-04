# Comparing `tmp/pyparc-2.0.3.tar.gz` & `tmp/pyparc-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparc-2.0.3.tar", last modified: Sat Jul  1 07:18:04 2023, max compression
+gzip compressed data, was "pyparc-2.0.4.tar", last modified: Tue Jul  4 12:24:14 2023, max compression
```

## Comparing `pyparc-2.0.3.tar` & `pyparc-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548613 pyparc-2.0.3/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.3/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:18:04.548488 pyparc-2.0.3/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)     3894 2023-07-01 06:50:16.000000 pyparc-2.0.3/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      827 2023-07-01 07:16:56.000000 pyparc-2.0.3/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-01 07:18:04.548654 pyparc-2.0.3/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.546802 pyparc-2.0.3/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.547584 pyparc-2.0.3/src/pyparc/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.3/src/pyparc/__init__.py
--rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.3/src/pyparc/parc.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548199 pyparc-2.0.3/src/pyparc.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      266 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       66 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        7 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548318 pyparc-2.0.3/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.3/tests/test_parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-04 12:24:14.622994 pyparc-2.0.4/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.4/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)     4522 2023-07-04 12:24:14.622872 pyparc-2.0.4/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)     3892 2023-07-01 14:40:32.000000 pyparc-2.0.4/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      832 2023-07-04 12:19:48.000000 pyparc-2.0.4/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-04 12:24:14.623033 pyparc-2.0.4/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-04 12:24:14.620684 pyparc-2.0.4/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-04 12:24:14.621320 pyparc-2.0.4/src/pyparc/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.4/src/pyparc/__init__.py
+-rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.4/src/pyparc/parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-04 12:24:14.622559 pyparc-2.0.4/src/pyparc.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)     4522 2023-07-04 12:24:14.000000 pyparc-2.0.4/src/pyparc.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      266 2023-07-04 12:24:14.000000 pyparc-2.0.4/src/pyparc.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-04 12:24:14.000000 pyparc-2.0.4/src/pyparc.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       71 2023-07-04 12:24:14.000000 pyparc-2.0.4/src/pyparc.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        7 2023-07-04 12:24:14.000000 pyparc-2.0.4/src/pyparc.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-04 12:24:14.622685 pyparc-2.0.4/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.4/tests/test_parc.py
```

### Comparing `pyparc-2.0.3/LICENSE.txt` & `pyparc-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.3/PKG-INFO` & `pyparc-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.3
+Version: 2.0.4
 Summary: PARC - Piecewise Affine Regression and Classification
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/parc
 Keywords: piecewise linear regression,piecewise linear classification,multivariate regression,multivariate classification,supervised learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,17 +51,16 @@
 pip install pyparc
 ~~~
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 Say we want to fit a piecewise affine model on a dataset of 1000 samples $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$ 
-$$
-	y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2
-$$
+
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig4.png" alt="drawing" width=55%/>
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig1.png" alt="drawing" width=40%/>
 
 
 We use 80% of the data for training (`X_train`,`Y_train`) and 20% for testing the model (`X_test`,`Y_test`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.3 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.4 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 computation for piecewise linear separation 2. Assigning the training points to
 different clusters on the basis of a criterion that balances prediction
 accuracy and piecewise-linear separability. For earlier Python versions of the
 code, see here.  ## Installation ~~~python pip install pyparc ~~~  ## Basic
 usage Say we want to fit a piecewise affine model on a dataset of 1000 samples
 $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated
 between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$
-$$ y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2 $$
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 [drawing] [drawing] We use 80% of the data for training (`X_train`,`Y_train`)
 and 20% for testing the model (`X_test`,`Y_test`). We want to train a piecewise
 affine model on a polyhedral partition with maximum 10 regions, with $\ell_2$-
 regularization coefficient $\alpha=10^{-4}$ and maximum 15 block-coordinate
 descent iterations of the algorithm: ~~~python from parc.parc import PARC
 predictor = PARC(K=10, alpha=1.0e-4, maxiter=15) # initialize PARC object
 categorical = False # targets are numeric # fit piecewise linear predictor
```

### Comparing `pyparc-2.0.3/README.md` & `pyparc-2.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 pip install pyparc
 ~~~
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 Say we want to fit a piecewise affine model on a dataset of 1000 samples $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$ 
-$$
-	y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2
-$$
+
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig4.png" alt="drawing" width=55%/>
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig1.png" alt="drawing" width=40%/>
 
 
 We use 80% of the data for training (`X_train`,`Y_train`) and 20% for testing the model (`X_test`,`Y_test`).
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
 computation for piecewise linear separation 2. Assigning the training points to
 different clusters on the basis of a criterion that balances prediction
 accuracy and piecewise-linear separability. For earlier Python versions of the
 code, see here.  ## Installation ~~~python pip install pyparc ~~~  ## Basic
 usage Say we want to fit a piecewise affine model on a dataset of 1000 samples
 $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated
 between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$
-$$ y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2 $$
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 [drawing] [drawing] We use 80% of the data for training (`X_train`,`Y_train`)
 and 20% for testing the model (`X_test`,`Y_test`). We want to train a piecewise
 affine model on a polyhedral partition with maximum 10 regions, with $\ell_2$-
 regularization coefficient $\alpha=10^{-4}$ and maximum 15 block-coordinate
 descent iterations of the algorithm: ~~~python from parc.parc import PARC
 predictor = PARC(K=10, alpha=1.0e-4, maxiter=15) # initialize PARC object
 categorical = False # targets are numeric # fit piecewise linear predictor
```

### Comparing `pyparc-2.0.3/pyproject.toml` & `pyparc-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyparc"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PARC - Piecewise Affine Regression and Classification"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["numpy","scipy","sklearn","matplotlib","pypoman","mip","faiss-cpu","pickle-mixin"]
+dependencies = ["numpy","scipy","scikit-learn","matplotlib","pypoman","mip","faiss-cpu","pickle-mixin"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["piecewise linear regression", "piecewise linear classification",
     "multivariate regression", "multivariate classification", "supervised learning"]
```

### Comparing `pyparc-2.0.3/src/pyparc/parc.py` & `pyparc-2.0.4/src/pyparc/parc.py`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.3/src/pyparc.egg-info/PKG-INFO` & `pyparc-2.0.4/src/pyparc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.3
+Version: 2.0.4
 Summary: PARC - Piecewise Affine Regression and Classification
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/parc
 Keywords: piecewise linear regression,piecewise linear classification,multivariate regression,multivariate classification,supervised learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,17 +51,16 @@
 pip install pyparc
 ~~~
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 Say we want to fit a piecewise affine model on a dataset of 1000 samples $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$ 
-$$
-	y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2
-$$
+
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig4.png" alt="drawing" width=55%/>
 <img src="http://cse.lab.imtlucca.it/~bemporad/parc/fig1.png" alt="drawing" width=40%/>
 
 
 We use 80% of the data for training (`X_train`,`Y_train`) and 20% for testing the model (`X_test`,`Y_test`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.3 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.4 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 computation for piecewise linear separation 2. Assigning the training points to
 different clusters on the basis of a criterion that balances prediction
 accuracy and piecewise-linear separability. For earlier Python versions of the
 code, see here.  ## Installation ~~~python pip install pyparc ~~~  ## Basic
 usage Say we want to fit a piecewise affine model on a dataset of 1000 samples
 $(x,y)$, where $x=(x_1,x_2)$ has two numeric components randomly generated
 between 0 and 1, and $y$ is obtained by the following nonlinear function of $x$
-$$ y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2 $$
+$$y(x_1,x_2)=\sin\left(4x_{1}-5\left(x_{2}-\frac{1}{2}\right)^2\right)+2x_2$$
 [drawing] [drawing] We use 80% of the data for training (`X_train`,`Y_train`)
 and 20% for testing the model (`X_test`,`Y_test`). We want to train a piecewise
 affine model on a polyhedral partition with maximum 10 regions, with $\ell_2$-
 regularization coefficient $\alpha=10^{-4}$ and maximum 15 block-coordinate
 descent iterations of the algorithm: ~~~python from parc.parc import PARC
 predictor = PARC(K=10, alpha=1.0e-4, maxiter=15) # initialize PARC object
 categorical = False # targets are numeric # fit piecewise linear predictor
```

### Comparing `pyparc-2.0.3/tests/test_parc.py` & `pyparc-2.0.4/tests/test_parc.py`

 * *Files identical despite different names*

