# Comparing `tmp/phlearn-1.1.0.tar.gz` & `tmp/phlearn-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlearn-1.1.0.tar", last modified: Thu Apr 27 14:10:25 2023, max compression
+gzip compressed data, was "phlearn-1.1.2.tar", last modified: Tue Jul  4 13:07:39 2023, max compression
```

## Comparing `phlearn-1.1.0.tar` & `phlearn-1.1.2.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.136832 phlearn-1.1.0/
--rw-r--r--   0 eeb        (501) staff       (20)     1075 2023-04-27 14:08:31.000000 phlearn-1.1.0/LICENSE.txt
--rw-r--r--   0 eeb        (501) staff       (20)     1020 2023-04-27 14:10:25.136383 phlearn-1.1.0/PKG-INFO
--rw-r--r--   0 eeb        (501) staff       (20)      513 2023-04-27 14:08:31.000000 phlearn-1.1.0/README.md
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.107239 phlearn-1.1.0/phlearn/
--rw-r--r--   0 eeb        (501) staff       (20)      640 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/__init__.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.116982 phlearn-1.1.0/phlearn/control/
--rw-r--r--   0 eeb        (501) staff       (20)      740 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     3971 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/casadiNN.py
--rw-r--r--   0 eeb        (501) staff       (20)     1386 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/casadiPH.py
--rw-r--r--   0 eeb        (501) staff       (20)    15597 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/mpc.py
--rw-r--r--   0 eeb        (501) staff       (20)     3017 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/phcontroller.py
--rw-r--r--   0 eeb        (501) staff       (20)     4708 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/pid.py
--rw-r--r--   0 eeb        (501) staff       (20)     2554 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/control/reference.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.122729 phlearn-1.1.0/phlearn/phnns/
--rw-r--r--   0 eeb        (501) staff       (20)     2075 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/__init__.py
--rwxr-xr-x   0 eeb        (501) staff       (20)    22515 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/conservative_dissipative_neural_network.py
--rw-r--r--   0 eeb        (501) staff       (20)    12511 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/dynamic_system_neural_network.py
--rw-r--r--   0 eeb        (501) staff       (20)    32704 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/models.py
--rw-r--r--   0 eeb        (501) staff       (20)    17459 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.123666 phlearn-1.1.0/phlearn/phnns/tests/
--rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/tests/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     2113 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/tests/test_phnns.py
--rw-r--r--   0 eeb        (501) staff       (20)    23204 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phnns/train_utils.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.131787 phlearn-1.1.0/phlearn/phsystems/
--rw-r--r--   0 eeb        (501) staff       (20)     1957 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/__init__.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     2867 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/allen_cahn_system.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     3281 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/bbm_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     4345 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/burgers_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     3001 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/cahn_hilliard_system.py
--rwxr-xr-x   0 eeb        (501) staff       (20)    13517 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/conservative_dissipative_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     3790 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/fvm.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     3063 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/heat_system.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     2983 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/kdv_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     2443 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/msd_system.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     3322 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/perona_malik_system.py
--rwxr-xr-x   0 eeb        (501) staff       (20)     3318 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/phase_system.py
--rw-r--r--   0 eeb        (501) staff       (20)    10873 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/pseudo_Hamiltonian_system.py
--rw-r--r--   0 eeb        (501) staff       (20)     7230 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tank_system.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.133056 phlearn-1.1.0/phlearn/phsystems/tests/
--rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tests/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     3051 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/phsystems/tests/test_phsystems.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.135517 phlearn-1.1.0/phlearn/utils/
--rw-r--r--   0 eeb        (501) staff       (20)      433 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/__init__.py
--rw-r--r--   0 eeb        (501) staff       (20)     4481 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/derivatives.py
--rw-r--r--   0 eeb        (501) staff       (20)     4293 2023-04-27 14:08:31.000000 phlearn-1.1.0/phlearn/utils/utils.py
-drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-04-27 14:10:25.110180 phlearn-1.1.0/phlearn.egg-info/
--rw-r--r--   0 eeb        (501) staff       (20)     1020 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/PKG-INFO
--rw-r--r--   0 eeb        (501) staff       (20)     1360 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/SOURCES.txt
--rw-r--r--   0 eeb        (501) staff       (20)        1 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/dependency_links.txt
--rw-r--r--   0 eeb        (501) staff       (20)      146 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/requires.txt
--rw-r--r--   0 eeb        (501) staff       (20)        8 2023-04-27 14:10:25.000000 phlearn-1.1.0/phlearn.egg-info/top_level.txt
--rw-r--r--   0 eeb        (501) staff       (20)       38 2023-04-27 14:10:25.136998 phlearn-1.1.0/setup.cfg
--rw-r--r--   0 eeb        (501) staff       (20)     1072 2023-04-27 14:08:31.000000 phlearn-1.1.0/setup.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.524093 phlearn-1.1.2/
+-rw-r--r--   0 eeb        (501) staff       (20)     1075 2023-04-27 14:08:31.000000 phlearn-1.1.2/LICENSE.txt
+-rw-r--r--   0 eeb        (501) staff       (20)     1120 2023-07-04 13:07:39.523692 phlearn-1.1.2/PKG-INFO
+-rw-r--r--   0 eeb        (501) staff       (20)      599 2023-07-04 13:06:56.000000 phlearn-1.1.2/README.md
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.502761 phlearn-1.1.2/phlearn/
+-rw-r--r--   0 eeb        (501) staff       (20)      640 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/__init__.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.509869 phlearn-1.1.2/phlearn/control/
+-rw-r--r--   0 eeb        (501) staff       (20)      740 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3971 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/casadiNN.py
+-rw-r--r--   0 eeb        (501) staff       (20)     1386 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/casadiPH.py
+-rw-r--r--   0 eeb        (501) staff       (20)    15601 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/control/mpc.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3017 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/phcontroller.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4708 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/pid.py
+-rw-r--r--   0 eeb        (501) staff       (20)     2554 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/control/reference.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.513980 phlearn-1.1.2/phlearn/phnns/
+-rw-r--r--   0 eeb        (501) staff       (20)     2388 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)    19754 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/dynamic_system_neural_network.py
+-rw-r--r--   0 eeb        (501) staff       (20)    14934 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/ode_models.py
+-rw-r--r--   0 eeb        (501) staff       (20)    16821 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/pde_models.py
+-rw-r--r--   0 eeb        (501) staff       (20)    17109 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/pseudo_hamiltonian_neural_network.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)    30027 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/pseudo_hamiltonian_pde_neural_network.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.514764 phlearn-1.1.2/phlearn/phnns/tests/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/phnns/tests/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)      628 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/tests/test_phnns.py
+-rw-r--r--   0 eeb        (501) staff       (20)    23458 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phnns/train_utils.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.515215 phlearn-1.1.2/phlearn/phsystems/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/__init__.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.516734 phlearn-1.1.2/phlearn/phsystems/ode/
+-rw-r--r--   0 eeb        (501) staff       (20)      800 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     2402 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/msd_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)    10359 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/pseudo_hamiltonian_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     7166 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/tank_system.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.517357 phlearn-1.1.2/phlearn/phsystems/ode/tests/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/tests/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3067 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/ode/tests/test_phsystems.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.520654 phlearn-1.1.2/phlearn/phsystems/pde/
+-rw-r--r--   0 eeb        (501) staff       (20)     1310 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/__init__.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     4543 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/allen_cahn_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     4966 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/bbm_system.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4899 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/cahn_hilliard_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     4701 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/heat_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     5084 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/kdv_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)     4978 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/perona_malik_system.py
+-rwxr-xr-x   0 eeb        (501) staff       (20)    13780 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/pde/pseudo_hamiltonian_pde_system.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.521602 phlearn-1.1.2/phlearn/phsystems/tests/
+-rw-r--r--   0 eeb        (501) staff       (20)        0 2023-04-27 14:08:31.000000 phlearn-1.1.2/phlearn/phsystems/tests/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     3071 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/phsystems/tests/test_phsystems.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.523172 phlearn-1.1.2/phlearn/utils/
+-rw-r--r--   0 eeb        (501) staff       (20)      316 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/utils/__init__.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4450 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/utils/derivatives.py
+-rw-r--r--   0 eeb        (501) staff       (20)     4233 2023-07-04 13:06:56.000000 phlearn-1.1.2/phlearn/utils/utils.py
+drwxr-xr-x   0 eeb        (501) staff       (20)        0 2023-07-04 13:07:39.506023 phlearn-1.1.2/phlearn.egg-info/
+-rw-r--r--   0 eeb        (501) staff       (20)     1120 2023-07-04 13:07:39.000000 phlearn-1.1.2/phlearn.egg-info/PKG-INFO
+-rw-r--r--   0 eeb        (501) staff       (20)     1487 2023-07-04 13:07:39.000000 phlearn-1.1.2/phlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 eeb        (501) staff       (20)        1 2023-07-04 13:07:39.000000 phlearn-1.1.2/phlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 eeb        (501) staff       (20)      138 2023-07-04 13:07:39.000000 phlearn-1.1.2/phlearn.egg-info/requires.txt
+-rw-r--r--   0 eeb        (501) staff       (20)        8 2023-07-04 13:07:39.000000 phlearn-1.1.2/phlearn.egg-info/top_level.txt
+-rw-r--r--   0 eeb        (501) staff       (20)       38 2023-07-04 13:07:39.524251 phlearn-1.1.2/setup.cfg
+-rw-r--r--   0 eeb        (501) staff       (20)     1078 2023-07-04 13:06:56.000000 phlearn-1.1.2/setup.py
```

### Comparing `phlearn-1.1.0/LICENSE.txt` & `phlearn-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/PKG-INFO` & `phlearn-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: phlearn
-Version: 1.1.0
-Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf
-Home-page: https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks
+Version: 1.1.2
+Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf and https://arxiv.org/abs/2304.14374
+Home-page: https://github.com/SINTEF/pseudo-hamiltonian-neural-networks
 Author: Sølve Eidnes
 Author-email: solve.eidnes@sintef.no
 License: MIT
 Keywords: pseudo-Hamiltonian neural networks
 Classifier: Development Status :: 5 - Production/Stable
 Provides-Extra: control
 License-File: LICENSE.txt
 
 # phlearn
-Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al. 2022)](https://arxiv.org/pdf/2206.02660.pdf).
+Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al., 2022)](https://arxiv.org/pdf/2206.02660.pdf) for ODEs and [(Eidnes and Lye, 2023)](https://arxiv.org/pdf/2304.14374.pdf) for PDEs.
 
 [Documentation available here](https://pseudo-Hamiltonian-neural-networks.readthedocs.io/en/latest/)
 
 - phlearn
     + phsystems
     + phnns
     + utils
```

### Comparing `phlearn-1.1.0/README.md` & `phlearn-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # phlearn
-Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al. 2022)](https://arxiv.org/pdf/2206.02660.pdf).
+Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al., 2022)](https://arxiv.org/pdf/2206.02660.pdf) for ODEs and [(Eidnes and Lye, 2023)](https://arxiv.org/pdf/2304.14374.pdf) for PDEs.
 
 [Documentation available here](https://pseudo-Hamiltonian-neural-networks.readthedocs.io/en/latest/)
 
 - phlearn
     + phsystems
     + phnns
     + utils
```

### Comparing `phlearn-1.1.0/phlearn/__init__.py` & `phlearn-1.1.2/phlearn/__init__.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/__init__.py` & `phlearn-1.1.2/phlearn/control/__init__.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/casadiNN.py` & `phlearn-1.1.2/phlearn/control/casadiNN.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/casadiPH.py` & `phlearn-1.1.2/phlearn/control/casadiPH.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/mpc.py` & `phlearn-1.1.2/phlearn/control/mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .phcontroller import PseudoHamiltonianController
-from ..phnns.models import R_estimator
+from ..phnns.ode_models import R_estimator
 from .casadiPH import CasadiPseudoHamiltonianSystem
 from .casadiNN import CasadiFCNN, get_pytorch_model_parameters, get_pytorch_model_architecture
 import numpy as np
 import torch
 
 try:
     import do_mpc
```

### Comparing `phlearn-1.1.0/phlearn/control/phcontroller.py` & `phlearn-1.1.2/phlearn/control/phcontroller.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/pid.py` & `phlearn-1.1.2/phlearn/control/pid.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/control/reference.py` & `phlearn-1.1.2/phlearn/control/reference.py`

 * *Files identical despite different names*

### Comparing `phlearn-1.1.0/phlearn/phnns/conservative_dissipative_neural_network.py` & `phlearn-1.1.2/phlearn/phnns/dynamic_system_neural_network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,107 @@
 import numpy as np
 from scipy.integrate import solve_ivp
-from scipy.sparse import diags
 import torch
 
-from .dynamic_system_neural_network import DynamicSystemNN
-from .models import PDEIntegralNN, A_estimator, S_estimator
+from ..utils.derivatives import time_derivative
 from ..utils.utils import to_tensor
+from .ode_models import BaselineNN, BaselineSplitNN
+from .pde_models import PDEBaselineNN, PDEBaselineSplitNN
 
-__all__ = ['ConservativeDissipativeNN', 'load_cdnn_model', 'store_cdnn_model']
 
-
-class ConservativeDissipativeNN(DynamicSystemNN):
+class DynamicSystemNN(torch.nn.Module):
     """
-    Description to be added
+    Base class for implementing neural networks estimating the right
+    hand side of equations of the form::
+
+        dx/dt = f(x, t) + u
+
+    where x is the system state, t is time and u is optional control
+    inputs.
+
+    Parameters
+    ----------
+    nstates : int
+        Number of system states.
+
+    rhs_model : callable, default None
+        Model estimating the right hand side of the above equation.
+        Should take inputs x and t, where x is a tensor of shape
+        (nsamples, nstates) and t is a tensor of shape (nsamples, 1),
+        and return a tensor of shape (nsamples, nstates), estimating the
+        time derivative of each state in each sample.
+
+    controller : callable, default None
+        Additional external ports set by a controller. Callable taking a
+        tensor x of shape (nstates,) and a scalar t as input and
+        returning a tensor of shape (nstates,). Note that this function
+        should not take batch inputs, and that when calling
+        PseudoHamiltonianNN.sample_trajectory when a controller is
+        provided, the Runge-Kutta-4 method will be used for integration
+        in favor of SciPy's solve_ivp.
+
+    init_sampler : callable, default None
+        Function for sampling initial conditions. Callable taking a
+        number specifying the number of inital conditions to sample, M,
+        as input and returning a tensor of shape (M, nstates) with
+        inital conditions for the system. This sampler is used when
+        calling :py:meth:`~DynamicSystemNN.simulate_trajectory` and
+        :py:meth:`~DynamicSystemNN.simulate_trajectories` if no initial
+        condition is provided. If not provided, initial conditions are
+        uniformly sampled from (0, 1).
+
+    ttype : torch type, default torch.float32
 
     """
 
-    def __init__(self,
-                 nstates,
-                 kernel_sizes=[1,3,1,0],
-                 structure_matrix=None,
-                 dissipation_matrix=None,
-                 symmetric_matrix=None,
-                 hamiltonian_true=None,
-                 grad_hamiltonian_true=None,
-                 dissintegral_true=None,
-                 grad_dissintegral_true=None,
-                 external_forces_true=None,
-                 hamiltonian_est=None,
-                 dissintegral_est=None,
-                 external_forces_est=None,
-                 **kwargs):
-        super().__init__(nstates, **kwargs)
-        self.hamiltonian = None
-        self.dissintegral = None
-        self.external_forces = None
-        self.hamiltonian_provided = False
-        self.grad_hamiltonian_provided = False
-        self.dissintegral_provided = False
-        self.grad_dissintegral_provided = False
-        self.external_forces_provided = False
-        self.spacedependent = False
+    def __init__(
+        self,
+        nstates,
+        rhs_model=None,
+        init_sampler=None,
+        controller=None,
+        ttype=torch.float32,
+    ):
+        super().__init__()
+        self.ttype = ttype
         self.nstates = nstates
-        self.kernel_sizes = kernel_sizes
-        self.structure_matrix = structure_matrix
-        self.dissipation_matrix = dissipation_matrix
-        self.symmetric_matrix = symmetric_matrix
-        self.hamiltonian_true = hamiltonian_true
-        self.grad_hamiltonian_true = grad_hamiltonian_true
-        self.dissintegral_true = dissintegral_true
-        self.grad_dissintegral_true = grad_dissintegral_true
-        self.external_forces_true = external_forces_true
-        self.external_forces_est = external_forces_est
-
-        if structure_matrix is None:
-            self.S = S_estimator(kernel_size=self.kernel_sizes[1])
-        elif not callable(structure_matrix):
-            self.S = self._structure_matrix
-        else:
-            self.S = structure_matrix
+        self.controller = controller
+        self.rhs_model = rhs_model
+        if init_sampler is not None:
+            self._initial_condition_sampler = init_sampler
+        self.x_dot = self._x_dot
 
-        if dissipation_matrix is None:
-            self.P = A_estimator(kernel_size=self.kernel_sizes[2])
-        elif not callable(dissipation_matrix):
-            self.P = self._dissipation_matrix
-        else:
-            self.P = dissipation_matrix
-            
-        if symmetric_matrix is None:
-            self.D_flat = A_estimator(kernel_size=self.kernel_sizes[0])
-        elif not callable(symmetric_matrix):
-            self.D_flat = self._symmetric_matrix
-        else:
-            self.D_flat = symmetric_matrix
+    def seed(self, seed):
+        """
+        Set the torch seed.
 
-        if hamiltonian_true is not None:
-            if grad_hamiltonian_true is None:
-                self.hamiltonian = hamiltonian_true
-                self.dH = self._dH_hamiltonian_true
-            else:
-                self.hamiltonian = self._hamiltonian_true
-                self.dH = self._grad_hamiltonian_true
-                self.grad_hamiltonian_provided = True
-            self.hamiltonian_provided = True
-        elif grad_hamiltonian_true is not None:
-            self.dH = self._grad_hamiltonian_true
-            self.grad_hamiltonian_provided = True
-        else:
-            if hamiltonian_est is not None:
-                self.hamiltonian = hamiltonian_est
-            else:
-                self.hamiltonian = PDEIntegralNN(nstates=self.nstates)
-            self.dH = self._dH_hamiltonian_est
+        Parameters
+        ----------
+        seed : int
 
-        if dissintegral_true is not None:
-            if grad_dissintegral_true is None:
-                self.dissintegral = dissintegral_true
-                self.dV = self._dV_dissintegral_true
-            else:
-                self.dissintegral = self._dissintegral_true
-                self.dV = self._grad_dissintegral_true
-                self.grad_dissintegral_provided = True
-            self.dissintegral_provided = True
-        elif grad_dissintegral_true is not None:
-            self.dV = self._grad_dissintegral_true
-            self.grad_dissintegral_provided = True
-        else:
-            if dissintegral_est is not None:
-                self.dissintegral = dissintegral_est
-            else:
-                self.dissintegral = PDEIntegralNN(nstates=self.nstates)
-            self.dV = self._dV_dissintegral_est
+        """
 
-        if external_forces_true is not None:
-            self.external_forces = self._external_forces_true
-            self.external_forces_provided = True
-        elif external_forces_est is not None:
-            self.external_forces = self._external_forces_est
-            self.spacedependent = external_forces_est.spacedependent
-
-    def _symmetric_matrix(self, x=None):
-        return to_tensor(self.symmetric_matrix, self.ttype)
-        
-    def _dissipation_matrix(self, x=None):
-        return to_tensor(self.dissipation_matrix, self.ttype)
-        
-    def _structure_matrix(self, x=None):
-        return to_tensor(self.structure_matrix, self.ttype)
-    
-    def _hamiltonian_true(self, x):
-        return self.hamiltonian_true(x).detach()
-
-    def _grad_hamiltonian_true(self, x):
-        return self.grad_hamiltonian_true(x).detach()
-
-    def _dissintegral_true(self, x):
-        return self.dissintegral_true(x).detach()
-
-    def _grad_dissintegral_true(self, x):
-        return self.grad_dissintegral_true(x).detach()
-
-    def _external_forces_true(self, x, t, xspatial=None):
-        return self.external_forces_true(x, t, xspatial).detach()
-    
-    def _external_forces_est(self, x, t, xspatial=None):
-        return self.external_forces_est(x, t, xspatial)
-    
-    def _external_forces_corrected(self, x, t, xspatial=None):
-        return (self.external_forces_original(x, t, xspatial) +
-                (-self.P().sum()*self.dV_original(torch.tensor(((0,),),dtype=self.ttype))))
-    
-    def external_forces_correction(self):
-        self.external_forces_original = self.external_forces
-        self.external_forces = self._external_forces_corrected
-
-    def _dH_hamiltonian_est(self, x):
-        x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.hamiltonian(x).sum(), x,
-                                   retain_graph=self.training,
-                                   create_graph=self.training)[0]
-
-    def _dH_hamiltonian_true(self, x):
-        x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.hamiltonian(x).sum(), x,
-                                   retain_graph=False,
-                                   create_graph=False)[0].detach()
-
-    def _dV_dissintegral_est(self, x):
-        x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.dissintegral(x).sum(), x,
-                                   retain_graph=self.training,
-                                   create_graph=self.training)[0]
-
-    def _dV_dissintegral_true(self, x):
-        x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.dissintegral(x).sum(), x,
-                                   retain_graph=False,
-                                   create_graph=False)[0].detach()
-
-    def _dV_corrected(self, x):
-        return (self.dV_original(x) - 
-                self.dV_original(torch.tensor(((0,),),dtype=self.ttype)))
-
-    def dV_correction(self):
-        self.dV_original = self.dV
-        self.dV = self._dV_corrected
-        
-    def _x_dot(self, x, t, u=None, xspatial=None):
-        x = to_tensor(x, self.ttype)
-        t = to_tensor(t, self.ttype)
-        u = to_tensor(u, self.ttype)
+        torch.manual_seed(seed)
 
