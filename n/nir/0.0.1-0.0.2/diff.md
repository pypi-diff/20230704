# Comparing `tmp/nir-0.0.1.tar.gz` & `tmp/nir-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nir-0.0.1.tar", last modified: Sun Jul  2 02:03:13 2023, max compression
+gzip compressed data, was "nir-0.0.2.tar", last modified: Tue Jul  4 21:52:06 2023, max compression
```

## Comparing `nir-0.0.1.tar` & `nir-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jens      (1000) users      (100)        0 2023-07-02 02:03:13.590662 nir-0.0.1/
--rw-r--r--   0 jens      (1000) users      (100)     2872 2023-07-02 02:03:13.590662 nir-0.0.1/PKG-INFO
--rw-r--r--   0 jens      (1000) users      (100)     1816 2023-07-01 21:30:28.000000 nir-0.0.1/README.md
-drwxr-xr-x   0 jens      (1000) users      (100)        0 2023-07-02 02:03:13.589661 nir-0.0.1/nir/
--rw-r--r--   0 jens      (1000) users      (100)       59 2023-07-02 00:15:07.000000 nir-0.0.1/nir/__init__.py
--rw-r--r--   0 jens      (1000) users      (100)     2252 2023-07-02 01:32:13.000000 nir-0.0.1/nir/ir.py
--rw-r--r--   0 jens      (1000) users      (100)     2215 2023-07-02 01:39:01.000000 nir-0.0.1/nir/read.py
-drwxr-xr-x   0 jens      (1000) users      (100)        0 2023-07-02 02:03:13.590662 nir-0.0.1/nir/test/
--rw-r--r--   0 jens      (1000) users      (100)      221 2023-07-02 01:29:08.000000 nir-0.0.1/nir/test/test_ir.py
--rw-r--r--   0 jens      (1000) users      (100)      967 2023-07-02 01:42:55.000000 nir-0.0.1/nir/test/test_readwrite.py
--rw-r--r--   0 jens      (1000) users      (100)     2351 2023-07-02 01:31:53.000000 nir-0.0.1/nir/write.py
-drwxr-xr-x   0 jens      (1000) users      (100)        0 2023-07-02 02:03:13.590662 nir-0.0.1/nir.egg-info/
--rw-r--r--   0 jens      (1000) users      (100)     2872 2023-07-02 02:03:13.000000 nir-0.0.1/nir.egg-info/PKG-INFO
--rw-r--r--   0 jens      (1000) users      (100)      256 2023-07-02 02:03:13.000000 nir-0.0.1/nir.egg-info/SOURCES.txt
--rw-r--r--   0 jens      (1000) users      (100)        1 2023-07-02 02:03:13.000000 nir-0.0.1/nir.egg-info/dependency_links.txt
--rw-r--r--   0 jens      (1000) users      (100)       11 2023-07-02 02:03:13.000000 nir-0.0.1/nir.egg-info/requires.txt
--rw-r--r--   0 jens      (1000) users      (100)        9 2023-07-02 02:03:13.000000 nir-0.0.1/nir.egg-info/top_level.txt
--rw-r--r--   0 jens      (1000) users      (100)     1299 2023-07-02 02:03:03.000000 nir-0.0.1/pyproject.toml
--rw-r--r--   0 jens      (1000) users      (100)       38 2023-07-02 02:03:13.590662 nir-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:52:06.380658 nir-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-04 21:52:06.380658 nir-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-04 21:51:58.000000 nir-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:52:06.380658 nir-0.0.2/nir/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 21:51:58.000000 nir-0.0.2/nir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-04 21:51:58.000000 nir-0.0.2/nir/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-04 21:51:58.000000 nir-0.0.2/nir/read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:52:06.380658 nir-0.0.2/nir/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-04 21:51:58.000000 nir-0.0.2/nir/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-04 21:51:58.000000 nir-0.0.2/nir/test/test_readwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-04 21:51:58.000000 nir-0.0.2/nir/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 21:52:06.380658 nir-0.0.2/nir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-04 21:52:06.000000 nir-0.0.2/nir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 21:52:06.000000 nir-0.0.2/nir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 21:52:06.000000 nir-0.0.2/nir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 21:52:06.000000 nir-0.0.2/nir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 21:52:06.000000 nir-0.0.2/nir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-04 21:51:58.000000 nir-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 21:52:06.380658 nir-0.0.2/setup.cfg
```

### Comparing `nir-0.0.1/nir/ir.py` & `nir-0.0.2/nir/ir.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 import typing
 
 import numpy as np
 
 
