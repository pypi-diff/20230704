# Comparing `tmp/celmech-1.0.4.tar.gz` & `tmp/celmech-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celmech-1.0.4.tar", last modified: Fri May 19 20:38:13 2023, max compression
+gzip compressed data, was "celmech-1.1.0.tar", last modified: Tue Jul  4 14:05:55 2023, max compression
```

## Comparing `celmech-1.0.4.tar` & `celmech-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.641662 celmech-1.0.4/
--rw-r--r--   0 dtamayo    (502) staff       (20)    35149 2022-08-19 22:47:33.000000 celmech-1.0.4/LICENSE
--rw-r--r--   0 dtamayo    (502) staff       (20)       87 2022-08-19 22:57:58.000000 celmech-1.0.4/MANIFEST.in
--rw-r--r--   0 dtamayo    (502) staff       (20)      815 2023-05-19 20:38:13.641407 celmech-1.0.4/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)      665 2022-08-19 22:47:33.000000 celmech-1.0.4/README.md
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.635088 celmech-1.0.4/celmech/
--rw-r--r--   0 dtamayo    (502) staff       (20)     1676 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/__init__.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    35161 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/canonical_transformations.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    48262 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/disturbing_function.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    20332 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/hamiltonian.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    18949 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/lie_transformations.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    32466 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/maps.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    24890 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/miscellaneous.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     1525 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/multiplanet_hamiltonian.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    15198 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/nbody_simulation_utilities.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    57551 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/numerical_resonance_models.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     3491 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/numerical_resonance_utils.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    17818 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/planar_poincare.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    42697 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/poincare.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     8846 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/poisson_series.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     5049 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/resonances.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     9401 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/rk_integrator.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    49319 2023-05-19 20:36:43.000000 celmech-1.0.4/celmech/secular.py
--rw-r--r--   0 dtamayo    (502) staff       (20)    26888 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/symplectic_evolution_operators.py
--rw-r--r--   0 dtamayo    (502) staff       (20)     3112 2022-08-19 22:47:33.000000 celmech-1.0.4/celmech/transformations.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.637843 celmech-1.0.4/celmech.egg-info/
--rw-r--r--   0 dtamayo    (502) staff       (20)      815 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/PKG-INFO
--rw-r--r--   0 dtamayo    (502) staff       (20)      858 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/SOURCES.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/dependency_links.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)        1 2022-08-19 22:55:59.000000 celmech-1.0.4/celmech.egg-info/not-zip-safe
--rw-r--r--   0 dtamayo    (502) staff       (20)       85 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/requires.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       19 2023-05-19 20:38:13.000000 celmech-1.0.4/celmech.egg-info/top_level.txt
--rw-r--r--   0 dtamayo    (502) staff       (20)       38 2023-05-19 20:38:13.641705 celmech-1.0.4/setup.cfg
--rw-r--r--   0 dtamayo    (502) staff       (20)     3240 2023-05-19 20:37:22.000000 celmech-1.0.4/setup.py
-drwxr-xr-x   0 dtamayo    (502) staff       (20)        0 2023-05-19 20:38:13.640989 celmech-1.0.4/src/
--rw-r--r--   0 dtamayo    (502) staff       (20)     4286 2023-05-19 20:37:22.000000 celmech-1.0.4/src/disturbing_function.c
--rw-r--r--   0 dtamayo    (502) staff       (20)    18820 2022-08-19 22:47:33.000000 celmech-1.0.4/src/fmft.c
--rw-r--r--   0 dtamayo    (502) staff       (20)      971 2022-08-19 22:47:33.000000 celmech-1.0.4/src/fmftPy.c
--rw-r--r--   0 dtamayo    (502) staff       (20)     2494 2022-08-19 22:47:33.000000 celmech-1.0.4/src/nrutil.c
--rw-r--r--   0 dtamayo    (502) staff       (20)      494 2022-08-19 22:47:33.000000 celmech-1.0.4/src/nrutil.h
--rw-r--r--   0 dtamayo    (502) staff       (20)     9536 2022-08-19 22:47:33.000000 celmech-1.0.4/src/poisson_series.c
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2023-07-04 14:05:55.774865 celmech-1.1.0/
+-rw-r--r--   0 shadden    (501) staff       (20)    35149 2022-12-05 17:40:33.000000 celmech-1.1.0/LICENSE
+-rw-r--r--   0 shadden    (501) staff       (20)       87 2022-12-05 17:40:33.000000 celmech-1.1.0/MANIFEST.in
+-rw-r--r--   0 shadden    (501) staff       (20)      815 2023-07-04 14:05:55.774412 celmech-1.1.0/PKG-INFO
+-rw-r--r--   0 shadden    (501) staff       (20)      665 2022-12-05 17:40:33.000000 celmech-1.1.0/README.md
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2023-07-04 14:05:55.760094 celmech-1.1.0/celmech/
+-rw-r--r--   0 shadden    (501) staff       (20)     1676 2022-05-19 20:35:01.000000 celmech-1.1.0/celmech/__init__.py
+-rw-r--r--   0 shadden    (501) staff       (20)    35161 2022-08-04 20:26:07.000000 celmech-1.1.0/celmech/canonical_transformations.py
+-rw-r--r--   0 shadden    (501) staff       (20)    48262 2022-08-29 17:39:06.000000 celmech-1.1.0/celmech/disturbing_function.py
+-rw-r--r--   0 shadden    (501) staff       (20)    20332 2023-02-01 14:49:11.000000 celmech-1.1.0/celmech/hamiltonian.py
+-rw-r--r--   0 shadden    (501) staff       (20)    18949 2022-05-19 20:35:01.000000 celmech-1.1.0/celmech/lie_transformations.py
+-rw-r--r--   0 shadden    (501) staff       (20)    32466 2023-05-29 15:35:14.000000 celmech-1.1.0/celmech/maps.py
+-rw-r--r--   0 shadden    (501) staff       (20)    24890 2023-04-14 13:56:22.000000 celmech-1.1.0/celmech/miscellaneous.py
+-rw-r--r--   0 shadden    (501) staff       (20)     1525 2017-08-31 19:32:04.000000 celmech-1.1.0/celmech/multiplanet_hamiltonian.py
+-rw-r--r--   0 shadden    (501) staff       (20)    15168 2023-06-29 21:29:44.000000 celmech-1.1.0/celmech/nbody_simulation_utilities.py
+-rw-r--r--   0 shadden    (501) staff       (20)    57551 2022-05-20 16:19:33.000000 celmech-1.1.0/celmech/numerical_resonance_models.py
+-rw-r--r--   0 shadden    (501) staff       (20)     3491 2022-05-19 20:35:01.000000 celmech-1.1.0/celmech/numerical_resonance_utils.py
+-rw-r--r--   0 shadden    (501) staff       (20)    17818 2020-08-14 20:13:35.000000 celmech-1.1.0/celmech/planar_poincare.py
+-rw-r--r--   0 shadden    (501) staff       (20)    42697 2022-07-27 18:46:02.000000 celmech-1.1.0/celmech/poincare.py
+-rw-r--r--   0 shadden    (501) staff       (20)     8846 2022-05-19 20:35:02.000000 celmech-1.1.0/celmech/poisson_series.py
+-rw-r--r--   0 shadden    (501) staff       (20)     5049 2020-01-28 16:42:51.000000 celmech-1.1.0/celmech/resonances.py
+-rw-r--r--   0 shadden    (501) staff       (20)     9401 2021-01-25 16:27:34.000000 celmech-1.1.0/celmech/rk_integrator.py
+-rw-r--r--   0 shadden    (501) staff       (20)    49321 2023-05-29 15:36:37.000000 celmech-1.1.0/celmech/secular.py
+-rw-r--r--   0 shadden    (501) staff       (20)    26888 2021-01-22 18:31:13.000000 celmech-1.1.0/celmech/symplectic_evolution_operators.py
+-rw-r--r--   0 shadden    (501) staff       (20)     3112 2020-09-08 19:07:09.000000 celmech-1.1.0/celmech/transformations.py
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2023-07-04 14:05:55.765117 celmech-1.1.0/celmech.egg-info/
+-rw-r--r--   0 shadden    (501) staff       (20)      815 2023-07-04 14:05:55.000000 celmech-1.1.0/celmech.egg-info/PKG-INFO
+-rw-r--r--   0 shadden    (501) staff       (20)      923 2023-07-04 14:05:55.000000 celmech-1.1.0/celmech.egg-info/SOURCES.txt
+-rw-r--r--   0 shadden    (501) staff       (20)        1 2023-07-04 14:05:55.000000 celmech-1.1.0/celmech.egg-info/dependency_links.txt
+-rw-r--r--   0 shadden    (501) staff       (20)        1 2017-08-31 19:32:30.000000 celmech-1.1.0/celmech.egg-info/not-zip-safe
+-rw-r--r--   0 shadden    (501) staff       (20)       85 2023-07-04 14:05:55.000000 celmech-1.1.0/celmech.egg-info/requires.txt
+-rw-r--r--   0 shadden    (501) staff       (20)       19 2023-07-04 14:05:55.000000 celmech-1.1.0/celmech.egg-info/top_level.txt
+-rw-r--r--   0 shadden    (501) staff       (20)       38 2023-07-04 14:05:55.775161 celmech-1.1.0/setup.cfg
+-rw-r--r--   0 shadden    (501) staff       (20)     3240 2023-07-04 14:05:28.000000 celmech-1.1.0/setup.py
+drwxr-xr-x   0 shadden    (501) staff       (20)        0 2023-07-04 14:05:55.773596 celmech-1.1.0/src/
+-rw-r--r--   0 shadden    (501) staff       (20)     4286 2023-07-04 14:05:28.000000 celmech-1.1.0/src/disturbing_function.c
+-rw-r--r--   0 shadden    (501) staff       (20)    18820 2020-08-14 20:13:36.000000 celmech-1.1.0/src/fmft.c
+-rw-r--r--   0 shadden    (501) staff       (20)      971 2022-05-19 20:01:57.000000 celmech-1.1.0/src/fmftPy.c
+-rw-r--r--   0 shadden    (501) staff       (20)    15192 2021-02-09 14:23:17.000000 celmech-1.1.0/src/moid_v4_fun.f
+-rw-r--r--   0 shadden    (501) staff       (20)     2494 2020-08-14 20:13:36.000000 celmech-1.1.0/src/nrutil.c
+-rw-r--r--   0 shadden    (501) staff       (20)      494 2020-08-14 20:13:36.000000 celmech-1.1.0/src/nrutil.h
+-rw-r--r--   0 shadden    (501) staff       (20)      483 2021-01-04 15:09:52.000000 celmech-1.1.0/src/poincare.c
+-rw-r--r--   0 shadden    (501) staff       (20)     9536 2021-01-22 18:31:13.000000 celmech-1.1.0/src/poisson_series.c
+-rw-r--r--   0 shadden    (501) staff       (20)    10205 2020-07-10 17:39:51.000000 celmech-1.1.0/src/poisson_series.h
+-rw-r--r--   0 shadden    (501) staff       (20)     1135 2020-07-10 17:45:01.000000 celmech-1.1.0/src/test.c
```

### Comparing `celmech-1.0.4/LICENSE` & `celmech-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/PKG-INFO` & `celmech-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.0.4
+Version: 1.1.0
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
 Platform: UNKNOWN