-        dynamics = torch.zeros_like(x)
-        
-        if self.kernel_sizes[1] > 0:
-            S = self.S()
-            if self.hamiltonian is not None:
-                dH = self.dH(x)
-            else:
-                dH = torch.zeros_like(x)
-            d = int((self.kernel_sizes[1]-1)/2)
-            dH_padded = torch.cat([dH[..., self.nstates-d:], dH, dH[..., :d]], dim=-1)
-            dynamics += torch.nn.functional.conv1d(dH_padded, S)
-        if self.kernel_sizes[2] > 0:
-            P = self.P()
-            if self.dissintegral is not None:
-                dV = self.dV(x)
-            else:
-                dV = torch.zeros_like(x)
-            d = int((self.kernel_sizes[2]-1)/2)
-            dV_padded = torch.cat([dV[..., self.nstates-d:], dV, dV[..., :d]], dim=-1)
-            dynamics -= torch.nn.functional.conv1d(dV_padded, P)
-        if self.kernel_sizes[3] > 0:
-            if self.external_forces is not None:
-                dynamics += self.kernel_sizes[3]*self.external_forces(x, t, xspatial)
-        return dynamics
+    def time_derivative(self, integrator, *args, **kwargs):
+        """
+        See :py:meth:~`utils.derivatives.time_derivative`
+        """
 
-    def lhs(self, dxdt):
-        dxdt = to_tensor(dxdt, self.ttype)
-        if self.kernel_sizes[0] == 1:
-            return dxdt
-        else:
-            R = self.D_flat()
-            d = int((self.kernel_sizes[0]-1)/2)
-            dxdt_padded = torch.cat([dxdt[..., self.nstates-d:], dxdt, dxdt[..., :d]], dim=-1)
-            Rdxdt = torch.nn.functional.conv1d(dxdt_padded, R)
-            return Rdxdt
+        return time_derivative(integrator, self.x_dot, *args, **kwargs)
 
-    def simulate_trajectory(self, integrator, t_sample, x0=None,
-                            xspatial=None, noise_std=0., reference=None):
+    def simulate_trajectory(
+        self,
+        integrator,
+        t_sample,
+        x0=None,
+        xspatial=None,
+        noise_std=0.0,
+        reference=None,
+    ):
         """
         Simulate a trajectory using the rhs_model and sample at times
         *t_sample*.
 
         Parameters
         ----------
         integrator : str or False
@@ -258,253 +127,407 @@
         -------
         xs : (T, N) tensor
         us : (T, N) tensor
 
         """
 
         x0 = to_tensor(x0)
-        M = x0.shape[0]
         if x0 is None:
             x0 = self._initial_condition_sampler(1)
-        if not integrator:
-            if self.kernel_sizes[0] == 1:
-                if xspatial is not None:
-                    x_dot = lambda t, x: self._x_dot(
-                                torch.tensor(x.reshape(1, x.shape[-1]),
-                                            dtype=self.ttype),
-                                torch.tensor(np.array(t).reshape((1, 1)),
-                                            dtype=self.ttype),
-                                xspatial=torch.tensor(np.array(xspatial).reshape(1, xspatial.shape[-1]),
-                                            dtype=self.ttype)
-                                ).detach().numpy().flatten()
-                else:
-                    x_dot = lambda t, x: self._x_dot(
-                                torch.tensor(x.reshape(1, x.shape[-1]),
-                                            dtype=self.ttype),
-                                torch.tensor(np.array(t).reshape((1, 1)),
-                                            dtype=self.ttype)
-                                ).detach().numpy().flatten()
+
+        if not integrator and self.controller is None:
+            if xspatial is not None:
+                x_dot = (
+                    lambda t, x: self._x_dot(
+                        torch.tensor(x.reshape(1, x.shape[-1]), dtype=self.ttype),
+                        torch.tensor(np.array(t).reshape((1, 1)), dtype=self.ttype),
+                        xspatial=torch.tensor(
+                            np.array(xspatial).reshape(1, xspatial.shape[-1]),
+                            dtype=self.ttype,
+                        ),
+                    )
+                    .detach()
+                    .numpy()
+                    .flatten()
+                )
             else:
-                d = int((self.kernel_sizes[0]-1)/2)
-                D_flat = self.D_flat().detach().numpy()
-                diagonals = np.concatenate([D_flat[0,:,(d+1):], D_flat[0], D_flat[0,:,:-(d+1)]], axis=1).T.repeat(M, axis=1)
-                offsets = np.concatenate([np.arange(-M+1,-M+1+d),np.arange(-d,d+1),np.arange(M-d,M)])
-                D = diags(diagonals, offsets, (M,M)).toarray()
-                if xspatial is not None:
-                    x_dot = lambda t, x: np.linalg.solve(
-                                D,
-                                self._x_dot(
-                                torch.tensor(x.reshape(1, x.shape[-1]),
-                                            dtype=self.ttype),
-                                torch.tensor(np.array(t).reshape((1, 1)),
-                                            dtype=self.ttype),
-                                xspatial=torch.tensor(np.array(xspatial).reshape(1, xspatial.shape[-1]),
-                                            dtype=self.ttype)
-                                ).detach().numpy().flatten())
-                else:
-                    x_dot = lambda t, x: np.linalg.solve(
-                                D,
-                                self._x_dot(
-                                torch.tensor(x.reshape(1, x.shape[-1]),
-                                            dtype=self.ttype),
-                                torch.tensor(np.array(t).reshape((1, 1)),
-                                            dtype=self.ttype)
-                                ).detach().numpy().flatten())
-            out_ivp = solve_ivp(fun=x_dot, t_span=(t_sample[0], t_sample[-1]),
-                                y0=x0.detach().numpy().flatten(),
-                                t_eval=t_sample, rtol=1e-10)
-            xs = out_ivp['y'].T
+                x_dot = (
+                    lambda t, x: self._x_dot(
+                        torch.tensor(x.reshape(1, x.shape[-1]), dtype=self.ttype),
+                        torch.tensor(np.array(t).reshape((1, 1)), dtype=self.ttype),
+                    )
+                    .detach()
+                    .numpy()
+                    .flatten()
+                )
+            out_ivp = solve_ivp(
+                fun=x_dot,
+                t_span=(t_sample[0], t_sample[-1]),
+                y0=x0.detach().numpy().flatten(),
+                t_eval=t_sample,
+                rtol=1e-10,
+            )
+            xs = out_ivp["y"].T
+            us = None
         else:
             t_sample = to_tensor(t_sample, self.ttype)
             if not integrator and self.controller is not None:
-                integrator = 'rk4'
-                print('Warning: Since the system contains a controller, '
-                      'the RK4 integrator is used to simulate the trajectory '
-                      'instead of solve_ivp.')
-            elif integrator.lower() not in ['euler', 'rk4']:
-                print('Warning: Only explicit integrators Euler and RK4 or no '
-                      'integrator (False) allowed for integration. Ignoring '
-                      f'integrator {integrator} and using RK4.')
-                integrator = 'rk4'
-
+                integrator = "rk4"
+                print(
+                    "Warning: Since the system contains a controller, "
+                    "the rk4 integrator is used to simulate the trajectory "
+                    "instead of solve_ivp."
+                )
+            elif integrator.lower() not in ["euler", "rk4"]:
+                print(
+                    "Warning: Only explicit integrators euler and rk4 or no "
+                    "integrator (False) allowed for inference. Ignoring "
+                    f"integrator {integrator} and using rk4."
+                )
+                integrator = "rk4"
+
+            if self.controller is not None:
+                self.controller.reset()
+                if reference is not None:
+                    self.controller.set_reference(reference)
             nsteps = t_sample.shape[0]
             x0 = x0.reshape(1, x0.shape[-1])
             xs = torch.zeros([nsteps, x0.shape[-1]])
             xs[0, :] = x0
 
-            if self.kernel_sizes[0] == 1:
-                if xspatial is not None:
-                    for i, t_step in enumerate(t_sample[:-1]):
-                        t_step = torch.squeeze(t_step).reshape(-1, 1)
-                        dt = t_sample[i + 1] - t_step
-                        I = np.eye(M)
-                        xs[i + 1, :] = xs[i, :] + dt*self.time_derivative(
-                            integrator, xs[i:i+1, :], xs[i:i+1, :],
-                            t_step, t_step, dt, xspatial=torch.tensor(np.array(xspatial).reshape(1,xspatial.shape[-1]),
-                                                                      dtype=self.ttype))
-                else:
-                    for i, t_step in enumerate(t_sample[:-1]):
-                        t_step = torch.squeeze(t_step).reshape(-1, 1)
-                        dt = t_sample[i + 1] - t_step
-                        I = np.eye(M)
-                        xs[i + 1, :] = xs[i, :] + dt*self.time_derivative(
-                            integrator, xs[i:i+1, :], xs[i:i+1, :],
-                            t_step, t_step, dt)
+            u = None
+            us = torch.zeros([nsteps - 1, x0.shape[-1]])
+
+            if xspatial is not None:
+                for i, t_step in enumerate(t_sample[:-1]):
+                    t_step = torch.squeeze(t_step).reshape(-1, 1)
+                    if self.controller is not None:
+                        u = to_tensor(self.controller(xs[i, :], t_step), self.ttype)
+                        us[i, :] = u
+                    dt = t_sample[i + 1] - t_step
+                    xs[i + 1, :] = xs[i, :] + dt * self.time_derivative(
+                        integrator,
+                        xs[i : i + 1, :],
+                        xs[i : i + 1, :],
+                        t_step,
+                        t_step,
+                        dt,
+                        u,
+                        xspatial=torch.tensor(
+                            np.array(xspatial).reshape(1, xspatial.shape[-1]),
+                            dtype=self.ttype,
+                        ),
+                    )
             else:
-                d = int((self.kernel_sizes[0]-1)/2)
-                D_flat = self.D_flat().detach().numpy()
-                diagonals = np.concatenate([D_flat[0,:,(d+1):], D_flat[0], D_flat[0,:,:-(d+1)]], axis=1).T.repeat(M, axis=1)
-                offsets = np.concatenate([np.arange(-M+1,-M+1+d),np.arange(-d,d+1),np.arange(M-d,M)])
-                D = diags(diagonals, offsets, (M,M)).toarray()
-                if xspatial is not None:
-                    for i, t_step in enumerate(t_sample[:-1]):
-                        t_step = torch.squeeze(t_step).reshape(-1, 1)
-                        dt = t_sample[i + 1] - t_step
-                        xs[i + 1, :] = xs[i, :] + dt*np.linalg.solve(
-                            D,
-                            self.time_derivative(
-                            integrator, xs[i:i+1, :], xs[i:i+1, :],
-                            t_step, t_step, dt, xspatial=torch.tensor(np.array(xspatial).reshape(1, xspatial.shape[-1]),
-                                                                      dtype=self.ttype)).detach().T).T
-                else:
-                    for i, t_step in enumerate(t_sample[:-1]):
-                        t_step = torch.squeeze(t_step).reshape(-1, 1)
-                        dt = t_sample[i + 1] - t_step
-                        xs[i + 1, :] = xs[i, :] + dt*np.linalg.solve(
-                            D,
-                            self.time_derivative(
-                            integrator, xs[i:i+1, :], xs[i:i+1, :],
-                            t_step, t_step, dt).detach().T).T
+                for i, t_step in enumerate(t_sample[:-1]):
+                    t_step = torch.squeeze(t_step).reshape(-1, 1)
+                    if self.controller is not None:
+                        u = to_tensor(self.controller(xs[i, :], t_step), self.ttype)
+                        us[i, :] = u
+                    dt = t_sample[i + 1] - t_step
+                    xs[i + 1, :] = xs[i, :] + dt * self.time_derivative(
+                        integrator,
+                        xs[i : i + 1, :],
+                        xs[i : i + 1, :],
+                        t_step,
+                        t_step,
+                        dt,
+                        u,
+                    )
+            xs = xs.detach().numpy()
+            if self.controller is not None:
+                us = us.detach().numpy()
+            else:
+                us = None
+
+        return xs, us
+
+    def simulate_trajectories(
+        self, ntrajectories, integrator, t_sample, x0=None, noise_std=0, references=None
+    ):
+        """
+        Calls :py:meth:`~DynamicSystemNN.simulate_trajectory`
+        *ntrajectories* times.
+
+        Parameters
+        ----------
+        integrator : str or False
+            Specifies which solver to use during simulation. If False,
+            the problem is left to scipy's solve_ivp. If 'euler', the system
+            is simulated with the forward Euler method.
+            If 'midpoint', 'rk4' or 'srk4' the system is simulated with
+            the classic Runge-Kutta-4 method.
+        t_sample : (T, 1) or (ntrajectories, T, 1) tensor or ndarray
+            Times at which the trajectory is sampled.
+        x0 : (ntrajectories, N) tensor or ndarray, default None
+            Initial condition. If None, an initial condition is sampled
+            with the internal sampler.
+        noise_std : number, default 0.
+            Standard deviation of Gaussian white noise added to the
+            samples of the trajectory.
+        references : list of phlearn.control.Reference, default
+        None
+            If the system has a controller a list of ntrajectories
+            reference objects may be passed.
+
+        Returns
+        -------
+        xs : (ntrajectories, T, N) tensor
+        t_sample : (ntrajectories, T, 1) tensor
+        us : (ntrajectories, T, N) tensor or None
+
+        """
+
+        if integrator in ("euler", "rk4") and self.controller is None:
+            if x0 is None:
+                x0 = self._initial_condition_sampler(ntrajectories, self.rng)
+            x0 = to_tensor(x0, self.ttype)
+            t_sample = to_tensor(t_sample, self.ttype)
+
+            if len(t_sample.shape) == 1:
+                t_sample = np.tile(t_sample, (ntrajectories, 1))
+
+            dt = t_sample[0, 1] - t_sample[0, 0]
+            nsteps = t_sample.shape[-1]
+            x0 = x0.reshape(ntrajectories, self.nstates)
+            t_sample = t_sample.reshape(ntrajectories, nsteps, 1)
+            xs = torch.zeros([ntrajectories, nsteps, self.nstates])
+            xs[:, 0, :] = x0
+            for i in range(nsteps - 1):
+                xs[:, i + 1, :] = xs[:, i] + dt * self.time_derivative(
+                    integrator,
+                    xs[i : i + 1, :],
+                    xs[i : i + 1, :],
+                    t_sample,
+                    t_sample,
+                    dt,
+                )
+
             xs = xs.detach().numpy()
+            t_sample = t_sample.detach().numpy()
+            us = None
+        else:
+            t_sample = np.atleast_2d(t_sample)
+            if t_sample.shape[0] == 1:
+                t_sample = np.repeat(t_sample, ntrajectories, 0)
+            else:
+                assert t_sample.shape[0] == ntrajectories
+            nsteps = t_sample.shape[-1]
+            xs = torch.zeros([ntrajectories, nsteps, self.nstates])
+            us = torch.zeros((ntrajectories, nsteps - 1, self.nstates))
+            if references is None:
+                references = [None] * ntrajectories
+
+            for i in range(ntrajectories):
+                xs[i], us[i] = self.simulate_trajectory(
+                    integrator=integrator,
+                    t_sample=t_sample[i],
+                    x0=x0[i],
+                    noise_std=noise_std,
+                    reference=references[i],
+                )
+
+            if self.controller is None:
+                us = None
+
+            if len(t_sample.shape) == 1:
+                t_sample = torch.tile(t_sample, (ntrajectories, 1))
+            t_sample = t_sample.reshape(ntrajectories, nsteps, 1)
+
+        return xs, t_sample, us
+
+    def set_controller(self, controller):
+        """
+        Set controller.
+        """
+
+        self.controller = controller
+
+    def lhs(self, dxdt):
+        return dxdt
 
-        return xs, None
+    def _x_dot(self, x, t, u=None, xspatial=None):
+        x = to_tensor(x, self.ttype)
+        t = to_tensor(t, self.ttype)
+        u = to_tensor(u, self.ttype)
+
+        if xspatial is not None:
+            xspatial = to_tensor(xspatial, self.ttype)
+            dynamics = self.rhs_model(x, t, xspatial)
+        else:
+            dynamics = self.rhs_model(x, t)
+        if u is not None:
+            dynamics += u
+        return dynamics
+
+    def _initial_condition_sampler(self, nsamples=1):
+        return 2 * torch.rand((nsamples, self.nstates), dtype=self.ttype) - 1
 
 
-def load_cdnn_model(modelpath):
+def load_baseline_model(modelpath):
     """
-    Loads a :py:class:`PseudoHamiltonianNN` that has been stored using the
-    :py:func:`store_phnn_model`. Assumes that the hamiltonian function
-    has either been provided or has been modeled with a
-    :py:class:`~.models.hamiltonianNN`, that the external forces
-    has either been provided or modelled with a
-    :py:class:`~.models.ExternalForcesNN`, and that the dissipation has
-    either been provided or been modelled with a
-    :py:class:`~.models.R_estimator` or a :py:class:`~.models.R_NN`.
+    Loads a :py:class:`BaslineNN` or a :py:class:`BaselineSplitNN`
+    that has been stored using the :py:meth:`store_baseline_model`.
 
     Parameters
     ----------
     modelpath : str
 
     Returns
     -------
-    model : PseudoHamiltonianNN
+    model : BaslineNN, BaselineSplitNN
     optimizer : torch.optim.Adam
     metadict : dict
         Contains information about the model and training details.
 
     """
 
     metadict = torch.load(modelpath)
 
-    model = metadict['model']
+    nstates = metadict["nstates"]
+    init_sampler = metadict["init_sampler"]
+    controller = metadict["controller"]
+    ttype = metadict["ttype"]
+
+    if "external_forces_filter_x" in metadict["rhs_model"].keys():
+        hidden_dim = metadict["rhs_model"]["hidden_dim"]
+        noutputs_x = metadict["rhs_model"]["noutputs_x"]
+        noutputs_t = metadict["rhs_model"]["noutputs_t"]
+        external_forces_filter_x = metadict["rhs_model"]["external_forces_filter_x"]
+        external_forces_filter_t = metadict["rhs_model"]["external_forces_filter_t"]
+        rhs_model = BaselineSplitNN(
+            nstates,
+            hidden_dim,
+            noutputs_x=noutputs_x,
+            noutputs_t=noutputs_t,
+            external_forces_filter_x=external_forces_filter_x,
+            external_forces_filter_t=external_forces_filter_t,
+            ttype=ttype,
+        )
+    elif "split" in metadict["rhs_model"].keys():
+        hidden_dim = metadict["rhs_model"]["hidden_dim"]
+        timedependent = metadict["rhs_model"]["timedependent"]
+        statedependent = metadict["rhs_model"]["statedependent"]
+        spacedependent = metadict["rhs_model"]["spacedependent"]
+        period = metadict["rhs_model"]["period"]
+        number_of_intermediate_outputs = metadict["rhs_model"][
+            "number_of_intermediate_outputs"
+        ]
+        rhs_model = PDEBaselineSplitNN(
+            nstates,
+            hidden_dim,
+            timedependent,
+            statedependent,
+            spacedependent,
+            period,
+            number_of_intermediate_outputs,
+        )
+    elif "spacedependent" in metadict["rhs_model"].keys():
+        hidden_dim = metadict["rhs_model"]["hidden_dim"]
+        timedependent = metadict["rhs_model"]["timedependent"]
+        statedependent = metadict["rhs_model"]["statedependent"]
+        spacedependent = metadict["rhs_model"]["spacedependent"]
+        period = metadict["rhs_model"]["period"]
+        number_of_intermediate_outputs = metadict["rhs_model"][
+            "number_of_intermediate_outputs"
+        ]
+        rhs_model = PDEBaselineNN(
+            nstates,
+            hidden_dim,
+            timedependent,
+            statedependent,
+            spacedependent,
+            period,
+            number_of_intermediate_outputs,
+        )
+    else:
+        hidden_dim = metadict["rhs_model"]["hidden_dim"]
+        timedependent = metadict["rhs_model"]["timedependent"]
+        statedependent = metadict["rhs_model"]["statedependent"]
+        rhs_model = BaselineNN(nstates, hidden_dim, timedependent, statedependent)
+    rhs_model.load_state_dict(metadict["rhs_model"]["state_dict"])
+
+    model = DynamicSystemNN(
+        nstates,
+        rhs_model=rhs_model,
+        init_sampler=init_sampler,
+        controller=controller,
+        ttype=ttype,
+    )
 
     optimizer = torch.optim.Adam(model.parameters())
-    optimizer.load_state_dict(metadict['traininginfo']['optimizer_state_dict'])
+    optimizer.load_state_dict(metadict["traininginfo"]["optimizer_state_dict"])
 
     return model, optimizer, metadict
 
 
-def store_cdnn_model(storepath, model, optimizer, **kwargs):
+def store_baseline_model(storepath, model, optimizer, **kwargs):
     """
-    Stores a :py:class:`ConservativeDissipativeNNNN` with additional information
-    to disc. The stored model can be read into memory again with
-    :py:func:`load_cdnn_model`.
+    Stores a :py:class:`BaslineNN` or a :py:class:`BaselineSplitNN`
+    with additional information to disc. The stored model can be
+    read into memory again with :py:meth:`load_baseline_model`.
 
     Parameters
     ----------
     storepath : str
-    model : ConservativeDissipativeNN
+    model : BaselineNN, BaselineSplitNN, PDEBaselineNN
     optimizer : torch optimizer
     * * kwargs : dict
         Contains additional information about for instance training
         hyperparameters and loss values.
 
     """
 
     metadict = {}
-    metadict['model'] = model
-    # metadict['nstates'] = model.nstates
-    # metadict['kernel_sizes'] = model.kernel_sizes
-    # metadict['structure_matrix'] = model.S().detach() # model.structure_matrix
-    # metadict['dissipation_matrix'] = model.P().detach() # model.dissipation_matrix
-    # metadict['symmetric_matrix'] = model.D_flat().detach() # model.symmetric_matrix
-    metadict['symmetric_matrix'] = None
-    # #metadict['structure_matrix'] = model.structure_matrix
-    # #metadict['dissipation_matrix'] = model.dissipation_matrix
-    # #metadict['symmetric_matrix'] = model.symmetric_matrix
-    # metadict['hamiltonian_provided'] = model.hamiltonian_provided
-    # metadict['grad_hamiltonian_provided'] = model.hamiltonian_provided
-    # metadict['dissintegral_provided'] = model.dissintegral_provided
-    # metadict['grad_dissintegral_provided'] = model.grad_dissintegral_provided
-    # metadict['external_forces_provided'] = model.external_forces_provided
-    # metadict['init_sampler'] = model._initial_condition_sampler
-    # metadict['ttype'] = model.ttype
 
-    metadict['traininginfo'] = {}
-    metadict['traininginfo']['optimizer_state_dict'] = optimizer.state_dict()
-    for key, value in kwargs.items():
-        metadict['traininginfo'][key] = value
+    metadict["nstates"] = model.nstates
+    metadict["init_sampler"] = model._initial_condition_sampler
+    metadict["controller"] = model.controller
+    metadict["ttype"] = model.ttype
+
+    if isinstance(model.rhs_model, BaselineNN):
+        metadict["rhs_model"] = {}
+        metadict["rhs_model"]["hidden_dim"] = model.rhs_model.hidden_dim
+        metadict["rhs_model"]["timedependent"] = model.rhs_model.timedependent
+        metadict["rhs_model"]["statedependent"] = model.rhs_model.statedependent
+        metadict["rhs_model"]["state_dict"] = model.rhs_model.state_dict()
+
+        metadict["traininginfo"] = {}
+        metadict["traininginfo"]["optimizer_state_dict"] = optimizer.state_dict()
+        for key, value in kwargs.items():
+            metadict["traininginfo"][key] = value
+
+    elif isinstance(model.rhs_model, BaselineSplitNN):
+        metadict["rhs_model"] = {}
+        metadict["rhs_model"]["hidden_dim"] = model.rhs_model.hidden_dim
+        metadict["rhs_model"]["noutputs_x"] = model.rhs_model.noutputs_x
+        metadict["rhs_model"]["noutputs_t"] = model.rhs_model.noutputs_t
+        metadict["rhs_model"][
+            "external_forces_filter_x"
+        ] = model.rhs_model.network_x.external_forces_filter.T
+        metadict["rhs_model"][
+            "external_forces_filter_t"
+        ] = model.rhs_model.network_t.external_forces_filter.T
+        metadict["rhs_model"]["state_dict"] = model.rhs_model.state_dict()
+
+    elif isinstance(model.rhs_model, PDEBaselineNN) or isinstance(
+        model.rhs_model, PDEBaselineSplitNN
+    ):
+        metadict["rhs_model"] = {}
+        metadict["rhs_model"]["hidden_dim"] = model.rhs_model.hidden_dim
+        metadict["rhs_model"]["timedependent"] = model.rhs_model.timedependent
+        metadict["rhs_model"]["statedependent"] = model.rhs_model.statedependent
+        metadict["rhs_model"]["spacedependent"] = model.rhs_model.spacedependent
+        metadict["rhs_model"]["period"] = model.rhs_model.period
+        metadict["rhs_model"][
+            "number_of_intermediate_outputs"
+        ] = model.rhs_model.number_of_intermediate_outputs
+        metadict["rhs_model"]["state_dict"] = model.rhs_model.state_dict()
+        if isinstance(model.rhs_model, PDEBaselineSplitNN):
+            metadict["rhs_model"]["split"] = model.rhs_model.split
 
-    # metadict['hamiltonian'] = {}
-    # metadict['grad_hamiltonian'] = {}
-    # metadict['dissintegral'] = {}
-    # metadict['grad_dissintegral'] = {}
-    # metadict['external_forces'] = {}
-
-    # if model.hamiltonian_provided:
-    #     metadict['hamiltonian']['true'] = model.hamiltonian_true
-    #     metadict['hamiltonian']['hidden_dim'] = None
-    #     metadict['hamiltonian']['state_dict'] = None
-    # else:
-    #     metadict['hamiltonian']['true'] = None
-    #     metadict['hamiltonian']['hidden_dim'] = model.hamiltonian.hidden_dim
-    #     metadict['hamiltonian']['state_dict'] = model.hamiltonian.state_dict()
-
-    # if model.grad_hamiltonian_provided:
-    #     metadict['grad_hamiltonian']['true'] = model.grad_hamiltonian_true
-    # else:
-    #     metadict['grad_hamiltonian']['true'] = None
-
-    # if model.dissintegral_provided:
-    #     metadict['dissintegral']['true'] = model.dissintegral_true
-    #     metadict['dissintegral']['hidden_dim'] = None
-    #     metadict['dissintegral']['state_dict'] = None
-    # else:
-    #     metadict['dissintegral']['true'] = None
-    #     metadict['dissintegral']['hidden_dim'] = model.dissintegral.hidden_dim
-    #     metadict['dissintegral']['state_dict'] = model.dissintegral.state_dict()
-
-    # if model.grad_dissintegral_provided:
-    #     metadict['grad_dissintegral']['true'] = model.grad_dissintegral_true
-    # else:
-    #     metadict['grad_dissintegral']['true'] = None
-
-    # if model.external_forces_provided:
-    #     metadict['external_forces']['true'] = model.external_forces_true
-    #     metadict['external_forces']['hidden_dim'] = None
-    #     metadict['external_forces']['timedependent'] = None
-    #     metadict['external_forces']['spacedependent'] = None
-    #     metadict['external_forces']['statedependent'] = None
-    #     metadict['external_forces']['period'] = None
-    #     metadict['external_forces']['ttype'] = None
-    #     metadict['external_forces']['state_dict'] = None
-    # else:
-    #     metadict['external_forces']['true'] = None
-    #     metadict['external_forces']['hidden_dim'] = model.external_forces.hidden_dim
-    #     metadict['external_forces']['timedependent'] = model.external_forces.timedependent
-    #     metadict['external_forces']['statedependent'] = model.external_forces.statedependent
-    #     metadict['external_forces']['spacedependent'] = model.external_forces.spacedependent
-    #     metadict['external_forces']['period'] = model.external_forces.period
-    #     metadict['external_forces']['ttype'] = model.external_forces.ttype
-    #     metadict['external_forces']['state_dict'] = model.external_forces.state_dict()
+    metadict["traininginfo"] = {}
+    metadict["traininginfo"]["optimizer_state_dict"] = optimizer.state_dict()
+    for key, value in kwargs.items():
+        metadict["traininginfo"][key] = value
 
