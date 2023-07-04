# Comparing `tmp/multipoles-0.3.0.tar.gz` & `tmp/multipoles-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multipoles-0.3.0.tar", last modified: Thu Sep 15 15:31:25 2022, max compression
+gzip compressed data, was "dist/multipoles-0.3.1.tar", last modified: Fri Nov 25 09:31:16 2022, max compression
```

## Comparing `multipoles-0.3.0.tar` & `multipoles-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-09-15 15:31:25.514648 multipoles-0.3.0/
--rw-r--r--   0 mbaer    (671849960) 579947404     1091 2022-09-15 15:31:25.514768 multipoles-0.3.0/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     4446 2022-09-15 15:29:04.000000 multipoles-0.3.0/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-09-15 15:31:25.512782 multipoles-0.3.0/multipoles/
--rw-r--r--   0 mbaer    (671849960) 579947404       66 2022-09-15 15:29:32.000000 multipoles-0.3.0/multipoles/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404    10977 2022-09-15 15:29:04.000000 multipoles-0.3.0/multipoles/expansion.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-09-15 15:31:25.514368 multipoles-0.3.0/multipoles.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404     1091 2022-09-15 15:31:25.000000 multipoles-0.3.0/multipoles.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      244 2022-09-15 15:31:25.000000 multipoles-0.3.0/multipoles.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-09-15 15:31:25.000000 multipoles-0.3.0/multipoles.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       12 2022-09-15 15:31:25.000000 multipoles-0.3.0/multipoles.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       11 2022-09-15 15:31:25.000000 multipoles-0.3.0/multipoles.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       79 2022-09-15 15:31:25.515340 multipoles-0.3.0/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404     1262 2022-09-15 15:30:19.000000 multipoles-0.3.0/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-11-25 09:31:16.383604 multipoles-0.3.1/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1091 2022-11-25 09:31:16.383968 multipoles-0.3.1/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     4446 2022-11-15 16:55:52.000000 multipoles-0.3.1/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-11-25 09:31:16.380221 multipoles-0.3.1/multipoles/
+-rw-r--r--   0 mbaer    (671849960) 579947404       66 2022-11-15 16:55:52.000000 multipoles-0.3.1/multipoles/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    11001 2022-11-15 16:56:41.000000 multipoles-0.3.1/multipoles/expansion.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-11-25 09:31:16.382647 multipoles-0.3.1/multipoles.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1091 2022-11-25 09:31:16.000000 multipoles-0.3.1/multipoles.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      244 2022-11-25 09:31:16.000000 multipoles-0.3.1/multipoles.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-11-25 09:31:16.000000 multipoles-0.3.1/multipoles.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       12 2022-11-25 09:31:16.000000 multipoles-0.3.1/multipoles.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       11 2022-11-25 09:31:16.000000 multipoles-0.3.1/multipoles.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       79 2022-11-25 09:31:16.384852 multipoles-0.3.1/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404     1262 2022-11-25 09:30:48.000000 multipoles-0.3.1/setup.py
```

### Comparing `multipoles-0.3.0/PKG-INFO` & `multipoles-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
```

### Comparing `multipoles-0.3.0/README.md` & `multipoles-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multipoles-0.3.0/multipoles/expansion.py` & `multipoles-0.3.1/multipoles/expansion.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     def _calc_multipole_coef(self, l, m):
 
         prefac = np.sqrt(4*np.pi/(2*l+1))
 
         if self.charge_dist['discrete']:
             q_lm = 0
             for chg in self.charges:
-                xyz = chg['xyz']
+                xyz = chg['xyz'] - self.center_of_charge
                 q = chg['q']
                 r, phi, theta = cartesian_to_spherical(*xyz)
                 Y_lm = sph_harm(m, l, phi, theta)
                 if self.exterior:
                   q_lm += q * r**l * np.conj(Y_lm)
                 else:
                   q_lm += q / r**(l+1) * np.conj(Y_lm)
```

### Comparing `multipoles-0.3.0/multipoles.egg-info/PKG-INFO` & `multipoles-0.3.1/multipoles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipoles
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for multipole expansions of electrostatic or gravitational potentials
 Home-page: https://github.com/maroba/multipoles
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: multipole expansion,physics,scientific-computing
 Platform: UNKNOWN
```

### Comparing `multipoles-0.3.0/setup.py` & `multipoles-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='multipoles',
-    version='0.3.0',
+    version='0.3.1',
     description='A Python package for multipole expansions of electrostatic or gravitational potentials',
     long_description="""*multipoles* is a Python package for multipole expansions of the solutions of the Poisson equation     
        (e.g. electrostatic or gravitational potentials). It can handle discrete and continuous charge or mass distributions.
     """,
 
     license='MIT',
     url='https://github.com/maroba/multipoles',
```