```

### Comparing `celmech-1.0.4/README.md` & `celmech-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/__init__.py` & `celmech-1.1.0/celmech/__init__.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/canonical_transformations.py` & `celmech-1.1.0/celmech/canonical_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/disturbing_function.py` & `celmech-1.1.0/celmech/disturbing_function.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/hamiltonian.py` & `celmech-1.1.0/celmech/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/lie_transformations.py` & `celmech-1.1.0/celmech/lie_transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/maps.py` & `celmech-1.1.0/celmech/maps.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/miscellaneous.py` & `celmech-1.1.0/celmech/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/multiplanet_hamiltonian.py` & `celmech-1.1.0/celmech/multiplanet_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/nbody_simulation_utilities.py` & `celmech-1.1.0/celmech/nbody_simulation_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         'Omega':np.zeros(shape),
         'a':np.zeros(shape),
         'Energy':np.zeros(N)
     }
     for i,sim in enumerate(sa):
         sim_results['time'][i] = sim.t
         orbits = get_orbits(sim)
-        sim_results['Energy'][i] = sim.calculate_energy()
+        sim_results['Energy'][i] = sim.energy()
         for j,orbit in enumerate(orbits):
             sim_results['P'][j,i] = orbit.P
             sim_results['e'][j,i] = orbit.e
             sim_results['l'][j,i] = orbit.l
             sim_results['pomega'][j,i] = orbit.pomega
             sim_results['a'][j,i] = orbit.a
             sim_results['omega'][j,i] = orbit.omega