-    torch.save(metadict, storepath)
+    torch.save(metadict, storepath)
```

### Comparing `phlearn-1.1.0/phlearn/phnns/pseudo_hamiltonian_neural_network.py` & `phlearn-1.1.2/phlearn/phnns/pseudo_hamiltonian_neural_network.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-
 import torch
 import numpy as np
 
 from .dynamic_system_neural_network import DynamicSystemNN
-from .models import HamiltonianNN, ExternalForcesNN, R_NN, R_estimator
+from .ode_models import HamiltonianNN, ExternalForcesNN, R_NN, R_estimator
 from ..utils.utils import to_tensor
 
-__all__ = ['PseudoHamiltonianNN', 'load_phnn_model', 'store_phnn_model']
-
 
 class PseudoHamiltonianNN(DynamicSystemNN):
     """
     Implements a pseudo-Hamiltonian neural network abiding to the
     pseudo-Hamiltonian formulation::
 
         dx/dt = (S(x) - R(x))*grad[H(x)] + F(x, t)
 
     where x is the system state, S is the skew-symmetric interconnection
     matrix, R is the positive semi-definite dissipation matrix, H is the
     Hamiltonian of the system and F is the external ports.
-    
+
     It is possible to provide function estimators like neural networks
     to model R, H and F. All estimators must subclass torch.nn.Module,
     such that gradients can be recorded with PyTorch.
 
     If R, H or F are known, they can be provided and used in favor of
     estimators. Note that R, H and F must be functions both taking as
     input and returning tensors, and that the gradients of H(x) must be
@@ -31,15 +28,15 @@
 
 
     parameters
     ----------
         nstates : int
             Number of system states.
 
-        structure_matrix : (N, N) tensor
+        skewsymmetric_matrix : (N, N) tensor
             Corresponds to the S matrix. Must either be a
             (nstates, nstates) tensor, or callable taking a tensor input
             of shape (nsamples, nstates) and returning an tensor of
             shape (nsamples, nstates, nstates).
 
         hamiltonian_true : callable, default None
             The known Hamiltonian H of the system. Callable taking a
@@ -83,60 +80,61 @@
         external_forces_est : callable
             Estimator for the external ports. Takes a tensor of shape
             (nsamples, nstates) as input, returning a tensor of shape
             (nsamples, nstates).
 
     """
 
-    def __init__(self,
-                 nstates,
-                 structure_matrix=None,
-                 hamiltonian_true=None,
-                 grad_hamiltonian_true=None,
-                 dissipation_true=None,
-                 external_forces_true=None,
-                 hamiltonian_est=None,
-                 dissipation_est=None,
-                 external_forces_est=None,
-                 **kwargs):
+    def __init__(
+        self,
+        nstates,
+        skewsymmetric_matrix=None,
+        hamiltonian_true=None,
+        grad_hamiltonian_true=None,
+        dissipation_true=None,
+        external_forces_true=None,
+        hamiltonian_est=None,
+        dissipation_est=None,
+        external_forces_est=None,
+        **kwargs
+    ):
         super().__init__(nstates, **kwargs)
-        
-        if structure_matrix is None:
+
+        if skewsymmetric_matrix is None:
             if nstates % 2 == 1:
                 raise Exception(
-                    "nstates must be even when structure_matrix not provided"
+                    "nstates must be even when skewsymmetric_matrix not provided"
                 )
             npos = nstates // 2
-            structure_matrix = np.block(
+            skewsymmetric_matrix = np.block(
                 [
                     [np.zeros([npos, npos]), np.eye(npos)],
                     [-np.eye(npos), np.zeros([npos, npos])],
                 ]
             )
-            
+
         self.S = None
         self.hamiltonian = None
         self.external_forces = None
         self.R = None
         self.hamiltonian_provided = False
         self.grad_hamiltonian_provided = False
         self.external_forces_provided = False
         self.dissipation_provided = False
         self.nstates = nstates
-        self.structure_matrix = structure_matrix
+        self.skewsymmetric_matrix = skewsymmetric_matrix
         self.hamiltonian_true = hamiltonian_true
         self.grad_hamiltonian_true = grad_hamiltonian_true
         self.dissipation_true = dissipation_true
         self.external_forces_true = external_forces_true
 
-        
-        if not callable(structure_matrix):
-            self.S = self._structure_matrix
+        if not callable(skewsymmetric_matrix):
+            self.S = self._skewsymmetric_matrix
         else:
-            self.S = structure_matrix
+            self.S = skewsymmetric_matrix
 
         if dissipation_true is not None:
             self.dissipation_provided = True
             if callable(dissipation_true):
                 self.R = self._dissipation_true_callable
             else:
                 self.R = self._dissipation_true_static
@@ -162,20 +160,20 @@
                 self.hamiltonian = HamiltonianNN(self.nstates)
             self.dH = self._dH_hamiltonian_est
 
         if external_forces_true is not None:
             self.external_forces = self._external_forces_true
             self.external_forces_provided = True
         elif external_forces_true is None and external_forces_est is None:
-            self.external_forces = lambda x,t: 0
+            self.external_forces = lambda x, t: 0
         else:
             self.external_forces = external_forces_est
 
-    def _structure_matrix(self, x):
-        return to_tensor(self.structure_matrix, self.ttype)
+    def _skewsymmetric_matrix(self, x):
+        return to_tensor(self.skewsymmetric_matrix, self.ttype)
 
     def _hamiltonian_true(self, x):
         return self.hamiltonian_true(x).detach()
 
     def _grad_hamiltonian_true(self, x):
         return self.grad_hamiltonian_true(x).detach()
 
@@ -186,39 +184,42 @@
         return self.dissipation_true(x).detach()
 
     def _dissipation_true_static(self, x):
         return to_tensor(self.dissipation_true, self.ttype)
 
     def _dH_hamiltonian_est(self, x):
         x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.hamiltonian(x).sum(), x,
-                                   retain_graph=self.training,
-                                   create_graph=self.training)[0]
+        return torch.autograd.grad(
+            self.hamiltonian(x).sum(),
+            x,
+            retain_graph=self.training,
+            create_graph=self.training,
+        )[0]
 
     def _dH_hamiltonian_true(self, x):
         x = x.detach().requires_grad_()
-        return torch.autograd.grad(self.hamiltonian(x).sum(), x,
-                                   retain_graph=False,
-                                   create_graph=False)[0].detach()
+        return torch.autograd.grad(
+            self.hamiltonian(x).sum(), x, retain_graph=False, create_graph=False
+        )[0].detach()
 
     def _x_dot(self, x, t, u=None, xspatial=None):
         x = to_tensor(x, self.ttype)
         t = to_tensor(t, self.ttype)
         u = to_tensor(u, self.ttype)
 
         S = self.S(x)
         R = self.R(x)
         dH = self.dH(x)
-        
+
         if (len(S.shape) == 3) or (len(R.shape) == 3):
-            dynamics = (torch.matmul(S - R, torch.atleast_3d(dH)
-                                     ).reshape(x.shape)
-                        + self.external_forces(x, t))
+            dynamics = torch.matmul(S - R, torch.atleast_3d(dH)).reshape(
+                x.shape
+            ) + self.external_forces(x, t)
         else:
-            dynamics = dH@(S.T - R.T) + self.external_forces(x, t)
+            dynamics = dH @ (S.T - R.T) + self.external_forces(x, t)
         if u is not None:
             dynamics += u
         return dynamics
 
 
 def load_phnn_model(modelpath):
     """
@@ -242,87 +243,95 @@
     metadict : dict
         Contains information about the model and training details.
 
     """
 
     metadict = torch.load(modelpath)
 
-    nstates = metadict['nstates']
-    structure_matrix = metadict['structure_matrix']
-    hamiltonian_provided = metadict['hamiltonian_provided']
-    grad_hamiltonian_provided = metadict['grad_hamiltonian_provided']
-    external_forces_provided = metadict['external_forces_provided']
-    dissipation_provided = metadict['dissipation_provided']
-    init_sampler = metadict['init_sampler']
-    controller = metadict['controller']
-    ttype = metadict['ttype']
+    nstates = metadict["nstates"]
+    skewsymmetric_matrix = metadict["skewsymmetric_matrix"]
+    hamiltonian_provided = metadict["hamiltonian_provided"]
+    grad_hamiltonian_provided = metadict["grad_hamiltonian_provided"]
+    external_forces_provided = metadict["external_forces_provided"]
+    dissipation_provided = metadict["dissipation_provided"]
+    init_sampler = metadict["init_sampler"]
+    controller = metadict["controller"]
+    ttype = metadict["ttype"]
 
     if hamiltonian_provided:
-        hamiltonian_true = metadict['hamiltonian']['true']
+        hamiltonian_true = metadict["hamiltonian"]["true"]
         hamiltonian_est = None
     else:
         hamiltonian_true = None
-        hidden_dim = metadict['hamiltonian']['hidden_dim']
+        hidden_dim = metadict["hamiltonian"]["hidden_dim"]
         hamiltonian_est = HamiltonianNN(nstates, hidden_dim)
-        hamiltonian_est.load_state_dict(
-            metadict['hamiltonian']['state_dict'].copy())
+        hamiltonian_est.load_state_dict(metadict["hamiltonian"]["state_dict"].copy())
 
     if grad_hamiltonian_provided:
-        grad_hamiltonian_true = metadict['grad_hamiltonian']['true']
+        grad_hamiltonian_true = metadict["grad_hamiltonian"]["true"]
     else:
         grad_hamiltonian_true = None
 
     if external_forces_provided:
-        external_forces_true = metadict['external_forces']['true']
+        external_forces_true = metadict["external_forces"]["true"]
         external_forces_est = None
     else:
         external_forces_true = None
-        noutputs = metadict['external_forces']['noutputs']
-        hidden_dim = metadict['external_forces']['hidden_dim']
-        timedependent = metadict['external_forces']['timedependent']
-        statedependent = metadict['external_forces']['statedependent']
-        external_forces_filter = metadict['external_forces']['external_forces_filter']
-        ttype = metadict['external_forces']['ttype']
-        external_forces_est = ExternalForcesNN(nstates, noutputs, hidden_dim,
-                                           timedependent, statedependent,
-                                           external_forces_filter, ttype)
+        noutputs = metadict["external_forces"]["noutputs"]
+        hidden_dim = metadict["external_forces"]["hidden_dim"]
+        timedependent = metadict["external_forces"]["timedependent"]
+        statedependent = metadict["external_forces"]["statedependent"]
+        external_forces_filter = metadict["external_forces"]["external_forces_filter"]
+        ttype = metadict["external_forces"]["ttype"]
+        external_forces_est = ExternalForcesNN(
+            nstates,
+            noutputs,
+            hidden_dim,
+            timedependent,
+            statedependent,
+            external_forces_filter,
+            ttype,
+        )
         external_forces_est.load_state_dict(
-            metadict['external_forces']['state_dict'].copy())
+            metadict["external_forces"]["state_dict"].copy()
+        )
 
     if dissipation_provided:
-        dissipation_true = metadict['dissipation']['true']
+        dissipation_true = metadict["dissipation"]["true"]
         dissipation_est = None
     else:
         dissipation_true = None
-        dissipation_type = metadict['dissipation']['type'].lower()
-        if 'r_estimator' in dissipation_type:
-            state_is_damped = metadict['dissipation']['state_is_damped']
-            ttype = metadict['dissipation']['ttype']
+        dissipation_type = metadict["dissipation"]["type"].lower()
+        if "r_estimator" in dissipation_type:
+            state_is_damped = metadict["dissipation"]["state_is_damped"]
+            ttype = metadict["dissipation"]["ttype"]
             dissipation_est = R_estimator(state_is_damped, ttype)
         else:
-            hidden_dim = metadict['dissipation']['hidden_dim']
-            diagonal = metadict['dissipation']['diagonal']
+            hidden_dim = metadict["dissipation"]["hidden_dim"]
+            diagonal = metadict["dissipation"]["diagonal"]
             dissipation_est = R_NN(nstates, hidden_dim, diagonal)
-        dissipation_est.load_state_dict(
-            metadict['dissipation']['state_dict'].copy())
+        dissipation_est.load_state_dict(metadict["dissipation"]["state_dict"].copy())
 
-    model = PseudoHamiltonianNN(nstates, structure_matrix,
-                              hamiltonian_true=hamiltonian_true,
-                              grad_hamiltonian_true=grad_hamiltonian_true,
-                              dissipation_true=dissipation_true,
-                              external_forces_true=external_forces_true,
-                              hamiltonian_est=hamiltonian_est,
-                              dissipation_est=dissipation_est,
-                              external_forces_est=external_forces_est,
-                              init_sampler=init_sampler,
-                              controller=controller,
-                              ttype=ttype)
+    model = PseudoHamiltonianNN(
+        nstates,
+        skewsymmetric_matrix,
+        hamiltonian_true=hamiltonian_true,
+        grad_hamiltonian_true=grad_hamiltonian_true,
+        dissipation_true=dissipation_true,
+        external_forces_true=external_forces_true,
+        hamiltonian_est=hamiltonian_est,
+        dissipation_est=dissipation_est,
+        external_forces_est=external_forces_est,
+        init_sampler=init_sampler,
+        controller=controller,
+        ttype=ttype,
+    )
 
     optimizer = torch.optim.Adam(model.parameters())
-    optimizer.load_state_dict(metadict['traininginfo']['optimizer_state_dict'])
+    optimizer.load_state_dict(metadict["traininginfo"]["optimizer_state_dict"])
 
     return model, optimizer, metadict
 
 
 def store_phnn_model(storepath, model, optimizer, **kwargs):
     """
     Stores a :py:class:`PseudoHamiltonianNN` with additional information
@@ -337,87 +346,93 @@
     * * kwargs : dict
         Contains additional information about for instance training
         hyperparameters and loss values.
 
     """
 
     metadict = {}
-    metadict['nstates'] = model.nstates
-    metadict['structure_matrix'] = model.structure_matrix
-    metadict['hamiltonian_provided'] = model.hamiltonian_provided
-    metadict['grad_hamiltonian_provided'] = model.grad_hamiltonian_provided
-    metadict['external_forces_provided'] = model.external_forces_provided
-    metadict['dissipation_provided'] = model.dissipation_provided
-    metadict['init_sampler'] = model._initial_condition_sampler
-    metadict['controller'] = model.controller
-    metadict['ttype'] = model.ttype
+    metadict["nstates"] = model.nstates
+    metadict["skewsymmetric_matrix"] = model.skewsymmetric_matrix
+    metadict["hamiltonian_provided"] = model.hamiltonian_provided
+    metadict["grad_hamiltonian_provided"] = model.grad_hamiltonian_provided
+    metadict["external_forces_provided"] = model.external_forces_provided
+    metadict["dissipation_provided"] = model.dissipation_provided
+    metadict["init_sampler"] = model._initial_condition_sampler
+    metadict["controller"] = model.controller
+    metadict["ttype"] = model.ttype
 
-    metadict = {att.__name__ : att for att in model.__attr__}
+    metadict = {att.__name__: att for att in model.__attr__}
 
-    metadict['traininginfo'] = {}
-    metadict['traininginfo']['optimizer_state_dict'] = optimizer.state_dict()
+    metadict["traininginfo"] = {}
+    metadict["traininginfo"]["optimizer_state_dict"] = optimizer.state_dict()
     for key, value in kwargs.items():
-        metadict['traininginfo'][key] = value
+        metadict["traininginfo"][key] = value
 
-    metadict['hamiltonian'] = {}
-    metadict['grad_hamiltonian'] = {}
-    metadict['external_forces'] = {}
-    metadict['dissipation'] = {}
+    metadict["hamiltonian"] = {}
+    metadict["grad_hamiltonian"] = {}
+    metadict["external_forces"] = {}
+    metadict["dissipation"] = {}
 
     if model.hamiltonian_provided:
-        metadict['hamiltonian']['true'] = model.hamiltonian_true
-        metadict['hamiltonian']['hidden_dim'] = None
-        metadict['hamiltonian']['state_dict'] = None
+        metadict["hamiltonian"]["true"] = model.hamiltonian_true
+        metadict["hamiltonian"]["hidden_dim"] = None
+        metadict["hamiltonian"]["state_dict"] = None
     else:
-        metadict['hamiltonian']['true'] = None
-        metadict['hamiltonian']['hidden_dim'] = model.hamiltonian.hidden_dim
-        metadict['hamiltonian']['state_dict'] = model.hamiltonian.state_dict()
+        metadict["hamiltonian"]["true"] = None
+        metadict["hamiltonian"]["hidden_dim"] = model.hamiltonian.hidden_dim
+        metadict["hamiltonian"]["state_dict"] = model.hamiltonian.state_dict()
 
     if model.grad_hamiltonian_provided:
-        metadict['grad_hamiltonian']['true'] = model.grad_hamiltonian_true
+        metadict["grad_hamiltonian"]["true"] = model.grad_hamiltonian_true
     else:
-        metadict['grad_hamiltonian']['true'] = None
+        metadict["grad_hamiltonian"]["true"] = None
 
     if model.external_forces_provided:
-        metadict['external_forces']['true'] = model.external_forces_true
-        metadict['external_forces']['noutputs'] = None
-        metadict['external_forces']['hidden_dim'] = None
-        metadict['external_forces']['timedependent'] = None
-        metadict['external_forces']['statedependent'] = None
-        metadict['external_forces']['external_forces_filter'] = None
-        metadict['external_forces']['ttype'] = None
-        metadict['external_forces']['state_dict'] = None
+        metadict["external_forces"]["true"] = model.external_forces_true
+        metadict["external_forces"]["noutputs"] = None
+        metadict["external_forces"]["hidden_dim"] = None
+        metadict["external_forces"]["timedependent"] = None
+        metadict["external_forces"]["statedependent"] = None
+        metadict["external_forces"]["external_forces_filter"] = None
+        metadict["external_forces"]["ttype"] = None
+        metadict["external_forces"]["state_dict"] = None
     else:
-        metadict['external_forces']['true'] = None
-        metadict['external_forces']['noutputs'] = model.external_forces.noutputs
-        metadict['external_forces']['hidden_dim'] = model.external_forces.hidden_dim
-        metadict['external_forces']['timedependent'] = model.external_forces.timedependent
-        metadict['external_forces']['statedependent'] = model.external_forces.statedependent
-        metadict['external_forces']['external_forces_filter'] = model.external_forces.external_forces_filter.T
-        metadict['external_forces']['ttype'] = model.external_forces.ttype
-        metadict['external_forces']['state_dict'] = model.external_forces.state_dict()
+        metadict["external_forces"]["true"] = None
+        metadict["external_forces"]["noutputs"] = model.external_forces.noutputs
+        metadict["external_forces"]["hidden_dim"] = model.external_forces.hidden_dim
+        metadict["external_forces"][
+            "timedependent"
+        ] = model.external_forces.timedependent
+        metadict["external_forces"][
+            "statedependent"
+        ] = model.external_forces.statedependent
+        metadict["external_forces"][
+            "external_forces_filter"
+        ] = model.external_forces.external_forces_filter.T
+        metadict["external_forces"]["ttype"] = model.external_forces.ttype
+        metadict["external_forces"]["state_dict"] = model.external_forces.state_dict()
 
     if model.dissipation_provided:
-        metadict['dissipation']['true'] = model.dissipation_true
-        metadict['dissipation']['type'] = None
-        metadict['dissipation']['state_is_damped'] = None
-        metadict['dissipation']['ttype'] = None
-        metadict['dissipation']['hidden_dim'] = None
-        metadict['dissipation']['diagonal'] = None
-        metadict['dissipation']['state_dict'] = None
+        metadict["dissipation"]["true"] = model.dissipation_true
+        metadict["dissipation"]["type"] = None
+        metadict["dissipation"]["state_is_damped"] = None
+        metadict["dissipation"]["ttype"] = None
+        metadict["dissipation"]["hidden_dim"] = None
+        metadict["dissipation"]["diagonal"] = None
+        metadict["dissipation"]["state_dict"] = None
 
     else:
-        metadict['dissipation']['true'] = None
-        metadict['dissipation']['type'] = str(type(model.R))
-        if 'r_estimator' in metadict['dissipation']['type'].lower():
-            metadict['dissipation']['state_is_damped'] = model.R.state_is_damped
-            metadict['dissipation']['ttype'] = model.R.ttype
-            metadict['dissipation']['hidden_dim'] = None
-            metadict['dissipation']['diagonal'] = None
+        metadict["dissipation"]["true"] = None
+        metadict["dissipation"]["type"] = str(type(model.R))
+        if "r_estimator" in metadict["dissipation"]["type"].lower():
+            metadict["dissipation"]["state_is_damped"] = model.R.state_is_damped
+            metadict["dissipation"]["ttype"] = model.R.ttype
+            metadict["dissipation"]["hidden_dim"] = None
+            metadict["dissipation"]["diagonal"] = None
         else:
-            metadict['dissipation']['state_is_damped'] = None
-            metadict['dissipation']['ttype'] = None
-            metadict['dissipation']['hidden_dim'] = model.R.hidden_dim
-            metadict['dissipation']['diagonal'] = model.R.diagonal
-        metadict['dissipation']['state_dict'] = model.R.state_dict()
+            metadict["dissipation"]["state_is_damped"] = None
+            metadict["dissipation"]["ttype"] = None
+            metadict["dissipation"]["hidden_dim"] = model.R.hidden_dim
+            metadict["dissipation"]["diagonal"] = model.R.diagonal
+        metadict["dissipation"]["state_dict"] = model.R.state_dict()
 
     torch.save(metadict, storepath)
```

### Comparing `phlearn-1.1.0/phlearn/phnns/train_utils.py` & `phlearn-1.1.2/phlearn/phnns/train_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,24 @@
 from tqdm import trange
 
 from .pseudo_hamiltonian_neural_network import (
     PseudoHamiltonianNN,
     load_phnn_model,
     store_phnn_model,
 )
