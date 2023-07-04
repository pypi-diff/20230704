# Comparing `tmp/cycless-0.2.tar.gz` & `tmp/cycless-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycless-0.2.tar", last modified: Mon Mar  6 12:24:09 2023, max compression
+gzip compressed data, was "cycless-0.3.1.tar", last modified: Tue Jul  4 12:47:41 2023, max compression
```

## Comparing `cycless-0.2.tar` & `cycless-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-03-06 12:24:09.279707 cycless-0.2/
--rw-r--r--   0 matto      (505) staff       (20)     1863 2023-03-06 12:24:09.279796 cycless-0.2/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)     1370 2022-05-05 05:13:24.000000 cycless-0.2/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-03-06 12:24:09.278455 cycless-0.2/cycless/
--rw-r--r--   0 matto      (505) staff       (20)       82 2023-03-06 12:23:37.000000 cycless-0.2/cycless/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     4811 2021-06-15 09:08:24.000000 cycless-0.2/cycless/cycles.py
--rw-r--r--   0 matto      (505) staff       (20)     2835 2021-06-15 09:02:06.000000 cycless-0.2/cycless/dicycles.py
--rw-r--r--   0 matto      (505) staff       (20)    13211 2023-03-06 12:23:32.000000 cycless-0.2/cycless/polyhed.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-03-06 12:24:09.279584 cycless-0.2/cycless.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)     1863 2023-03-06 12:24:09.000000 cycless-0.2/cycless.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      259 2023-03-06 12:24:09.000000 cycless-0.2/cycless.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2023-03-06 12:24:09.000000 cycless-0.2/cycless.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       56 2023-03-06 12:24:09.000000 cycless-0.2/cycless.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)        8 2023-03-06 12:24:09.000000 cycless-0.2/cycless.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2023-03-06 12:24:09.281801 cycless-0.2/setup.cfg
--rwxr-xr-x   0 matto      (505) staff       (20)     1436 2021-06-15 09:02:05.000000 cycless-0.2/setup.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-07-04 12:47:41.189682 cycless-0.3.1/
+-rw-r--r--   0 matto      (505) staff       (20)     2634 2023-07-04 12:47:41.189763 cycless-0.3.1/PKG-INFO
+-rw-r--r--   0 matto      (505) staff       (20)     2139 2023-07-04 12:46:27.000000 cycless-0.3.1/README.md
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-07-04 12:47:41.188719 cycless-0.3.1/cycless/
+-rw-r--r--   0 matto      (505) staff       (20)       84 2023-07-04 12:45:54.000000 cycless-0.3.1/cycless/__init__.py
+-rw-r--r--   0 matto      (505) staff       (20)     4811 2021-06-15 09:08:24.000000 cycless-0.3.1/cycless/cycles.py
+-rw-r--r--   0 matto      (505) staff       (20)     2835 2021-06-15 09:02:06.000000 cycless-0.3.1/cycless/dicycles.py
+-rw-r--r--   0 matto      (505) staff       (20)    13216 2023-07-04 12:45:14.000000 cycless-0.3.1/cycless/polyhed.py
+-rw-r--r--   0 matto      (505) staff       (20)     3024 2023-03-28 03:47:34.000000 cycless-0.3.1/cycless/simplex.py
+drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-07-04 12:47:41.189547 cycless-0.3.1/cycless.egg-info/
+-rw-r--r--   0 matto      (505) staff       (20)     2634 2023-07-04 12:47:41.000000 cycless-0.3.1/cycless.egg-info/PKG-INFO
+-rw-r--r--   0 matto      (505) staff       (20)      278 2023-07-04 12:47:41.000000 cycless-0.3.1/cycless.egg-info/SOURCES.txt
+-rw-r--r--   0 matto      (505) staff       (20)        1 2023-07-04 12:47:41.000000 cycless-0.3.1/cycless.egg-info/dependency_links.txt
+-rw-r--r--   0 matto      (505) staff       (20)       56 2023-07-04 12:47:41.000000 cycless-0.3.1/cycless.egg-info/requires.txt
+-rw-r--r--   0 matto      (505) staff       (20)        8 2023-07-04 12:47:41.000000 cycless-0.3.1/cycless.egg-info/top_level.txt
+-rw-r--r--   0 matto      (505) staff       (20)      108 2023-07-04 12:47:41.190459 cycless-0.3.1/setup.cfg
+-rwxr-xr-x   0 matto      (505) staff       (20)     1436 2021-06-15 09:02:05.000000 cycless-0.3.1/setup.py
```

### Comparing `cycless-0.2/PKG-INFO` & `cycless-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycless
-Version: 0.2
+Version: 0.3.1
 Summary: A collection of algorithms for cycles in a graph.
 Home-page: https://github.com/vitroid/cycles/
 Author: Masakazu Matsumoto
 Author-email: vitroid@gmail.com
 License: MIT
 Keywords: cycles,graph
 Classifier: Development Status :: 4 - Beta