@@ -125,15 +125,15 @@
         'a':np.zeros(shape),
         'Energy':np.zeros(N)
     }
     for i,sim_extra in enumerate(sa):
         sim,extra = sim_extra
         sim_results['time'][i] = sim.t
         orbits = get_orbits(sim)
-        sim_results['Energy'][i] = sim.calculate_energy()
+        sim_results['Energy'][i] = sim.energy()
         for j,orbit in enumerate(orbits):
             sim_results['P'][j,i] = orbit.P
             sim_results['e'][j,i] = orbit.e
             sim_results['l'][j,i] = orbit.l
             sim_results['pomega'][j,i] = orbit.pomega
             sim_results['a'][j,i] = orbit.a
             sim_results['omega'][j,i] = orbit.omega
@@ -324,15 +324,15 @@
     Mtot = np.array([p.m for p in sim.particles[:sim.N_real]]).sum()
     for p in sim.particles[:sim.N_real]:
         p.x -= m/Mtot*x
         p.y -= m/Mtot*y
         p.z -= m/Mtot*z
 
 def _compute_transformation_angles(sim):
-    Gtot_vec = sim.calculate_angular_momentum()
+    Gtot_vec = sim.angular_momentum()
     Gtot_vec = np.array(Gtot_vec)
     Gtot = np.sqrt(Gtot_vec @ Gtot_vec)
     Ghat = Gtot_vec / Gtot
     Ghat_z = Ghat[-1]
     Ghat_perp = np.sqrt(1 - Ghat_z**2)
     theta1 = np.pi/2 - np.arctan2(Ghat[1],Ghat[0])
     theta2 = np.pi/2 - np.arctan2(Ghat_z,Ghat_perp)