-Edges = typing.NewType("Edges", list[typing.Tuple[int, int]])
+Edges = typing.NewType("Edges", typing.List[typing.Tuple[int, int]])
 
 
 @dataclass
 class NIR:
     """Neural Intermediate Representation (NIR)"""
 
     nodes: typing.List[typing.Any]  # List of computational nodes
@@ -43,31 +43,31 @@
 class LIF(NIRNode):
     """Leaky integrate and-fire-neuron model.
 
     The leaky integrate-and-fire neuron model is defined by the following equations:
     $$
     \tau \dot{v} = (v_{leak} - v) + R I
     z = \being{cases}
-        1 & v > theta \\
+        1 & v > v_th \\
         0 & else
     \end{cases}
     v = \begin{cases}
-        v-theta & z=1 \\
+        v-v_{th} & z=1 \\
         v & else
     \end{cases}
     $$
     Where $\tau$ is the time constant, $v$ is the membrane potential,
-    $v_{leak}$ is the leak voltage, $R$ is the resistance, $theta$ is
+    $v_{leak}$ is the leak voltage, $R$ is the resistance, $v_th$ is
     the firing threshold, and $I$ is the input current.
     """
 
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
-    theta: np.ndarray  # Firing threshold
+    v_th: np.ndarray  # Firing threshold
 
 
 @dataclass
 class Linear(NIRNode):
 
     weights: np.ndarray  # Weights M * N
     bias: np.ndarray  # Bias M
```

### Comparing `nir-0.0.1/nir/read.py` & `nir-0.0.2/nir/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 )
             elif node["type"][()] == b"LIF":
                 nodes.append(
                     nir.LIF(
                         tau=node["tau"][()],
                         r=node["r"][()],
                         v_leak=node["v_leak"][()],
-                        theta=node["theta"][()],
+                        v_th=node["v_th"][()],
                     )
                 )
             elif node["type"][()] == b"Linear":
                 nodes.append(
                     nir.Linear(
                         weights=node["weights"][()],
                         bias=node["bias"][()],
```

### Comparing `nir-0.0.1/nir/test/test_readwrite.py` & `nir-0.0.2/nir/test/test_readwrite.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,11 +28,11 @@
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
 
 def test_leaky_integrator_and_fire():
     ir = nir.NIR(
-        nodes=[nir.Linear(weights=[1], bias=0), nir.LIF(tau=1, r=2, v_leak=3, theta=4)],
+        nodes=[nir.Linear(weights=[1], bias=0), nir.LIF(tau=1, r=2, v_leak=3, v_th=4)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
```

### Comparing `nir-0.0.1/nir/write.py` & `nir-0.0.2/nir/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             }
         elif isinstance(node, nir.LIF):
             return {
                 "type": "LIF",
                 "tau": node.tau,
                 "r": node.r,
                 "v_leak": node.v_leak,
-                "theta": node.theta,
+                "v_th": node.v_th,
             }
         elif isinstance(node, nir.Linear):
             return {
                 "type": "Linear",
                 "weights": node.weights,
                 "bias": node.bias,
             }
```

### Comparing `nir-0.0.1/pyproject.toml` & `nir-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nir"
-version = "0.0.1"
+version = "0.0.2"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
-  { name = "Felix Bauer", email = "felix.bauer@synsen.ai" },
+  { name = "Felix Bauer", email = "felix.bauer@synsense.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
   { name = "Jens Egholm Pedersen", email = "jens@jepedersen.dk" },
   { name = "Sadique Sheik", email = "sadique.sheik@synsense.ai" },
 ]
 readme = "README.md"
@@ -24,11 +24,15 @@
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+
 dependencies = [ "numpy", "h5py" ]
 
+[project.urls]
+homepage = "https://github.com/neuromorphs/nir"
+
 [tool.setuptools.packages]
-find = {} 
+find = {}
```

