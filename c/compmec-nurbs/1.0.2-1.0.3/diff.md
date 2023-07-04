# Comparing `tmp/compmec_nurbs-1.0.2.tar.gz` & `tmp/compmec_nurbs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compmec_nurbs-1.0.2.tar", max compression
+gzip compressed data, was "compmec_nurbs-1.0.3.tar", max compression
```

## Comparing `compmec_nurbs-1.0.2.tar` & `compmec_nurbs-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35142 2022-12-11 01:01:19.314696 compmec_nurbs-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1846 2022-12-11 01:01:19.314696 compmec_nurbs-1.0.2/README.md
--rw-r--r--   0        0        0      543 2022-12-11 01:01:19.314696 compmec_nurbs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3180 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/__classes__.py
--rw-r--r--   0        0        0      232 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/__init__.py
--rw-r--r--   0        0        0    31998 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/algorithms.py
--rw-r--r--   0        0        0     9471 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/basefunctions.py
--rw-r--r--   0        0        0    14321 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/curves.py
--rw-r--r--   0        0        0    11098 2022-12-11 01:01:19.318696 compmec_nurbs-1.0.2/src/compmec/nurbs/knotspace.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.2/setup.py
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35142 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1846 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/README.md
+-rw-r--r--   0        0        0      543 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3063 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/src/compmec/nurbs/__classes__.py
+-rw-r--r--   0        0        0      220 2023-07-04 19:15:02.366392 compmec_nurbs-1.0.3/src/compmec/nurbs/__init__.py
+-rw-r--r--   0        0        0    10541 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/algorithms.py
+-rw-r--r--   0        0        0    12759 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/curves.py
+-rw-r--r--   0        0        0     8233 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/functions.py
+-rw-r--r--   0        0        0     8362 2023-07-04 19:15:02.370392 compmec_nurbs-1.0.3/src/compmec/nurbs/knotspace.py
+-rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.3/PKG-INFO
```

### Comparing `compmec_nurbs-1.0.2/LICENSE.md` & `compmec_nurbs-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compmec_nurbs-1.0.2/README.md` & `compmec_nurbs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `compmec_nurbs-1.0.2/pyproject.toml` & `compmec_nurbs-1.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compmec-nurbs"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 readme = "README.md"
 authors = ["Carlos Adir <carlos.adir@gmail.com>"]
 packages = [{ include = "compmec/nurbs", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `compmec_nurbs-1.0.2/src/compmec/nurbs/__classes__.py` & `compmec_nurbs-1.0.3/src/compmec/nurbs/__classes__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 from typing import Any, Optional, Tuple, Union
 
 import numpy as np
 
 
-class Interface_KnotVector(abc.ABC):
+class Intface_KnotVector(abc.ABC):
     @abc.abstractproperty
     def degree(self) -> int:
         raise NotImplementedError
 
     @abc.abstractproperty
     def npts(self) -> int:
         raise NotImplementedError