```

### Comparing `celmech-1.0.4/celmech/numerical_resonance_models.py` & `celmech-1.1.0/celmech/numerical_resonance_models.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/numerical_resonance_utils.py` & `celmech-1.1.0/celmech/numerical_resonance_utils.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/planar_poincare.py` & `celmech-1.1.0/celmech/planar_poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/poincare.py` & `celmech-1.1.0/celmech/poincare.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/poisson_series.py` & `celmech-1.1.0/celmech/poisson_series.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/resonances.py` & `celmech-1.1.0/celmech/resonances.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/rk_integrator.py` & `celmech-1.1.0/celmech/rk_integrator.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/secular.py` & `celmech-1.1.0/celmech/secular.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         for i,particle in enumerate(self.particles):
             if i==0:
                 continue # skip the star
             m,mu,M,Lambda = symbols('m{0},mu{0},M{0},Lambda{0}'.format(i)) 
             self.params.update({m:particle.m,mu:particle.mu,M:particle.M,Lambda:particle.Lambda})
         self.ecc_entries  = {(j,i):S(0) for i in xrange(1,self.N) for j in xrange(1,i+1)}
         self.inc_entries  = {(j,i):S(0) for i in xrange(1,self.N) for j in xrange(1,i+1)}
-        self.tol = np.min([p.m for p in self.particles[1:]]) * np.finfo(np.float).eps
+        self.tol = np.min([p.m for p in self.particles[1:]]) * np.finfo(np.float64).eps
         ps = self.particles[1:]
         self.eta0_vec = np.array([p.eta for p in ps])
         self.kappa0_vec = np.array([p.kappa for p in ps]) 
         self.rho0_vec = np.array([p.rho for p in ps])
         self.sigma0_vec = np.array([p.sigma for p in ps]) 
         self._update()
     @classmethod