@@ -20,24 +20,64 @@
 
 Some codes come from [https://github.com/vitroid/Polyhed](vitroid/Polyhed) and [https://github.com/vitroid/countrings](vitroid/countrings) are integrated and improved.
 
 ## cycles.py
 
 A simple algorithm to enumerate all irreducible cycles of n-members and smaller in an undirected graph. [Matsumoto 2007]
 
+```python
+import cycless.cycles as cy
+import networkx as nx
+
+g = nx.cubical_graph()
+
+for cycle in cy.cycles_iter(g, maxsize=6):
+    print(cycle)
+```
+
 ## dicycles.py
 
-An algorithm to enumerate the irreducible cycles of a size in a dircted graph. [Matsumoto 2021]
+An algorithm to enumerate the directed cycles of a size in a dircted graph. [Matsumoto 2021]
+
+```python
+from genice2.genice import GenIce
+from genice2.plugin import Lattice, Format, Molecule
+import cycless.dicycles as dc
+
+# Generate an ice I structure as a directed graph
+lattice    = Lattice("1h") 
+formatter  = Format("raw", stage=(3,))
+raw = GenIce(lattice, signature="ice 1h", rep=[2,2,2]).generate_ice(formatter)
+
+for cycle in dc.dicycles_iter(raw['digraph'], size=6):
+    print(cycle)
+```
 
 ## polyhed.py
 
 An algorithm to enumerate the quasi-polyhedral hull made of cycles in an undirected graph. A quasi-polyhedral hull (vitrite) obeys the following conditions: [Matsumoto 2007]
 
 1. The surface of the hull is made of irreducible cycles.
 2. Two or three cycles shares a vertex of the hull.
 3. Two cycles shares an edge of the hull.
 4. Its Euler index (F-E+V) is two.
 
+```python
+import cycless.cycles as cy
+import cycless.polyhed as ph
+import networkx as nx
+
+g = nx.dodecahedral_graph()
+
+cycles = [cycle for cycle in cy.cycles_iter(g, maxsize=6)]
+for polyhed in ph.polyhedra_iter(cycles):
+    print(polyhed)
+```
+
+## simplex.py
+
+Enumerate triangle, tetrahedral, and octahedral subgraphs found in the given graph.
+
 ## References
 
 1. M. Matsumoto, A. Baba, and I. Ohmine, Topological building blocks of hydrogen bond network in water, J. Chem. Phys. 127, 134504 (2007). http://doi.org/10.1063/1.2772627
-2. Masakazu Matsumoto, Takuma Yagasaki, Hideki Tanaka et al. Hyperhomogeneity of hydrogen-disordered ice and its origin: the residual entropy compatible with the disparity in hydrogen bond energy, 22 January 2021, PREPRINT (Version 1) available at Research Square [https://doi.org/10.21203/rs.3.rs-143208/v1]
+2. Matsumoto, M., Yagasaki, T. & Tanaka, H. On the anomalous homogeneity of hydrogen-disordered ice and its origin. J. Chem. Phys. 155, 164502 (2021). https://doi.org/10.1063/5.0065215
```

### Comparing `cycless-0.2/README.md` & `cycless-0.3.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,64 @@
 
 Some codes come from [https://github.com/vitroid/Polyhed](vitroid/Polyhed) and [https://github.com/vitroid/countrings](vitroid/countrings) are integrated and improved.
 
 ## cycles.py
 
 A simple algorithm to enumerate all irreducible cycles of n-members and smaller in an undirected graph. [Matsumoto 2007]
 
+```python
+import cycless.cycles as cy
+import networkx as nx
+
+g = nx.cubical_graph()
+
+for cycle in cy.cycles_iter(g, maxsize=6):
+    print(cycle)
+```
+
 ## dicycles.py
 
-An algorithm to enumerate the irreducible cycles of a size in a dircted graph. [Matsumoto 2021]
+An algorithm to enumerate the directed cycles of a size in a dircted graph. [Matsumoto 2021]
+
+```python
+from genice2.genice import GenIce
+from genice2.plugin import Lattice, Format, Molecule
+import cycless.dicycles as dc
+
+# Generate an ice I structure as a directed graph
+lattice    = Lattice("1h") 
+formatter  = Format("raw", stage=(3,))
+raw = GenIce(lattice, signature="ice 1h", rep=[2,2,2]).generate_ice(formatter)
+
+for cycle in dc.dicycles_iter(raw['digraph'], size=6):
+    print(cycle)
+```
 
 ## polyhed.py
 
 An algorithm to enumerate the quasi-polyhedral hull made of cycles in an undirected graph. A quasi-polyhedral hull (vitrite) obeys the following conditions: [Matsumoto 2007]
 
 1. The surface of the hull is made of irreducible cycles.
 2. Two or three cycles shares a vertex of the hull.
 3. Two cycles shares an edge of the hull.
 4. Its Euler index (F-E+V) is two.
 
+```python
+import cycless.cycles as cy
+import cycless.polyhed as ph
+import networkx as nx
+
+g = nx.dodecahedral_graph()
+
+cycles = [cycle for cycle in cy.cycles_iter(g, maxsize=6)]
+for polyhed in ph.polyhedra_iter(cycles):
+    print(polyhed)
+```
+
+## simplex.py
+
+Enumerate triangle, tetrahedral, and octahedral subgraphs found in the given graph.
+
 ## References
 
 1. M. Matsumoto, A. Baba, and I. Ohmine, Topological building blocks of hydrogen bond network in water, J. Chem. Phys. 127, 134504 (2007). http://doi.org/10.1063/1.2772627
-2. Masakazu Matsumoto, Takuma Yagasaki, Hideki Tanaka et al. Hyperhomogeneity of hydrogen-disordered ice and its origin: the residual entropy compatible with the disparity in hydrogen bond energy, 22 January 2021, PREPRINT (Version 1) available at Research Square [https://doi.org/10.21203/rs.3.rs-143208/v1]
+2. Matsumoto, M., Yagasaki, T. & Tanaka, H. On the anomalous homogeneity of hydrogen-disordered ice and its origin. J. Chem. Phys. 155, 164502 (2021). https://doi.org/10.1063/5.0065215
```

### Comparing `cycless-0.2/cycless/cycles.py` & `cycless-0.3.1/cycless/cycles.py`

 * *Files identical despite different names*

### Comparing `cycless-0.2/cycless/dicycles.py` & `cycless-0.3.1/cycless/dicycles.py`

 * *Files identical despite different names*

### Comparing `cycless-0.2/cycless/polyhed.py` & `cycless-0.3.1/cycless/polyhed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 #
 # Simplified from github/Vitrite
 
 import sys
-import networkx as nx
-from logging import getLogger
 from collections import defaultdict
+from logging import getLogger
+
+import networkx as nx
 import numpy as np
 
 from cycless.cycles import cycles_iter
 
 
 def cage_to_graph(cage, ringlist):
     "Convert a cage as a set of cycles to a graph. "
     g = nx.Graph()
     for ring in cage:
         nodes = ringlist[ring]
-        g.add_cycle(nodes)
+        nx.add_cycle(g, nodes)
         # for i in range(len(nodes)):
         #     g.add_edge(nodes[i-1], nodes[i])
     return g
 
 
 def _reorder(cycle, first, second):
     "Reorder the cycle noders so as to start from the first node."
```

### Comparing `cycless-0.2/cycless.egg-info/PKG-INFO` & `cycless-0.3.1/cycless.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycless
-Version: 0.2
+Version: 0.3.1
 Summary: A collection of algorithms for cycles in a graph.
 Home-page: https://github.com/vitroid/cycles/
 Author: Masakazu Matsumoto
 Author-email: vitroid@gmail.com
 License: MIT
 Keywords: cycles,graph
 Classifier: Development Status :: 4 - Beta
@@ -20,24 +20,64 @@
 
 Some codes come from [https://github.com/vitroid/Polyhed](vitroid/Polyhed) and [https://github.com/vitroid/countrings](vitroid/countrings) are integrated and improved.
 
 ## cycles.py
 
 A simple algorithm to enumerate all irreducible cycles of n-members and smaller in an undirected graph. [Matsumoto 2007]
 
+```python
+import cycless.cycles as cy
+import networkx as nx
+
+g = nx.cubical_graph()
+
+for cycle in cy.cycles_iter(g, maxsize=6):
+    print(cycle)
+```
+
 ## dicycles.py
 
-An algorithm to enumerate the irreducible cycles of a size in a dircted graph. [Matsumoto 2021]
+An algorithm to enumerate the directed cycles of a size in a dircted graph. [Matsumoto 2021]
+
+```python
+from genice2.genice import GenIce
+from genice2.plugin import Lattice, Format, Molecule
+import cycless.dicycles as dc
+
+# Generate an ice I structure as a directed graph
+lattice    = Lattice("1h") 
+formatter  = Format("raw", stage=(3,))
+raw = GenIce(lattice, signature="ice 1h", rep=[2,2,2]).generate_ice(formatter)
+
+for cycle in dc.dicycles_iter(raw['digraph'], size=6):
+    print(cycle)
+```
 
 ## polyhed.py
 
 An algorithm to enumerate the quasi-polyhedral hull made of cycles in an undirected graph. A quasi-polyhedral hull (vitrite) obeys the following conditions: [Matsumoto 2007]
 
 1. The surface of the hull is made of irreducible cycles.
 2. Two or three cycles shares a vertex of the hull.
 3. Two cycles shares an edge of the hull.
 4. Its Euler index (F-E+V) is two.
 
+```python
+import cycless.cycles as cy
+import cycless.polyhed as ph
+import networkx as nx
+
+g = nx.dodecahedral_graph()
+
+cycles = [cycle for cycle in cy.cycles_iter(g, maxsize=6)]
+for polyhed in ph.polyhedra_iter(cycles):
+    print(polyhed)
+```
+
+## simplex.py
+
+Enumerate triangle, tetrahedral, and octahedral subgraphs found in the given graph.
+
 ## References
 
 1. M. Matsumoto, A. Baba, and I. Ohmine, Topological building blocks of hydrogen bond network in water, J. Chem. Phys. 127, 134504 (2007). http://doi.org/10.1063/1.2772627
-2. Masakazu Matsumoto, Takuma Yagasaki, Hideki Tanaka et al. Hyperhomogeneity of hydrogen-disordered ice and its origin: the residual entropy compatible with the disparity in hydrogen bond energy, 22 January 2021, PREPRINT (Version 1) available at Research Square [https://doi.org/10.21203/rs.3.rs-143208/v1]
+2. Matsumoto, M., Yagasaki, T. & Tanaka, H. On the anomalous homogeneity of hydrogen-disordered ice and its origin. J. Chem. Phys. 155, 164502 (2021). https://doi.org/10.1063/5.0065215
```

### Comparing `cycless-0.2/setup.py` & `cycless-0.3.1/setup.py`

 * *Files identical despite different names*