@@ -18,54 +18,55 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def verify_valid_span(self, u: Tuple[float]):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def span(self, u: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
+    def span(self, knot: np.ndarray) -> np.ndarray:
         raise NotImplementedError
 
     @abc.abstractmethod
     def insert_knot(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
     @abc.abstractmethod
     def remove_knot(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
     @abc.abstractmethod
     def __eq__(self, obj: object) -> bool:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def __ne__(self, obj: object) -> bool:
-        return not self.__eq__(obj)
+        raise NotImplementedError
 
 
-class Interface_BaseFunction_Evaluator_BaseCurve(abc.ABC):
+class Intface_BaseFunction_Evaluator_BaseCurve(abc.ABC):
     @abc.abstractproperty
-    def knotvector(self) -> Interface_KnotVector:
+    def knotvector(self) -> Intface_KnotVector:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __call__(self, u: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def __call__(self, u: np.ndarray) -> np.ndarray:
         raise NotImplementedError
 
 
-class Interface_Evaluator(Interface_BaseFunction_Evaluator_BaseCurve):
+class Intface_Evaluator(Intface_BaseFunction_Evaluator_BaseCurve):
     @abc.abstractproperty
     def first_index(self) -> Union[int, slice]:
         raise NotImplementedError
 
     @abc.abstractproperty
-    def first_index(self) -> Union[int, slice]:
+    def second_index(self) -> Union[int, slice]:
         raise NotImplementedError
 
 
-class Interface_BaseFunction_BaseCurve(Interface_BaseFunction_Evaluator_BaseCurve):
+class Intface_BaseFunction_BaseCurve(Intface_BaseFunction_Evaluator_BaseCurve):
     @abc.abstractproperty
     def degree(self) -> int:
         raise NotImplementedError
 
     @abc.abstractproperty
     def npts(self) -> int:
         raise NotImplementedError
@@ -74,41 +75,38 @@
     def knot_insert(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
     @abc.abstractmethod
     def knot_remove(self, knot: float, times: Optional[int] = 1):
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def derivate(self):
-        raise NotImplementedError
-
 
-class Interface_BaseFunction(Interface_BaseFunction_BaseCurve):
+class Intface_BaseFunction(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
-    def __init__(self, knotvector: Interface_KnotVector):
+    def __init__(self, knotvector: Intface_KnotVector):
         raise NotImplementedError
 
     @abc.abstractmethod
     def __getitem__(self, tup: Any) -> Union[float, np.ndarray]:
         raise NotImplementedError
 
 
-class Interface_BaseCurve(Interface_BaseFunction_BaseCurve):
+class Intface_BaseCurve(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
-    def __init__(self, knotvector: Interface_KnotVector, ctrlpoints: np.ndarray):
+    def __init__(self, knotvector: Intface_KnotVector, ctrlpoints: np.ndarray):
         raise NotImplementedError
 
     @abc.abstractproperty
-    def F(self) -> Interface_BaseFunction:
+    def F(self) -> Intface_BaseFunction:
         raise NotImplementedError
 
     @abc.abstractproperty
     def ctrlpoints(self) -> np.ndarray:
         raise NotImplementedError
 
     @abc.abstractmethod
     def __eq__(self, obj: object) -> bool:
         raise NotImplementedError
 
+    @abc.abstractmethod
     def __ne__(self, obj: object) -> bool:
-        return not self.__eq__(obj)
+        raise NotImplementedError
```

### Comparing `compmec_nurbs-1.0.2/src/compmec/nurbs/basefunctions.py` & `compmec_nurbs-1.0.3/src/compmec/nurbs/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,18 @@
 import abc
-from typing import Any, Iterable, Optional, Tuple, Type, Union
+from typing import Any, Optional, Tuple, Union
 
 import numpy as np
 
-from compmec.nurbs.__classes__ import Interface_BaseFunction, Interface_Evaluator
+from compmec.nurbs.__classes__ import Intface_BaseFunction, Intface_Evaluator
+from compmec.nurbs.algorithms import N, R
 from compmec.nurbs.knotspace import KnotVector
 
 
-def N(i: int, j: int, k: int, u: float, U: KnotVector) -> float:
-    """
-    Returns the value of N_{ij}(u) in the interval [u_{k}, u_{k+1}]
-    Remember that N_{i, j}(u) = 0   if  ( u not in [U[i], U[i+j+1]] )
-    """
-
-    npts, degree = U.npts, U.degree
-
-    if k < i:
-        return 0
-    if j == 0:
-        if i == k:
-            return 1
-        if i + 1 == npts and k == npts:
-            return 1
-        return 0
-    if i + j < k:
-        return 0
-
-    if U[i] == U[i + j]:
-        factor1 = 0
-    else:
-        factor1 = (u - U[i]) / (U[i + j] - U[i])
-
-    if U[i + j + 1] == U[i + 1]:
-        factor2 = 0
-    else:
-        factor2 = (U[i + j + 1] - u) / (U[i + j + 1] - U[i + 1])
-
-    result = factor1 * N(i, j - 1, k, u, U) + factor2 * N(i + 1, j - 1, k, u, U)
-    return result
-
-
-def R(i: int, j: int, k: int, u: float, U: KnotVector, w: Tuple[float]) -> float:
-    """
-    Returns the value of R_{ij}(u) in the interval [u_{k}, u_{k+1}]
-    """
-    Niju = N(i, j, k, u, U)
-    if Niju == 0:
-        return 0
-    npts = len(w)
-    soma = 0
-    for z in range(npts):
-        soma += w[z] * N(z, j, k, u, U)
-    return w[i] * Niju / soma
-
-
-class BaseFunction(Interface_BaseFunction):
+class BaseFunction(Intface_BaseFunction):
     def __init__(self, knotvector: KnotVector):
         self.__U = KnotVector(knotvector)
 
     @property
     def degree(self) -> int:
         return self.__U.degree
 
@@ -66,22 +20,26 @@
     def npts(self) -> int:
         return self.__U.npts
 
     @property
     def knotvector(self) -> KnotVector:
         return self.__U
 
+    @property
+    def knots(self) -> Tuple[float]:
+        return self.__U.knots
+
     def knot_insert(self, knot: float, times: Optional[int] = 1):
         self.knotvector.knot_insert(knot, times)
 
     def knot_remove(self, knot: float, times: Optional[int] = 1):
         self.knotvector.knot_remove(knot, times)
 
 
-class BaseEvaluator(Interface_Evaluator):
+class BaseEvaluator(Intface_Evaluator):
     def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
         self.__U = F.knotvector
         self.__first_index = i
         self.__second_index = j
         self.__A = F.A
 
     @property
@@ -130,15 +88,15 @@
         if i is slice, u is np.ndarray, ndim = k -> np.ndarray, ndim = k+1
         """
         u = np.array(u, dtype="float64")
         span = self.__U.span(u)
         span = np.array(span, dtype="int16")
         return self.compute_all(u, span)
 
-    def __call__(self, u: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def __call__(self, u: np.ndarray) -> np.ndarray:
         result = self.evalf(u)
         result = self.__A @ result
         return result[self.first_index]
 
 
 class SplineEvaluatorClass(BaseEvaluator):
     def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
@@ -150,15 +108,18 @@
 
 class RationalEvaluatorClass(BaseEvaluator):
     def __init__(self, F: BaseFunction, i: Union[int, slice], j: int):
         super().__init__(F, i, j)
         self.__weights = F.weights
 
     def compute_one_value(self, i: int, u: float, span: int) -> float:
-        return R(i, self.second_index, span, u, self.knotvector, self.__weights)
+        j = self.second_index
+        U = self.knotvector
+        w = self.__weights
+        return R(i, j, span, u, U, w)
 
 
 class BaseFunctionDerivable(BaseFunction):
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
         self.__q = self.degree
         self.__A = np.eye(self.npts, dtype="float64")
@@ -197,15 +158,16 @@
             if not (-self.npts <= index < self.npts):
                 raise IndexError
 
     def __valid_second_index(self, index: int):
         if not isinstance(index, int):
             raise TypeError
         if not (0 <= index <= self.degree):
-            error_msg = f"Second index (={index}) must be in [0, {self.degree}]"
+            error_msg = f"Second index (={index}) "
+            error_msg += f"must be in [0, {self.degree}]"
             raise IndexError(error_msg)
 
     @abc.abstractmethod
     def create_evaluator_instance(self, i: Union[int, slice], j: int):
         raise NotImplementedError
 
     def __getitem__(self, tup: Any):
@@ -215,30 +177,30 @@
             i, j = tup
         else:
             i, j = tup, self.q
         self.__valid_first_index(i)
         self.__valid_second_index(j)
         return self.create_evaluator_instance(i, j)
 
-    def __call__(self, u: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def __call__(self, u: np.ndarray) -> np.ndarray:
         i, j = slice(None, None, None), self.degree
         evaluator = self.create_evaluator_instance(i, j)
         return evaluator(u)
 
     def __eq__(self, obj: object) -> bool:
         if type(self) != type(obj):
             raise TypeError
         if self.knotvector != obj.knotvector:
             return False
         if self.q != obj.q:
             return False
         return True
 
 
-class SplineBaseFunction(BaseFunctionGetItem):
+class SplineFunction(BaseFunctionGetItem):
     def __doc__(self):
         """
         This function is recursively determined like
 
         N_{i, 0}(u) = { 1   if  knotvector[i] <= u < knotvector[i+1]
                       { 0   else
 
@@ -258,15 +220,15 @@
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
 
     def create_evaluator_instance(self, i: Union[int, slice], j: int):
         return SplineEvaluatorClass(self, i, j)
 
 
-class RationalBaseFunction(BaseFunctionGetItem):
+class RationalFunction(BaseFunctionGetItem):
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
 
     def create_evaluator_instance(self, i: Union[int, slice], j: int):
         return RationalEvaluatorClass(self, i, j)
 
     def __eq__(self, obj):
@@ -276,27 +238,22 @@
             return False
         return True
 
     @property
     def weights(self):
         try:
             return self.__weights
-        except AttributeError as e:
+        except AttributeError:
             self.__weights = np.ones(self.npts, dtype="float64")
         return self.__weights
 
     @weights.setter
     def weights(self, value: Tuple[float]):
-        try:
-            value = np.array(value, dtype="float64")
-        except Exception as e:
-            raise TypeError(f"Input is not valid. Type = {type(value)}, not np.ndarray")
+        value = np.array(value, dtype="float64")
         if value.ndim != 1:
-            raise ValueError(f"Input must be 1D array")
+            raise ValueError("Input must be 1D array")
         if len(value) != self.npts:
-            raise ValueError(
-                f"Input must have same number of points as knotvector.npts"
-            )
-        value = np.array(value, dtype="float64")
+            error_msg = "Lenght of weights must be equal to knotvector.npts"
+            raise ValueError(error_msg)
         if np.any(value <= 0):
             raise ValueError("All the weights must be positive")
         self.__weights = value
```

### Comparing `compmec_nurbs-1.0.2/PKG-INFO` & `compmec_nurbs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compmec-nurbs
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Carlos Adir
 Author-email: carlos.adir@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