-from .conservative_dissipative_neural_network import (
-    ConservativeDissipativeNN,
+from .pseudo_hamiltonian_pde_neural_network import (
+    PseudoHamiltonianPDENN,
     load_cdnn_model,
-    store_cdnn_model
+    store_cdnn_model,
 )
-from ..phsystems.pseudo_Hamiltonian_system import PseudoHamiltonianSystem
-from ..phsystems.conservative_dissipative_system import ConservativeDissipativeSystem
-from .models import load_baseline_model, store_baseline_model
-
-__all__ = [
-    "generate_dataset",
-    "train",
-    "compute_validation_loss",
-    "batch_data",
-    "train_one_epoch",
-    "l1_loss_pHnn",
-    "npoints_to_ntrajectories_tsample",
-    "EarlyStopping",
-    "load_dynamic_system_model",
-    "store_dynamic_system_model",
-]
-
+from ..phsystems.ode.pseudo_hamiltonian_system import PseudoHamiltonianSystem
+from ..phsystems.pde.pseudo_hamiltonian_pde_system import (
+    PseudoHamiltonianPDESystem,
+)
+from .dynamic_system_neural_network import load_baseline_model, store_baseline_model
 
 def generate_dataset(
     pH_system,
     ntrajectories,
     t_sample,
     true_derivatives=False,
     nsamples=None,
@@ -105,18 +93,18 @@
     x = np.zeros((ntrajectories, traj_length, nstates))
     dxdt = np.zeros((ntrajectories, traj_length, nstates))
     t = np.zeros((ntrajectories, traj_length))
     u = np.zeros((ntrajectories, traj_length - 1, nstates))
     if references is None:
         references = [None] * ntrajectories
 
-    for i in range(ntrajectories):
+    for i in tqdm(range(ntrajectories)):
         x[i], dxdt[i], t[i], u[i] = pH_system.sample_trajectory(
             t_sample, noise_std=noise_std, reference=references[i]
-                                                                )
+        )
 
     dt = torch.tensor([t[0, 1] - t[0, 0]], dtype=ttype)
 
     if isinstance(pH_system, PseudoHamiltonianSystem):
         x_start = torch.tensor(x[:, :-1], dtype=ttype).reshape(-1, nstates)
         x_end = torch.tensor(x[:, 1:], dtype=ttype).reshape(-1, nstates)
         t_start = torch.tensor(t[:, :-1], dtype=ttype).reshape(-1, 1)
@@ -126,40 +114,40 @@
             u = torch.zeros_like(x_start, dtype=ttype)
         else:
             u = torch.tensor(u[:, :-1], dtype=ttype).reshape(-1, nstates)
         if true_derivatives:
             dxdt = torch.tensor(dxdt[:, :-1], dtype=ttype).reshape(-1, nstates)
         else:
             dxdt = (x_end - x_start).clone().detach() / dt[0, 0]
-    elif isinstance(pH_system, ConservativeDissipativeSystem):
+    elif isinstance(pH_system, PseudoHamiltonianPDESystem):
         x_start = torch.tensor(x[:, :-1], dtype=ttype).reshape(-1, 1, nstates)
         x_end = torch.tensor(x[:, 1:], dtype=ttype).reshape(-1, 1, nstates)
         t_start = torch.tensor(t[:, :-1], dtype=ttype).reshape(-1, 1, 1)
         t_end = torch.tensor(t[:, 1:], dtype=ttype).reshape(-1, 1, 1)
         dt = dt * torch.ones_like(t_start, dtype=ttype)
         u = torch.zeros_like(x_start, dtype=ttype)
         if true_derivatives:
-            dxdt = torch.tensor(
-                dxdt[:, :-1], dtype=ttype).reshape(-1, 1, nstates)
+            dxdt = torch.tensor(dxdt[:, :-1], dtype=ttype).reshape(-1, 1, nstates)
         else:
             dxdt = (x_end - x_start).clone().detach() / dt[0, 0]
-        xspatial = torch.tensor(np.repeat(xspatial.reshape(1, 1, -1), dxdt.shape[0], axis=0),
-                                dtype=ttype).reshape(dxdt.shape[0], 1, -1)
+        xspatial = torch.tensor(
+            np.repeat(xspatial.reshape(1, 1, -1), dxdt.shape[0], axis=0), dtype=ttype
+        ).reshape(dxdt.shape[0], 1, -1)
     else:
-        print('Unknown system')
+        print("Unknown system")
         return
 
     if nsamples is not None:
         x_start, x_end = x_start[:nsamples], x_end[:nsamples]
         t_start, t_end = t_start[:nsamples], t_end[:nsamples]
         dxdt = dxdt[:nsamples]
 
     if isinstance(pH_system, PseudoHamiltonianSystem):
         return (x_start, x_end, t_start, t_end, dt, u), dxdt
-    elif isinstance(pH_system, ConservativeDissipativeSystem):
+    elif isinstance(pH_system, PseudoHamiltonianPDESystem):
         return (x_start, x_end, t_start, t_end, dt, u, xspatial), dxdt
 
 
 def train(
     model,
     integrator,
     traindata,
@@ -243,16 +231,15 @@
     traindata_batched = batch_data(traindata, batch_size, shuffle)
     if batch_size_val is not None:
         valdata_batched = batch_data(traindata, batch_size, False)
     else:
         valdata_batched = None
 
     if optimizer is None:
-        optimizer = torch.optim.Adam(
-            model.parameters(), lr=1e-3, weight_decay=1e-4)
+        optimizer = torch.optim.Adam(model.parameters(), lr=1e-3, weight_decay=1e-4)
 
     vloss = None
     vloss_best = np.inf
     newbest = True
     early_stopping = None
 
     if early_stopping_patience is not None:
@@ -265,107 +252,114 @@
                 ".", ""
             ).replace("-", "").replace(":", "").replace(" ", "")
         if not os.path.exists(store_best_dir):
             os.makedirs(store_best_dir)
         best_path = None
 
     best_model = model
-    for epoch in range(epochs):
-        if shuffle:
-            traindata_batched = batch_data(traindata, batch_size, shuffle)
-        model.train(True)
-        start = datetime.datetime.now()
-        avg_loss = train_one_epoch(
-            model,
-            traindata_batched,
-            loss_fn,
-            optimizer,
-            integrator,
-            l1_param_forces,
-            l1_param_dissipation,
-        )
-        end = datetime.datetime.now()
-        model.train(False)
-
-        if verbose:
-            if epoch % 1 == 0:
-                print(f"\nEpoch {epoch+1}")
-                print(
-                    f"Training loss: {np.format_float_scientific(avg_loss, 2)}")
-                delta = end - start
-                print(
-                    "Epoch training time:"
-                    f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
-                    "seconds"
-                )
-
-        if valdata is not None:
+    with trange(epochs) as step_range:
+        for epoch in step_range:
+            if shuffle:
+                traindata_batched = batch_data(traindata, batch_size, shuffle)
+            model.train(True)
             start = datetime.datetime.now()
-            vloss = compute_validation_loss(
-                model, integrator, valdata, valdata_batched, loss_fn
+            avg_loss = train_one_epoch(
+                model,
+                traindata_batched,
+                loss_fn,
+                optimizer,
+                integrator,
+                l1_param_forces,
+                l1_param_dissipation,
             )
             end = datetime.datetime.now()
+            model.train(False)
+
             if verbose:
-                print(
-                    "Validation loss: " f"{np.format_float_scientific(vloss, 2)}")
-                delta = end - start
-                print(
-                    "Validation loss computed in"
-                    f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
-                    "seconds"
+                step_range.set_postfix(epoch=epoch, loss=avg_loss)
+            # if verbose:
+            #     if epoch % 1 == 0:
+            #         print(f"\nEpoch {epoch+1}")
+            #         print(
+            #             f"Training loss: {np.format_float_scientific(avg_loss, 2)}")
+            #         delta = end - start
+            #         print(
+            #             "Epoch training time:"
+            #             f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
+            #             "seconds"
+            #         )
+
+            if valdata is not None:
+                start = datetime.datetime.now()
+                vloss = compute_validation_loss(
+                    model, integrator, valdata, valdata_batched, loss_fn
                 )
-            if vloss <= vloss_best:
-                newbest = True
+                end = datetime.datetime.now()
                 if verbose:
-                    print("New best validation loss")
-                vloss_best = vloss
-                if return_best:
-                    best_model = copy.deepcopy(model)
-
-            if early_stopping is not None:
-                if early_stopping(vloss):
+                    print("Validation loss: " f"{np.format_float_scientific(vloss, 2)}")
+                    delta = end - start
+                    print(
+                        "Validation loss computed in"
+                        f" {delta.seconds:d}.{int(delta.microseconds / 1e4):d}"
+                        "seconds"
+                    )
+                if vloss <= vloss_best:
+                    newbest = True
                     if verbose:
-                        print(f"Early stopping at epoch {epoch+1}/{epochs}")
-                    break
-        else:
-            newbest = True
-        if store_best and newbest:
-            if best_path is not None:
-                try:
-                    os.remove(best_path)
-                except:
-                    print("The best model is gone.")
-            if modelname is None:
-                best_path = os.path.join(
-                    store_best_dir,
-                    str(datetime.datetime.now())
-                    .replace(".", "")
-                    .replace("-", "")
-                    .replace(":", "")
-                    .replace(" ", "")
-                    + ".model",
-                )
+                        print("New best validation loss")
+                    vloss_best = vloss
+                    if return_best:
+                        best_model = copy.deepcopy(model)
+
+                if early_stopping is not None:
+                    if early_stopping(vloss):
+                        if verbose:
+                            print(f"Early stopping at epoch {epoch+1}/{epochs}")
+                        break
             else:
-                best_path = os.path.join(store_best_dir, modelname)
-            trainingdetails["epochs"] = epoch + 1
-            trainingdetails["val_loss"] = vloss
-            trainingdetails["train_loss"] = avg_loss
-            store_dynamic_system_model(
-                best_path, model, optimizer, **trainingdetails)
-            if verbose:
-                print(f"Stored new best model {best_path}")
-            newbest = False
+                newbest = True
+            if store_best and newbest:
+                if best_path is not None:
+                    try:
+                        os.remove(best_path)
+                    except:
+                        print("The best model is gone.")
+                if modelname is None:
+                    best_path = os.path.join(
+                        store_best_dir,
+                        str(datetime.datetime.now())
+                        .replace(".", "")
+                        .replace("-", "")
+                        .replace(":", "")
+                        .replace(" ", "")
+                        + ".model",
+                    )
+                else:
+                    best_path = os.path.join(store_best_dir, modelname)
+                trainingdetails["epochs"] = epoch + 1
+                trainingdetails["val_loss"] = vloss
+                trainingdetails["train_loss"] = avg_loss
+                store_dynamic_system_model(
+                    best_path, model, optimizer, **trainingdetails
+                )
+                if verbose:
+                    print(f"Stored new best model {best_path}")
+                newbest = False
 
-    if isinstance(best_model, ConservativeDissipativeNN) and best_model.external_forces is not None:
+    if (
+        isinstance(best_model, PseudoHamiltonianPDENN)
+        and best_model.external_forces is not None
+    ):
         best_model.dV_correction()
         best_model.external_forces_correction()
         if store_best:
             store_dynamic_system_model(
-                best_path, best_model, optimizer, **trainingdetails)
-    
+                best_path, best_model, optimizer, **trainingdetails
+            )
+
     return best_model, vloss
 
 
 def compute_validation_loss(
     model, integrator, valdata=None, valdata_batched=None, loss_fn=torch.nn.MSELoss()
 ):
     """
@@ -396,24 +390,24 @@
     vloss : float
 
     """
 
     vloss = 0
     if valdata_batched is not None:
         for input_tuple, dxdt in valdata_batched:
-            if isinstance(model, ConservativeDissipativeNN):
+            if isinstance(model, PseudoHamiltonianPDENN):
                 lhs_hat = model.time_derivative(integrator, *input_tuple)
                 lhs = model.lhs(dxdt)
                 vloss += loss_fn(lhs_hat, lhs)
             else:
                 dxdt_hat = model.time_derivative(integrator, *input_tuple)
                 vloss += loss_fn(dxdt_hat, dxdt)
         vloss = vloss / len(valdata_batched)
     else:
-        if isinstance(model, ConservativeDissipativeNN):
+        if isinstance(model, PseudoHamiltonianPDENN):
             lhs_hat = model.time_derivative(integrator, *valdata[0])
             lhs = model.lhs(valdata[1])
             vloss += loss_fn(lhs_hat, lhs)
         else:
             dxdt_hat = model.time_derivative(integrator, *valdata[0])
             vloss = loss_fn(dxdt_hat, valdata[1])
     return float(vloss.detach().numpy())
@@ -440,15 +434,15 @@
     if shuffle:
         permutation = torch.randperm(nsamples)
     else:
         permutation = torch.arange(nsamples)
     nbatches = np.ceil(nsamples / batch_size).astype(int)
     batched = [(None, None)] * nbatches
     for i in range(0, nbatches):
-        indices = permutation[i * batch_size: (i + 1) * batch_size]
+        indices = permutation[i * batch_size : (i + 1) * batch_size]
         input_tuple = [data[0][j][indices] for j in range(len(data[0]))]
         dxdt = data[1][indices]
         batched[i] = (input_tuple, dxdt)
     return batched
 
 
 def train_one_epoch(
@@ -486,42 +480,46 @@
 
     """
 
     running_loss = 0.0
     optimizer.zero_grad()
     for input_tuple, dxdt in traindata_batched:
         with torch.cuda.amp.autocast():
-            if isinstance(model, ConservativeDissipativeNN):
+            if isinstance(model, PseudoHamiltonianPDENN):
                 lhs_hat = model.time_derivative(integrator, *input_tuple)
                 lhs = model.lhs(dxdt)
                 loss = loss_fn(lhs_hat, lhs)
             else:
                 dxdt_hat = model.time_derivative(integrator, *input_tuple)
                 loss = loss_fn(dxdt_hat, dxdt)
-            if (isinstance(model, PseudoHamiltonianNN) or
-                isinstance(model, ConservativeDissipativeNN)) and (
-                (l1_param_forces > 0) or (l1_param_dissipation > 0)
-            ):
+            if (
+                isinstance(model, PseudoHamiltonianNN)
+                or isinstance(model, PseudoHamiltonianPDENN)
+            ) and ((l1_param_forces > 0) or (l1_param_dissipation > 0)):
                 loss += l1_loss_pHnn(
                     model,
                     l1_param_forces,
                     l1_param_dissipation,
                     input_tuple[0],
                     input_tuple[2],
-                    input_tuple[6] if isinstance(model, ConservativeDissipativeNN) else None
+                    input_tuple[6]
+                    if isinstance(model, PseudoHamiltonianPDENN)
+                    else None,
                 )
         loss.backward()
         optimizer.step()
         optimizer.zero_grad()
         running_loss += loss.item()
 
     return running_loss / len(traindata_batched)
 
 
-def l1_loss_pHnn(pHnn_model, l1_param_forces, l1_param_dissipation, x, t=None, xspatial=None):
+def l1_loss_pHnn(
+    pHnn_model, l1_param_forces, l1_param_dissipation, x, t=None, xspatial=None
+):
     """
     Compute L1 penalty loss of external force and dissipation terms::
 
         L1 = l1_param_forces * | f(x, t) | + l1_param_dissipation * | R(x) |
 
     Parameters
     ----------
@@ -538,39 +536,45 @@
     """
     penalty = 0
     if (
         isinstance(pHnn_model.external_forces, nn.Module)
         and (l1_param_forces > 0)
         and (not pHnn_model.external_forces_provided)
     ):
-        penalty += l1_param_forces * \
-            torch.abs(pHnn_model.external_forces(x, t)).mean()
+        penalty += l1_param_forces * torch.abs(pHnn_model.external_forces(x, t)).mean()
     if (
         isinstance(pHnn_model, PseudoHamiltonianNN)
         and isinstance(pHnn_model.R, nn.Module)
         and (l1_param_dissipation > 0)
         and (not pHnn_model.R_provided)
     ):
         penalty += l1_param_dissipation * torch.abs(pHnn_model.R(x)).mean()
     if (
-        isinstance(pHnn_model, ConservativeDissipativeNN)
+        isinstance(pHnn_model, PseudoHamiltonianPDENN)
         and (l1_param_forces > 0)
         and (not pHnn_model.external_forces_provided)
         and (pHnn_model.kernel_sizes[3] > 0)
     ):
-        penalty += l1_param_forces * \
-            torch.abs(pHnn_model.external_forces(x, t, xspatial)-pHnn_model.external_forces(torch.zeros_like(x), t, xspatial)).mean()
+        penalty += (
+            l1_param_forces
+            * torch.abs(
+                pHnn_model.external_forces(x, t, xspatial)
+                - pHnn_model.external_forces(torch.zeros_like(x), t, xspatial)
+            ).mean()
+        )
     if (
-        isinstance(pHnn_model, ConservativeDissipativeNN)
+        isinstance(pHnn_model, PseudoHamiltonianPDENN)
         and (l1_param_dissipation > 0)
         and ((pHnn_model.kernel_sizes[0] > 1) or (pHnn_model.kernel_sizes[2] > 1))
     ):
-        penalty += l1_param_dissipation * \
-            (torch.abs(pHnn_model.D_flat().sum()-1.).mean()+torch.abs(pHnn_model.P().sum()-1.).mean())
-    
+        penalty += l1_param_dissipation * (
+            torch.abs(pHnn_model.A().sum() - 1.0).mean()
+            + torch.abs(pHnn_model.R().sum() - 1.0).mean()
+        )
+
     return penalty
 
 
 def npoints_to_ntrajectories_tsample(npoints, tmax, dt):
     """
     Compute number of trajectories and the necessary sample time to
     achieve *npoints* samples from trajectories lasting *tmax* time with
@@ -649,28 +653,28 @@
     """
     Loads a DynamicSystemNN from disk. See
     :py:meth:~`pseudo_hamiltonian_neural_network.load_phnn_model` and
     :py:meth:~`model.load_baseline_model`.
     """
 
     metadict = torch.load(modelpath)
-    if 'dissipation_provided' in metadict.keys():
+    if "dissipation_provided" in metadict.keys():
         return load_phnn_model(modelpath)
-    elif 'symmetric_matrix' in metadict.keys():  # fix
+    elif "lhs_matrix" in metadict.keys():  # fix
         return load_cdnn_model(modelpath)
     else:
         return load_baseline_model(modelpath)
 
 
 def store_dynamic_system_model(storepath, model, optimizer, **kwargs):
     """
     Stores a DynamicSystemNN to disk. See
     :py:meth:~`port_hamiltonian_neural_network.store_phnn_model` and
     :py:meth:~`model.store_baseline_model`.
     """
 
     if isinstance(model, PseudoHamiltonianNN):
         store_phnn_model(storepath, model, optimizer, **kwargs)
-    elif isinstance(model, ConservativeDissipativeNN):
+    elif isinstance(model, PseudoHamiltonianPDENN):
         store_cdnn_model(storepath, model, optimizer, **kwargs)
     else:
         store_baseline_model(storepath, model, optimizer, **kwargs)
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/burgers_system.py` & `phlearn-1.1.2/phlearn/phsystems/pde/heat_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,158 +1,156 @@
 import numpy as np
-
-# import autograd.numpy as np
-# from autograd import jacobian
-# import numpy.linalg as la
 from scipy.sparse import spdiags
-import numpy.linalg as la
-from .fvm import Burgers, solve
-
 
+from .pseudo_hamiltonian_pde_system import PseudoHamiltonianPDESystem
 
-from .conservative_dissipative_system import (
-    ConservativeDissipativeSystem,
-)  # Should be changed to preservation-dissipation system
 
-__all__ = ["BurgersSystem", "init_burgers", "initial_condition_burgers"]
+class HeatEquationSystem(PseudoHamiltonianPDESystem):
+    """
+    Implements a discretization of the heat equation with an
+    optional external force,
 
+    u_t - u_xx = f(u,t,x),
+
+    on the pseudo-Hamiltonian formulation
+
+    du/dt = -grad[V(u)] + F(u,t,x)
+
+    where u is a vector of the system states at the spatial points given by
+    x, and t is time.
+
+    The system is by default integrated in time using the implicit midpoint method. 
+    The line 'self.sample_trajectory = self.sample_trajectory_midpoint' can be 
+    commented out to instead use the RK45 method of scipy.
+
+    Parameters
+    ----------
+    x : nparray, default np.linspace(0, 1.0 - 1/100, 100)
+        The spatial discretization points.
+    nu : number, default -1.0
+        The parameter nu in the Cahn-Hilliard equation.
+    alpha : number, default 1.0
+        The parameter alpha in the Cahn-Hilliard equation.
+    mu : number, default -0.001
+        The parameter mu in the Cahn-Hilliard equation.
+    init_sampler : callable, default None
+        Function for sampling initial conditions. Callable taking
+        a numpy random generator as input and returning an ndarray
+        of shape same as x with initial conditions for the system.
+        This sampler is used when calling
+        CahnHilliardSystem.sample_trajectory if no initial
+        condition is provided.
+    kwargs : any, optional
+        Keyword arguments that are passed to PseudoHamiltonianPDESystem
+        constructor.
 
-class BurgersSystem(ConservativeDissipativeSystem):
     """
-    Add description (see ODE examples)
 
-    """
 
     def __init__(
         self,
-        x=np.linspace(0, 20.0 - 0.2, 100),
-        eta=6.0,
-        gamma=1.0,
-        nu=0.0,
-        force=None,
-        force_jac=None,
+        x=np.linspace(0, 6.0 - 6 / 300, 300),
+        nu=1.0,
+        init_sampler=None,
         **kwargs
     ):
         M = x.size
         dx = x[-1] / (M - 1)
         e = np.ones(M)
-        deltafx = 1 / dx * spdiags([e, -e, e], np.array([-M + 1, 0, 1]), M, M)
-        delta2cx = (
+        # Forward difference matrix:
+        Dp = (
+            1 / dx * spdiags([e, -e, e], np.array([-M + 1, 0, 1]), M, M).toarray()
+        )
+        # Central difference matrix:
+        D1 = (
+            0.5
+            / dx
+            * spdiags([e, -e, e, -e], np.array([-M + 1, -1, 1, M - 1]), M, M).toarray()
+        )  
+        # 2nd order central difference matrix:
+        D2 = (
             1
             / dx**2
-            * spdiags([e, e, -2 * e, e, e], np.array([-M + 1, -1, 0, 1, M - 1]), M, M)
-        )
-        Dp = deltafx.toarray()  # Fix this so it doesn't go via spdiags
-        D2 = delta2cx.toarray()
-        deltacx = (
-            0.5 / dx * spdiags([e, -e, e, -e], np.array([-M + 1, -1, 1, M - 1]), M, M)
-        )
-        D1 = deltacx.toarray()
-        structure_matrix = D1
-        self.structure_matrix_flat = 0.5 / dx * np.array([[[-1, 0, 1]]])
+            * spdiags(
+                [e, e, -2 * e, e, e], np.array([-M + 1, -1, 0, 1, M - 1]), M, M
+            ).toarray()
+        )  
+        skewsymmetric_matrix = D1
         self.x = x
         self.M = M
-        self.eta = eta
-        self.gamma = gamma
         self.D2 = D2
 
         def ham(u):
-            return np.sum(
-                1 / 6 * eta * u**3 - (0.5 * gamma**2 * (np.matmul(Dp, u.T)) ** 2).T,
-                axis=1,
-            )
+            return np.sum(np.zeros_like(u), axis=1)
+
+        def dissintegral(u):
+            return np.sum(0.5 * nu * (np.matmul(Dp, u.T) ** 2).T, axis=1)
 
         def ham_grad(u):
-            return 0.5 * eta * u**2 + (gamma**2 * np.matmul(D2, u.T)).T
+            return np.zeros_like(u)
+
+        def dissintegral_grad(u):
+            return -nu * u @ D2
+
+        def ham_hessian(u):
+            return np.zeros_like(D1)
+
+        def dissintegral_hessian(u):
+            return -nu * D2
+
+        if init_sampler is None:
+            init_sampler = initial_condition_heat(x)
 
         super().__init__(
             nstates=M,
-            skewsymmetric_matrix=structure_matrix,
+            skewsymmetric_matrix=skewsymmetric_matrix,
             hamiltonian=ham,
+            dissintegral=dissintegral,
             grad_hamiltonian=ham_grad,
+            grad_dissintegral=dissintegral_grad,
+            hess_hamiltonian=ham_hessian,
+            hess_dissintegral=dissintegral_hessian,
+            init_sampler=init_sampler,
             **kwargs
         )
 
-    def sample_trajectory(self, t, x0=None, noise_std=0, reference=None):
-        """
-        Samples a trajectory of the system at times *t*.
-
-        Parameters
-        ----------
-        t : (T, 1) ndarray
-            Times at which the trajectory is sampled.
-        x0 : (N,) ndarray, default None
-            Initial condition.
-        noise_std : number, default 0.
-            Standard deviation of Gaussian white noise added to the
-            samples of the trajectory.
-        reference : porthamiltonian.control.Reference, default None
-            If the system has a controller a reference object may be
-            passed.
-
-        Returns
-        -------
-        x : (T, N) ndarray
-        dxdt : (T, N) ndarray
-        t : (T, 1) ndarray
-        us : (T, N) ndarray
-
-        """
-
-        if x0 is None:
-            x0 = self._initial_condition_sampler(self.rng)
-
-        x = np.zeros([t.shape[0], x0.shape[-1]])
-        dxdt = np.zeros_like(x)
-        us = np.zeros([t.shape[0] - 1, x0.shape[-1]])
-        x[0, :] = x0
-        _, u, all_u, du_dts = solve(
-            x0, t[-1], x.shape[1], x.shape[0], Burgers(), x_end=self.x.amax()
-        )
-        assert noise_std == 0
-        return all_u, du_dts, t, us
+        self.skewsymmetric_matrix_flat = 0.5 / dx * np.array([[[-1, 0, 1]]])
 
 
-def init_burgers():
+def initial_condition_heat(x=np.linspace(0, 6.0 - 6 / 300, 300)):
     """
-    Initialize a standard Burgers system
+    Creates an initial condition sampler for the heat eqation.
+
+    Parameters
+    ----------
+    x : numpy.ndarray, optional
+        Spatial grid on which to create the initial conditions. The default is 
+        an equidistant grid between 0 and 5.98 with step size 0.02.
 
     Returns
     -------
-    BurgersSystem
-
+    callable
+        A function that takes a numpy random generator as input and returns an
+        initial state on the spatial grid x.
     """
-    x_end = 20
-    x_points = 100
-    dx = x_end / x_points
-    x = np.linspace(0, x_end - dx, x_points)
-    eta = 6.0
-    gamma = 1.0
-
-    return BurgersSystem(
-        x=x, eta=eta, gamma=gamma, init_sampler=initial_condition_burgers(x, eta)
-    )
 
-
-def initial_condition_burgers(x=np.linspace(0, 20.0 - 0.2, 100), eta=6.0):
-    """
-    Add description (see ODE examples)
-
-    """
     M = x.size
     P = (x[-1] - x[0]) * M / (M - 1)
-    sech = lambda a: 1 / np.cosh(a)
 
     def sampler(rng):
-        k1, k2 = rng.uniform(0.5, 2.0, 2)
-        d1 = rng.uniform(0.2, 0.3, 1)
-        d2 = d1 + rng.uniform(0.2, 0.5, 1)
+        d1, d2 = rng.uniform(0.3, 3, 2)
+        c1, c2 = rng.uniform(0.5, 1.5, 2)
+        k1 = rng.uniform(0.5, 3.0, 1)
+        k2 = rng.uniform(10.0, 20.0, 1)
+        n1 = rng.uniform(20.0, 40.0, 1)
+        n2 = rng.uniform(0.05, 0.15, 1)
         u0 = 0
-        u0 += (-6.0 / -eta) * 2 * k1**2 * sech(k1 * (x - P * d1)) ** 2
-        u0 += (-6.0 / -eta) * 2 * k2**2 * sech(k2 * (x - P * d2)) ** 2
-        u0 = np.concatenate([u0[M:], u0[:M]], axis=-1)
-        # Diversifying between having the smaller wave to the left or right of the bigger one:
-        if np.random.randint(0, 2) == 1:
-            u0 = u0[::-1].copy()
+        u0 += (
+            rng.uniform(-5.0, 5.0, 1)
+            - c1 * np.tanh(n1 * (x - d1))
+            + c1 * np.tanh(n1 * (x - P + d1))
+        )
+        u0 += -c2 * np.tanh(n1 * (x - d2)) + c2 * np.tanh(n1 * (x - P + d2))
+        u0 += n2 * np.sin(k1 * np.pi * x) ** 2 * np.sin(k2 * np.pi * x)
         return u0
 
-    return sampler
+    return sampler
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/conservative_dissipative_system.py` & `phlearn-1.1.2/phlearn/phsystems/pde/pseudo_hamiltonian_pde_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-
 import autograd.numpy as np
 import autograd
 from scipy.integrate import solve_ivp
 
-from ..utils.derivatives import time_derivative
-from ..utils.utils import midpoint_method
-
-__all__ = ['ConservativeDissipativeSystem', 'zero_force']
+from ...utils.derivatives import time_derivative
+from ...utils.utils import midpoint_method
 
 
-class ConservativeDissipativeSystem():
+class PseudoHamiltonianPDESystem:
     """
-    Implements a conservative-dissipative system of the form::
+    Implements a spatially discretized pseudo-Hamiltonian PDE system of the form:
+
+        dx/dt = S*grad[H(x)] - R*grad[V(x)] + F(x, t, xspatial)
 
-        dx/dt = S(x)*grad[H(x)] - R(x)*grad[V(x)] + F(x, t)
+    where x is the system state, A is a symmetric matrix, S is a skew-symmetric matrix,
+    R is the symmetric dissipation matrix, H and V are discretized integrals of the systemm,
+    F is the external force depending on state, time and space.
 
-    where x is the system state, S is the interconection matrix,
-    H is the Hamiltonian of the system, V is the dissipating integral,
-    F is the external forces.
+    What is x here is usually u in the literature, and xspatial is x. We use x for
+    the state to be consistent with the ODE case.
 
     Parameters
     ----------
         nstates : int
             Number of system states N.
 
         skewsymmetric_matrix : (N, N) ndarray or callable, default None
@@ -85,52 +85,66 @@
             of shape (nstates,) with inital conditions for the system.
             This sampler is used when calling
             PseudoHamiltonianSystem.sample_trajectory if no initial
             condition is provided.
 
     """
 
-    def __init__(self, nstates, lhs_matrix=None,
-                 skewsymmetric_matrix=None,
-                 dissipation_matrix=None,
-                 hamiltonian=None, dissintegral=None,
-                 grad_hamiltonian=None, grad_dissintegral=None,
-                 hess_hamiltonian=None, hess_dissintegral=None,
-                 external_forces=None, jac_external_forces=None,
-                 controller=None,
-                 init_sampler=None):
-
+    def __init__(
+        self,
+        nstates,
+        lhs_matrix=None,
+        skewsymmetric_matrix=None,
+        dissipation_matrix=None,
+        hamiltonian=None,
+        dissintegral=None,
+        grad_hamiltonian=None,
+        grad_dissintegral=None,
+        hess_hamiltonian=None,
+        hess_dissintegral=None,
+        external_forces=None,
+        jac_external_forces=None,
+        controller=None,
+        init_sampler=None,
+    ):
         self.nstates = nstates
 
         self.lhs_matrix_provided = True
         if lhs_matrix is None:
             lhs_matrix = np.eye(nstates)
             self.lhs_matrix_provided = False
 
         self.lhs_matrix = lhs_matrix
-        self.A = lambda x: lhs_matrix # check if this is necessary
-        
+        self.A = lambda x: lhs_matrix 
+
         if skewsymmetric_matrix is None:
             npos = nstates // 2
             skewsymmetric_matrix = np.block(
-                [[np.zeros([npos, npos]), np.eye(npos)],
-                 [-np.eye(npos), np.zeros([npos, npos])]])
+                [
+                    [np.zeros([npos, npos]), np.eye(npos)],
+                    [-np.eye(npos), np.zeros([npos, npos])],
+                ]
+            )
 
         if not callable(skewsymmetric_matrix):
             self.skewsymmetric_matrix = skewsymmetric_matrix
             self.S = lambda x: skewsymmetric_matrix
         else:
             self.skewsymmetric_matrix = None
             self.S = skewsymmetric_matrix
 
         if dissipation_matrix is None:
             dissipation_matrix = np.eye(nstates)
 
         self.dissipation_matrix = dissipation_matrix
-        self.R = lambda x: dissipation_matrix # check if this is necessary
+        self.R = lambda x: dissipation_matrix
+
+        self.skewsymmetric_matrix_flat = np.array([[[-1, 0, 1]]])
+        self.dissipation_matrix_flat = np.array([[[1]]])
+        self.lhs_matrix_flat = np.array([[[1]]])
 
         self.H = hamiltonian
         self.dH = grad_hamiltonian
         self.ddH = hess_hamiltonian
         if grad_hamiltonian is None:
             self.dH = self._dH
         if hess_hamiltonian is None:
@@ -200,24 +214,24 @@
             dH = self.dH(x)
         else:
             dH = np.zeros_like(x)
         if self.V is not None:
             dV = self.dV(x)
         else:
             dV = np.zeros_like(x)
-        if (len(S.shape) == 3):
-            dynamics = ((np.matmul(S, np.atleast_3d(dH))
-                        - np.matmul(R,np.atleast_3d(dV))).reshape(x.shape)
-                        + self.external_forces(x, t))
+        if len(S.shape) == 3:
+            dynamics = (
+                np.matmul(S, np.atleast_3d(dH)) - np.matmul(R, np.atleast_3d(dV))
+            ).reshape(x.shape) + self.external_forces(x, t)
         else:
-            dynamics = dH@(S.T) - dV@R + self.external_forces(x, t)
+            dynamics = dH @ (S.T) - dV @ R + self.external_forces(x, t)
         if u is not None:
             dynamics += u
         return dynamics
-    
+
     def x_dot_jacobian(self, x, t, u=None):
         """
         Computes the Jacobian of the right hand side of the pseudo-
         Hamiltonian equation.
 
         Parameters
         ----------
@@ -232,18 +246,18 @@
         """
 
         S = self.S(x)
         R = self.R(x)
         jacobian = np.zeros_like(S)
         if self.H is not None:
             ddH = self.ddH(x)
-            jacobian += np.matmul(S,ddH)
+            jacobian += np.matmul(S, ddH)
         if self.V is not None:
             ddV = self.ddV(x)
-            jacobian -= np.matmul(R,ddV)
+            jacobian -= np.matmul(R, ddV)
         if self.external_forces_jacobian is not None:
             jacobian += self.external_forces_jacobian(x, t)
         return jacobian
 
     def sample_trajectory(self, t, x0=None, noise_std=0, reference=None):
         """
         Samples a trajectory of the system at times *t*, found by using the
@@ -272,32 +286,35 @@
         """
 
         if x0 is None:
             x0 = self._initial_condition_sampler(self.rng)
 
         if self.lhs_matrix_provided:
             lhs_matrix_inv = np.linalg.inv(self.lhs_matrix)
-            x_dot = lambda t, x: np.matmul(lhs_matrix_inv,
-                                           self.x_dot(x.reshape(1, x.shape[-1]),
-                                           np.array(t).reshape((1, 1))).T).T
+            x_dot = lambda t, x: np.matmul(
+                lhs_matrix_inv,
+                self.x_dot(x.reshape(1, x.shape[-1]), np.array(t).reshape((1, 1))).T,
+            ).T
         else:
-            x_dot = lambda t, x: self.x_dot(x.reshape(1, x.shape[-1]),
-                                            np.array(t).reshape((1, 1)))
-        out_ivp = solve_ivp(fun=x_dot, t_span=(t[0], t[-1]), y0=x0,
-                            t_eval=t, rtol=1e-10)
-        x, t = out_ivp['y'].T, out_ivp['t'].T
+            x_dot = lambda t, x: self.x_dot(
+                x.reshape(1, x.shape[-1]), np.array(t).reshape((1, 1))
+            )
+        out_ivp = solve_ivp(
+            fun=x_dot, t_span=(t[0], t[-1]), y0=x0, t_eval=t, rtol=1e-10
+        )
+        x, t = out_ivp["y"].T, out_ivp["t"].T
         dxdt = self.x_dot(x, t)
         us = None
 
         # Add noise:
-        x += self.rng.normal(size=x.shape)*noise_std
-        dxdt += self.rng.normal(size=dxdt.shape)*noise_std
+        x += self.rng.normal(size=x.shape) * noise_std
+        dxdt += self.rng.normal(size=dxdt.shape) * noise_std
 
         return x, dxdt, t, us
-    
+
     def sample_trajectory_midpoint(self, t, x0=None, noise_std=0, reference=None):
         """
         Samples a trajectory of the system at times *t*, found by using the
         implicit midpoint method for temporal integration, starting from the
         initial state x0. Newton's method is used for solving the system of
         nonlinear equations at each integration step.
 
@@ -328,56 +345,59 @@
         x = np.zeros([t.shape[0], x0.shape[-1]])
         dxdt = np.zeros_like(x)
         us = np.zeros([t.shape[0] - 1, x0.shape[-1]])
         x[0, :] = x0
 
         M = x0.shape[-1]
         if self.lhs_matrix_provided:
-            lhs_matrix_inv = np.linalg.inv(self.lhs_matrix)
-            f = lambda u, t: np.linalg.solve(self.lhs_matrix, self.x_dot(u,t))
-            Df = lambda u, t: np.linalg.solve(self.lhs_matrix, self.x_dot_jacobian(u,t))
+            f = lambda u, t: np.linalg.solve(self.lhs_matrix, self.x_dot(u, t))
+            Df = lambda u, t: np.linalg.solve(
+                self.lhs_matrix, self.x_dot_jacobian(u, t)
+            )
         else:
-            f = lambda u, t: self.x_dot(u,t)
-            Df = lambda u, t: self.x_dot_jacobian(u,t)
+            f = lambda u, t: self.x_dot(u, t)
+            Df = lambda u, t: self.x_dot_jacobian(u, t)
         for i, t_step in enumerate(t[:-1]):
             dt = t[i + 1] - t[i]
-            dxdt[i, :] = f(x[i,:], t[i])
-            x[i+1,:] = midpoint_method(x[i,:],x[i,:],t[i],f,Df,dt,M,1e-12,5)
+            dxdt[i, :] = f(x[i, :], t[i])
+            x[i + 1, :] = midpoint_method(
+                x[i, :], x[i, :], t[i], f, Df, dt, M, 1e-12, 5
+            )
 
         # Add noise:
-        x += self.rng.normal(size=x.shape)*noise_std
-        dxdt += self.rng.normal(size=dxdt.shape)*noise_std
+        x += self.rng.normal(size=x.shape) * noise_std
+        dxdt += self.rng.normal(size=dxdt.shape) * noise_std
 
         return x, dxdt, t, us
 
     def _dH(self, x):
         H = lambda x: self.H(x).sum()
         return autograd.grad(H)(x)
 
     def _dV(self, x):
         V = lambda x: self.V(x).sum()
         return autograd.grad(V)(x)
-    
+
     def _ddH(self, x):
         H = lambda x: self.H(x).sum()
         return autograd.hessian(H)(x)
 
     def _ddV(self, x):
         H = lambda x: self.H(x).sum()
         return autograd.hessian(H)(x)
-    
+
     def _jacforce(self, x, t):
         external_forces_x = lambda x: self.external_forces(x, t)
         return autograd.jacobian(external_forces_x)(x)
 
     def _initial_condition_sampler(self, rng=None):
         if rng is None:
             assert self.rng is not None
             rng = self.rng
-        return rng.uniform(low=-1., high=1.0, size=self.nstates)
+        return rng.uniform(low=-1.0, high=1.0, size=self.nstates)
 
 
 def zero_force(x, t=None):
     """
     A force term that is always zero.
 
     Parameters
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/msd_system.py` & `phlearn-1.1.2/phlearn/phsystems/ode/msd_system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-
 import numpy as np
 
-from .pseudo_Hamiltonian_system import PseudoHamiltonianSystem
-
-__all__ = ['MassSpringDamperSystem', 'init_msdsystem',
-           'initial_condition_radial']
+from .pseudo_hamiltonian_system import PseudoHamiltonianSystem
 
 
 class MassSpringDamperSystem(PseudoHamiltonianSystem):
     """
     Implements a general forced and damped mass-spring system as a
     pseudo-Hamiltonian formulation::
 
@@ -29,24 +25,30 @@
         Scalar damping coefficient. Corresponds to c.
     kwargs  : any, optional
         Keyword arguments that are passed to PseudoHamiltonianSystem constructor.
 
     """
 
     def __init__(self, mass=1.0, spring_constant=1.0, damping=0.3, **kwargs):
-        R = np.array([[0, 0], [0, damping]])
+        R = np.diag([0, damping])
+        M = np.diag([spring_constant / 2, 1 / (2 * mass)])
 
-        def ham(x):
-            return np.dot(x**2, np.array([spring_constant / 2, 1/(2*mass)]))
+        def hamiltonian(x):
+            return x.T @ M @ x
 
-        def ham_grad(x):
-            return np.matmul(x, np.diag([spring_constant, 1/mass]))
+        def hamiltonian_grad(x):
+            return 2 * M @ x
 
-        super().__init__(nstates=2, hamiltonian=ham, grad_hamiltonian=ham_grad,
-                         dissipation_matrix=R, **kwargs)
+        super().__init__(
+            nstates=2,
+            hamiltonian=hamiltonian,
+            grad_hamiltonian=hamiltonian_grad,
+            dissipation_matrix=R,
+            **kwargs
+        )
 
 
 def init_msdsystem():
     """
     Initialize a standard example of a damped mass-spring system affected by a
     sine force.
 
@@ -55,33 +57,35 @@
     MassSpringDamperSystem
 
     """
     f0 = 1.0
     omega = 3
 
     def F(x, t):
-        return (f0*np.sin(omega*t)).reshape(x[..., 1:].shape)*np.array([0, 1])
+        return (f0 * np.sin(omega * t)).reshape(x[..., 1:].shape) * np.array([0, 1])
 
     return MassSpringDamperSystem(
-        external_forces=F, init_sampler=initial_condition_radial(1, 4.5))
+        external_forces=F, init_sampler=initial_condition_radial(1, 4.5)
+    )
 
 
 def initial_condition_radial(r_min, r_max):
     """
     Creates an initial condition sampler that draws samples uniformly
     from the disk r_min <= x^Tx < r_max.
 
     Returns
     -------
     callable
         Function taking a numpy random generator and returning an
         initial state of size 2.
 
     """
+
     def sampler(rng):
         r = (r_max - r_min) * np.sqrt(rng.uniform(size=1)) + r_min
-        theta = 2.*np.pi * rng.uniform(size=1)
+        theta = 2.0 * np.pi * rng.uniform(size=1)
         q = r * np.cos(theta)
         p = r * np.sin(theta)
         return np.array([q, p]).flatten()
 
     return sampler
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/pseudo_Hamiltonian_system.py` & `phlearn-1.1.2/phlearn/phsystems/ode/pseudo_hamiltonian_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import numpy as np
 from scipy.integrate import solve_ivp
 import torch
 
-from ..utils.derivatives import time_derivative
-
-__all__ = ["PseudoHamiltonianSystem", "zero_force"]
+from ...utils.derivatives import time_derivative
 
 
 class PseudoHamiltonianSystem:
     """
     Implements a pseudo-Hamiltonian system of the form::
 
         dx/dt = (S(x) - R(x))*grad[H(x)] + F(x, t)
 
-    where x is the system state, S is the skew-synnetric interconnection
+    where x is the system state, S is the skew-symmetric interconnection
     matrix, R is the positive semi-definite dissipation matrix, H is the
     Hamiltonian of the systemm, F is the external force(s).
 
     Parameters
     ----------
         nstates : int
             Number of system states N.
 
-        structure_matrix : (N, N) ndarray or callable, default None
+        skewsymmetric_matrix : (N, N) ndarray or callable, default None
             Corresponds to the S matrix. Must either be an
             ndarray, or callable taking an ndarray
             input of shape (nsamples, nstates) and returning an ndarray
             of shape (nsamples, nstates, nstates). If None,
             the system is assumed to be canonical, and the
             S matrix is set to be [[0, I_N], [-I_N, 0]].
 
@@ -77,56 +75,55 @@
             condition is provided.
 
     """
 
     def __init__(
         self,
         nstates,
-        structure_matrix=None,
+        skewsymmetric_matrix=None,
         dissipation_matrix=None,
         hamiltonian=None,
         grad_hamiltonian=None,
         external_forces=None,
         controller=None,
-        init_sampler=None,
-    ):
+        init_sampler=None,    ):
         self.nstates = nstates
 
         if (
-            structure_matrix is not None
-            and not callable(structure_matrix)
-            and not np.allclose(structure_matrix, -structure_matrix.T, atol=1e-15)
+            skewsymmetric_matrix is not None
+            and not callable(skewsymmetric_matrix)
+            and not np.allclose(skewsymmetric_matrix, -skewsymmetric_matrix.T, atol=1e-15)
         ):
-            raise Exception("structure_matrix must be skew-symmetric")
+            raise Exception("skewsymmetric_matrix must be skew-symmetric")
 
         if hamiltonian is None and grad_hamiltonian is None:
             raise Exception(
                 "Either one of hamiltonian or grad_hamiltonian must be provided"
             )
 
-        if structure_matrix is None:
+        if skewsymmetric_matrix is None:
             if nstates % 2 == 1:
                 raise Exception(
-                    "nstates must be even when structure_matrix not provided"
+                    "nstates must be even when skewsymmetric_matrix not provided"
                 )
 
             npos = nstates // 2
-            structure_matrix = np.block(
+            skewsymmetric_matrix = np.block(
                 [
                     [np.zeros([npos, npos]), np.eye(npos)],
                     [-np.eye(npos), np.zeros([npos, npos])],
                 ]
             )
 
-        if not callable(structure_matrix):
-            self.structure_matrix = structure_matrix
-            self.S = lambda x: structure_matrix
+        if not callable(skewsymmetric_matrix):
+            self.skewsymmetric_matrix = skewsymmetric_matrix
+            self.S = lambda x: skewsymmetric_matrix
         else:
-            self.structure_matrix = None
-            self.S = structure_matrix
+            self.skewsymmetric_matrix = None
+            self.S = skewsymmetric_matrix
 
         if dissipation_matrix is None:
             dissipation_matrix = np.zeros((self.nstates, self.nstates))
 
         if not callable(dissipation_matrix):
             if len(dissipation_matrix.shape) == 1:
                 dissipation_matrix = np.diag(dissipation_matrix)
@@ -186,31 +183,22 @@
         (..., N) ndarray
 
         """
 
         S = self.S(x)
         R = self.R(x)
         dH = self.dH(x.T).T
-        
+
         if (len(S.shape) == 3) or (len(R.shape) == 3):
             dynamics = np.matmul(S - R, np.atleast_3d(dH)).reshape(
                 x.shape
-            ) + self.external_forces(x, t)
+            ) + self.external_forces(x, t).reshape(x.shape)
         else:
-            def F(x, t):
-                """Temporary wrapper function for external force to allow user defined
-                force that takes x of shape (nstates, 1) and t as a float.
-                Putting this here as I don't know how this would affect the
-                above logical block. TODO this is creating a ragged array from
-                list of lists and needs fixed."""
-                return np.array([Fxy for Fxy in map(self.external_forces, x, t)])
-            
-            dynamics = dH @ (S.T - R.T) + F(x, t)
-            # dynamics = dH @ (S.T - R.T) + self.external_forces(x, t)
-            
+            dynamics = dH @ (S.T - R.T) + self.external_forces(x, t).reshape(x.shape)
+
         if u is not None:
             dynamics += u
 
         return dynamics
 
     def sample_trajectory(self, t, x0=None, noise_std=0, reference=None):
         """
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/tank_system.py` & `phlearn-1.1.2/phlearn/phsystems/ode/tank_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 
 import numbers
 
 import networkx as nx
 import numpy as np
 
-from .pseudo_Hamiltonian_system import PseudoHamiltonianSystem
-
-__all__ = ['TankSystem', 'init_tanksystem',
-           'init_tanksystem_leaky']
+from .pseudo_hamiltonian_system import PseudoHamiltonianSystem
 
 
 class TankSystem(PseudoHamiltonianSystem):
     """
     Implements a pseudo-Hamiltonian version of a coupled tanks system::
 
           .      | -R_p   B^T |
@@ -91,15 +88,15 @@
             B = np.array(nx.linalg.graphmatrix.incidence_matrix(
                 system_graph, oriented=True).todense())
         else:
             self.npipes = npipes
             self.ntanks = ntanks
             B = incidence_matrix
 
-        structure_matrix = np.block(
+        skewsymmetric_matrix = np.block(
             [[np.zeros((self.npipes, self.npipes)), B.T],
              [-B, np.zeros((self.ntanks, self.ntanks))]])
 
         nstates = self.npipes + self.ntanks
 
         if dissipation_pipes is None:
             dissipation_pipes = np.zeros((nstates, nstates))
@@ -116,31 +113,30 @@
         if isinstance(A, numbers.Number):
             A = A*np.ones(self.ntanks)
 
         self.Hvec = np.concatenate((1/J, rho*g / A))
         super().__init__(nstates,
                          hamiltonian=self.H_tanksystem,
                          grad_hamiltonian=self.dH_tanksystem,
-                         structure_matrix=structure_matrix,
+                         skewsymmetric_matrix=skewsymmetric_matrix,
                          dissipation_matrix=dissipation,
                          **kwargs)
 
     def H_tanksystem(self, x, t=None):
         return x**2 @ self.Hvec / 2
 
     def dH_tanksystem(self, x, t=None):
-        return x * self.Hvec
+        return (x.T * self.Hvec).T
 
     def pipeflows(self, x):
         return x[..., :self.npipes]
 
     def tanklevels(self, x):
         return x[..., self.npipes:]
 
-
 def init_tanksystem(u=None):
     """
     Initialize standard tank system.
 
     Parameters
     ----------
     u : phlearn.control.PseudoHamiltonianController, defult None
```

### Comparing `phlearn-1.1.0/phlearn/phsystems/tests/test_phsystems.py` & `phlearn-1.1.2/phlearn/phsystems/ode/tests/test_phsystems.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # TODO: Have ignored controller for now. I.e., assumed controller = None throughout
 
 # When developing tests, from the top level dir (i.e., phlearn) run
 # python3 -m phlearn.phnns.tests.test_phsystems
 # to run this as a module, allowing use of relative imports
 
 import numpy as np
-from ..pseudo_Hamiltonian_system import PseudoHamiltonianSystem
+from ..pseudo_hamiltonian_system import PseudoHamiltonianSystem
 import torch
 
 
 N_STATES = 10
 N_TIMESTEPS = 100
 
 X_RAND = np.random.rand(N_STATES)
@@ -60,35 +60,35 @@
         DISSIPATION_MATRIX, phs.R(X_RAND)
     ), "dissipation_matrix not returned"
 
 
 def test_structure_matrix_is_returned():
     psh_kwargs_loc = psh_kwargs
     n = psh_kwargs["nstates"]
-    phs = PseudoHamiltonianSystem(structure_matrix=STRUCTURE_MATRIX, **psh_kwargs_loc)
+    phs = PseudoHamiltonianSystem(skewsymmetric_matrix=STRUCTURE_MATRIX, **psh_kwargs_loc)
     assert np.array_equal(
         STRUCTURE_MATRIX, phs.S(X_RAND)
-    ), "structure_matrix not returned"
+    ), "skewsymmetric_matrix not returned"
 
 
 def test_dH_calculated_correctly():
     phs = PseudoHamiltonianSystem(**psh_kwargs)
     assert np.allclose(phs.dH(X_RAND), 2 * X_RAND), "grad_H computed incorrectly"
 
 
 def test_x_dot():
     phs = PseudoHamiltonianSystem(
         dissipation_matrix=lambda x: DISSIPATION_MATRIX,
-        structure_matrix=lambda x: STRUCTURE_MATRIX,
+        skewsymmetric_matrix=lambda x: STRUCTURE_MATRIX,
         external_forces=lambda x, t: EXTERNAL_FORCE,
         **psh_kwargs
     )
     x_dot = dH(X_RAND) @ (STRUCTURE_MATRIX.T - DISSIPATION_MATRIX.T) + EXTERNAL_FORCE
     assert np.allclose(phs.x_dot(X_RAND, T_AXIS), x_dot), "x_dot() returns incorrect ODE"
 
 
 def test_sample_trajectory_on_const_ode():
-    phs = PseudoHamiltonianSystem(structure_matrix=0 * STRUCTURE_MATRIX, **psh_kwargs)
+    phs = PseudoHamiltonianSystem(skewsymmetric_matrix=0 * STRUCTURE_MATRIX, **psh_kwargs)
     x, _, _, _ = phs.sample_trajectory(t=[0, 1], x0=X_RAND, noise_std=0)
     assert np.allclose(
         x[-1], X_RAND
     ), "Solution of a constant ODE does not remain constant"
```

### Comparing `phlearn-1.1.0/phlearn/utils/derivatives.py` & `phlearn-1.1.2/phlearn/utils/derivatives.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 import numpy as np
 
-__all__ = ['time_derivative']
-
 
 def time_derivative(integrator, x_dot, x_start, x_end,
                     t_start, t_end, dt, u=None, xspatial=None):
     """
     Computes the time derivative of x using the provided function *x_dot*.
 
     Parameters
```

### Comparing `phlearn-1.1.0/phlearn/utils/utils.py` & `phlearn-1.1.2/phlearn/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import torch
 import numpy as np
 import numpy.linalg as la
 import matplotlib.pyplot as plt
 import imageio
 from IPython.display import display, Video, Image
 
-__all__ = ['to_tensor', 'midpoint_method', 'create_video']
-
 
 def to_tensor(x, ttype=torch.float32):
     """
     Converts the input to a torch tensor if the input is not None.
 
     Parameters
     ----------
```

### Comparing `phlearn-1.1.0/phlearn.egg-info/PKG-INFO` & `phlearn-1.1.2/phlearn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: phlearn
-Version: 1.1.0
-Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf
-Home-page: https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks
+Version: 1.1.2
+Summary: A package for simulating and learning pseudo-Hamiltonian systems. For further details, see https://arxiv.org/pdf/2206.02660.pdf and https://arxiv.org/abs/2304.14374
+Home-page: https://github.com/SINTEF/pseudo-hamiltonian-neural-networks
 Author: Sølve Eidnes
 Author-email: solve.eidnes@sintef.no
 License: MIT
 Keywords: pseudo-Hamiltonian neural networks
 Classifier: Development Status :: 5 - Production/Stable
 Provides-Extra: control
 License-File: LICENSE.txt
 
 # phlearn
-Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al. 2022)](https://arxiv.org/pdf/2206.02660.pdf).
+Package for modelling pseudo-Hamiltonian systems with neural networks as described in [(Eidnes et al., 2022)](https://arxiv.org/pdf/2206.02660.pdf) for ODEs and [(Eidnes and Lye, 2023)](https://arxiv.org/pdf/2304.14374.pdf) for PDEs.
 
 [Documentation available here](https://pseudo-Hamiltonian-neural-networks.readthedocs.io/en/latest/)
 
 - phlearn
     + phsystems
     + phnns
     + utils
```

### Comparing `phlearn-1.1.0/phlearn.egg-info/SOURCES.txt` & `phlearn-1.1.2/phlearn.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,35 @@
 phlearn/control/casadiNN.py
 phlearn/control/casadiPH.py
 phlearn/control/mpc.py
 phlearn/control/phcontroller.py
 phlearn/control/pid.py
 phlearn/control/reference.py
 phlearn/phnns/__init__.py
-phlearn/phnns/conservative_dissipative_neural_network.py
 phlearn/phnns/dynamic_system_neural_network.py
-phlearn/phnns/models.py
+phlearn/phnns/ode_models.py
+phlearn/phnns/pde_models.py
 phlearn/phnns/pseudo_hamiltonian_neural_network.py
+phlearn/phnns/pseudo_hamiltonian_pde_neural_network.py
 phlearn/phnns/train_utils.py
 phlearn/phnns/tests/__init__.py
 phlearn/phnns/tests/test_phnns.py
 phlearn/phsystems/__init__.py
-phlearn/phsystems/allen_cahn_system.py
-phlearn/phsystems/bbm_system.py
-phlearn/phsystems/burgers_system.py
-phlearn/phsystems/cahn_hilliard_system.py
-phlearn/phsystems/conservative_dissipative_system.py
-phlearn/phsystems/fvm.py
-phlearn/phsystems/heat_system.py
-phlearn/phsystems/kdv_system.py
-phlearn/phsystems/msd_system.py
-phlearn/phsystems/perona_malik_system.py
-phlearn/phsystems/phase_system.py
-phlearn/phsystems/pseudo_Hamiltonian_system.py
-phlearn/phsystems/tank_system.py
+phlearn/phsystems/ode/__init__.py
+phlearn/phsystems/ode/msd_system.py
+phlearn/phsystems/ode/pseudo_hamiltonian_system.py
+phlearn/phsystems/ode/tank_system.py
+phlearn/phsystems/ode/tests/__init__.py
+phlearn/phsystems/ode/tests/test_phsystems.py
+phlearn/phsystems/pde/__init__.py
+phlearn/phsystems/pde/allen_cahn_system.py
+phlearn/phsystems/pde/bbm_system.py
+phlearn/phsystems/pde/cahn_hilliard_system.py
+phlearn/phsystems/pde/heat_system.py
+phlearn/phsystems/pde/kdv_system.py
+phlearn/phsystems/pde/perona_malik_system.py
+phlearn/phsystems/pde/pseudo_hamiltonian_pde_system.py
 phlearn/phsystems/tests/__init__.py
 phlearn/phsystems/tests/test_phsystems.py
 phlearn/utils/__init__.py
 phlearn/utils/derivatives.py
 phlearn/utils/utils.py
```

### Comparing `phlearn-1.1.0/setup.py` & `phlearn-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setuptools.setup(
     name='phlearn',
-    version='1.1.0',
+    version='1.1.2',
     author='Sølve Eidnes',
     author_email='solve.eidnes@sintef.no',
     description=('A package for simulating and learning pseudo-Hamiltonian systems.'
-                 ' For further details, see https://arxiv.org/pdf/2206.02660.pdf'),
+                 ' For further details, see https://arxiv.org/pdf/2206.02660.pdf and https://arxiv.org/abs/2304.14374'),
     keywords='pseudo-Hamiltonian neural networks',
-    url="https://gitlab.sintef.no/hybrid-machine-learning/pseudo-Hamiltonian-neural-networks",
+    url="https://github.com/SINTEF/pseudo-hamiltonian-neural-networks",
     packages=setuptools.find_packages(),
     long_description=read('README.md'),
     classifiers=[
         'Development Status :: 5 - Production/Stable'
     ],
     license='MIT',
     install_requires=[
-        'networkx==2.7.1',
-        'numpy==1.22.3',
-        'torchvision==0.11.3',
-        'scipy==1.8.0',
+        'networkx>=2.7.1',
+        'numpy>=1.22.3',
+        'torchvision',
+        'scipy>=1.8.0',
         'torch',
         'torchaudio',
         'matplotlib',
         'imageio',
         'tqdm',
         'autograd',
         'IPython',
```