```

### Comparing `celmech-1.0.4/celmech/symplectic_evolution_operators.py` & `celmech-1.1.0/celmech/symplectic_evolution_operators.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech/transformations.py` & `celmech-1.1.0/celmech/transformations.py`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/celmech.egg-info/PKG-INFO` & `celmech-1.1.0/celmech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celmech
-Version: 1.0.4
+Version: 1.1.0
 Summary: Open source tools for celestial mechanics
 Home-page: http://github.com/shadden/celmech
 Author: Dan Tamayo, Sam Hadden
 Author-email: tamayo.daniel@gmail.com, shadden1107@gmail.com
 License: GPL
 Keywords: astronomy astrophysics celestial-mechanics orbits orbital-mechanics
 Platform: UNKNOWN
```

### Comparing `celmech-1.0.4/celmech.egg-info/SOURCES.txt` & `celmech-1.1.0/celmech.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -26,10 +26,14 @@
 celmech.egg-info/dependency_links.txt
 celmech.egg-info/not-zip-safe
 celmech.egg-info/requires.txt
 celmech.egg-info/top_level.txt
 src/disturbing_function.c
 src/fmft.c
 src/fmftPy.c
+src/moid_v4_fun.f
 src/nrutil.c
 src/nrutil.h
-src/poisson_series.c
+src/poincare.c
+src/poisson_series.c
+src/poisson_series.h
+src/test.c
```

### Comparing `celmech-1.0.4/setup.py` & `celmech-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Try to get git hash
 try:
     import subprocess
     ghash = subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii")
     ghash_arg = "-DCELMECHGITHASH="+ghash.strip()
 except:
-    ghash_arg = "-DCELMECHGITHASH=255ba6181dbc18d75b9a177ea5ab1505c2487ff6" #GITHASHAUTOUPDATE
+    ghash_arg = "-DCELMECHGITHASH=044ab2f25459990b473eff5f7bd25adc0e48f84c" #GITHASHAUTOUPDATE
 
 extra_link_args=[]
 if sys.platform == 'darwin':
     from distutils import sysconfig
     vars = sysconfig.get_config_vars()
     vars['LDSHARED'] = vars['LDSHARED'].replace('-bundle', '-shared')
     extra_link_args=['-Wl,-install_name,@rpath/libcelmech'+suffix]
@@ -45,15 +45,15 @@
     packages = ['theano', 'sympy>=1.1.1', 'numpy', 'scipy>=1.2.0', 'reboundx>=3.1.0', 'rebound>=3.5.11', 'mpmath>=1.0.0']
     try:
         install_requires += packages
     except:
         install_requires = packages
 
 setup(name='celmech',
-    version='1.0.4',
+    version='1.1.0',
     description='Open source tools for celestial mechanics',
     url='http://github.com/shadden/celmech',
     author='Dan Tamayo, Sam Hadden',
     author_email='tamayo.daniel@gmail.com, shadden1107@gmail.com',
     license='GPL',
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `celmech-1.0.4/src/disturbing_function.c` & `celmech-1.1.0/src/disturbing_function.c`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #include <stdio.h>
 #include <assert.h>
 
 #define STRINGIFY(s) str(s)
 #define str(s) #s
 
 const char* celmech_build_str = __DATE__ " " __TIME__; // Date and time build string. 
-const char* celmech_version_str = "1.0.4";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
+const char* celmech_version_str = "1.1.0";         // **VERSIONLINE** This line gets updated automatically. Do not edit manually.
 const char* celmech_githash_str = STRINGIFY(CELMECHGITHASH);             // This line gets updated automatically. Do not edit manually.
 
 double laplace(double s, int i, int j, double a);
 double GeneralOrderCoefficient(int res_j, int order, int epower,double a);
 
 int binomialCoeff(int n, int k)
 {
```

### Comparing `celmech-1.0.4/src/fmft.c` & `celmech-1.1.0/src/fmft.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/src/fmftPy.c` & `celmech-1.1.0/src/fmftPy.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/src/nrutil.c` & `celmech-1.1.0/src/nrutil.c`

 * *Files identical despite different names*

### Comparing `celmech-1.0.4/src/poisson_series.c` & `celmech-1.1.0/src/poisson_series.c`

 * *Files identical despite different names*

