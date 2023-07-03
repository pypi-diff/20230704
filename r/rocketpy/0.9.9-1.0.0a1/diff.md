# Comparing `tmp/rocketpy-0.9.9.tar.gz` & `tmp/rocketpy-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketpy-0.9.9.tar", last modified: Sat Jan  8 23:10:02 2022, max compression
+gzip compressed data, was "rocketpy-1.0.0a1.tar", last modified: Mon Jul  3 23:43:01 2023, max compression
```

## Comparing `rocketpy-0.9.9.tar` & `rocketpy-1.0.0a1.tar`

### file list

```diff
@@ -1,20 +1,82 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1079 2022-01-08 23:09:08.000000 rocketpy-0.9.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    13285 2022-01-08 23:10:02.237356 rocketpy-0.9.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12744 2022-01-08 23:09:08.000000 rocketpy-0.9.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/rocketpy/
--rw-rw-r--   0 travis    (2000) travis    (2000)   143398 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Environment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150672 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Flight.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88141 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41975 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/Rocket.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29902 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/SolidMotor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2022-01-08 23:09:11.000000 rocketpy-0.9.9/rocketpy/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-01-08 23:10:02.237356 rocketpy-0.9.9/rocketpy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13285 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2022-01-08 23:10:02.000000 rocketpy-0.9.9/rocketpy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-01-08 23:10:02.237356 rocketpy-0.9.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      808 2022-01-08 23:09:11.000000 rocketpy-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.124276 rocketpy-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 23:42:49.000000 rocketpy-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-03 23:43:01.120276 rocketpy-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-07-03 23:42:49.000000 rocketpy-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.112275 rocketpy-1.0.0a1/rocketpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    55413 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/AeroSurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Components.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147569 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101288 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/EnvironmentAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153074 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Flight.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125969 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Parachute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50019 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/Rocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.116275 rocketpy-1.0.0a1/rocketpy/motors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/Fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21935 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/HybridMotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19194 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/LiquidMotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/Motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28511 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/SolidMotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47937 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/Tank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/TankGeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/motors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.116275 rocketpy-1.0.0a1/rocketpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/aero_surface_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.116275 rocketpy-1.0.0a1/rocketpy/plots/compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/compare/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57769 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/compare/compare_flights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64633 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/environment_analysis_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/environment_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28746 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/flight_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/fluid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/hybrid_motor_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/liquid_motor_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/motor_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/rocket_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/solid_motor_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/tank_geometry_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/plots/tank_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.120276 rocketpy-1.0.0a1/rocketpy/prints/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/aero_surface_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/compare_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/environment_analysis_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/environment_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/flight_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/fluid_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/hybrid_motor_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/liquid_motor_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/motor_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/parachute_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/rocket_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/solid_motor_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/tank_geometry_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/prints/tank_prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35156 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/rocketpy/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.112275 rocketpy-1.0.0a1/rocketpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-03 23:43:01.000000 rocketpy-1.0.0a1/rocketpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-03 23:43:01.000000 rocketpy-1.0.0a1/rocketpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:43:01.000000 rocketpy-1.0.0a1/rocketpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 23:43:01.000000 rocketpy-1.0.0a1/rocketpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 23:43:01.000000 rocketpy-1.0.0a1/rocketpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:43:01.124276 rocketpy-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:43:01.120276 rocketpy-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_environment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34754 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_flight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21453 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_rocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_solidmotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_tank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_tools_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_tools_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-03 23:42:50.000000 rocketpy-1.0.0a1/tests/test_utilities.py
```

### Comparing `rocketpy-0.9.9/LICENSE` & `rocketpy-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketpy-0.9.9/PKG-INFO` & `rocketpy-1.0.0a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,31 @@
-Metadata-Version: 2.1
-Name: rocketpy
-Version: 0.9.9
-Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/giovaniceotto/RocketPy
-Author: Giovani Hidalgo Ceotto
-Author-email: ghceotto@gmail.com
-Maintainer: RocketPy Developers
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![RocketPy Logo](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
+![RocketPy Logo](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
 
 <br>
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RocketPy-Team/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
 [![PyPI](https://img.shields.io/pypi/v/rocketpy?color=g)](https://pypi.org/project/rocketpy/)
 [![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://docs.rocketpy.org/en/latest/?badge=latest)
-[![Build Status](https://app.travis-ci.com/Projeto-Jupiter/RocketPy.svg?branch=master)](https://app.travis-ci.com/Projeto-Jupiter/RocketPy)
-[![Contributors](https://img.shields.io/github/contributors/Projeto-Jupiter/rocketpy)](https://github.com/Projeto-Jupiter/RocketPy/graphs/contributors)
+[![Build Status](https://app.travis-ci.com/RocketPy-Team/RocketPy.svg?branch=master)](https://app.travis-ci.com/RocketPy-Team/RocketPy)
+[![Contributors](https://img.shields.io/github/contributors/RocketPy-Team/rocketpy)](https://github.com/RocketPy-Team/RocketPy/graphs/contributors)
 [![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
+[![Sponsor RocketPy](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/RocketPy-Team)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/rocketpy)
 [![DOI](https://img.shields.io/badge/DOI-10.1061%2F%28ASCE%29AS.1943--5525.0001331-blue.svg)](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331)
 
 <img src="https://static.scarf.sh/a.png?x-pxid=6f4094ab-00fa-4a8d-9247-b7ed27e7164d" />
 
 # RocketPy
-RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
+
+RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high-fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profiles, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
 
 <br>
 
 ## Main features
+
 <details>
 <summary>Nonlinear 6 degrees of freedom simulations</summary>
 <ul>
   <li>Rigorous treatment of mass variation effects</li>
   <li>Solved using LSODA with adjustable error tolerances</li>
   <li>Highly optimized to run fast</li>
 </ul>
@@ -69,17 +55,18 @@
 <ul>
   <li>Test the exact code that will fly</li>
   <li>Sensor data can be augmented with noise</li>
 </ul>
 </details>
 
 <details>
-<summary>Solid motors models</summary>
+<summary>Solid, Hybrid and Liquid motors models</summary>
 <ul>
   <li>Burn rate and mass variation properties from thrust curve</li>
+  <li>Define custom rocket tanks based on their flux data</li>
   <li>CSV and ENG file support</li>
 </ul>
 </details>
 
 <details>
 <summary>Monte Carlo simulations</summary>
 <ul>
@@ -88,61 +75,70 @@
 </ul>
 </details>
 
 <details>
 <summary>Flexible and modular</summary>
 <ul>
   <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
-  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
+  <li>Non-standard flights (e.g. parachute drop test from a helicopter)</li>
   <li>Multi-stage rockets</li>
   <li>Custom continuous and discrete control laws</li>
   <li>Create new classes (e.g. other types of motors)</li>
 </ul>
 </details>
 
+<details>
+<summary>Integration with MATLAB®</summary>
+<ul>
+  <li>Straightforward way to run RocketPy from MATLAB®</li>
+  <li>Convert RocketPy results to MATLAB® variables so that they can be processed by MATLAB®</li>
+</ul>
+</details>
+
 <br>
 
 ## Validation
 
 RocketPy's features have been validated in our latest [research article published in the Journal of Aerospace Engineering](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331).
 
 The table below shows a comparison between experimental data and the output from RocketPy.
 Flight data and rocket parameters used in this comparison were kindly provided by [EPFL Rocket Team](https://github.com/EPFLRocketTeam) and [Notre Dame Rocket Team](https://ndrocketry.weebly.com/).
 
-|         Mission         |    Result Paramater    | RocketPy  | Measured  | Relative Error |
-|:-----------------------:|:-----------------------|:---------:|:---------:|:--------------:|
-|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**   |
-|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**   |
-|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **4.24 %**   |
-|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**  |
-|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**  |
-|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**   |
+|         Mission         |    Result Parameter    | RocketPy  | Measured  | Relative Error  |
+|:-----------------------:|:-----------------------|:---------:|:---------:|:---------------:|
+|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**    |
+|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**    |
+|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **-4.24 %**   |
+|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**   |
+|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**   |
+|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**    |
 
 <br>
 
 ## Documentation
 
 Check out documentation details using the links below:
 
-  - [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
-  - [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
-  - [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
+- [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
+- [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
+- [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
 
 <br>
 
 # Join Our Community!
-RocketPy is growing fast! Many university groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
+
+RocketPy is growing fast! Many university groups and rocket hobbyists have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
 
 If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
 
 <br>
 
 # Previewing
 
-You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb).  No installation required!
+You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/RocketPy-Team/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb). No installation is required!
 
 When you are ready to run RocketPy locally, you can read the *Getting Started* section!
 
 <br>
 
 # Getting Started
 
@@ -157,188 +153,226 @@
 For other installation options, visit our [Installation Docs](https://docs.rocketpy.org/en/latest/user/installation.html).
 To learn more about RocketPy's requirements, visit our [Requirements Docs](https://docs.rocketpy.org/en/latest/user/requirements.html).
 
 <br>
 
 ## Running Your First Simulation
 
-In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _nbks_ folder. Open _Getting Started - Examples.ipynb_ and you are ready to go.
+In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _docs/notebooks_ folder. Open _getting_started.ipynb_ and you are ready to go.
 
 Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
 
 - Environment - Keeps data related to weather.
-- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
+- Motor - Subdivided into SolidMotor, HybridMotor and LiquidMotor. Keeps data related to rocket motors.
 - Rocket - Keeps data related to a rocket.
 - Flight - Runs the simulation and keeps the results.
 
 The following image shows how the four main classes interact with each other:
 
-![Diagram](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
+![Diagram](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
 
 A typical workflow starts with importing these classes from RocketPy:
 
 ```python
 from rocketpy import Environment, Rocket, SolidMotor, Flight
 ```
 
+An optional step is to import datetime, which is used to define the date of the simulation:
+
+```python
+import datetime
+```
+
 Then create an Environment object. To learn more about it, you can use:
 
 ```python
 help(Environment)
 ```
 
 A sample code is:
 
 ```python
-Env = Environment(
-    railLength=5.2,
+env = Environment(
     latitude=32.990254,
     longitude=-106.974998,
     elevation=1400,
-    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
 ) 
 
-Env.setAtmosphericModel(type='Forecast', file='GFS')
+tomorrow = datetime.date.today() + datetime.timedelta(days=1)
+
+env.set_date(
+  (tomorrow.year, tomorrow.month, tomorrow.day, 12), timezone="America/Denver"
+) # Tomorrow's date in year, month, day, hour UTC format
+
+env.set_atmospheric_model(type='Forecast', file='GFS')
 ```
 
 This can be followed up by starting a Solid Motor object. To get help on it, just use:
 
 ```python
 help(SolidMotor)
 ```
 
 A sample Motor object can be created by the following code:
 
 ```python
 Pro75M1670 = SolidMotor(
-    thrustSource="../data/motors/Cesaroni_M1670.eng",
-    burnOut=3.9,
-    grainNumber=5,
-    grainSeparation=5/1000,
-    grainDensity=1815,
-    grainOuterRadius=33/1000,
-    grainInitialInnerRadius=15/1000,
-    grainInitialHeight=120/1000,
-    nozzleRadius=33/1000,
-    throatRadius=11/1000,
-    interpolationMethod='linear'
+    thrust_source="data/motors/Cesaroni_M1670.eng",
+    dry_mass=1.815,
+    dry_inertia=(0.125, 0.125, 0.002),
+    center_of_dry_mass=0.317,
+    grains_center_of_mass_position=0.397,
+    burn_time=3.9,
+    grain_number=5,
+    grain_separation=0.005,
+    grain_density=1815,
+    grain_outer_radius=0.033,
+    grain_initial_inner_radius=0.015,
+    grain_initial_height=0.12,
+    nozzle_radius=0.033,
+    throat_radius=0.011,
+    interpolation_method="linear",
+    nozzle_position=0,
+    coordinate_system_orientation="nozzle_to_combustion_chamber",
 )
 ```
 
 With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
 
 ```python
 help(Rocket)
 ```
 
 A sample code to create a Rocket is:
 
 ```python
-Calisto = Rocket(
-    motor=Pro75M1670,
-    radius=127/2000,
-    mass=19.197-2.956,
-    inertiaI=6.60,
-    inertiaZ=0.0351,
-    distanceRocketNozzle=-1.255,
-    distanceRocketPropellant=-0.85704,
-    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
-    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
+calisto = Rocket(
+    radius=0.0635,
+    mass=14.426,  # without motor
+    inertia=(6.321, 6.321, 0.034),
+    power_off_drag="data/calisto/powerOffDragCurve.csv",
+    power_on_drag="data/calisto/powerOnDragCurve.csv",
+    center_of_mass_without_motor=0,
+    coordinate_system_orientation="tail_to_nose",
 )
 
-Calisto.setRailButtons([0.2, -0.5])
+buttons = calisto.set_rail_buttons(
+    upper_button_position=0.0818,
+    lower_button_position=-0.6182,
+    angular_position=45,
+)
+
+calisto.add_motor(Pro75M1670, position=-1.255)
 
-NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
+nose = calisto.add_nose(
+    length=0.55829, kind="vonKarman", position=1.278
+)
 
-FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
+fins = calisto.add_trapezoidal_fins(
+    n=4,
+    root_chord=0.120,
+    tip_chord=0.040,
+    span=0.100,
+    sweep_length=None,
+    cant_angle=0,
+    position=-1.04956,
+)
 
-Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
+tail = calisto.add_tail(
+    top_radius=0.0635, bottom_radius=0.0435, length=0.060, position=-1.194656
+)
 ```
 
 You may want to add parachutes to your rocket as well:
 
 ```python
-def drogueTrigger(p, y):
-    return True if y[5] < 0 else False
-
-def mainTrigger(p, y):
-    return True if y[5] < 0 and y[2] < 800 else False
+main = calisto.add_parachute(
+    name="main",
+    cd_s=10.0,
+    trigger=800,  # ejection altitude in meters
+    sampling_rate=105,
+    lag=1.5,
+    noise=(0, 8.3, 0.5),
+)
 
-Main = Calisto.addParachute('Main',
-                            CdS=10.0,
-                            trigger=mainTrigger, 
-                            samplingRate=105,
-                            lag=1.5,
-                            noise=(0, 8.3, 0.5))
-
-Drogue = Calisto.addParachute('Drogue',
-                              CdS=1.0,
-                              trigger=drogueTrigger, 
-                              samplingRate=105,
-                              lag=1.5,
-                              noise=(0, 8.3, 0.5))
+drogue = calisto.add_parachute(
+    name="drogue",
+    cd_s=1.0,
+    trigger="apogee",  # ejection at apogee
+    sampling_rate=105,
+    lag=1.5,
+    noise=(0, 8.3, 0.5),
+)
 ```
 
 Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
 
 ```python
 help(Flight)
 ```
 
 To actually create a Flight object, use:
 
 ```python
-TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
+test_flight = Flight(
+  rocket=calisto, environment=env, rail_length=5.2, inclination=85, heading=0
+)
 ```
 
-Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
+Once the Flight object is created, your simulation is done! Use the following code to get a summary of the results:
 
 ```python
-TestFlight.info()
+test_flight.info()
 ```
 
-To seel all available results, use:
+To see all available results, use:
 
 ```python
-TestFlight.allInfo()
+test_flight.all_info()
 ```
 
-Here is just a quick taste of what RocketPy is able to calculate. There are hundred of plots and data points computed by RocketPy to enhance your analyses.
+Here is just a quick taste of what RocketPy is able to calculate. There are hundreds of plots and data points computed by RocketPy to enhance your analyses.
+
+![6-DOF Trajectory Plot](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/rocketpy_example_trajectory.svg)
 
-![6-DOF Trajectory Plot](docs/static/rocketpy_example_trajectory.svg)
+If you want to see the trajectory on Google Earth, RocketPy acn easily export a KML file for you:
+
+```python
+test_flight.export_kml(file_name="test_flight.kml")
+```
 
 <br>
 
 # Authors and Contributors
 
 This package was originally created by [Giovani Ceotto](https://github.com/giovaniceotto/) as part of his work at [Projeto Jupiter](https://github.com/Projeto-Jupiter/). [Rodrigo Schmitt](https://github.com/rodrigo-schmitt/) was one of the first contributors.
 
 Later, [Guilherme Fernandes](https://github.com/Gui-FernandesBR/) and [Lucas Azevedo](https://github.com/lucasfourier/) joined the team to work on the expansion and sustainability of this project.
 
-Since then, the [RocketPy Team](https://github.com/orgs/Projeto-Jupiter/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
+Since then, the [RocketPy Team](https://github.com/orgs/RocketPy-Team/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
 
-[![GitHub Contributors Image](https://contrib.rocks/image?repo=Projeto-Jupiter/RocketPy)](https://github.com/Projeto-Jupiter/RocketPy/contributors)
+[![GitHub Contributors Image](https://contrib.rocks/image?repo=RocketPy-Team/RocketPy)](https://github.com/RocketPy-Team/RocketPy/contributors)
 
-See a [detailed list of contributors](https://github.com/Projeto-Jupiter/RocketPy/contributors) who are actively working on RocketPy.
+See a [detailed list of contributors](https://github.com/RocketPy-Team/RocketPy/contributors) who are actively working on RocketPy.
 
 ## Supporting RocketPy and Contributing
 
-The easiest way to help RocketPy is to demonstrate your support by starring our repository! ![GitHub Repo stars](https://img.shields.io/github/stars/Projeto-Jupiter/RocketPy?style=social)
+The easiest way to help RocketPy is to demonstrate your support by starring our repository!
+[![starcharts stargazers over time](https://starchart.cc/rocketpy-team/rocketpy.svg)](https://starchart.cc/rocketpy-team/rocketpy)
 
-<br>
+You can also become a [sponsor](https://github.com/sponsors/RocketPy-Team) and help us financially to keep the project going.
 
 If you are actively using RocketPy in one of your projects, reaching out to our core team via [Discord](https://discord.gg/b6xYnNh) and providing feedback can help improve RocketPy a lot!
 
-And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more on how you can contribute with the development of this next-gen trajectory simulation solution for rocketry.
+And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/RocketPy-Team/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more about how you can contribute to the development of this next-gen trajectory simulation solution for rocketry.
 
 <br>
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/LICENSE) file for details
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/RocketPy-Team/RocketPy/blob/master/LICENSE) file for details
 
 <br>
 
 ## Release Notes
-Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/Projeto-Jupiter/RocketPy/releases).
-
 
+Want to know which bugs have been fixed and the new features of each version? Check out the [release notes](https://github.com/RocketPy-Team/RocketPy/releases).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rocketpy-0.9.9/rocketpy/Environment.py` & `rocketpy-1.0.0a1/rocketpy/Environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,315 +1,322 @@
 # -*- coding: utf-8 -*-
 
 __author__ = "Giovani Hidalgo Ceotto, Guilherme Fernandes Alves, Lucas Azevedo Pezente, Oscar Mauricio Prada Ramirez, Lucas Kierulff Balabram"
-__copyright__ = "Copyright 20XX, Projeto Jupiter"
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __license__ = "MIT"
 
-import re
-import math
 import bisect
+import json
+import re
 import warnings
-import time
 from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
 
 import numpy as np
-from scipy import integrate
-from scipy import linalg
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
+import numpy.ma as ma
+import pytz
 import requests
+from collections import namedtuple
+from rocketpy.Function import funcify_method
 
-# import ee
+from .Function import Function
+
+from .plots.environment_plots import _EnvironmentPlots
+from .prints.environment_prints import _EnvironmentPrints
 
 try:
     import netCDF4
-    from netCDF4 import Dataset
 except ImportError:
+    has_netCDF4 = False
     warnings.warn(
         "Unable to load netCDF4. NetCDF files and OPeNDAP will not be imported.",
         ImportWarning,
     )
+else:
+    has_netCDF4 = True
 
-from .Function import Function
+
+def requires_netCDF4(func):
+    def wrapped_func(*args, **kwargs):
+        if has_netCDF4:
+            func(*args, **kwargs)
+        else:
+            raise ImportError(
+                "This feature requires netCDF4 to be installed. Install it with `pip install netCDF4`"
+            )
+
+    return wrapped_func
 
 
 class Environment:
     """Keeps all environment information stored, such as wind and temperature
-    conditions, as well as gravity and rail length.
+    conditions, as well as gravity.
 
     Attributes
     ----------
 
         Constants
-        Environment.earthRadius : float
+        Environment.earth_radius : float
             Value of Earth's Radius = 6.3781e6 m.
-        Environment.airGasConstant : float
+        Environment.air_gas_constant : float
             Value of Air's Gas Constant = 287.05287 J/K/Kg
 
-        Gravity and Launch Rail Length:
-        Environment.rl : float
-            Launch rail length in meters.
-        Environment.g : float
+        Gravity:
+        Environment.gravity : float
             Positive value of gravitational acceleration in m/s^2.
 
         Coordinates and Date:
-        Environment.lat : float
+        Environment.latitude : float
             Launch site latitude.
-        Environment.lon : float
+        Environment.longitude : float
             Launch site longitude.
         Environment.datum: string
-            The desired reference ellipsoide model, the following options are
+            The desired reference ellipsoid model, the following options are
             available: "SAD69", "WGS84", "NAD83", and "SIRGAS2000". The default
             is "SIRGAS2000", then this model will be used if the user make some
             typing mistake
-        Environment.initialEast: float
+        Environment.initial_east: float
             Launch site East UTM coordinate
-        Environment.initialNorth:  float
+        Environment.initial_north:  float
             Launch site North UTM coordinate
-        Environment.initialUtmZone: int
+        Environment.initial_utm_zone: int
             Launch site UTM zone number
-        Environment.initialUtmLetter: string
+        Environment.initial_utm_letter: string
             Launch site UTM letter, to keep the latitude band and describe the
             UTM Zone
-        Environment.initialHemisphere: string
+        Environment.initial_hemisphere: string
             Launch site S/N hemisphere
-        Environment.initialEW: string
+        Environment.initial_ew: string
             Launch site E/W hemisphere
         Environment.elevation : float
             Launch site elevation.
         Environment.date : datetime
-            Date time of launch.
+            Date time of launch in UTC.
+        Environment.local_date : datetime
+                    Date time of launch in the local time zone, defined by Environment.timezone.
+        Environment.timezone : string
+                    Local time zone specification. See pytz for time zone info.
 
         Topographic information:
-        Environment.elevLonArray: array
+        Environment.elev_lon_array: array
             Unidimensional array containing the longitude coordinates
-        Environment.elevLatArray: array
+        Environment.elev_lat_array: array
             Unidimensional array containing the latitude coordinates
-        Environment.elevArray: array
+        Environment.elev_array: array
             Two-dimensional Array containing the elevation information
-        Environment.topographicProfileActivated: bool
-            True if the user already set a topographic plofile
+        Environment.topographic_profile_activated: bool
+            True if the user already set a topographic profile
 
         Atmosphere Static Conditions:
-        Environment.maxExpectedHeight : float
+        Environment.max_expected_height : float
             Maximum altitude in meters to keep weather data.
             Used especially for plotting range.
             Can be altered as desired.
-        Environment.pressureISA : Function
+        Environment.pressure_ISA : Function
             Air pressure in Pa as a function of altitude as defined
             by the International Standard Atmosphere ISO 2533.
-            Only defined after load Environment.loadInternationalStandardAtmosphere
+            Only defined after load Environment.load_international_standard_atmosphere
             has been called.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.temperatureISA : Function
+        Environment.temperature_ISA : Function
             Air temperature in K as a function of altitude  as defined
             by the International Standard Atmosphere ISO 2533.
-            Only defined after load Environment.loadInternationalStandardAtmosphere
+            Only defined after load Environment.load_international_standard_atmosphere
             has been called.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
         Environment.pressure : Function
             Air pressure in Pa as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
         Environment.temperature : Function
             Air temperature in K as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.speedOfSound : Function
+        Environment.speed_of_sound : Function
             Speed of sound in air in m/s as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
         Environment.density : Function
             Air density in kg/m³ as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.dynamicViscosity : Function
+        Environment.dynamic_viscosity : Function
             Air dynamic viscosity in Pa s as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
 
         Atmosphere Wind Conditions:
-        Environment.windSpeed : Function
+        Environment.wind_speed : Function
             Wind speed in m/s as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.windDirection : Function
+        Environment.wind_direction : Function
             Wind direction (from which the wind blows)
             in degrees relative to north (positive clockwise)
             as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.windHeading : Function
+        Environment.wind_heading : Function
             Wind heading (direction towards which the wind blows)
             in degrees relative to north (positive clockwise)
             as a function of altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.windVelocityX : Function
+        Environment.wind_velocity_x : Function
             Wind U, or X (east) component of wind velocity in m/s as a function of
             altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
-        Environment.windVelocityY : Function
+        Environment.wind_velocity_y : Function
             Wind V, or Y (east) component of wind velocity in m/s as a function of
             altitude.
             Can be accessed as regular array, or called
             as a function. See Function for more information.
 
         Atmospheric Model Details
-        Environment.atmosphericModelType : string
+        Environment.atmospheric_model_type : string
             Describes the atmospheric model which is being used.
-            Can only assume the following values: 'StandardAtmosphere',
-            'CustomAtmosphere', 'WyomingSounding', 'NOAARucSounding',
+            Can only assume the following values: 'standard_atmosphere',
+            'custom_atmosphere', 'wyoming_sounding', 'NOAARucSounding',
             'Forecast', 'Reanalysis', 'Ensemble'.
-        Environment.atmosphericModelFile : string
+        Environment.atmospheric_model_file : string
             Address of the file used for the atmospheric model being used.
-            Only defined for 'WyomingSounding', 'NOAARucSounding',
+            Only defined for 'wyoming_sounding', 'NOAARucSounding',
             'Forecast', 'Reanalysis', 'Ensemble'
-        Environment.atmosphericModelDict : dictionary
+        Environment.atmospheric_model_dict : dictionary
             Dictionary used to properly interpret netCDF and OPeNDAP
             files. Only defined for 'Forecast', 'Reanalysis', 'Ensemble'.
-        Environment.atmosphericModelInitDate : datetime
-            Datetime object instance of first availabe date in netCDF
+        Environment.atmospheric_model_init_date : datetime
+            Datetime object instance of first available date in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelEndDate : datetime
-            Datetime object instance of last availabe date in netCDF
+        Environment.atmospheric_model_end_date : datetime
+            Datetime object instance of last available date in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelInterval : int
+        Environment.atmospheric_model_interval : int
             Hour step between weather condition used in netCDF and
             OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelInitLat : float
+        Environment.atmospheric_model_init_lat : float
             Latitude of vertex just before the launch site in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelEndLat : float
+        Environment.atmospheric_model_end_lat : float
             Latitude of vertex just after the launch site in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelInitLon : float
+        Environment.atmospheric_model_init_lon : float
             Longitude of vertex just before the launch site in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
-        Environment.atmosphericModelEndLon : float
+        Environment.atmospheric_model_end_lon : float
             Longitude of vertex just after the launch site in netCDF
             and OPeNDAP files when using 'Forecast', 'Reanalysis' or
             'Ensemble'.
 
         Atmospheric Model Storage
-        Environment.latArray : array
+        Environment.lat_array : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of latitudes
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
-        Environment.lonArray : array
+        Environment.lon_array : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of longitudes
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
-        Environment.lonIndex : int
+        Environment.lon_index : int
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. Index to a grid longitude which
-            is just over the launch site longitude, while lonIndex - 1
+            is just over the launch site longitude, while lon_index - 1
             points to a grid longitude which is just under the launch
             site longitude.
-        Environment.latIndex : int
+        Environment.lat_index : int
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. Index to a grid latitude which
-            is just over the launch site latitude, while lonIndex - 1
+            is just over the launch site latitude, while lon_index - 1
             points to a grid latitude which is just under the launch
             site latitude.
         Environment.geopotentials : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of geopotential heights
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
-        Environment.windUs : array
+        Environment.wind_us : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of wind U (east) component
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
-        Environment.windVs : array
+        Environment.wind_vs : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of wind V (north) component
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
         Environment.levels : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. List of pressure levels available
             in the file.
         Environment.temperatures : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. 2x2 matrix for each pressure level of temperatures
             corresponding to the vertices of the grid cell which surrounds
             the launch site.
-        Environment.timeArray : array
+        Environment.time_array : array
             Defined if netCDF or OPeNDAP file is used, for Forecasts,
             Reanalysis and Ensembles. Array of dates available in the
             file.
         Environment.height : array
            Defined if netCDF or OPeNDAP file is used, for Forecasts,
            Reanalysis and Ensembles. List of geometric height
            corresponding to launch site location.
 
         Atmospheric Model Ensemble Specific Data
-        Environment.levelEnsemble : array
+        Environment.level_ensemble : array
             Only defined when using Ensembles.
-        Environment.heightEnsemble : array
+        Environment.height_ensemble : array
             Only defined when using Ensembles.
-        Environment.temperatureEnsemble : array
+        Environment.temperature_ensemble : array
             Only defined when using Ensembles.
-        Environment.windUEnsemble : array
+        Environment.wind_u_ensemble : array
             Only defined when using Ensembles.
-        Environment.windVEnsemble : array
+        Environment.wind_v_ensemble : array
             Only defined when using Ensembles.
-        Environment.windHeadingEnsemble : arrray
+        Environment.wind_heading_ensemble : array
             Only defined when using Ensembles.
-        Environment.windDirectionEnsemble : array
+        Environment.wind_direction_ensemble : array
             Only defined when using Ensembles.
-        Environment.windSpeedEnsemble : array
+        Environment.wind_speed_ensemble : array
             Only defined when using Ensembles.
-        Environment.numEnsembleMembers : int
+        Environment.num_ensemble_members : int
             Number of ensemble members. Only defined when using Ensembles.
-        Environment.ensembleMember : int
+        Environment.ensemble_member : int
             Current selected ensemble member. Only defined when using Ensembles.
     """
 
     def __init__(
         self,
-        railLength,
-        gravity=9.80665,
+        gravity=None,
         date=None,
         latitude=0,
         longitude=0,
         elevation=0,
         datum="SIRGAS2000",
+        timezone="UTC",
     ):
         """Initialize Environment class, saving launch rail length,
         launch date, location coordinates and elevation. Note that
         by default the standard atmosphere is loaded until another
-        atmospheric model is used. See Environment.setAtmosphericModel
-        for details.
 
         Parameters
         ----------
-        railLength : scalar
-            Length in which the rocket will be attached to the rail, only
-            moving along a fixed direction, that is, the line parallel to the
-            rail.
-        gravity : scalar, optional
+        gravity : int, float, callable, string, array, optional
             Surface gravitational acceleration. Positive values point the
-            acceleration down. Default value is 9.80665.
+            acceleration down. If None, the Somigliana formula is used to
         date : array, optional
             Array of length 4, stating (year, month, day, hour (UTC))
             of rocket launch. Must be given if a Forecast, Reanalysis
             or Ensemble, will be set as an atmospheric model.
         latitude : float, optional
             Latitude in degrees (ranging from -90 to 90) of rocket
             launch location. Must be given if a Forecast, Reanalysis
@@ -322,95 +329,135 @@
             Open-Elevation will be used to compute elevation.
         elevation : float, optional
             Elevation of launch site measured as height above sea
             level in meters. Alternatively, can be set as
             'Open-Elevation' which uses the Open-Elevation API to
             find elevation data. For this option, latitude and
             longitude must also be specified. Default value is 0.
-        datum:
+        datum : string
+            The desired reference ellipsoidal model, the following options are
+            available: "SAD69", "WGS84", "NAD83", and "SIRGAS2000". The default
+            is "SIRGAS2000", then this model will be used if the user make some
+            typing mistake.
+        timezone : string, optional
+            Name of the time zone. To see all time zones, import pytz and run
 
         Returns
         -------
         None
         """
-        # Save launch rail length
-        self.rL = railLength
+        # Initialize constants
+        self.earth_radius = 6.3781 * (10**6)
+        self.air_gas_constant = 287.05287  # in J/K/Kg
+        self.standard_g = 9.80665
 
-        # Save gravity value
-        self.g = gravity
+        # Initialize atmosphere
+        self.set_atmospheric_model("standard_atmosphere")
 
-        # Save datum
-        self.datum = datum
+        # Save latitude and longitude
+        if latitude != None and longitude != None:
+            self.set_location(latitude, longitude)
+        else:
+            self.latitude, self.longitude = None, None
 
         # Save date
         if date != None:
-            self.setDate(date)
+            self.set_date(date, timezone)
         else:
             self.date = None
+            self.datetime_date = None
+            self.local_date = None
+            self.timezone = None
 
-        # Initialize constants
-        self.earthRadius = 6.3781 * (10 ** 6)
-        self.airGasConstant = 287.05287  # in J/K/Kg
+        # Initialize Earth geometry and save datum
+        self.datum = datum
+        self.ellipsoid = self.set_earth_geometry(datum)
+
+        # Set gravity model
+        self.gravity = self.set_gravity_model(gravity)
+
+        # Initialize plots and prints objects
+        self.prints = _EnvironmentPrints(self)
 
         # Initialize atmosphere
-        self.setAtmosphericModel("StandardAtmosphere")
+        self.set_atmospheric_model("standard_atmosphere")
 
         # Save latitude and longitude
+        self.latitude = latitude
+        self.longitude = longitude
         if latitude != None and longitude != None:
-            self.setLocation(latitude, longitude)
+            self.set_location(latitude, longitude)
         else:
-            self.lat, self.lon = None, None
+            self.latitude, self.longitude = None, None
 
         # Store launch site coordinates referenced to UTM projection system
-        if self.lat > -80 and self.lat < 84:
-            convert = self.geodesicToUtm(self.lat, self.lon, self.datum)
-            self.initialNorth = convert[1]
-            self.initialEast = convert[0]
-            self.initialUtmZone = convert[2]
-            self.initialUtmLetter = convert[3]
-            self.initialHemisphere = convert[4]
-            self.initialEW = convert[5]
+        if self.latitude > -80 and self.latitude < 84:
+            convert = self.geodesic_to_utm(self.latitude, self.longitude)
+
+            self.initial_north = convert[1]
+            self.initial_east = convert[0]
+            self.initial_utm_zone = convert[2]
+            self.initial_utm_letter = convert[3]
+            self.initial_hemisphere = convert[4]
+            self.initial_ew = convert[5]
 
         # Save elevation
-        self.setElevation(elevation)
+        self.elevation = elevation
+        self.set_elevation(elevation)
 
         # Recalculate Earth Radius
-        self.earthRadius = self.calculateEarthRadius(self.lat, self.datum)  # in m
+        self.earth_radius = self.calculate_earth_radius(self.latitude)  # in m
+
+        # Initialize plots and prints object
+        self.plots = _EnvironmentPlots(self)
 
         return None
 
-    def setDate(self, date):
+    def set_date(self, date, timezone="UTC"):
         """Set date and time of launch and update weather conditions if
         date dependent atmospheric model is used.
 
         Parameters
         ----------
-        date : Date
-            Date object specifying launch date and time.
+        date : Datetime
+            Datetime object specifying launch date and time.
+        timezone : string, optional
+            Name of the time zone. To see all time zones, import pytz and run
+        print(pytz.all_timezones). Default time zone is "UTC".
 
         Return
         ------
         None
         """
-        # Store date
-        self.date = datetime(*date)
+        # Store date and configure time zone
+        self.timezone = timezone
+        tz = pytz.timezone(self.timezone)
+        if type(date) != datetime:
+            local_date = datetime(*date)
+        else:
+            local_date = date
+        if local_date.tzinfo == None:
+            local_date = tz.localize(local_date)
+        self.date = date
+        self.local_date = local_date
+        self.datetime_date = self.local_date.astimezone(pytz.UTC)
 
         # Update atmospheric conditions if atmosphere type is Forecast,
         # Reanalysis or Ensemble
         try:
-            if self.atmosphericModelType in ["Forecast", "Reanalysis", "Ensemble"]:
-                self.setAtmosphericModel(
-                    self.atmosphericModelFile, self.atmosphericModelDict
+            if self.atmospheric_model_type in ["Forecast", "Reanalysis", "Ensemble"]:
+                self.set_atmospheric_model(
+                    self.atmospheric_model_file, self.atmospheric_model_dict
                 )
         except AttributeError:
             pass
 
         return None
 
-    def setLocation(self, latitude, longitude):
+    def set_location(self, latitude, longitude):
         """Set latitude and longitude of launch and update atmospheric
         conditions if location dependent model is being used.
 
         Parameters
         ----------
         latitude : float
             Latitude of launch site. May range from -90 to 90
@@ -420,78 +467,139 @@
             or from -180 to 180 degrees.
 
         Return
         ------
         None
         """
         # Store latitude and longitude
-        self.lat = latitude
-        self.lon = longitude
+        self.latitude = latitude
+        self.longitude = longitude
 
         # Update atmospheric conditions if atmosphere type is Forecast,
         # Reanalysis or Ensemble
-        if self.atmosphericModelType in ["Forecast", "Reanalysis", "Ensemble"]:
-            self.setAtmosphericModel(
-                self.atmosphericModelFile, self.atmosphericModelDict
+        if self.atmospheric_model_type in ["Forecast", "Reanalysis", "Ensemble"]:
+            self.set_atmospheric_model(
+                self.atmospheric_model_file, self.atmospheric_model_dict
             )
 
         # Return None
 
-    def setElevation(self, elevation="Open-Elevation"):
+    def set_gravity_model(self, gravity):
+        """Sets the gravity model to be used in the simulation based
+        on the given user input to the gravity parameter.
+
+        Parameters
+        ----------
+        gravity : None or Function source
+
+        Returns
+        -------
+        Function
+            Function object representing the gravity model.
+        """
+        if gravity is None:
+            return self.somigliana_gravity.set_discrete(
+                0, self.max_expected_height, 100
+            )
+        else:
+            return Function(gravity, "height (m)", "gravity (m/s²)").set_discrete(
+                0, self.max_expected_height, 100
+            )
+
+    @funcify_method("height (m)", "gravity (m/s²)")
+    def somigliana_gravity(self, height):
+        """Computes the gravity acceleration with the Somigliana formula.
+        An height correction is applied to the normal gravity that is
+        accurate for heights used in aviation. The formula is based on the
+        WGS84 ellipsoid, but is accurate for other reference ellipsoids.
+
+        Parameters
+        ----------
+        height : float
+            Height above the reference ellipsoid in meters.
+
+        Returns
+        -------
+        Function
+            Function object representing the gravity model.
+        """
+        a = 6378137.0  # semi_major_axis
+        f = 1 / 298.257223563  # flattening_factor
+        m_rot = 3.449786506841e-3  # rotation_factor
+        g_e = 9.7803253359  # normal gravity at equator
+        k_somgl = 1.931852652458e-3  # normal gravity formula const.
+        first_ecc_sqrd = 6.694379990141e-3  # square of first eccentricity
+
+        # Compute quantities
+        sin_lat_sqrd = (np.sin(self.latitude * np.pi / 180)) ** 2
+
+        gravity_somgl = g_e * (
+            (1 + k_somgl * sin_lat_sqrd) / (np.sqrt(1 - first_ecc_sqrd * sin_lat_sqrd))
+        )
+        height_correction = (
+            1
+            - height * 2 / a * (1 + f + m_rot - 2 * f * sin_lat_sqrd)
+            + 3 * height**2 / a**2
+        )
+
+        return height_correction * gravity_somgl
+
+    def set_elevation(self, elevation="Open-Elevation"):
         """Set elevation of launch site given user input or using the
         Open-Elevation API.
 
         Parameters
         ----------
         elevation : float, string, optional
             Elevation of launch site measured as height above sea
             level in meters.
             Alternatively, can be set as 'Open-Elevation' which uses
             the Open-Elevation API to find elevation data. For this
             option, latitude and longitude must have already been
-            specified. See Environment.setLocation for more details.
+            specified. See Environment.set_location for more details.
 
         Return
         ------
         None
         """
         if elevation != "Open-Elevation" and elevation != "SRTM":
             self.elevation = elevation
-        # elif elevation == "SRTM" and self.lat != None and self.lon != None:
+        # elif elevation == "SRTM" and self.latitude != None and self.longitude != None:
         #     # Trigger the authentication flow.
         #     #ee.Authenticate()
         #     # Initialize the library.
         #     ee.Initialize()
 
         #     # Calculate elevation
         #     dem  = ee.Image('USGS/SRTMGL1_003')
-        #     xy   = ee.Geometry.Point([self.lon, self.lat])
+        #     xy   = ee.Geometry.Point([self.longitude, self.latitude])
         #     elev = dem.sample(xy, 30).first().get('elevation').getInfo()
 
         #     self.elevation = elev
 
-        elif self.lat != None and self.lon != None:
+        elif self.latitude != None and self.longitude != None:
             try:
                 print("Fetching elevation from open-elevation.com...")
                 requestURL = "https://api.open-elevation.com/api/v1/lookup?locations={:f},{:f}".format(
-                    self.lat, self.lon
+                    self.latitude, self.longitude
                 )
                 response = requests.get(requestURL)
                 results = response.json()["results"]
                 self.elevation = results[0]["elevation"]
-                print("Elevation received: ", self.elevation)
+                print("Elevation received:", self.elevation)
             except:
-                raise RuntimeError("Unabel to reach Open-Elevation API servers.")
+                raise RuntimeError("Unable to reach Open-Elevation API servers.")
         else:
             raise ValueError(
                 "Latitude and longitude must be set to use"
-                " Open-Elevation API. See Environment.setLocation."
+                " Open-Elevation API. See Environment.set_location."
             )
 
-    def setTopographicProfile(self, type, file, dictionary="netCDF4", crs=None):
+    @requires_netCDF4
+    def set_topographic_profile(self, type, file, dictionary="netCDF4", crs=None):
         """[UNDER CONSTRUCTION] Defines the Topographic profile, importing data
         from previous downloaded files. Mainly data from the Shuttle Radar
         Topography Mission (SRTM) and NASA Digital Elevation Model will be used
         but other models and methods can be implemented in the future.
         So far, this function can only handle data from NASADEM, available at:
         https://cmr.earthdata.nasa.gov/search/concepts/C1546314436-LPDAAC_ECS.html
 
@@ -511,38 +619,38 @@
         crs : string, optional
             Coordinate reference system, by default None, which will use the crs
             provided by the file.
         """
 
         if type == "NASADEM_HGT":
             if dictionary == "netCDF4":
-                rootgrp = Dataset(file, "r", format="NETCDF4")
-                self.elevLonArray = rootgrp.variables["lon"][:].tolist()
-                self.elevLatArray = rootgrp.variables["lat"][:].tolist()
-                self.elevArray = rootgrp.variables["NASADEM_HGT"][:].tolist()
+                rootgrp = netCDF4.Dataset(file, "r", format="NETCDF4")
+                self.elev_lon_array = rootgrp.variables["lon"][:].tolist()
+                self.elev_lat_array = rootgrp.variables["lat"][:].tolist()
+                self.elev_array = rootgrp.variables["NASADEM_HGT"][:].tolist()
                 # crsArray = rootgrp.variables['crs'][:].tolist().
-                self.topographicProfileActivated = True
+                self.topographic_profile_activated = True
 
                 print("Region covered by the Topographical file: ")
                 print(
                     "Latitude from {:.6f}° to {:.6f}°".format(
-                        self.elevLatArray[-1], self.elevLatArray[0]
+                        self.elev_lat_array[-1], self.elev_lat_array[0]
                     )
                 )
                 print(
                     "Longitude from {:.6f}° to {:.6f}°".format(
-                        self.elevLonArray[0], self.elevLonArray[-1]
+                        self.elev_lon_array[0], self.elev_lon_array[-1]
                     )
                 )
 
         return None
 
-    def getElevationFromTopograghicProfile(self, lat, lon):
-        """Function which receives as inputs the coordinates of a point and finds its
-        elevation in the provided Topographic Profile
+    def get_elevation_from_topographic_profile(self, lat, lon):
+        """Function which receives as inputs the coordinates of a point and
+        finds its elevation in the provided Topographic Profile.
 
         Parameters
         ----------
         lat : float
             latitude of the point.
         lon : float
             longitude of the point.
@@ -555,112 +663,112 @@
         Raises
         ------
         ValueError
             [description]
         ValueError
             [description]
         """
-        if self.topographicProfileActivated == False:
+        if self.topographic_profile_activated == False:
             print(
-                "You must define a Topographic profile first, please use the method Environment.setTopograghicProfile()"
+                "You must define a Topographic profile first, please use the method Environment.set_topographic_profile()"
             )
             return None
 
         # Find latitude index
         # Check if reversed or sorted
-        if self.elevLatArray[0] < self.elevLatArray[-1]:
-            # Deal with sorted self.elevLatArray
-            latIndex = bisect.bisect(self.elevLatArray, lat)
-        else:
-            # Deal with reversed self.elevLatArray
-            self.elevLatArray.reverse()
-            latIndex = len(self.elevLatArray) - bisect.bisect_left(
-                self.elevLatArray, lat
+        if self.elev_lat_array[0] < self.elev_lat_array[-1]:
+            # Deal with sorted self.elev_lat_array
+            lat_index = bisect.bisect(self.elev_lat_array, lat)
+        else:
+            # Deal with reversed self.elev_lat_array
+            self.elev_lat_array.reverse()
+            lat_index = len(self.elev_lat_array) - bisect.bisect_left(
+                self.elev_lat_array, lat
             )
-            self.elevLatArray.reverse()
+            self.elev_lat_array.reverse()
         # Take care of latitude value equal to maximum longitude in the grid
         if (
-            latIndex == len(self.elevLatArray)
-            and self.elevLatArray[latIndex - 1] == lat
+            lat_index == len(self.elev_lat_array)
+            and self.elev_lat_array[lat_index - 1] == lat
         ):
-            latIndex = latIndex - 1
+            lat_index = lat_index - 1
         # Check if latitude value is inside the grid
-        if latIndex == 0 or latIndex == len(self.elevLatArray):
+        if lat_index == 0 or lat_index == len(self.elev_lat_array):
             raise ValueError(
                 "Latitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    lat, self.elevLatArray[0], self.elevLatArray[-1]
+                    lat, self.elev_lat_array[0], self.elev_lat_array[-1]
                 )
             )
 
         # Find longitude index
         # Determine if file uses -180 to 180 or 0 to 360
-        if self.elevLonArray[0] < 0 or self.elevLonArray[-1] < 0:
+        if self.elev_lon_array[0] < 0 or self.elev_lon_array[-1] < 0:
             # Convert input to -180 - 180
             lon = lon if lon < 180 else -180 + lon % 180
         else:
             # Convert input to 0 - 360
             lon = lon % 360
         # Check if reversed or sorted
-        if self.elevLonArray[0] < self.elevLonArray[-1]:
-            # Deal with sorted self.elevLonArray
-            lonIndex = bisect.bisect(self.elevLonArray, lon)
-        else:
-            # Deal with reversed self.elevLonArray
-            self.elevLonArray.reverse()
-            lonIndex = len(self.elevLonArray) - bisect.bisect_left(
-                self.elevLonArray, lon
+        if self.elev_lon_array[0] < self.elev_lon_array[-1]:
+            # Deal with sorted self.elev_lon_array
+            lon_index = bisect.bisect(self.elev_lon_array, lon)
+        else:
+            # Deal with reversed self.elev_lon_array
+            self.elev_lon_array.reverse()
+            lon_index = len(self.elev_lon_array) - bisect.bisect_left(
+                self.elev_lon_array, lon
             )
-            self.elevLonArray.reverse()
+            self.elev_lon_array.reverse()
         # Take care of longitude value equal to maximum longitude in the grid
         if (
-            lonIndex == len(self.elevLonArray)
-            and self.elevLonArray[lonIndex - 1] == lon
+            lon_index == len(self.elev_lon_array)
+            and self.elev_lon_array[lon_index - 1] == lon
         ):
-            lonIndex = lonIndex - 1
+            lon_index = lon_index - 1
         # Check if longitude value is inside the grid
-        if lonIndex == 0 or lonIndex == len(self.elevLonArray):
+        if lon_index == 0 or lon_index == len(self.elev_lon_array):
             raise ValueError(
                 "Longitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    lon, self.elevLonArray[0], self.elevLonArray[-1]
+                    lon, self.elev_lon_array[0], self.elev_lon_array[-1]
                 )
             )
 
         # Get the elevation
-        elevation = self.elevArray[latIndex][lonIndex]
+        elevation = self.elev_array[lat_index][lon_index]
 
         return elevation
 
-    def setAtmosphericModel(
+    def set_atmospheric_model(
         self,
         type,
         file=None,
         dictionary=None,
         pressure=None,
         temperature=None,
         wind_u=0,
         wind_v=0,
     ):
         """Defines an atmospheric model for the Environment.
         Supported functionality includes using data from the
         International Standard Atmosphere, importing data from
         weather reanalysis, forecasts and ensemble forecasts,
-        importing data from upper air soundings and inputing
+        importing data from upper air soundings and inputting
         data as custom functions, arrays or csv files.
 
         Parameters
         ----------
         type : string
             One of the following options:
-            - 'StandardAtmosphere': sets pressure and temperature
+            - 'standard_atmosphere': sets pressure and temperature
             profiles corresponding to the International Standard
             Atmosphere defined by ISO 2533 and ranging from -2 km
             to 80 km of altitude above sea level. Note that the wind
             profiles are set to zero when this type is chosen.
 
-            - 'WyomingSounding': sets pressure, temperature, wind-u
+            - 'wyoming_sounding': sets pressure, temperature, wind-u
             and wind-v profiles and surface elevation obtained from
             an upper air sounding given by the file parameter through
             an URL. This URL should point to a data webpage given by
             selecting plot type as text: list, a station and a time at
             http://weather.uwyo.edu/upperair/sounding.html.
             An example of a valid link would be:
             http://weather.uwyo.edu/cgi-bin/sounding?region=samer&TYPE=TEXT%3ALIST&YEAR=2019&MONTH=02&FROM=0200&TO=0200&STNM=82599
@@ -674,14 +782,18 @@
             initial data source, specifying the station through it's
             WMO-ID and opting for the ASCII (GSD format) button, the
             following example URL opens up: https://rucsoundings.noaa.gov/get_raobs.cgi?data_source=RAOB&latest=latest&start_year=2019&start_month_name=Feb&start_mday=5&start_hour=12&start_min=0&n_hrs=1.0&fcst_len=shortest&airport=83779&text=Ascii%20text%20%28GSD%20format%29&hydrometeors=false&start=latest
             Any ASCII GSD format page from this server can be read,
             so information from virtual soundings such as GFS and NAM
             can also be imported.
 
+            - 'windy_atmosphere': sets pressure, temperature, wind-u and wind-v
+            profiles and surface elevation obtained from the Windy API. See file
+            argument to specify the model as either ECMWF, GFS or ICON.
+
             - 'Forecast': sets pressure, temperature, wind-u and wind-v
             profiles and surface elevation obtained from a weather
             forecast file in netCDF format or from an OPeNDAP URL, both
             given through the file parameter. When this type
             is chosen, the date and location of the launch
             should already have been set through the date and
             location parameters when initializing the Environment.
@@ -736,35 +848,39 @@
             supplied through the dictionary parameter in order for the
             dataset to be accurately read. Lastly, the dataset must use
             a rectangular grid sorted in either ascending or descending
             order of latitude and longitude. By default the first ensemble
             forecast is activated. To activate other ensemble forecasts
             see Environment.selectEnsembleMemberMember().
 
-            - 'CustomAtmosphere': sets pressure, temperature, wind-u
+            - 'custom_atmosphere': sets pressure, temperature, wind-u
             and wind-v profiles given though the pressure, temperature,
             wind-u and wind-v parameters of this method. If pressure
             or temperature is not given, it will default to the
             International Standard Atmosphere. If the wind components
             are not given, it will default to 0.
+
         file : string, optional
             String that must be given when type is either
-            'WyomingSounding', 'Forecast', 'Reanalysis' or 'Ensemble'.
+            'wyoming_sounding', 'Forecast', 'Reanalysis', 'Ensemble' or 'Windy'.
             It specifies the location of the data given, either through
             a local file address or a URL.
             If type is 'Forecast', this parameter can also be either
             'GFS', 'FV3', 'RAP' or 'NAM' for latest of these forecasts.
             References: GFS: Global - 0.25deg resolution - Updates every 6 hours, forecast for 81 points spaced by 3 hours
                         FV3: Global - 0.25deg resolution - Updates every 6 hours, forecast for 129 points spaced by 3 hours
                         RAP: Regional USA - 0.19deg resolution - Updates hourly, forecast for 40 points spaced hourly
                         NAM: Regional CONUS Nest - 5 km resolution - Updates every 6 hours, forecast for 21 points spaced by 3 hours
             If type is 'Ensemble', this parameter can also be either
             'GEFS', or 'CMC' for the latest of these ensembles.
             References: GEFS: Global, bias-corrected, 0.5deg resolution, 21 forecast members, Updates every 6 hours, forecast for 65 points spaced by 4 hours
                        CMC: Global, 0.5deg resolution, 21 forecast members, Updates every 12 hours, forecast for 65 points spaced by 4 hours
+            If type is 'Windy', this parameter can be either 'GFS', 'ECMWF', 'ICON' or
+            'ICONEU'
+            Default in this case is 'ecmwf'.
         dictionary : dictionary, string, optional
             Dictionary that must be given when type is either
             'Forecast', 'Reanalysis' or 'Ensemble'.
             It specifies the dictionary to be used when reading netCDF
             and OPeNDAP files, allowing the correct retrieval of data.
             Acceptable values include 'ECMWF', 'NOAA' and 'UCAR' for
             default dictionaries which can generally be used to read
@@ -785,30 +901,30 @@
             'surface_geopotential_height': 'hgtsfc',
                     'geopotential_height': 'hgtprs',
                            'geopotential': None,
                                  'u_wind': 'ugrdprs',
                                  'v_wind': 'vgrdprs'}
         pressure : float, string, array, callable, optional
             This defines the atmospheric pressure profile.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             than the the Standard Atmosphere pressure will be used.
             If a float is given, it will define a constant pressure
             profile. The float should be in units of Pa.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the pressure in Pa.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, pressure in Pa).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding pressure in Pa.
         temperature : float, string, array, callable, optional
             This defines the atmospheric temperature profile.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             than the the Standard Atmosphere temperature will be used.
             If a float is given, it will define a constant temperature
             profile. The float should be in units of K.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the temperature in K.
@@ -816,15 +932,15 @@
             of coordinates (height in meters, temperature in K).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding temperature in K.
         wind_u : float, string, array, callable, optional
             This defines the atmospheric wind-u profile, corresponding
             the the magnitude of the wind speed heading East.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             it will be assumed to be constant and equal to 0.
             If a float is given, it will define a constant wind-u
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-u in m/s.
@@ -832,15 +948,15 @@
             coordinates (height in meters, wind-u in m/s).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-u in m/s.
         wind_v : float, string, array, callable, optional
             This defines the atmospheric wind-v profile, corresponding
             the the magnitude of the wind speed heading North.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             it will be assumed to be constant and equal to 0.
             If a float is given, it will define a constant wind-v
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-v in m/s.
@@ -851,27 +967,27 @@
             level in meters and return a corresponding wind-v in m/s.
 
         Return
         ------
         None
         """
         # Save atmospheric model type
-        self.atmosphericModelType = type
+        self.atmospheric_model_type = type
 
         # Handle each case
-        if type == "StandardAtmosphere":
-            self.processStandardAtmosphere()
-        elif type == "WyomingSounding":
-            self.processWyomingSounding(file)
+        if type == "standard_atmosphere":
+            self.process_standard_atmosphere()
+        elif type == "wyoming_sounding":
+            self.process_wyoming_sounding(file)
             # Save file
-            self.atmosphericModelFile = file
+            self.atmospheric_model_file = file
         elif type == "NOAARucSounding":
-            self.processNOAARUCSounding(file)
+            self.process_noaaruc_sounding(file)
             # Save file
-            self.atmosphericModelFile = file
+            self.atmospheric_model_file = file
         elif type == "Forecast" or type == "Reanalysis":
             # Process default forecasts if requested
             if file == "GFS":
                 # Define dictionary
                 dictionary = {
                     "time": "time",
                     "latitude": "lat",
@@ -881,30 +997,30 @@
                     "surface_geopotential_height": "hgtsfc",
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=6 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=6 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/gfs_0p25/gfs{:04d}{:02d}{:02d}/gfs_0p25_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        6 * (timeAttempt.hour // 6),
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        6 * (time_attempt.hour // 6),
                     )
                     try:
-                        self.processForecastReanalysis(file, dictionary)
+                        self.process_forecast_reanalysis(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for GFS through " + file
                     )
             elif file == "FV3":
                 # Define dictionary
                 dictionary = {
@@ -916,30 +1032,30 @@
                     "surface_geopotential_height": "hgtsfc",
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=6 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=6 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/gfs_0p25_parafv3/gfs{:04d}{:02d}{:02d}/gfs_0p25_parafv3_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        6 * (timeAttempt.hour // 6),
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        6 * (time_attempt.hour // 6),
                     )
                     try:
-                        self.processForecastReanalysis(file, dictionary)
+                        self.process_forecast_reanalysis(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for FV3 through " + file
                     )
             elif file == "NAM":
                 # Define dictionary
                 dictionary = {
@@ -951,30 +1067,30 @@
                     "surface_geopotential_height": "hgtsfc",
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=6 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=6 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/nam/nam{:04d}{:02d}{:02d}/nam_conusnest_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        6 * (timeAttempt.hour // 6),
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        6 * (time_attempt.hour // 6),
                     )
                     try:
-                        self.processForecastReanalysis(file, dictionary)
+                        self.process_forecast_reanalysis(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for NAM through " + file
                     )
             elif file == "RAP":
                 # Define dictionary
                 dictionary = {
@@ -986,30 +1102,30 @@
                     "surface_geopotential_height": "hgtsfc",
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=1 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=1 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/rap/rap{:04d}{:02d}{:02d}/rap_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        timeAttempt.hour,
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        time_attempt.hour,
                     )
                     try:
-                        self.processForecastReanalysis(file, dictionary)
+                        self.process_forecast_reanalysis(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for RAP through " + file
                     )
             # Process other forecasts or reanalysis
             else:
                 # Check if default dictionary was requested
@@ -1040,18 +1156,18 @@
                         "v_wind": "vgrdprs",
                     }
                 elif dictionary is None:
                     raise TypeError(
                         "Please specify a dictionary or choose a default one such as ECMWF or NOAA."
                     )
                 # Process forecast or reanalysis
-                self.processForecastReanalysis(file, dictionary)
+                self.process_forecast_reanalysis(file, dictionary)
             # Save dictionary and file
-            self.atmosphericModelFile = file
-            self.atmosphericModelDict = dictionary
+            self.atmospheric_model_file = file
+            self.atmospheric_model_dict = dictionary
         elif type == "Ensemble":
             # Process default forecasts if requested
             if file == "GEFS":
                 # Define dictionary
                 dictionary = {
                     "time": "time",
                     "latitude": "lat",
@@ -1062,30 +1178,30 @@
                     "surface_geopotential_height": None,
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=6 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=6 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/gens_bc/gens{:04d}{:02d}{:02d}/gep_all_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        6 * (timeAttempt.hour // 6),
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        6 * (time_attempt.hour // 6),
                     )
                     try:
-                        self.processEnsemble(file, dictionary)
+                        self.process_ensemble(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for GEFS through " + file
                     )
             elif file == "CMC":
                 # Define dictionary
                 dictionary = {
@@ -1098,30 +1214,30 @@
                     "surface_geopotential_height": None,
                     "geopotential_height": "hgtprs",
                     "geopotential": None,
                     "u_wind": "ugrdprs",
                     "v_wind": "vgrdprs",
                 }
                 # Attempt to get latest forecast
-                timeAttempt = datetime.utcnow()
+                time_attempt = datetime.utcnow()
                 success = False
-                attemptCount = 0
-                while not success and attemptCount < 10:
-                    timeAttempt -= timedelta(hours=12 * attemptCount)
+                attempt_count = 0
+                while not success and attempt_count < 10:
+                    time_attempt -= timedelta(hours=12 * attempt_count)
                     file = "https://nomads.ncep.noaa.gov/dods/cmcens/cmcens{:04d}{:02d}{:02d}/cmcens_all_{:02d}z".format(
-                        timeAttempt.year,
-                        timeAttempt.month,
-                        timeAttempt.day,
-                        12 * (timeAttempt.hour // 12),
+                        time_attempt.year,
+                        time_attempt.month,
+                        time_attempt.day,
+                        12 * (time_attempt.hour // 12),
                     )
                     try:
-                        self.processEnsemble(file, dictionary)
+                        self.process_ensemble(file, dictionary)
                         success = True
                     except OSError:
-                        attemptCount += 1
+                        attempt_count += 1
                 if not success:
                     raise RuntimeError(
                         "Unable to load latest weather data for CMC through " + file
                     )
             # Process other forecasts or reanalysis
             else:
                 # Check if default dictionary was requested
@@ -1150,115 +1266,117 @@
                         "surface_geopotential_height": None,
                         "geopotential_height": "hgtprs",
                         "geopotential": None,
                         "u_wind": "ugrdprs",
                         "v_wind": "vgrdprs",
                     }
                 # Process forecast or reanalysis
-                self.processEnsemble(file, dictionary)
+                self.process_ensemble(file, dictionary)
             # Save dictionary and file
-            self.atmosphericModelFile = file
-            self.atmosphericModelDict = dictionary
-        elif type == "CustomAtmosphere":
-            self.processCustomAtmosphere(pressure, temperature, wind_u, wind_v)
+            self.atmospheric_model_file = file
+            self.atmospheric_model_dict = dictionary
+        elif type == "custom_atmosphere":
+            self.process_custom_atmosphere(pressure, temperature, wind_u, wind_v)
+        elif type == "Windy":
+            self.process_windy_atmosphere(file)
         else:
             raise ValueError("Unknown model type.")
 
         # Calculate air density
-        self.calculateDensityProfile()
+        self.calculate_density_profile()
 
         # Calculate speed of sound
-        self.calculateSpeedOfSoundProfile()
+        self.calculate_speed_of_sound_profile()
 
         # Update dynamic viscosity
-        self.calculateDynamicViscosity()
+        self.calculate_dynamic_viscosity()
 
         return None
 
-    def processStandardAtmosphere(self):
+    def process_standard_atmosphere(self):
         """Sets pressure and temperature profiles corresponding to the
         International Standard Atmosphere defined by ISO 2533 and
         ranging from -2 km to 80 km of altitude above sea level. Note
         that the wind profiles are set to zero.
 
         Parameters
         ---------
         None
 
         Returns
         -------
         None
         """
         # Load international standard atmosphere
-        self.loadInternationalStandardAtmosphere()
+        self.load_international_standard_atmosphere()
 
         # Save temperature, pressure and wind profiles
-        self.pressure = self.pressureISA
-        self.temperature = self.temperatureISA
-        self.windDirection = Function(
+        self.pressure = self.pressure_ISA
+        self.temperature = self.temperature_ISA
+        self.wind_direction = Function(
             0,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
-        self.windHeading = Function(
+        self.wind_heading = Function(
             0,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
-        self.windSpeed = Function(
+        self.wind_speed = Function(
             0,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
-        self.windVelocityX = Function(
+        self.wind_velocity_x = Function(
             0,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
+        self.wind_velocity_y = Function(
             0,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
 
         # Set maximum expected height
-        self.maxExpectedHeight = 80000
+        self.max_expected_height = 80000
 
         return None
 
-    def processCustomAtmosphere(
+    def process_custom_atmosphere(
         self, pressure=None, temperature=None, wind_u=0, wind_v=0
     ):
         """Import pressure, temperature and wind profile given by user.
 
         Parameters
         ----------
         pressure : float, string, array, callable, optional
             This defines the atmospheric pressure profile.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             than the the Standard Atmosphere pressure will be used.
             If a float is given, it will define a constant pressure
             profile. The float should be in units of Pa.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the pressure in Pa.
             If an array is given, it is expected to be a list or array
             of coordinates (height in meters, pressure in Pa).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding pressure in Pa.
         temperature : float, string, array, callable, optional
             This defines the atmospheric temperature profile.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             than the the Standard Atmosphere temperature will be used.
             If a float is given, it will define a constant temperature
             profile. The float should be in units of K.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the temperature in K.
@@ -1266,15 +1384,15 @@
             of coordinates (height in meters, temperature in K).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding temperature in K.
         wind_u : float, string, array, callable, optional
             This defines the atmospheric wind-u profile, corresponding
             the the magnitude of the wind speed heading East.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             it will be assumed constant and 0.
             If a float is given, it will define a constant wind-u
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-u in m/s.
@@ -1282,15 +1400,15 @@
             coordinates (height in meters, wind-u in m/s).
             Finally, a callable or function is also accepted. The
             function should take one argument, the height above sea
             level in meters and return a corresponding wind-u in m/s.
         wind_v : float, string, array, callable, optional
             This defines the atmospheric wind-v profile, corresponding
             the the magnitude of the wind speed heading North.
-            Should be given if the type parameter is 'CustomAtmosphere'. If not,
+            Should be given if the type parameter is 'custom_atmosphere'. If not,
             it will be assumed constant and 0.
             If a float is given, it will define a constant wind-v
             profile. The float should be in units of m/s.
             If a string is given, it should point to a .CSV file
             containing at most one header line and two columns of data.
             The first column must be the geometric height above sea level in
             meters while the second column must be the wind-v in m/s.
@@ -1301,103 +1419,259 @@
             level in meters and return a corresponding wind-v in m/s.
 
         Return
         ------
         None
         """
         # Initialize an estimate of the maximum expected atmospheric model height
-        maxExpectedHeight = 1000
+        max_expected_height = 1000
 
         # Save pressure profile
         if pressure is None:
             # Use standard atmosphere
-            self.pressure = self.pressureISA
+            self.pressure = self.pressure_ISA
         else:
             # Use custom input
             self.pressure = Function(
                 pressure,
                 inputs="Height Above Sea Level (m)",
                 outputs="Pressure (Pa)",
                 interpolation="linear",
             )
             # Check maximum height of custom pressure input
             if not callable(self.pressure.source):
-                maxExpectedHeight = max(self.pressure[-1, 0], maxExpectedHeight)
+                max_expected_height = max(self.pressure[-1, 0], max_expected_height)
 
         # Save temperature profile
         if temperature is None:
             # Use standard atmosphere
-            self.temperature = self.temperatureISA
+            self.temperature = self.temperature_ISA
         else:
             self.temperature = Function(
                 temperature,
                 inputs="Height Above Sea Level (m)",
                 outputs="Temperature (K)",
                 interpolation="linear",
             )
             # Check maximum height of custom temperature input
             if not callable(self.temperature.source):
-                maxExpectedHeight = max(self.temperature[-1, 0], maxExpectedHeight)
+                max_expected_height = max(self.temperature[-1, 0], max_expected_height)
 
         # Save wind profile
-        self.windVelocityX = Function(
+        self.wind_velocity_x = Function(
             wind_u,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
+        self.wind_velocity_y = Function(
             wind_v,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
         # Check maximum height of custom wind input
-        if not callable(self.windVelocityX.source):
-            maxExpectedHeight = max(self.windVelocityX[-1, 0], maxExpectedHeight)
-        if not callable(self.windVelocityY.source):
-            maxExpectedHeight = max(self.windVelocityY[-1, 0], maxExpectedHeight)
+        if not callable(self.wind_velocity_x.source):
+            max_expected_height = max(self.wind_velocity_x[-1, 0], max_expected_height)
+        if not callable(self.wind_velocity_y.source):
+            max_expected_height = max(self.wind_velocity_y[-1, 0], max_expected_height)
 
         # Compute wind profile direction and heading
-        windHeading = (
-            lambda h: np.arctan2(self.windVelocityX(h), self.windVelocityY(h))
+        wind_heading = (
+            lambda h: np.arctan2(self.wind_velocity_x(h), self.wind_velocity_y(h))
             * (180 / np.pi)
             % 360
         )
-        self.windHeading = Function(
-            windHeading,
+        self.wind_heading = Function(
+            wind_heading,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
 
-        windDirection = lambda h: (windHeading(h) - 180) % 360
-        self.windDirection = Function(
-            windDirection,
+        def wind_direction(h):
+            return (wind_heading(h) - 180) % 360
+
+        self.wind_direction = Function(
+            wind_direction,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
 
-        windSpeed = lambda h: np.sqrt(
-            self.windVelocityX(h) ** 2 + self.windVelocityY(h) ** 2
-        )
-        self.windSpeed = Function(
-            windSpeed,
+        def wind_speed(h):
+            return np.sqrt(self.wind_velocity_x(h) ** 2 + self.wind_velocity_y(h) ** 2)
+
+        self.wind_speed = Function(
+            wind_speed,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
 
         # Save maximum expected height
-        self.maxExpectedHeight = maxExpectedHeight
+        self.max_expected_height = max_expected_height
 
         return None
 
-    def processWyomingSounding(self, file):
+    def process_windy_atmosphere(self, model="ECMWF"):
+        """Process data from Windy.com to retrieve atmospheric forecast data.
+
+        Parameters
+        ----------
+        model : string, optional
+            The atmospheric model to use. Default is 'ECMWF'. Options are:
+            'ECMWF' for the ECMWF-HRES model, 'GFS' for the GFS model, 'ICON'
+            for the ICON-Global model or 'ICONEU' for the ICON-EU model.
+        """
+
+        # Process the model string
+        model = model.lower()
+        if model[-1] == "u":  # case iconEu
+            model = "".join([model[:4], model[4].upper(), model[4 + 1 :]])
+        # Load data from Windy.com: json file
+        url = f"https://node.windy.com/forecast/meteogram/{model}/{self.latitude}/{self.longitude}/?step=undefined"
+        try:
+            response = requests.get(url).json()
+        except:
+            if model == "iconEu":
+                raise ValueError(
+                    "Could not get a valid response for Icon-EU from Windy. Check if the latitude and longitude coordinates set are inside Europe.",
+                )
+            raise
+
+        # Determine time index from model
+        time_array = np.array(response["data"]["hours"])
+        time_units = "milliseconds since 1970-01-01 00:00:00"
+        launch_time_in_units = netCDF4.date2num(self.datetime_date, time_units)
+        # Find the index of the closest time in time_array to the launch time
+        time_index = (np.abs(time_array - launch_time_in_units)).argmin()
+
+        # Define available pressure levels
+        pressure_levels = np.array(
+            [1000, 950, 925, 900, 850, 800, 700, 600, 500, 400, 300, 250, 200, 150]
+        )
+
+        # Process geopotential height array
+        geopotential_height_array = np.array(
+            [response["data"][f"gh-{pL}h"][time_index] for pL in pressure_levels]
+        )
+        # Convert geopotential height to geometric altitude (ASL)
+        R = self.earth_radius
+        altitude_array = R * geopotential_height_array / (R - geopotential_height_array)
+
+        # Process temperature array (in Kelvin)
+        temperature_array = np.array(
+            [response["data"][f"temp-{pL}h"][time_index] for pL in pressure_levels]
+        )
+
+        # Process wind-u and wind-v array (in m/s)
+        wind_u_array = np.array(
+            [response["data"][f"wind_u-{pL}h"][time_index] for pL in pressure_levels]
+        )
+        wind_v_array = np.array(
+            [response["data"][f"wind_v-{pL}h"][time_index] for pL in pressure_levels]
+        )
+
+        # Determine wind speed, heading and direction
+        wind_speed_array = np.sqrt(wind_u_array**2 + wind_v_array**2)
+        wind_heading_array = (
+            np.arctan2(wind_u_array, wind_v_array) * (180 / np.pi) % 360
+        )
+        wind_direction_array = (wind_heading_array - 180) % 360
+
+        # Combine all data into big array
+        data_array = np.ma.column_stack(
+            [
+                100 * pressure_levels,  # Convert hPa to Pa
+                altitude_array,
+                temperature_array,
+                wind_u_array,
+                wind_v_array,
+                wind_heading_array,
+                wind_direction_array,
+                wind_speed_array,
+            ]
+        )
+
+        # Save atmospheric data
+        self.pressure = Function(
+            data_array[:, (1, 0)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Pressure (Pa)",
+            interpolation="linear",
+        )
+        self.temperature = Function(
+            data_array[:, (1, 2)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Temperature (K)",
+            interpolation="linear",
+        )
+        self.wind_direction = Function(
+            data_array[:, (1, 6)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Wind Direction (Deg True)",
+            interpolation="linear",
+        )
+        self.wind_heading = Function(
+            data_array[:, (1, 5)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Wind Heading (Deg True)",
+            interpolation="linear",
+        )
+        self.wind_speed = Function(
+            data_array[:, (1, 7)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Wind Speed (m/s)",
+            interpolation="linear",
+        )
+        self.wind_velocity_x = Function(
+            data_array[:, (1, 3)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Wind Velocity X (m/s)",
+            interpolation="linear",
+        )
+        self.wind_velocity_y = Function(
+            data_array[:, (1, 4)],
+            inputs="Height Above Sea Level (m)",
+            outputs="Wind Velocity Y (m/s)",
+            interpolation="linear",
+        )
+
+        # Save maximum expected height
+        self.max_expected_height = max(altitude_array[0], altitude_array[-1])
+
+        # Get elevation data from file
+        self.elevation = response["header"]["elevation"]
+
+        # Compute info data
+        self.atmospheric_model_init_date = netCDF4.num2date(
+            time_array[0], units=time_units
+        )
+        self.atmospheric_model_end_date = netCDF4.num2date(
+            time_array[-1], units=time_units
+        )
+        self.atmospheric_model_interval = netCDF4.num2date(
+            (time_array[-1] - time_array[0]) / (len(time_array) - 1), units=time_units
+        ).hour
+        self.atmospheric_model_init_lat = self.latitude
+        self.atmospheric_model_end_lat = self.latitude
+        self.atmospheric_model_init_lon = self.longitude
+        self.atmospheric_model_end_lon = self.longitude
+
+        # Save debugging data
+        self.geopotentials = geopotential_height_array
+        self.wind_us = wind_u_array
+        self.wind_vs = wind_v_array
+        self.levels = pressure_levels
+        self.temperatures = temperature_array
+        self.time_array = time_array
+        self.height = altitude_array
+
+    def process_wyoming_sounding(self, file):
         """Import and process the upper air sounding data from Wyoming
         Upper Air Soundings database given by the url in file. Sets
         pressure, temperature, wind-u, wind-v profiles and surface elevation.
 
         Parameters
         ----------
         file : string
@@ -1422,15 +1696,15 @@
                 + " Check station number and date."
             )
         if response.text == "Invalid OUTPUT: specified\n":
             raise ValueError(
                 "Invalid OUTPUT: specified. Make sure the output is Text: List."
             )
 
-        # Process Wyoming Souding by finding data table and station info
+        # Process Wyoming Sounding by finding data table and station info
         response_split_text = re.split("(<.{0,1}PRE>)", response.text)
         data_table = response_split_text[2]
         station_info = response_split_text[6]
 
         # Transform data table into np array
         data_array = []
         for line in data_table.split("\n")[
@@ -1466,63 +1740,63 @@
         data_array[:, 5] = (
             data_array[:, 6] + 180
         ) % 360  # Convert wind direction to wind heading
         data_array[:, 3] = data_array[:, 7] * np.sin(data_array[:, 5] * np.pi / 180)
         data_array[:, 4] = data_array[:, 7] * np.cos(data_array[:, 5] * np.pi / 180)
 
         # Convert geopotential height to geometric height
-        R = self.earthRadius
+        R = self.earth_radius
         data_array[:, 1] = R * data_array[:, 1] / (R - data_array[:, 1])
 
         # Save atmospheric data
-        self.windDirection = Function(
+        self.wind_direction = Function(
             data_array[:, (1, 6)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
-        self.windHeading = Function(
+        self.wind_heading = Function(
             data_array[:, (1, 5)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
-        self.windSpeed = Function(
+        self.wind_speed = Function(
             data_array[:, (1, 7)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
-        self.windVelocityX = Function(
+        self.wind_velocity_x = Function(
             data_array[:, (1, 3)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
+        self.wind_velocity_y = Function(
             data_array[:, (1, 4)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
 
         # Retrieve station elevation from station info
         station_elevation_text = station_info.split("\n")[6]
 
         # Convert station elevation text into float value
         self.elevation = float(
-            re.findall("[0-9]+\.[0-9]+|[0-9]+", station_elevation_text)[0]
+            re.findall(r"[0-9]+\.[0-9]+|[0-9]+", station_elevation_text)[0]
         )
 
         # Save maximum expected height
-        self.maxExpectedHeight = data_array[-1, 1]
+        self.max_expected_height = data_array[-1, 1]
 
         return None
 
-    def processNOAARUCSounding(self, file):
+    def process_noaaruc_sounding(self, file):
         """Import and process the upper air sounding data from NOAA
         Ruc Soundings database (https://rucsoundings.noaa.gov/) given as
         ASCII GSD format pages passed by its url to the file parameter. Sets
         pressure, temperature, wind-u, wind-v profiles and surface elevation.
 
         Parameters
         ----------
@@ -1591,32 +1865,32 @@
                     # Check if values exist
                     if max(columns) != 99999:
                         # Save value
                         temperature_array.append(columns)
         temperature_array = np.array(temperature_array)
 
         # Extract wind speed and direction as a function of height
-        windSpeed_array = []
-        windDirection_array = []
+        wind_speed_array = []
+        wind_direction_array = []
         for line in lines:
             # Split line into columns
             columns = re.split(" +", line)[1:]
             if len(columns) >= 6:
                 if columns[0] in ["4", "5", "6", "7", "8", "9"]:
                     # Convert columns to floats
                     columns = np.array(columns, dtype=float)
                     # Select relevant columns
                     columns = columns[[2, 5, 6]]
                     # Check if values exist
                     if max(columns) != 99999:
                         # Save value
-                        windDirection_array.append(columns[[0, 1]])
-                        windSpeed_array.append(columns[[0, 2]])
-        windSpeed_array = np.array(windSpeed_array)
-        windDirection_array = np.array(windDirection_array)
+                        wind_direction_array.append(columns[[0, 1]])
+                        wind_speed_array.append(columns[[0, 2]])
+        wind_speed_array = np.array(wind_speed_array)
+        wind_direction_array = np.array(wind_direction_array)
 
         # Converts 10*hPa to Pa and save values
         pressure_array[:, 1] = 10 * pressure_array[:, 1]
         self.pressure = Function(
             pressure_array,
             inputs="Height Above Sea Level (m)",
             outputs="Pressure (Pa)",
@@ -1631,66 +1905,67 @@
             temperature_array,
             inputs="Height Above Sea Level (m)",
             outputs="Temperature (K)",
             interpolation="linear",
         )
 
         # Process wind-u and wind-v
-        windSpeed_array[:, 1] = (
-            windSpeed_array[:, 1] * 1.852 / 3.6
+        wind_speed_array[:, 1] = (
+            wind_speed_array[:, 1] * 1.852 / 3.6
         )  # Converts Knots to m/s
-        windHeading_array = windDirection_array[:, :] * 1
+        windHeading_array = wind_direction_array[:, :] * 1
         windHeading_array[:, 1] = (
-            windDirection_array[:, 1] + 180
+            wind_direction_array[:, 1] + 180
         ) % 360  # Convert wind direction to wind heading
-        windU = windSpeed_array[:, :] * 1
-        windV = windSpeed_array[:, :] * 1
-        windU[:, 1] = windSpeed_array[:, 1] * np.sin(
+        wind_u = wind_speed_array[:, :] * 1
+        wind_v = wind_speed_array[:, :] * 1
+        wind_u[:, 1] = wind_speed_array[:, 1] * np.sin(
             windHeading_array[:, 1] * np.pi / 180
         )
-        windV[:, 1] = windSpeed_array[:, 1] * np.cos(
+        wind_v[:, 1] = wind_speed_array[:, 1] * np.cos(
             windHeading_array[:, 1] * np.pi / 180
         )
 
         # Save wind data
-        self.windDirection = Function(
-            windDirection_array,
+        self.wind_direction = Function(
+            wind_direction_array,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
-        self.windHeading = Function(
+        self.wind_heading = Function(
             windHeading_array,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
-        self.windSpeed = Function(
-            windSpeed_array,
+        self.wind_speed = Function(
+            wind_speed_array,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
-        self.windVelocityX = Function(
-            windU,
+        self.wind_velocity_x = Function(
+            wind_u,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
-            windV,
+        self.wind_velocity_y = Function(
+            wind_v,
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
 
         # Save maximum expected height
-        self.maxExpectedHeight = pressure_array[-1, 0]
+        self.max_expected_height = pressure_array[-1, 0]
 
-    def processForecastReanalysis(self, file, dictionary):
+    @requires_netCDF4
+    def process_forecast_reanalysis(self, file, dictionary):
         """Import and process atmospheric data from weather forecasts
         and reanalysis given as netCDF or OPeNDAP files.
         Sets pressure, temperature, wind-u and wind-v
         profiles and surface elevation obtained from a weather
         file in netCDF format or from an OPeNDAP URL, both
         given through the file parameter. The date and location of the launch
         should already have been set through the date and
@@ -1734,182 +2009,187 @@
                                  'v_wind': 'vgrdprs'}
 
         Returns
         -------
         None
         """
         # Check if date, lat and lon are known
-        if self.date is None:
+        if self.datetime_date is None:
             raise TypeError(
                 "Please specify Date (array-like) when "
                 "initializing this Environment. "
-                "Alternatively, use the Environment.setDate"
+                "Alternatively, use the Environment.set_date"
                 " method."
             )
-        if self.lat is None:
+        if self.latitude is None:
             raise TypeError(
                 "Please specify Location (lat, lon). when "
                 "initializing this Environment. "
                 "Alternatively, use the Environment."
-                "setLocation method."
+                "set_location method."
             )
 
         # Read weather file
-        weatherData = netCDF4.Dataset(file)
+        weather_data = netCDF4.Dataset(file)
 
         # Get time, latitude and longitude data from file
-        timeArray = weatherData.variables[dictionary["time"]]
-        lonArray = weatherData.variables[dictionary["longitude"]][:].tolist()
-        latArray = weatherData.variables[dictionary["latitude"]][:].tolist()
+        time_array = weather_data.variables[dictionary["time"]]
+        lon_array = weather_data.variables[dictionary["longitude"]][:].tolist()
+        lat_array = weather_data.variables[dictionary["latitude"]][:].tolist()
 
         # Find time index
-        timeIndex = netCDF4.date2index(
-            self.date, timeArray, calendar="gregorian", select="nearest"
+        time_index = netCDF4.date2index(
+            self.datetime_date, time_array, calendar="gregorian", select="nearest"
         )
         # Convert times do dates and numbers
-        inputTimeNum = netCDF4.date2num(
-            self.date, timeArray.units, calendar="gregorian"
+        input_time_num = netCDF4.date2num(
+            self.datetime_date, time_array.units, calendar="gregorian"
         )
-        fileTimeNum = timeArray[timeIndex]
-        fileTimeDate = netCDF4.num2date(
-            timeArray[timeIndex], timeArray.units, calendar="gregorian"
+        file_time_num = time_array[time_index]
+        file_time_date = netCDF4.num2date(
+            time_array[time_index], time_array.units, calendar="gregorian"
         )
         # Check if time is inside range supplied by file
-        if timeIndex == 0 and inputTimeNum < fileTimeNum:
+        if time_index == 0 and input_time_num < file_time_num:
             raise ValueError(
                 "Chosen launch time is not available in the provided file, which starts at {:}.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
-        elif timeIndex == len(timeArray) - 1 and inputTimeNum > fileTimeNum:
+        elif time_index == len(time_array) - 1 and input_time_num > file_time_num:
             raise ValueError(
                 "Chosen launch time is not available in the provided file, which ends at {:}.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
         # Check if time is exactly equal to one in the file
-        if inputTimeNum != fileTimeNum:
+        if input_time_num != file_time_num:
             warnings.warn(
                 "Exact chosen launch time is not available in the provided file, using {:} UTC instead.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
 
         # Find longitude index
         # Determine if file uses -180 to 180 or 0 to 360
-        if lonArray[0] < 0 or lonArray[-1] < 0:
+        if lon_array[0] < 0 or lon_array[-1] < 0:
             # Convert input to -180 - 180
-            lon = self.lon if self.lon < 180 else -180 + self.lon % 180
+            lon = (
+                self.longitude if self.longitude < 180 else -180 + self.longitude % 180
+            )
         else:
             # Convert input to 0 - 360
-            lon = self.lon % 360
+            lon = self.longitude % 360
         # Check if reversed or sorted
-        if lonArray[0] < lonArray[-1]:
-            # Deal with sorted lonArray
-            lonIndex = bisect.bisect(lonArray, lon)
-        else:
-            # Deal with reversed lonArray
-            lonArray.reverse()
-            lonIndex = len(lonArray) - bisect.bisect_left(lonArray, lon)
-            lonArray.reverse()
+        if lon_array[0] < lon_array[-1]:
+            # Deal with sorted lon_array
+            lon_index = bisect.bisect(lon_array, lon)
+        else:
+            # Deal with reversed lon_array
+            lon_array.reverse()
+            lon_index = len(lon_array) - bisect.bisect_left(lon_array, lon)
+            lon_array.reverse()
         # Take care of longitude value equal to maximum longitude in the grid
-        if lonIndex == len(lonArray) and lonArray[lonIndex - 1] == lon:
-            lonIndex = lonIndex - 1
+        if lon_index == len(lon_array) and lon_array[lon_index - 1] == lon:
+            lon_index = lon_index - 1
         # Check if longitude value is inside the grid
-        if lonIndex == 0 or lonIndex == len(lonArray):
+        if lon_index == 0 or lon_index == len(lon_array):
             raise ValueError(
                 "Longitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    lon, lonArray[0], lonArray[-1]
+                    lon, lon_array[0], lon_array[-1]
                 )
             )
 
         # Find latitude index
         # Check if reversed or sorted
-        if latArray[0] < latArray[-1]:
-            # Deal with sorted latArray
-            latIndex = bisect.bisect(latArray, self.lat)
-        else:
-            # Deal with reversed latArray
-            latArray.reverse()
-            latIndex = len(latArray) - bisect.bisect_left(latArray, self.lat)
-            latArray.reverse()
+        if lat_array[0] < lat_array[-1]:
+            # Deal with sorted lat_array
+            lat_index = bisect.bisect(lat_array, self.latitude)
+        else:
+            # Deal with reversed lat_array
+            lat_array.reverse()
+            lat_index = len(lat_array) - bisect.bisect_left(lat_array, self.latitude)
+            lat_array.reverse()
         # Take care of latitude value equal to maximum longitude in the grid
-        if latIndex == len(latArray) and latArray[latIndex - 1] == self.lat:
-            latIndex = latIndex - 1
+        if lat_index == len(lat_array) and lat_array[lat_index - 1] == self.latitude:
+            lat_index = lat_index - 1
         # Check if latitude value is inside the grid
-        if latIndex == 0 or latIndex == len(latArray):
+        if lat_index == 0 or lat_index == len(lat_array):
             raise ValueError(
                 "Latitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    self.lat, latArray[0], latArray[-1]
+                    self.latitude, lat_array[0], lat_array[-1]
                 )
             )
 
         # Get pressure level data from file
         try:
             levels = (
-                100 * weatherData.variables[dictionary["level"]][:]
+                100 * weather_data.variables[dictionary["level"]][:]
             )  # Convert mbar to Pa
         except:
             raise ValueError(
                 "Unable to read pressure levels from file. Check file and dictionary."
             )
 
         # Get geopotential data from file
         try:
-            geopotentials = weatherData.variables[dictionary["geopotential_height"]][
-                timeIndex, :, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)
+            geopotentials = weather_data.variables[dictionary["geopotential_height"]][
+                time_index, :, (lat_index - 1, lat_index), (lon_index - 1, lon_index)
             ]
         except:
             try:
                 geopotentials = (
-                    weatherData.variables[dictionary["geopotential"]][
-                        timeIndex, :, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)
+                    weather_data.variables[dictionary["geopotential"]][
+                        time_index,
+                        :,
+                        (lat_index - 1, lat_index),
+                        (lon_index - 1, lon_index),
                     ]
-                    / self.g
+                    / self.standard_g
                 )
             except:
                 raise ValueError(
-                    "Unable to read geopontential height"
+                    "Unable to read geopotential height"
                     " nor geopotential from file. At least"
                     " one of them is necessary. Check "
                     " file and dictionary."
                 )
 
         # Get temperature from file
         try:
-            temperatures = weatherData.variables[dictionary["temperature"]][
-                timeIndex, :, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)
+            temperatures = weather_data.variables[dictionary["temperature"]][
+                time_index, :, (lat_index - 1, lat_index), (lon_index - 1, lon_index)
             ]
         except:
             raise ValueError(
                 "Unable to read temperature from file. Check file and dictionary."
             )
 
         # Get wind data from file
         try:
-            windUs = weatherData.variables[dictionary["u_wind"]][
-                timeIndex, :, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)
+            wind_us = weather_data.variables[dictionary["u_wind"]][
+                time_index, :, (lat_index - 1, lat_index), (lon_index - 1, lon_index)
             ]
         except:
             raise ValueError(
                 "Unable to read wind-u component. Check file and dictionary."
             )
         try:
-            windVs = weatherData.variables[dictionary["v_wind"]][
-                timeIndex, :, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)
+            wind_vs = weather_data.variables[dictionary["v_wind"]][
+                time_index, :, (lat_index - 1, lat_index), (lon_index - 1, lon_index)
             ]
         except:
             raise ValueError(
                 "Unable to read wind-v component. Check file and dictionary."
             )
 
         # Prepare for bilinear interpolation
-        x, y = self.lat, lon
-        x1, y1 = latArray[latIndex - 1], lonArray[lonIndex - 1]
-        x2, y2 = latArray[latIndex], lonArray[lonIndex]
+        x, y = self.latitude, lon
+        x1, y1 = lat_array[lat_index - 1], lon_array[lon_index - 1]
+        x2, y2 = lat_array[lat_index], lon_array[lon_index]
 
         # Determine geopotential in lat, lon
         f_x1_y1 = geopotentials[:, 0, 0]
         f_x1_y2 = geopotentials[:, 0, 1]
         f_x2_y1 = geopotentials[:, 1, 0]
         f_x2_y2 = geopotentials[:, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
@@ -1922,114 +2202,113 @@
         f_x2_y1 = temperatures[:, 1, 0]
         f_x2_y2 = temperatures[:, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
         temperature = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind u in lat, lon
-        f_x1_y1 = windUs[:, 0, 0]
-        f_x1_y2 = windUs[:, 0, 1]
-        f_x2_y1 = windUs[:, 1, 0]
-        f_x2_y2 = windUs[:, 1, 1]
+        f_x1_y1 = wind_us[:, 0, 0]
+        f_x1_y2 = wind_us[:, 0, 1]
+        f_x2_y1 = wind_us[:, 1, 0]
+        f_x2_y2 = wind_us[:, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
-        windU = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
+        wind_u = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind v in lat, lon
-        f_x1_y1 = windVs[:, 0, 0]
-        f_x1_y2 = windVs[:, 0, 1]
-        f_x2_y1 = windVs[:, 1, 0]
-        f_x2_y2 = windVs[:, 1, 1]
+        f_x1_y1 = wind_vs[:, 0, 0]
+        f_x1_y2 = wind_vs[:, 0, 1]
+        f_x2_y1 = wind_vs[:, 1, 0]
+        f_x2_y2 = wind_vs[:, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
-        windV = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
+        wind_v = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind speed, heading and direction
-        windSpeed = np.sqrt(windU ** 2 + windV ** 2)
-        windHeading = np.arctan2(windU, windV) * (180 / np.pi) % 360
-        windDirection = (windHeading - 180) % 360
+        wind_speed = np.sqrt(wind_u**2 + wind_v**2)
+        wind_heading = np.arctan2(wind_u, wind_v) * (180 / np.pi) % 360
+        wind_direction = (wind_heading - 180) % 360
 
         # Convert geopotential height to geometric height
-        R = self.earthRadius
+        R = self.earth_radius
         height = R * height / (R - height)
 
         # Combine all data into big array
         data_array = np.ma.column_stack(
             [
                 levels,
                 height,
                 temperature,
-                windU,
-                windV,
-                windHeading,
-                windDirection,
-                windSpeed,
+                wind_u,
+                wind_v,
+                wind_heading,
+                wind_direction,
+                wind_speed,
             ]
         )
 
         # Remove lines with masked content
         if np.any(data_array.mask):
             data_array = np.ma.compress_rows(data_array)
             warnings.warn(
                 "Some values were missing from this weather dataset, therefore, certain pressure levels were removed."
             )
-
         # Save atmospheric data
         self.pressure = Function(
             data_array[:, (1, 0)],
             inputs="Height Above Sea Level (m)",
             outputs="Pressure (Pa)",
             interpolation="linear",
         )
         self.temperature = Function(
             data_array[:, (1, 2)],
             inputs="Height Above Sea Level (m)",
             outputs="Temperature (K)",
             interpolation="linear",
         )
-        self.windDirection = Function(
+        self.wind_direction = Function(
             data_array[:, (1, 6)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
-        self.windHeading = Function(
+        self.wind_heading = Function(
             data_array[:, (1, 5)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
-        self.windSpeed = Function(
+        self.wind_speed = Function(
             data_array[:, (1, 7)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
-        self.windVelocityX = Function(
+        self.wind_velocity_x = Function(
             data_array[:, (1, 3)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
+        self.wind_velocity_y = Function(
             data_array[:, (1, 4)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
 
         # Save maximum expected height
-        self.maxExpectedHeight = max(height[0], height[-1])
+        self.max_expected_height = max(height[0], height[-1])
 
         # Get elevation data from file
         if dictionary["surface_geopotential_height"] is not None:
             try:
-                elevations = weatherData.variables[
+                elevations = weather_data.variables[
                     dictionary["surface_geopotential_height"]
-                ][timeIndex, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)]
+                ][time_index, (lat_index - 1, lat_index), (lon_index - 1, lon_index)]
                 f_x1_y1 = elevations[0, 0]
                 f_x1_y2 = elevations[0, 1]
                 f_x2_y1 = elevations[1, 0]
                 f_x2_y2 = elevations[1, 1]
                 f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + (
                     (x - x1) / (x2 - x1)
                 ) * f_x2_y1
@@ -2041,49 +2320,50 @@
                 ) * f_x_y2
             except:
                 raise ValueError(
                     "Unable to read surface elevation data. Check file and dictionary."
                 )
 
         # Compute info data
-        self.atmosphericModelInitDate = netCDF4.num2date(
-            timeArray[0], timeArray.units, calendar="gregorian"
+        self.atmospheric_model_init_date = netCDF4.num2date(
+            time_array[0], time_array.units, calendar="gregorian"
         )
-        self.atmosphericModelEndDate = netCDF4.num2date(
-            timeArray[-1], timeArray.units, calendar="gregorian"
+        self.atmospheric_model_end_date = netCDF4.num2date(
+            time_array[-1], time_array.units, calendar="gregorian"
         )
-        self.atmosphericModelInterval = netCDF4.num2date(
-            (timeArray[-1] - timeArray[0]) / (len(timeArray) - 1),
-            timeArray.units,
+        self.atmospheric_model_interval = netCDF4.num2date(
+            (time_array[-1] - time_array[0]) / (len(time_array) - 1),
+            time_array.units,
             calendar="gregorian",
         ).hour
-        self.atmosphericModelInitLat = latArray[0]
-        self.atmosphericModelEndLat = latArray[-1]
-        self.atmosphericModelInitLon = lonArray[0]
-        self.atmosphericModelEndLon = lonArray[-1]
+        self.atmospheric_model_init_lat = lat_array[0]
+        self.atmospheric_model_end_lat = lat_array[-1]
+        self.atmospheric_model_init_lon = lon_array[0]
+        self.atmospheric_model_end_lon = lon_array[-1]
 
         # Save debugging data
-        self.latArray = latArray
-        self.lonArray = lonArray
-        self.lonIndex = lonIndex
-        self.latIndex = latIndex
+        self.lat_array = lat_array
+        self.lon_array = lon_array
+        self.lon_index = lon_index
+        self.lat_index = lat_index
         self.geopotentials = geopotentials
-        self.windUs = windUs
-        self.windVs = windVs
+        self.wind_us = wind_us
+        self.wind_vs = wind_vs
         self.levels = levels
         self.temperatures = temperatures
-        self.timeArray = timeArray
+        self.time_array = time_array
         self.height = height
 
         # Close weather data
-        weatherData.close()
+        weather_data.close()
 
         return None
 
-    def processEnsemble(self, file, dictionary):
+    @requires_netCDF4
+    def process_ensemble(self, file, dictionary):
         """Import and process atmospheric data from weather ensembles
         given as netCDF or OPeNDAP files.
         Sets pressure, temperature, wind-u and wind-v
         profiles and surface elevation obtained from a weather
         ensemble file in netCDF format or from an OPeNDAP URL, both
         given through the file parameter. The date and location of the launch
         should already have been set through the date and
@@ -2129,204 +2409,207 @@
                                  'v_wind': 'vgrdprs'}
 
         Returns
         -------
         None
         """
         # Check if date, lat and lon are known
-        if self.date is None:
+        if self.datetime_date is None:
             raise TypeError(
                 "Please specify Date (array-like) when "
                 "initializing this Environment. "
-                "Alternatively, use the Environment.setDate"
+                "Alternatively, use the Environment.set_date"
                 " method."
             )
-        if self.lat is None:
+        if self.latitude is None:
             raise TypeError(
                 "Please specify Location (lat, lon). when "
                 "initializing this Environment. "
                 "Alternatively, use the Environment."
-                "setLocation method."
+                "set_location method."
             )
 
         # Read weather file
-        weatherData = netCDF4.Dataset(file)
+        weather_data = netCDF4.Dataset(file)
 
         # Get time, latitude and longitude data from file
-        timeArray = weatherData.variables[dictionary["time"]]
-        lonArray = weatherData.variables[dictionary["longitude"]][:].tolist()
-        latArray = weatherData.variables[dictionary["latitude"]][:].tolist()
+        time_array = weather_data.variables[dictionary["time"]]
+        lon_array = weather_data.variables[dictionary["longitude"]][:].tolist()
+        lat_array = weather_data.variables[dictionary["latitude"]][:].tolist()
 
         # Find time index
-        timeIndex = netCDF4.date2index(
-            self.date, timeArray, calendar="gregorian", select="nearest"
+        time_index = netCDF4.date2index(
+            self.datetime_date, time_array, calendar="gregorian", select="nearest"
         )
         # Convert times do dates and numbers
-        inputTimeNum = netCDF4.date2num(
-            self.date, timeArray.units, calendar="gregorian"
+        input_time_num = netCDF4.date2num(
+            self.datetime_date, time_array.units, calendar="gregorian"
         )
-        fileTimeNum = timeArray[timeIndex]
-        fileTimeDate = netCDF4.num2date(
-            timeArray[timeIndex], timeArray.units, calendar="gregorian"
+        file_time_num = time_array[time_index]
+        file_time_date = netCDF4.num2date(
+            time_array[time_index], time_array.units, calendar="gregorian"
         )
         # Check if time is inside range supplied by file
-        if timeIndex == 0 and inputTimeNum < fileTimeNum:
+        if time_index == 0 and input_time_num < file_time_num:
             raise ValueError(
                 "Chosen launch time is not available in the provided file, which starts at {:}.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
-        elif timeIndex == len(timeArray) - 1 and inputTimeNum > fileTimeNum:
+        elif time_index == len(time_array) - 1 and input_time_num > file_time_num:
             raise ValueError(
                 "Chosen launch time is not available in the provided file, which ends at {:}.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
         # Check if time is exactly equal to one in the file
-        if inputTimeNum != fileTimeNum:
+        if input_time_num != file_time_num:
             warnings.warn(
                 "Exact chosen launch time is not available in the provided file, using {:} UTC instead.".format(
-                    fileTimeDate
+                    file_time_date
                 )
             )
 
         # Find longitude index
         # Determine if file uses -180 to 180 or 0 to 360
-        if lonArray[0] < 0 or lonArray[-1] < 0:
+        if lon_array[0] < 0 or lon_array[-1] < 0:
             # Convert input to -180 - 180
-            lon = self.lon if self.lon < 180 else -180 + self.lon % 180
+            lon = (
+                self.longitude if self.longitude < 180 else -180 + self.longitude % 180
+            )
         else:
             # Convert input to 0 - 360
-            lon = self.lon % 360
+            lon = self.longitude % 360
         # Check if reversed or sorted
-        if lonArray[0] < lonArray[-1]:
-            # Deal with sorted lonArray
-            lonIndex = bisect.bisect(lonArray, lon)
-        else:
-            # Deal with reversed lonArray
-            lonArray.reverse()
-            lonIndex = len(lonArray) - bisect.bisect_left(lonArray, lon)
-            lonArray.reverse()
+        if lon_array[0] < lon_array[-1]:
+            # Deal with sorted lon_array
+            lon_index = bisect.bisect(lon_array, lon)
+        else:
+            # Deal with reversed lon_array
+            lon_array.reverse()
+            lon_index = len(lon_array) - bisect.bisect_left(lon_array, lon)
+            lon_array.reverse()
         # Take care of longitude value equal to maximum longitude in the grid
-        if lonIndex == len(lonArray) and lonArray[lonIndex - 1] == lon:
-            lonIndex = lonIndex - 1
+        if lon_index == len(lon_array) and lon_array[lon_index - 1] == lon:
+            lon_index = lon_index - 1
         # Check if longitude value is inside the grid
-        if lonIndex == 0 or lonIndex == len(lonArray):
+        if lon_index == 0 or lon_index == len(lon_array):
             raise ValueError(
                 "Longitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    lon, lonArray[0], lonArray[-1]
+                    lon, lon_array[0], lon_array[-1]
                 )
             )
 
         # Find latitude index
         # Check if reversed or sorted
-        if latArray[0] < latArray[-1]:
-            # Deal with sorted latArray
-            latIndex = bisect.bisect(latArray, self.lat)
-        else:
-            # Deal with reversed latArray
-            latArray.reverse()
-            latIndex = len(latArray) - bisect.bisect_left(latArray, self.lat)
-            latArray.reverse()
+        if lat_array[0] < lat_array[-1]:
+            # Deal with sorted lat_array
+            lat_index = bisect.bisect(lat_array, self.latitude)
+        else:
+            # Deal with reversed lat_array
+            lat_array.reverse()
+            lat_index = len(lat_array) - bisect.bisect_left(lat_array, self.latitude)
+            lat_array.reverse()
         # Take care of latitude value equal to maximum longitude in the grid
-        if latIndex == len(latArray) and latArray[latIndex - 1] == self.lat:
-            latIndex = latIndex - 1
+        if lat_index == len(lat_array) and lat_array[lat_index - 1] == self.latitude:
+            lat_index = lat_index - 1
         # Check if latitude value is inside the grid
-        if latIndex == 0 or latIndex == len(latArray):
+        if lat_index == 0 or lat_index == len(lat_array):
             raise ValueError(
                 "Latitude {:f} not inside region covered by file, which is from {:f} to {:f}.".format(
-                    self.lat, latArray[0], latArray[-1]
+                    self.latitude, lat_array[0], lat_array[-1]
                 )
             )
 
         # Get ensemble data from file
         try:
-            numMembers = len(weatherData.variables[dictionary["ensemble"]][:])
+            numMembers = len(weather_data.variables[dictionary["ensemble"]][:])
         except:
             raise ValueError(
                 "Unable to read ensemble data from file. Check file and dictionary."
             )
 
         # Get pressure level data from file
         try:
             levels = (
-                100 * weatherData.variables[dictionary["level"]][:]
+                100 * weather_data.variables[dictionary["level"]][:]
             )  # Convert mbar to Pa
         except:
             raise ValueError(
                 "Unable to read pressure levels from file. Check file and dictionary."
             )
 
         ##
-        inverseDictionary = {v: k for k, v in dictionary.items()}
-        paramDictionary = {
-            "time": timeIndex,
+        inverse_dictionary = {v: k for k, v in dictionary.items()}
+        param_dictionary = {
+            "time": time_index,
             "ensemble": range(numMembers),
             "level": range(len(levels)),
-            "latitude": (latIndex - 1, latIndex),
-            "longitude": (lonIndex - 1, lonIndex),
+            "latitude": (lat_index - 1, lat_index),
+            "longitude": (lon_index - 1, lon_index),
         }
         ##
 
         # Get geopotential data from file
         try:
-            dimensions = weatherData.variables[
+            dimensions = weather_data.variables[
                 dictionary["geopotential_height"]
             ].dimensions[:]
             params = tuple(
-                [paramDictionary[inverseDictionary[dim]] for dim in dimensions]
+                [param_dictionary[inverse_dictionary[dim]] for dim in dimensions]
             )
-            geopotentials = weatherData.variables[dictionary["geopotential_height"]][
+            geopotentials = weather_data.variables[dictionary["geopotential_height"]][
                 params
             ]
         except:
             try:
-                dimensions = weatherData.variables[
+                dimensions = weather_data.variables[
                     dictionary["geopotential"]
                 ].dimensions[:]
                 params = tuple(
-                    [paramDictionary[inverseDictionary[dim]] for dim in dimensions]
+                    [param_dictionary[inverse_dictionary[dim]] for dim in dimensions]
                 )
                 geopotentials = (
-                    weatherData.variables[dictionary["geopotential"]][params] / self.g
+                    weather_data.variables[dictionary["geopotential"]][params]
+                    / self.standard_g
                 )
             except:
                 raise ValueError(
-                    "Unable to read geopontential height"
+                    "Unable to read geopotential height"
                     " nor geopotential from file. At least"
                     " one of them is necessary. Check "
                     " file and dictionary."
                 )
 
         # Get temperature from file
         try:
-            temperatures = weatherData.variables[dictionary["temperature"]][params]
+            temperatures = weather_data.variables[dictionary["temperature"]][params]
         except:
             raise ValueError(
                 "Unable to read temperature from file. Check file and dictionary."
             )
 
         # Get wind data from file
         try:
-            windUs = weatherData.variables[dictionary["u_wind"]][params]
+            wind_us = weather_data.variables[dictionary["u_wind"]][params]
         except:
             raise ValueError(
                 "Unable to read wind-u component. Check file and dictionary."
             )
         try:
-            windVs = weatherData.variables[dictionary["v_wind"]][params]
+            wind_vs = weather_data.variables[dictionary["v_wind"]][params]
         except:
             raise ValueError(
                 "Unable to read wind-v component. Check file and dictionary."
             )
 
         # Prepare for bilinear interpolation
-        x, y = self.lat, lon
-        x1, y1 = latArray[latIndex - 1], lonArray[lonIndex - 1]
-        x2, y2 = latArray[latIndex], lonArray[lonIndex]
+        x, y = self.latitude, lon
+        x1, y1 = lat_array[lat_index - 1], lon_array[lon_index - 1]
+        x2, y2 = lat_array[lat_index], lon_array[lon_index]
 
         # Determine geopotential in lat, lon
         f_x1_y1 = geopotentials[:, :, 0, 0]
         f_x1_y2 = geopotentials[:, :, 0, 1]
         f_x2_y1 = geopotentials[:, :, 1, 0]
         f_x2_y2 = geopotentials[:, :, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
@@ -2339,60 +2622,60 @@
         f_x2_y1 = temperatures[:, :, 1, 0]
         f_x2_y2 = temperatures[:, :, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
         temperature = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind u in lat, lon
-        f_x1_y1 = windUs[:, :, 0, 0]
-        f_x1_y2 = windUs[:, :, 0, 1]
-        f_x2_y1 = windUs[:, :, 1, 0]
-        f_x2_y2 = windUs[:, :, 1, 1]
+        f_x1_y1 = wind_us[:, :, 0, 0]
+        f_x1_y2 = wind_us[:, :, 0, 1]
+        f_x2_y1 = wind_us[:, :, 1, 0]
+        f_x2_y2 = wind_us[:, :, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
-        windU = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
+        wind_u = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind v in lat, lon
-        f_x1_y1 = windVs[:, :, 0, 0]
-        f_x1_y2 = windVs[:, :, 0, 1]
-        f_x2_y1 = windVs[:, :, 1, 0]
-        f_x2_y2 = windVs[:, :, 1, 1]
+        f_x1_y1 = wind_vs[:, :, 0, 0]
+        f_x1_y2 = wind_vs[:, :, 0, 1]
+        f_x2_y1 = wind_vs[:, :, 1, 0]
+        f_x2_y2 = wind_vs[:, :, 1, 1]
         f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + ((x - x1) / (x2 - x1)) * f_x2_y1
         f_x_y2 = ((x2 - x) / (x2 - x1)) * f_x1_y2 + ((x - x1) / (x2 - x1)) * f_x2_y2
-        windV = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
+        wind_v = ((y2 - y) / (y2 - y1)) * f_x_y1 + ((y - y1) / (y2 - y1)) * f_x_y2
 
         # Determine wind speed, heading and direction
-        windSpeed = np.sqrt(windU ** 2 + windV ** 2)
-        windHeading = np.arctan2(windU, windV) * (180 / np.pi) % 360
-        windDirection = (windHeading - 180) % 360
+        wind_speed = np.sqrt(wind_u**2 + wind_v**2)
+        wind_heading = np.arctan2(wind_u, wind_v) * (180 / np.pi) % 360
+        wind_direction = (wind_heading - 180) % 360
 
         # Convert geopotential height to geometric height
-        R = self.earthRadius
+        R = self.earth_radius
         height = R * height / (R - height)
 
         # Save ensemble data
-        self.levelEnsemble = levels
-        self.heightEnsemble = height
-        self.temperatureEnsemble = temperature
-        self.windUEnsemble = windU
-        self.windVEnsemble = windV
-        self.windHeadingEnsemble = windHeading
-        self.windDirectionEnsemble = windDirection
-        self.windSpeedEnsemble = windSpeed
-        self.numEnsembleMembers = numMembers
+        self.level_ensemble = levels
+        self.height_ensemble = height
+        self.temperature_ensemble = temperature
+        self.wind_u_ensemble = wind_u
+        self.wind_v_ensemble = wind_v
+        self.wind_heading_ensemble = wind_heading
+        self.wind_direction_ensemble = wind_direction
+        self.wind_speed_ensemble = wind_speed
+        self.num_ensemble_members = numMembers
 
         # Activate default ensemble
-        self.selectEnsembleMember()
+        self.select_ensemble_member()
 
         # Get elevation data from file
         if dictionary["surface_geopotential_height"] is not None:
             try:
-                elevations = weatherData.variables[
+                elevations = weather_data.variables[
                     dictionary["surface_geopotential_height"]
-                ][timeIndex, (latIndex - 1, latIndex), (lonIndex - 1, lonIndex)]
+                ][time_index, (lat_index - 1, lat_index), (lon_index - 1, lon_index)]
                 f_x1_y1 = elevations[0, 0]
                 f_x1_y2 = elevations[0, 1]
                 f_x2_y1 = elevations[1, 0]
                 f_x2_y2 = elevations[1, 1]
                 f_x_y1 = ((x2 - x) / (x2 - x1)) * f_x1_y1 + (
                     (x - x1) / (x2 - x1)
                 ) * f_x2_y1
@@ -2404,91 +2687,91 @@
                 ) * f_x_y2
             except:
                 raise ValueError(
                     "Unable to read surface elevation data. Check file and dictionary."
                 )
 
         # Compute info data
-        self.atmosphericModelInitDate = netCDF4.num2date(
-            timeArray[0], timeArray.units, calendar="gregorian"
+        self.atmospheric_model_init_date = netCDF4.num2date(
+            time_array[0], time_array.units, calendar="gregorian"
         )
-        self.atmosphericModelEndDate = netCDF4.num2date(
-            timeArray[-1], timeArray.units, calendar="gregorian"
+        self.atmospheric_model_end_date = netCDF4.num2date(
+            time_array[-1], time_array.units, calendar="gregorian"
         )
-        self.atmosphericModelInterval = netCDF4.num2date(
-            (timeArray[-1] - timeArray[0]) / (len(timeArray) - 1),
-            timeArray.units,
+        self.atmospheric_model_interval = netCDF4.num2date(
+            (time_array[-1] - time_array[0]) / (len(time_array) - 1),
+            time_array.units,
             calendar="gregorian",
         ).hour
-        self.atmosphericModelInitLat = latArray[0]
-        self.atmosphericModelEndLat = latArray[-1]
-        self.atmosphericModelInitLon = lonArray[0]
-        self.atmosphericModelEndLon = lonArray[-1]
+        self.atmospheric_model_init_lat = lat_array[0]
+        self.atmospheric_model_end_lat = lat_array[-1]
+        self.atmospheric_model_init_lon = lon_array[0]
+        self.atmospheric_model_end_lon = lon_array[-1]
 
         # Save debugging data
-        self.latArray = latArray
-        self.lonArray = lonArray
-        self.lonIndex = lonIndex
-        self.latIndex = latIndex
+        self.lat_array = lat_array
+        self.lon_array = lon_array
+        self.lon_index = lon_index
+        self.lat_index = lat_index
         self.geopotentials = geopotentials
-        self.windUs = windUs
-        self.windVs = windVs
+        self.wind_us = wind_us
+        self.wind_vs = wind_vs
         self.levels = levels
         self.temperatures = temperatures
-        self.timeArray = timeArray
+        self.time_array = time_array
         self.height = height
 
         # Close weather data
-        weatherData.close()
+        weather_data.close()
 
         return None
 
-    def selectEnsembleMember(self, member=0):
+    def select_ensemble_member(self, member=0):
         """Activates ensemble member, meaning that all atmospheric
         variables read from the Environment instance will correspond
         to the desired ensemble member.
 
         Parameters
         ---------
         member : int
             Ensemble member to be activated. Starts from 0.
 
         Returns
         -------
         None
         """
         # Verify ensemble member
-        if member >= self.numEnsembleMembers:
+        if member >= self.num_ensemble_members:
             raise ValueError(
                 "Please choose member from 0 to {:d}".format(
-                    self.numEnsembleMembers - 1
+                    self.num_ensemble_members - 1
                 )
             )
 
         # Read ensemble member
-        levels = self.levelEnsemble[:]
-        height = self.heightEnsemble[member, :]
-        temperature = self.temperatureEnsemble[member, :]
-        windU = self.windUEnsemble[member, :]
-        windV = self.windVEnsemble[member, :]
-        windHeading = self.windHeadingEnsemble[member, :]
-        windDirection = self.windDirectionEnsemble[member, :]
-        windSpeed = self.windSpeedEnsemble[member, :]
+        levels = self.level_ensemble[:]
+        height = self.height_ensemble[member, :]
+        temperature = self.temperature_ensemble[member, :]
+        wind_u = self.wind_u_ensemble[member, :]
+        wind_v = self.wind_v_ensemble[member, :]
+        wind_heading = self.wind_heading_ensemble[member, :]
+        wind_direction = self.wind_direction_ensemble[member, :]
+        wind_speed = self.wind_speed_ensemble[member, :]
 
         # Combine all data into big array
         data_array = np.ma.column_stack(
             [
                 levels,
                 height,
                 temperature,
-                windU,
-                windV,
-                windHeading,
-                windDirection,
-                windSpeed,
+                wind_u,
+                wind_v,
+                wind_heading,
+                wind_direction,
+                wind_speed,
             ]
         )
 
         # Remove lines with masked content
         if np.any(data_array.mask):
             data_array = np.ma.compress_rows(data_array)
             warnings.warn(
@@ -2504,66 +2787,66 @@
         )
         self.temperature = Function(
             data_array[:, (1, 2)],
             inputs="Height Above Sea Level (m)",
             outputs="Temperature (K)",
             interpolation="linear",
         )
-        self.windDirection = Function(
+        self.wind_direction = Function(
             data_array[:, (1, 6)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Direction (Deg True)",
             interpolation="linear",
         )
-        self.windHeading = Function(
+        self.wind_heading = Function(
             data_array[:, (1, 5)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Heading (Deg True)",
             interpolation="linear",
         )
-        self.windSpeed = Function(
+        self.wind_speed = Function(
             data_array[:, (1, 7)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Speed (m/s)",
             interpolation="linear",
         )
-        self.windVelocityX = Function(
+        self.wind_velocity_x = Function(
             data_array[:, (1, 3)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity X (m/s)",
             interpolation="linear",
         )
-        self.windVelocityY = Function(
+        self.wind_velocity_y = Function(
             data_array[:, (1, 4)],
             inputs="Height Above Sea Level (m)",
             outputs="Wind Velocity Y (m/s)",
             interpolation="linear",
         )
 
         # Save maximum expected height
-        self.maxExpectedHeight = max(height[0], height[-1])
+        self.max_expected_height = max(height[0], height[-1])
 
         # Save ensemble member
-        self.ensembleMember = member
+        self.ensemble_member = member
 
         # Update air density
-        self.calculateDensityProfile()
+        self.calculate_density_profile()
 
         # Update speed of sound
-        self.calculateSpeedOfSoundProfile()
+        self.calculate_speed_of_sound_profile()
 
         # Update dynamic viscosity
-        self.calculateDynamicViscosity()
+        self.calculate_dynamic_viscosity()
 
         return None
 
-    def loadInternationalStandardAtmosphere(self):
+    def load_international_standard_atmosphere(self):
         """Defines the pressure and temperature profile functions set
         by ISO 2533 for the International Standard atmosphere and saves
-        them as self.pressureISA and self.temperatureISA.
+        them as self.pressure_ISA and self.temperature_ISA.
 
         Parameters
         ---------
         None
 
         Returns
         -------
@@ -2612,132 +2895,133 @@
             1.10906e2,
             6.69384e1,
             3.95639e0,
             8.86272e-2,
         ]  # in Pa
 
         # Convert geopotential height to geometric height
-        ER = self.earthRadius
+        ER = self.earth_radius
         height = [ER * H / (ER - H) for H in geopotential_height]
-        height = geopotential_height
 
         # Save international standard atmosphere temperature profile
-        self.temperatureISA = Function(
+        self.temperature_ISA = Function(
             np.column_stack([height, temperature]),
             inputs="Height Above Sea Level (m)",
             outputs="Temperature (K)",
             interpolation="linear",
         )
 
         # Get gravity and R
-        g = self.g
-        R = self.airGasConstant
+        g = self.standard_g
+        R = self.air_gas_constant
 
-        # Create function to compute pressure profile
+        # Create function to compute pressure at a given geometric height
         def pressure_function(h):
             # Convert geometric to geopotential height
             H = ER * h / (ER + h)
-            H = h
 
+            # Check if height is within bounds, return extrapolated value if not
             if H < -2000:
                 return pressure[0]
             elif H > 80000:
                 return pressure[-1]
 
             # Find layer that contains height h
             layer = bisect.bisect(geopotential_height, H) - 1
 
             # Retrieve layer base geopotential height, temp, beta and pressure
             Hb = geopotential_height[layer]
             Tb = temperature[layer]
             Pb = pressure[layer]
             B = beta[layer]
 
-            # Compute presure
+            # Compute pressure
             if B != 0:
                 P = Pb * (1 + (B / Tb) * (H - Hb)) ** (-g / (B * R))
             else:
                 T = Tb + B * (H - Hb)
                 P = Pb * np.exp(-(H - Hb) * (g / (R * T)))
 
             # Return answer
             return P
 
         # Save international standard atmosphere pressure profile
-        self.pressureISA = Function(
+        self.pressure_ISA = Function(
             pressure_function,
             inputs="Height Above Sea Level (m)",
             outputs="Pressure (Pa)",
         )
 
         return None
 
-    def calculateDensityProfile(self):
+    def calculate_density_profile(self):
         """Compute the density of the atmosphere as a function of
         height by using the formula rho = P/(RT). This function is
         automatically called whenever a new atmospheric model is set.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         """
         # Retrieve pressure P, gas constant R and temperature T
         P = self.pressure
-        R = self.airGasConstant
+        R = self.air_gas_constant
         T = self.temperature
 
         # Compute density using P/RT
         D = P / (R * T)
 
         # Set new output for the calculated density
-        D.setOutputs("Air Density (kg/m³)")
+        D.set_outputs("Air Density (kg/m³)")
 
         # Save calculated density
         self.density = D
 
         return None
 
-    def calculateSpeedOfSoundProfile(self):
+    def calculate_speed_of_sound_profile(self):
         """Compute the speed of sound in the atmosphere as a function
         of height by using the formula a = sqrt(gamma*R*T). This
         function is automatically called whenever a new atmospheric
         model is set.
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         """
         # Retrieve gas constant R and temperature T
-        R = self.airGasConstant
+        R = self.air_gas_constant
         T = self.temperature
-        G = 1.4  # Unused variable, why?
+        G = 1.4
 
         # Compute speed of sound using sqrt(gamma*R*T)
-        a = (1.4 * R * T) ** 0.5
+        a = (G * R * T) ** 0.5
 
         # Set new output for the calculated speed of sound
-        a.setOutputs("Speed of Sound (m/s)")
+        a.set_outputs("Speed of Sound (m/s)")
 
         # Save calculated speed of sound
-        self.speedOfSound = a
+        self.speed_of_sound = a
 
         return None
 
-    def calculateDynamicViscosity(self):
+    def calculate_dynamic_viscosity(self):
         """Compute the dynamic viscosity of the atmosphere as a function of
         height by using the formula given in ISO 2533 u = B*T^(1.5)/(T+S).
         This function is automatically called whenever a new atmospheric model is set.
+        Warning: This equation is invalid for very high or very low temperatures
+        and under conditions occurring at altitudes above 90 km.
 
         Parameters
         ----------
         None
 
         Returns
         -------
@@ -2748,61 +3032,62 @@
         B = 1.458e-6  # Kg/m/s/K^0.5
         S = 110.4  # K
 
         # Compute dynamic viscosity using u = B*T^(1.4)/(T+S) (See ISO2533)
         u = (B * T ** (1.5)) / (T + S)
 
         # Set new output for the calculated density
-        u.setOutputs("Dynamic Viscosity (Pa s)")
+        u.set_outputs("Dynamic Viscosity (Pa s)")
 
         # Save calculated density
-        self.dynamicViscosity = u
+        self.dynamic_viscosity = u
 
         return None
 
-    def addWindGust(self, windGustX, windGustY):
+    def add_wind_gust(self, wind_gust_x, wind_gust_y):
         """Adds a function to the current stored wind profile, in order to
         simulate a wind gust.
 
         Parameters
         ----------
-        windGustX : float, callable
+        wind_gust_x : float, callable
             Callable, function of altitude, which will be added to the
             x velocity of the current stored wind profile. If float is given,
             it will be considered as a constant function in altitude.
-        windGustY : float, callable
+        wind_gust_y : float, callable
             Callable, function of altitude, which will be added to the
             y velocity of the current stored wind profile. If float is given,
             it will be considered as a constant function in altitude.
 
         Returns
         -------
         None
         """
-        # Recalculate windVelocityX and windVelocityY
-        self.windVelocityX = self.windVelocityX + windGustX
-        self.windVelocityY = self.windVelocityY + windGustY
-
-        # Reset windVelocityX and windVelocityY details
-        self.windVelocityX.setInputs("Height (m)")
-        self.windVelocityX.setOutputs("Wind Velocity X (m/s)")
-        self.windVelocityY.setInputs("Height (m)")
-        self.windVelocityY.setOutputs("Wind Velocity Y (m/s)")
+        # Recalculate wind_velocity_x and wind_velocity_y
+        self.wind_velocity_x = self.wind_velocity_x + wind_gust_x
+        self.wind_velocity_y = self.wind_velocity_y + wind_gust_y
+
+        # Reset wind_velocity_x and wind_velocity_y details
+        self.wind_velocity_x.set_inputs("Height (m)")
+        self.wind_velocity_x.set_outputs("Wind Velocity X (m/s)")
+        self.wind_velocity_y.set_inputs("Height (m)")
+        self.wind_velocity_y.set_outputs("Wind Velocity Y (m/s)")
 
         # Reset wind heading and velocity magnitude
-        self.windHeading = Function(
+        self.wind_heading = Function(
             lambda h: (180 / np.pi)
-            * np.arctan2(self.windVelocityX(h), self.windVelocityY(h))
+            * np.arctan2(self.wind_velocity_x(h), self.wind_velocity_y(h))
             % 360,
             "Height (m)",
             "Wind Heading (degrees)",
             extrapolation="constant",
         )
-        self.windSpeed = Function(
-            lambda h: (self.windVelocityX(h) ** 2 + self.windVelocityY(h) ** 2) ** 0.5,
+        self.wind_speed = Function(
+            lambda h: (self.wind_velocity_x(h) ** 2 + self.wind_velocity_y(h) ** 2)
+            ** 0.5,
             "Height (m)",
             "Wind Speed (m/s)",
             extrapolation="constant",
         )
 
         return None
 
@@ -2814,390 +3099,271 @@
         ----------
         None
 
         Return
         ------
         None
         """
-        # Print launch site details
-        print("Launch Site Details")
-        print("\nLaunch Rail Length: ", self.rL, " m")
-        if self.date != None:
-            print("Launch Date: ", self.date, " UTC")
-        if self.lat != None and self.lon != None:
-            print("Launch Site Latitude: {:.5f}°".format(self.lat))
-            print("Launch Site Longitude: {:.5f}°".format(self.lon))
-        print("Reference Datum: " + self.datum)
-        print(
-            "Launch Site UTM coordinates: {:.2f} ".format(self.initialEast)
-            + self.initialEW
-            + "    {:.2f} ".format(self.initialNorth)
-            + self.initialHemisphere
-        )
-        print("Launch Site UTM zone:", str(self.initialUtmZone) + self.initialUtmLetter)
-        print("Launch Site Surface Elevation: {:.1f} m".format(self.elevation))
-
-        # Print atmospheric model details
-        print("\n\nAtmospheric Model Details")
-        modelType = self.atmosphericModelType
-        print("\nAtmospheric Model Type: ", modelType)
-        print(
-            modelType
-            + " Maximum Height: {:.3f} km".format(self.maxExpectedHeight / 1000)
-        )
-        if modelType in ["Forecast", "Reanalysis", "Ensemble"]:
-            # Determine time period
-            initDate = self.atmosphericModelInitDate
-            endDate = self.atmosphericModelEndDate
-            interval = self.atmosphericModelInterval
-            print(modelType + " Time Period: From ", initDate, " to ", endDate, " UTC")
-            print(modelType + " Hour Interval: ", interval, " hrs")
-            # Determine latitude and longitude range
-            initLat = self.atmosphericModelInitLat
-            endLat = self.atmosphericModelEndLat
-            initLon = self.atmosphericModelInitLon
-            endLon = self.atmosphericModelEndLon
-            print(modelType + " Latitude Range: From ", initLat, "° To ", endLat, "°")
-            print(modelType + " Longitude Range: From ", initLon, "° To ", endLon, "°")
-        if modelType == "Ensemble":
-            print("Number of Ensemble Members: ", self.numEnsembleMembers)
-            print("Selected Ensemble Member: ", self.ensembleMember, " (Starts from 0)")
-
-        # Print atmospheric conditions
-        print("\n\nSurface Atmospheric Conditions")
-        print("\nSurface Wind Speed: {:.2f} m/s".format(self.windSpeed(self.elevation)))
-        print(
-            "Surface Wind Direction: {:.2f}°".format(self.windDirection(self.elevation))
-        )
-        print("Surface Wind Heading: {:.2f}°".format(self.windHeading(self.elevation)))
-        print(
-            "Surface Pressure: {:.2f} hPa".format(self.pressure(self.elevation) / 100)
-        )
-        print("Surface Temperature: {:.2f} K".format(self.temperature(self.elevation)))
-        print("Surface Air Density: {:.3f} kg/m³".format(self.density(self.elevation)))
-        print(
-            "Surface Speed of Sound: {:.2f} m/s".format(
-                self.speedOfSound(self.elevation)
-            )
-        )
-
-        # Plot graphs
-        print("\n\nAtmospheric Model Plots")
-        # Create height grid
-        grid = np.linspace(self.elevation, self.maxExpectedHeight)
-
-        # Create figure
-        plt.figure(figsize=(9, 4.5))
-
-        # Create wind speed and wind direction subplot
-        ax1 = plt.subplot(121)
-        ax1.plot(
-            [self.windSpeed(i) for i in grid], grid, "#ff7f0e", label="Speed of Sound"
-        )
-        ax1.set_xlabel("Wind Speed (m/s)", color="#ff7f0e")
-        ax1.tick_params("x", colors="#ff7f0e")
-        ax1up = ax1.twiny()
-        ax1up.plot(
-            [self.windDirection(i) for i in grid],
-            grid,
-            color="#1f77b4",
-            label="Density",
-        )
-        ax1up.set_xlabel("Wind Direction (°)", color="#1f77b4")
-        ax1up.tick_params("x", colors="#1f77b4")
-        ax1up.set_xlim(0, 360)
-        ax1.set_ylabel("Height Above Sea Level (m)")
-        ax1.grid(True)
-
-        # Create density and speed of sound subplot
-        ax2 = plt.subplot(122)
-        ax2.plot(
-            [self.speedOfSound(i) for i in grid],
-            grid,
-            "#ff7f0e",
-            label="Speed of Sound",
-        )
-        ax2.set_xlabel("Speed of Sound (m/s)", color="#ff7f0e")
-        ax2.tick_params("x", colors="#ff7f0e")
-        ax2up = ax2.twiny()
-        ax2up.plot(
-            [self.density(i) for i in grid], grid, color="#1f77b4", label="Density"
-        )
-        ax2up.set_xlabel("Density (kg/m³)", color="#1f77b4")
-        ax2up.tick_params("x", colors="#1f77b4")
-        ax2.set_ylabel("Height Above Sea Level (m)")
-        ax2.grid(True)
 
-        plt.subplots_adjust(wspace=0.5)
-        plt.show()
+        self.prints.all()
+        self.plots.info()
+        return None
 
-    def allInfo(self):
+    def all_info(self):
         """Prints out all data and graphs available about the Environment.
 
         Parameters
         ----------
         None
 
         Return
         ------
         None
         """
-        # Print gravity details
-        print("Gravity Details")
-        print("\nAcceleration of Gravity: " + str(self.g) + " m/s²")
-
-        # Print launch site details
-        print("\n\nLaunch Site Details")
-        print("\nLaunch Rail Length: ", self.rL, " m")
-        if self.date != None:
-            print("Launch Date: ", self.date, " UTC")
-        if self.lat != None and self.lon != None:
-            print("Launch Site Latitude: {:.5f}°".format(self.lat))
-            print("Launch Site Longitude: {:.5f}°".format(self.lon))
-        print("Launch Site Surface Elevation: {:.1f} m".format(self.elevation))
-
-        # Print atmospheric model details
-        print("\n\nAtmospheric Model Details")
-        modelType = self.atmosphericModelType
-        print("\nAtmospheric Model Type: ", modelType)
-        print(
-            modelType
-            + " Maximum Height: {:.3f} km".format(self.maxExpectedHeight / 1000)
-        )
-        if modelType in ["Forecast", "Reanalysis", "Ensemble"]:
-            # Determine time period
-            initDate = self.atmosphericModelInitDate
-            endDate = self.atmosphericModelEndDate
-            interval = self.atmosphericModelInterval
-            print(modelType + " Time Period: From ", initDate, " to ", endDate, " UTC")
-            print(modelType + " Hour Interval: ", interval, " hrs")
-            # Determine latitude and longitude range
-            initLat = self.atmosphericModelInitLat
-            endLat = self.atmosphericModelEndLat
-            initLon = self.atmosphericModelInitLon
-            endLon = self.atmosphericModelEndLon
-            print(modelType + " Latitude Range: From ", initLat, "° To ", endLat, "°")
-            print(modelType + " Longitude Range: From ", initLon, "° To ", endLon, "°")
-        if modelType == "Ensemble":
-            print("Number of Ensemble Members: ", self.numEnsembleMembers)
-            print("Selected Ensemble Member: ", self.ensembleMember, " (Starts from 0)")
-
-        # Print atmospheric conditions
-        print("\n\nSurface Atmospheric Conditions")
-        print("\nSurface Wind Speed: {:.2f} m/s".format(self.windSpeed(self.elevation)))
-        print(
-            "Surface Wind Direction: {:.2f}°".format(self.windDirection(self.elevation))
-        )
-        print("Surface Wind Heading: {:.2f}°".format(self.windHeading(self.elevation)))
-        print(
-            "Surface Pressure: {:.2f} hPa".format(self.pressure(self.elevation) / 100)
-        )
-        print("Surface Temperature: {:.2f} K".format(self.temperature(self.elevation)))
-        print("Surface Air Density: {:.3f} kg/m³".format(self.density(self.elevation)))
-        print(
-            "Surface Speed of Sound: {:.2f} m/s".format(
-                self.speedOfSound(self.elevation)
-            )
-        )
-
-        # Plot graphs
-        print("\n\nAtmospheric Model Plots")
-        # Create height grid
-        grid = np.linspace(self.elevation, self.maxExpectedHeight)
-
-        # Create figure
-        plt.figure(figsize=(9, 9))
-
-        # Create wind speed and wind direction subplot
-        ax1 = plt.subplot(221)
-        ax1.plot(
-            [self.windSpeed(i) for i in grid], grid, "#ff7f0e", label="Speed of Sound"
-        )
-        ax1.set_xlabel("Wind Speed (m/s)", color="#ff7f0e")
-        ax1.tick_params("x", colors="#ff7f0e")
-        ax1up = ax1.twiny()
-        ax1up.plot(
-            [self.windDirection(i) for i in grid],
-            grid,
-            color="#1f77b4",
-            label="Density",
-        )
-        ax1up.set_xlabel("Wind Direction (°)", color="#1f77b4")
-        ax1up.tick_params("x", colors="#1f77b4")
-        ax1up.set_xlim(0, 360)
-        ax1.set_ylabel("Height Above Sea Level (m)")
-        ax1.grid(True)
-
-        # Create density and speed of sound subplot
-        ax2 = plt.subplot(222)
-        ax2.plot(
-            [self.speedOfSound(i) for i in grid],
-            grid,
-            "#ff7f0e",
-            label="Speed of Sound",
-        )
-        ax2.set_xlabel("Speed of Sound (m/s)", color="#ff7f0e")
-        ax2.tick_params("x", colors="#ff7f0e")
-        ax2up = ax2.twiny()
-        ax2up.plot(
-            [self.density(i) for i in grid], grid, color="#1f77b4", label="Density"
-        )
-        ax2up.set_xlabel("Density (kg/m³)", color="#1f77b4")
-        ax2up.tick_params("x", colors="#1f77b4")
-        ax2.set_ylabel("Height Above Sea Level (m)")
-        ax2.grid(True)
-
-        # Create wind u and wind v subplot
-        ax3 = plt.subplot(223)
-        ax3.plot([self.windVelocityX(i) for i in grid], grid, label="Wind U")
-        ax3.plot([self.windVelocityY(i) for i in grid], grid, label="Wind V")
-        ax3.legend(loc="best").set_draggable(True)
-        ax3.set_ylabel("Height Above Sea Level (m)")
-        ax3.set_xlabel("Wind Speed (m/s)")
-        ax3.grid(True)
-
-        # Create pressure and temperature subplot
-        ax4 = plt.subplot(224)
-        ax4.plot(
-            [self.pressure(i) / 100 for i in grid], grid, "#ff7f0e", label="Pressure"
-        )
-        ax4.set_xlabel("Pressure (hPa)", color="#ff7f0e")
-        ax4.tick_params("x", colors="#ff7f0e")
-        ax4up = ax4.twiny()
-        ax4up.plot(
-            [self.temperature(i) for i in grid],
-            grid,
-            color="#1f77b4",
-            label="Temperature",
-        )
-        ax4up.set_xlabel("Temperature (K)", color="#1f77b4")
-        ax4up.tick_params("x", colors="#1f77b4")
-        ax4.set_ylabel("Height Above Sea Level (m)")
-        ax4.grid(True)
 
-        plt.subplots_adjust(wspace=0.5, hspace=0.3)
-        plt.show()
+        self.prints.all()
+        self.plots.all()
 
-        # Plot ensemble member comparison
-        if self.atmosphericModelType != "Ensemble":
-            return None
+        return None
 
-        print("\n\nEnsemble Members Comparison")
-        currentMember = self.ensembleMember
+    def all_plot_info_returned(self):
+        """Returns a dictionary with all plot information available about the Environment.
 
-        # Create figure
-        plt.figure(figsize=(9, 13.5))
+        Parameters
+        ----------
+        None
 
-        # Create wind u subplot
-        ax5 = plt.subplot(321)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax5.plot([self.windVelocityX(i) for i in grid], grid, label=i)
-        # ax5.legend(loc='best').set_draggable(True)
-        ax5.set_ylabel("Height Above Sea Level (m)")
-        ax5.set_xlabel("Wind Speed (m/s)")
-        ax5.set_title("Wind U - Ensemble Members")
-        ax5.grid(True)
-
-        # Create wind v subplot
-        ax6 = plt.subplot(322)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax6.plot([self.windVelocityY(i) for i in grid], grid, label=i)
-        # ax6.legend(loc='best').set_draggable(True)
-        ax6.set_ylabel("Height Above Sea Level (m)")
-        ax6.set_xlabel("Wind Speed (m/s)")
-        ax6.set_title("Wind V - Ensemble Members")
-        ax6.grid(True)
-
-        # Create wind speed subplot
-        ax7 = plt.subplot(323)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax7.plot([self.windSpeed(i) for i in grid], grid, label=i)
-        # ax7.legend(loc='best').set_draggable(True)
-        ax7.set_ylabel("Height Above Sea Level (m)")
-        ax7.set_xlabel("Wind Speed (m/s)")
-        ax7.set_title("Wind Speed Magnitude - Ensemble Members")
-        ax7.grid(True)
-
-        # Create wind direction subplot
-        ax8 = plt.subplot(324)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax8.plot([self.windDirection(i) for i in grid], grid, label=i)
-        # ax8.legend(loc='best').set_draggable(True)
-        ax8.set_ylabel("Height Above Sea Level (m)")
-        ax8.set_xlabel("Degrees True (°)")
-        ax8.set_title("Wind Direction - Ensemble Members")
-        ax8.grid(True)
-
-        # Create pressure subplot
-        ax9 = plt.subplot(325)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax9.plot([self.pressure(i) for i in grid], grid, label=i)
-        # ax9.legend(loc='best').set_draggable(True)
-        ax9.set_ylabel("Height Above Sea Level (m)")
-        ax9.set_xlabel("Pressure (P)")
-        ax9.set_title("Pressure - Ensemble Members")
-        ax9.grid(True)
-
-        # Create temperature subplot
-        ax10 = plt.subplot(326)
-        for i in range(self.numEnsembleMembers):
-            self.selectEnsembleMember(i)
-            ax10.plot([self.temperature(i) for i in grid], grid, label=i)
-        # ax10.legend(loc='best').set_draggable(True)
-        ax10.set_ylabel("Height Above Sea Level (m)")
-        ax10.set_xlabel("Temperature (K)")
-        ax10.set_title("Temperature - Ensemble Members")
-        ax10.grid(True)
-
-        # Display plot
-        plt.subplots_adjust(wspace=0.5, hspace=0.3)
-        plt.show()
+        Returns
+        ------
+        plotInfo : Dict
+            Dict of data relevant to plot externally
+        """
+        grid = np.linspace(self.elevation, self.max_expected_height)
+        plotInfo = dict(
+            grid=[i for i in grid],
+            windSpeed=[self.wind_speed(i) for i in grid],
+            windDirection=[self.wind_direction(i) for i in grid],
+            speed_of_sound=[self.speed_of_sound(i) for i in grid],
+            density=[self.density(i) for i in grid],
+            windVelX=[self.wind_velocity_x(i) for i in grid],
+            windVelY=[self.wind_velocity_y(i) for i in grid],
+            pressure=[self.pressure(i) / 100 for i in grid],
+            temperature=[self.temperature(i) for i in grid],
+        )
+        if self.atmospheric_model_type != "Ensemble":
+            return plotInfo
+        currentMember = self.ensemble_member
+        # List for each ensemble
+        plotInfo["ensembleWindVelocityX"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensembleWindVelocityX"].append(
+                [self.wind_velocity_x(i) for i in grid]
+            )
+        plotInfo["ensembleWindVelocityY"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensembleWindVelocityY"].append(
+                [self.wind_velocity_y(i) for i in grid]
+            )
+        plotInfo["ensembleWindSpeed"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensembleWindSpeed"].append([self.wind_speed(i) for i in grid])
+        plotInfo["ensembleWindDirection"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensembleWindDirection"].append(
+                [self.wind_direction(i) for i in grid]
+            )
+        plotInfo["ensemblePressure"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensemblePressure"].append([self.pressure(i) for i in grid])
+        plotInfo["ensembleTemperature"] = []
+        for i in range(self.num_ensemble_members):
+            self.select_ensemble_member(i)
+            plotInfo["ensembleTemperature"].append([self.temperature(i) for i in grid])
 
         # Clean up
-        self.selectEnsembleMember(currentMember)
+        self.select_ensemble_member(currentMember)
+        return plotInfo
+
+    def all_info_returned(self):
+        """Returns as dicts all data available about the Environment.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        ------
+        info: Dict
+            Information relevant about the Environment class.
+        """
+
+        # Dictionary creation, if not commented follows the SI
+        info = dict(
+            grav=self.gravity,
+            elevation=self.elevation,
+            modelType=self.atmospheric_model_type,
+            modelTypeMaxExpectedHeight=self.max_expected_height,
+            windSpeed=self.wind_speed(self.elevation),
+            windDirection=self.wind_direction(self.elevation),
+            windHeading=self.wind_heading(self.elevation),
+            surfacePressure=self.pressure(self.elevation) / 100,  # in hPa
+            surfaceTemperature=self.temperature(self.elevation),
+            surfaceAirDensity=self.density(self.elevation),
+            surfaceSpeedOfSound=self.speed_of_sound(self.elevation),
+        )
+        if self.datetime_date != None:
+            info["launch_date"] = self.datetime_date.strftime("%Y-%d-%m %H:%M:%S")
+        if self.latitude != None and self.longitude != None:
+            info["lat"] = self.latitude
+            info["lon"] = self.longitude
+        if info["modelType"] in ["Forecast", "Reanalysis", "Ensemble"]:
+            info["initDate"] = self.atmospheric_model_init_date.strftime(
+                "%Y-%d-%m %H:%M:%S"
+            )
+            info["endDate"] = self.atmospheric_model_end_date.strftime(
+                "%Y-%d-%m %H:%M:%S"
+            )
+            info["interval"] = self.atmospheric_model_interval
+            info["initLat"] = self.atmospheric_model_init_lat
+            info["endLat"] = self.atmospheric_model_end_lat
+            info["initLon"] = self.atmospheric_model_init_lon
+            info["endLon"] = self.atmospheric_model_end_lon
+        if info["modelType"] == "Ensemble":
+            info["numEnsembleMembers"] = self.num_ensemble_members
+            info["selectedEnsembleMember"] = self.ensemble_member
+        return info
+
+    def export_environment(self, filename="environment"):
+        """Export important attributes of Environment class to a .json file,
+        saving all the information needed to recreate the same environment using
+        customAtmosphere.
+
+        Parameters
+        ----------
+        filename
+
+        Return
+        ------
+        None
+        """
+
+        try:
+            atmospheric_model_file = self.atmospheric_model_file
+            atmospheric_model_dict = self.atmospheric_model_dict
+        except AttributeError:
+            atmospheric_model_file = ""
+            atmospheric_model_dict = ""
+
+        self.exportEnvDictionary = {
+            "gravity": self.gravity(self.elevation),
+            "date": [
+                self.datetime_date.year,
+                self.datetime_date.month,
+                self.datetime_date.day,
+                self.datetime_date.hour,
+            ],
+            "latitude": self.latitude,
+            "longitude": self.longitude,
+            "elevation": self.elevation,
+            "datum": self.datum,
+            "timezone": self.timezone,
+            "max_expected_height": float(self.max_expected_height),
+            "atmospheric_model_type": self.atmospheric_model_type,
+            "atmospheric_model_file": atmospheric_model_file,
+            "atmospheric_model_dict": atmospheric_model_dict,
+            "atmosphericModelPressureProfile": ma.getdata(
+                self.pressure.get_source()
+            ).tolist(),
+            "atmosphericModelTemperatureProfile": ma.getdata(
+                self.temperature.get_source()
+            ).tolist(),
+            "atmosphericModelWindVelocityXProfile": ma.getdata(
+                self.wind_velocity_x.get_source()
+            ).tolist(),
+            "atmosphericModelWindVelocityYProfile": ma.getdata(
+                self.wind_velocity_y.get_source()
+            ).tolist(),
+        }
+
+        f = open(filename + ".json", "w")
+
+        # write json object to file
+        f.write(
+            json.dumps(self.exportEnvDictionary, sort_keys=False, indent=4, default=str)
+        )
+
+        # close file
+        f.close()
+        print("Your Environment file was saved, check it out: " + filename + ".json")
+        print(
+            "You can use it in the future by using the customAtmosphere atmospheric model."
+        )
 
         return None
 
+    def set_earth_geometry(self, datum):
+        """Sets the Earth geometry for the Environment class based on the
+        datum provided.
+
+        Parameters
+        ----------
+        datum: str
+            The datum to be used for the Earth geometry.
+
+        Returns
+        -------
+        earthGeometry: namedtuple
+            The namedtuple containing the Earth geometry.
+        """
+        geodesy = namedtuple("earthGeometry", "semi_major_axis flattening")
+        ellipsoid = {
+            "SIRGAS2000": geodesy(6378137.0, 1 / 298.257223563),
+            "SAD69": geodesy(6378160.0, 1 / 298.25),
+            "NAD83": geodesy(6378137.0, 1 / 298.257024899),
+            "WGS84": geodesy(6378137.0, 1 / 298.257223563),
+        }
+        try:
+            return ellipsoid[datum]
+        except KeyError:
+            raise AttributeError(
+                f"The reference system {datum} for Earth geometry " "is not recognized."
+            )
+
     # Auxiliary functions - Geodesic Coordinates
-    def geodesicToUtm(self, lat, lon, datum):
+    def geodesic_to_utm(self, lat, lon):
         """Function which converts geodetic coordinates, i.e. lat/lon, to UTM
         projection coordinates. Can be used only for latitudes between -80.00°
         and 84.00°
 
         Parameters
         ----------
         lat : float
             The latitude coordinates of the point of analysis, must be contained
             between -80.00° and 84.00°
         lon : float
-            The longitude coordinates of the point of analysis, must be contained
-            between -180.00° and 180.00°
-        datum : string
-            The desired reference ellipsoide model, the following options are
-            available: "SAD69", "WGS84", "NAD83", and "SIRGAS2000". The default
-            is "SIRGAS2000", then this model will be used if the user make some
-            typing mistake
+            The longitude coordinates of the point of analysis, must be
+            contained between -180.00° and 180.00°
 
         Returns
         -------
         x: float
             East coordinate, always positive
         y:
             North coordinate, always positive
-        utmZone: int
-            The number of the UTM zone of the point of analysis, can vary between
-            1 and 60
-        utmLetter: string
-            The letter of the UTM zone of the point of analysis, can vary between
-            C and X, omitting the letters "I" and "O"
+        utm_zone: int
+            The number of the UTM zone of the point of analysis, can vary
+            between 1 and 60
+        utm_letter: string
+            The letter of the UTM zone of the point of analysis, can vary
+            between C and X, omitting the letters "I" and "O"
         hemis: string
             Returns "S" for southern hemisphere and "N" for Northern hemisphere
         EW: string
             Returns "W" for western hemisphere and "E" for eastern hemisphere
         """
 
         # Calculate the central meridian of UTM zone
@@ -3216,27 +3382,16 @@
                 lon_mc = (div * 6 + 3) * signal
                 EW = "W"
         else:
             lon_mc = 3
             EW = "W|E"
 
         # Select the desired datum (i.e. the ellipsoid parameters)
-        if datum == "SAD69":
-            semiMajorAxis = 6378160.0
-            flattening = 1 / 298.25
-        elif datum == "WGS84":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
-        elif datum == "NAD83":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257024899
-        else:
-            # SIRGAS2000
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
+        flattening = self.ellipsoid.flattening
+        semi_major_axis = self.ellipsoid.semi_major_axis
 
         # Evaluate the hemisphere and determine the N coordinate at the Equator
         if lat < 0:
             N0 = 10000000
             hemis = "S"
         else:
             N0 = 0
@@ -3245,224 +3400,196 @@
         # Convert the input lat and lon to radians
         lat = lat * np.pi / 180
         lon = lon * np.pi / 180
         lon_mc = lon_mc * np.pi / 180
 
         # Evaluate reference parameters
         K0 = 1 - 1 / 2500
-        e2 = 2 * flattening - flattening ** 2
+        e2 = 2 * flattening - flattening**2
         e2lin = e2 / (1 - e2)
 
         # Evaluate auxiliary parameters
         A = e2 * e2
         B = A * e2
         C = np.sin(2 * lat)
         D = np.sin(4 * lat)
         E = np.sin(6 * lat)
         F = (1 - e2 / 4 - 3 * A / 64 - 5 * B / 256) * lat
         G = (3 * e2 / 8 + 3 * A / 32 + 45 * B / 1024) * C
         H = (15 * A / 256 + 45 * B / 1024) * D
         I = (35 * B / 3072) * E
 
         # Evaluate other reference parameters
-        n = semiMajorAxis / ((1 - e2 * (np.sin(lat) ** 2)) ** 0.5)
+        n = semi_major_axis / ((1 - e2 * (np.sin(lat) ** 2)) ** 0.5)
         t = np.tan(lat) ** 2
         c = e2lin * (np.cos(lat) ** 2)
         ag = (lon - lon_mc) * np.cos(lat)
-        m = semiMajorAxis * (F - G + H - I)
+        m = semi_major_axis * (F - G + H - I)
 
         # Evaluate new auxiliary parameters
         J = (1 - t + c) * ag * ag * ag / 6
-        K = (5 - 18 * t + t * t + 72 * c - 58 * e2lin) * (ag ** 5) / 120
+        K = (5 - 18 * t + t * t + 72 * c - 58 * e2lin) * (ag**5) / 120
         L = (5 - t + 9 * c + 4 * c * c) * ag * ag * ag * ag / 24
-        M = (61 - 58 * t + t * t + 600 * c - 330 * e2lin) * (ag ** 6) / 720
+        M = (61 - 58 * t + t * t + 600 * c - 330 * e2lin) * (ag**6) / 720
 
         # Evaluate the final coordinates
         x = 500000 + K0 * n * (ag + J + K)
         y = N0 + K0 * (m + n * np.tan(lat) * (ag * ag / 2 + L + M))
 
         # Convert the output lat and lon to degrees
         lat = lat * 180 / np.pi
         lon = lon * 180 / np.pi
         lon_mc = lon_mc * 180 / np.pi
 
         # Calculate the UTM zone number
-        utmZone = int((lon_mc + 183) / 6)
+        utm_zone = int((lon_mc + 183) / 6)
 
         # Calculate the UTM zone letter
         letters = "CDEFGHJKLMNPQRSTUVWXX"
-        utmLetter = letters[int(80 + lat) >> 3]
+        utm_letter = letters[int(80 + lat) >> 3]
 
-        return x, y, utmZone, utmLetter, hemis, EW
+        return x, y, utm_zone, utm_letter, hemis, EW
 
-    def utmToGeodesic(self, x, y, utmZone, hemis, datum):
+    def utm_to_geodesic(self, x, y, utm_zone, hemis):
         """Function to convert UTM coordinates to geodesic coordinates
         (i.e. latitude and longitude). The latitude should be between -80°
         and 84°
 
         Parameters
         ----------
         x : float
             East UTM coordinate in meters
         y : float
             North UTM coordinate in meters
-        utmZone : int
-            The number of the UTM zone of the point of analysis, can vary between
-            1 and 60
+        utm_zone : int
+            The number of the UTM zone of the point of analysis, can vary
+            between 1 and 60
         hemis : string
-            Equals to "S" for southern hemisphere and "N" for Northern hemisphere
-        datum : string
-            The desired reference ellipsoide model, the following options are
-            available: "SAD69", "WGS84", "NAD83", and "SIRGAS2000". The default
-            is "SIRGAS2000", then this model will be used if the user make some
-            typing mistake
+            Equals to "S" for southern hemisphere and "N" for Northern
+            hemisphere
 
         Returns
         -------
         lat: float
-            latitude of the analysed point
+            latitude of the analyzed point
         lon: float
-            latitude of the analysed point
+            latitude of the analyzed point
         """
 
         if hemis == "N":
             y = y + 10000000
 
         # Calculate the Central Meridian from the UTM zone number
-        centralMeridian = utmZone * 6 - 183  # degrees
+        central_meridian = utm_zone * 6 - 183  # degrees
 
         # Select the desired datum
-        if datum == "SAD69":
-            semiMajorAxis = 6378160.0
-            flattening = 1 / 298.25
-        elif datum == "WGS84":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
-        elif datum == "NAD83":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257024899
-        else:
-            # SIRGAS2000
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
+        flattening = self.ellipsoid.flattening
+        semi_major_axis = self.ellipsoid.semi_major_axis
 
         # Calculate reference values
         K0 = 1 - 1 / 2500
-        e2 = 2 * flattening - flattening ** 2
+        e2 = 2 * flattening - flattening**2
         e2lin = e2 / (1 - e2)
         e1 = (1 - (1 - e2) ** 0.5) / (1 + (1 - e2) ** 0.5)
 
         # Calculate auxiliary values
         A = e2 * e2
         B = A * e2
         C = e1 * e1
         D = e1 * C
         E = e1 * D
 
         m = (y - 10000000) / K0
-        mi = m / (semiMajorAxis * (1 - e2 / 4 - 3 * A / 64 - 5 * B / 256))
+        mi = m / (semi_major_axis * (1 - e2 / 4 - 3 * A / 64 - 5 * B / 256))
 
         # Calculate other auxiliary values
         F = (3 * e1 / 2 - 27 * D / 32) * np.sin(2 * mi)
         G = (21 * C / 16 - 55 * E / 32) * np.sin(4 * mi)
         H = (151 * D / 96) * np.sin(6 * mi)
 
         lat1 = mi + F + G + H
         c1 = e2lin * (np.cos(lat1) ** 2)
         t1 = np.tan(lat1) ** 2
-        n1 = semiMajorAxis / ((1 - e2 * (np.sin(lat1) ** 2)) ** 0.5)
+        n1 = semi_major_axis / ((1 - e2 * (np.sin(lat1) ** 2)) ** 0.5)
         quoc = (1 - e2 * np.sin(lat1) * np.sin(lat1)) ** 3
-        r1 = semiMajorAxis * (1 - e2) / (quoc ** 0.5)
+        r1 = semi_major_axis * (1 - e2) / (quoc**0.5)
         d = (x - 500000) / (n1 * K0)
 
         # Calculate other auxiliary values
         I = (5 + 3 * t1 + 10 * c1 - 4 * c1 * c1 - 9 * e2lin) * d * d * d * d / 24
         J = (
             (61 + 90 * t1 + 298 * c1 + 45 * t1 * t1 - 252 * e2lin - 3 * c1 * c1)
-            * (d ** 6)
+            * (d**6)
             / 720
         )
         K = d - (1 + 2 * t1 + c1) * d * d * d / 6
         L = (
             (5 - 2 * c1 + 28 * t1 - 3 * c1 * c1 + 8 * e2lin + 24 * t1 * t1)
-            * (d ** 5)
+            * (d**5)
             / 120
         )
 
         # Finally calculate the coordinates in lat/lot
         lat = lat1 - (n1 * np.tan(lat1) / r1) * (d * d / 2 - I + J)
-        lon = centralMeridian * np.pi / 180 + (K + L) / np.cos(lat1)
+        lon = central_meridian * np.pi / 180 + (K + L) / np.cos(lat1)
 
         # Convert final lat/lon to Degrees
         lat = lat * 180 / np.pi
         lon = lon * 180 / np.pi
 
         return lat, lon
 
-    def calculateEarthRadius(self, lat, datum):
+    def calculate_earth_radius(self, lat):
         """Simple function to calculate the Earth Radius at a specific latitude
         based on ellipsoidal reference model (datum). The earth radius here is
         assumed as the distance between the ellipsoid's center of gravity and a
         point on ellipsoid surface at the desired
         Pay attention: The ellipsoid is an approximation for the earth model and
-        will obviously output an estimate of the perfect distance between earth's
-        relief and its center of gravity.
+        will obviously output an estimate of the perfect distance between
+        earth's relief and its center of gravity.
 
         Parameters
         ----------
         lat : float
             latitude in which the Earth radius will be calculated
-        datum : string
-            The desired reference ellipsoide model, the following options are
-            available: "SAD69", "WGS84", "NAD83", and "SIRGAS2000". The default
-            is "SIRGAS2000", then this model will be used if the user make some
-            typing mistake
 
         Returns
         -------
         float:
             Earth Radius at the desired latitude in meters
         """
         # Select the desired datum (i.e. the ellipsoid parameters)
-        if datum == "SAD69":
-            semiMajorAxis = 6378160.0
-            flattening = 1 / 298.25
-        elif datum == "WGS84":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
-        elif datum == "NAD83":
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257024899
-        else:
-            # SIRGAS2000
-            semiMajorAxis = 6378137.0
-            flattening = 1 / 298.257223563
+        flattening = self.ellipsoid.flattening
+        semi_major_axis = self.ellipsoid.semi_major_axis
 
         # Calculate the semi minor axis length
-        # semiMinorAxis = semiMajorAxis - semiMajorAxis*(flattening**(-1))
-        semiMinorAxis = semiMajorAxis * (1 - flattening)
+        # semi_minor_axis = semi_major_axis - semi_major_axis*(flattening**(-1))
+        semi_minor_axis = semi_major_axis * (1 - flattening)
 
         # Convert latitude to radians
         lat = lat * np.pi / 180
 
         # Calculate the Earth Radius in meters
-        eRadius = np.sqrt(
+        e_radius = np.sqrt(
             (
-                (np.cos(lat) * (semiMajorAxis ** 2)) ** 2
-                + (np.sin(lat) * (semiMinorAxis ** 2)) ** 2
+                (np.cos(lat) * (semi_major_axis**2)) ** 2
+                + (np.sin(lat) * (semi_minor_axis**2)) ** 2
+            )
+            / (
+                (np.cos(lat) * semi_major_axis) ** 2
+                + (np.sin(lat) * semi_minor_axis) ** 2
             )
-            / ((np.cos(lat) * semiMajorAxis) ** 2 + (np.sin(lat) * semiMinorAxis) ** 2)
         )
 
-        # Convert latitude to degress
+        # Convert latitude to degrees
         lat = lat * 180 / np.pi
 
-        return eRadius
+        return e_radius
 
-    def decimalDegressToArcSeconds(self, angle):
+    def decimal_degrees_to_arc_seconds(self, angle):
         """Function to convert an angle in decimal degrees to deg/min/sec.
          Converts (°) to (° ' ")
 
         Parameters
         ----------
         angle : float
             The angle that you need convert to deg/min/sec. Must be given in
@@ -3471,15 +3598,15 @@
         Returns
         -------
         deg: float
             The degrees.
         min: float
             The arc minutes. 1 arc-minute = (1/60)*degree
         sec: float
-            The arc Seconds. 1 arc-second = (1/360)*degree
+            The arc Seconds. 1 arc-second = (1/3600)*degree
         """
 
         if angle < 0:
             signal = -1
         else:
             signal = 1
 
@@ -3487,28 +3614,7 @@
         min = abs(signal * angle - deg) * 60 // 1
         sec = abs((signal * angle - deg) * 60 - min) * 60
         # print("The angle {:f} is equals to {:.0f}º {:.0f}' {:.3f}'' ".format(
         #    angle, signal*deg, min, sec
         # ))
 
         return deg, min, sec
-
-    def printEarthDetails(self):
-        """[UNDER CONSTRUCTION]
-        Function to print information about the Earth Model used in the
-        Environment Class
-
-        """
-        # Print launch site details
-        # print("Launch Site Details")
-        # print("Launch Site Latitude: {:.5f}°".format(self.lat))
-        # print("Launch Site Longitude: {:.5f}°".format(self.lon))
-        # print("Reference Datum: " + self.datum)
-        # print("Launch Site UTM coordinates: {:.2f} ".format(self.initialEast)
-        #    + self.initialEW + "    {:.2f} ".format(self.initialNorth) + self.initialHemisphere
-        # )
-        # print("Launch Site UTM zone number: ", self.initialUtmZone)
-        # print("Launch Site Surface Elevation: {:.1f} m".format(self.elevation))
-        print("Earth Radius at Launch site: {:.1f} m".format(self.earthRadius))
-        print("Gravity acceleration at launch site: Still not implemented :(")
-
-        return None
```

### Comparing `rocketpy-0.9.9/rocketpy/Flight.py` & `rocketpy-1.0.0a1/rocketpy/Flight.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 
-__author__ = "Giovani Hidalgo Ceotto, João Lemes Gribel Soares"
-__copyright__ = "Copyright 20XX, Projeto Jupiter"
+__author__ = (
+    "Giovani Hidalgo Ceotto, Guilherme Fernandes Alves, João Lemes Gribel Soares"
+)
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __license__ = "MIT"
 
-import re
 import math
-import bisect
-import warnings
 import time
-from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
+import warnings
+from copy import deepcopy
+from functools import cached_property
 
+import matplotlib.pyplot as plt
 import numpy as np
+import simplekml
 from scipy import integrate
-from scipy import linalg
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
 
-from .Function import Function
+from .Function import Function, funcify_method
+from .plots.flight_plots import _FlightPlots
+from .prints.flight_prints import _FlightPrints
+from .tools import Matrix, Vector
 
 
 class Flight:
     """Keeps all flight information and has a method to simulate flight.
 
     Attributes
     ----------
@@ -34,67 +34,70 @@
             weather condition. See Environment class for more details.
         Flight.rocket : Rocket
             Rocket class describing rocket. See Rocket class for more
             details.
         Flight.parachutes : Parachutes
             Direct link to parachutes of the Rocket. See Rocket class
             for more details.
-        Flight.frontalSurfaceWind : float
+        Flight.frontal_surface_wind : float
             Surface wind speed in m/s aligned with the launch rail.
-        Flight.lateralSurfaceWind : float
+        Flight.lateral_surface_wind : float
             Surface wind speed in m/s perpendicular to launch rail.
 
         Helper classes:
-        Flight.flightPhases : class
+        Flight.FlightPhases : class
             Helper class to organize and manage different flight phases.
-        Flight.timeNodes : class
+        Flight.TimeNodes : class
             Helper class to manage time discretization during simulation.
 
         Helper functions:
-        Flight.timeIterator : function
+        Flight.time_iterator : function
             Helper iterator function to generate time discretization points.
 
         Helper parameters:
-        Flight.effective1RL : float
+        Flight.rail_length : float, int
+            Launch rail length in meters.
+        Flight.effective_1rl : float
             Original rail length minus the distance measured from nozzle exit
             to the upper rail button. It assumes the nozzle to be aligned with
             the beginning of the rail.
-        Flight.effective2RL : float
+        Flight.effective2rl : float
             Original rail length minus the distance measured from nozzle exit
             to the lower rail button. It assumes the nozzle to be aligned with
             the beginning of the rail.
+        Flight.name: str
+            Name of the flight.
 
 
         Numerical Integration settings:
-        Flight.maxTime : int, float
+        Flight.max_time : int, float
             Maximum simulation time allowed. Refers to physical time
             being simulated, not time taken to run simulation.
-        Flight.maxTimeStep : int, float
+        Flight.max_time_step : int, float
             Maximum time step to use during numerical integration in seconds.
-        Flight.minTimeStep : int, float
+        Flight.min_time_step : int, float
             Minimum time step to use during numerical integration in seconds.
         Flight.rtol : int, float
             Maximum relative error tolerance to be tolerated in the
             numerical integration scheme.
         Flight.atol : int, float
             Maximum absolute error tolerance to be tolerated in the
             integration scheme.
-        Flight.timeOvershoot : bool, optional
+        Flight.time_overshoot : bool, optional
             If True, decouples ODE time step from parachute trigger functions
             sampling rate. The time steps can overshoot the necessary trigger
             function evaluation points and then interpolation is used to
             calculate them and feed the triggers. Can greatly improve run
             time in some cases.
-        Flight.terminateOnApogee : bool
+        Flight.terminate_on_apogee : bool
             Whether to terminate simulation when rocket reaches apogee.
         Flight.solver : scipy.integrate.LSODA
             Scipy LSODA integration scheme.
 
         State Space Vector Definition:
-        (Only available after Flight.postProcess has been called.)
         Flight.x : Function
             Rocket's X coordinate (positive east) as a function of time.
         Flight.y : Function
             Rocket's Y coordinate (positive north) as a function of time.
         Flight.z : Function
             Rocket's z coordinate (positive up) as a function of time.
         Flight.vx : Function
@@ -119,110 +122,115 @@
             Rocket's angular velocity Omega 2 as a function of time.
             Direction 2 is in the rocket's body axis and points perpendicular
             to the rocket's axis of cylindrical symmetry and direction 1.
         Flight.w3 : Function
             Rocket's angular velocity Omega 3 as a function of time.
             Direction 3 is in the rocket's body axis and points in the
             direction of cylindrical symmetry.
+        Flight.latitude: Function
+            Rocket's latitude coordinates (positive North) as a function of time.
+            The Equator has a latitude equal to 0, by convention.
+        Flight.longitude: Function
+            Rocket's longitude coordinates (positive East) as a function of time.
+            Greenwich meridian has a longitude equal to 0, by convention.
 
         Solution attributes:
         Flight.inclination : int, float
             Launch rail inclination angle relative to ground, given in degrees.
         Flight.heading : int, float
             Launch heading angle relative to north given in degrees.
-        Flight.initialSolution : list
-            List defines initial condition - [tInit, xInit,
-            yInit, zInit, vxInit, vyInit, vzInit, e0Init, e1Init,
-            e2Init, e3Init, w1Init, w2Init, w3Init]
-        Flight.tInitial : int, float
+        Flight.initial_solution : list
+            List defines initial condition - [tInit, x_init,
+            y_init, z_init, vx_init, vy_init, vz_init, e0_init, e1_init,
+            e2_init, e3_init, w1_init, w2_init, w3_init]
+        Flight.t_initial : int, float
             Initial simulation time in seconds. Usually 0.
         Flight.solution : list
             Solution array which keeps results from each numerical
             integration.
         Flight.t : float
             Current integration time.
         Flight.y : list
             Current integration state vector u.
-        Flight.postProcessed : bool
+        Flight.post_processed : bool
             Defines if solution data has been post processed.
 
         Solution monitor attributes:
-        Flight.initialSolution : list
-            List defines initial condition - [tInit, xInit,
-            yInit, zInit, vxInit, vyInit, vzInit, e0Init, e1Init,
-            e2Init, e3Init, w1Init, w2Init, w3Init]
-        Flight.outOfRailTime : int, float
+        Flight.initial_solution : list
+            List defines initial condition - [tInit, x_init,
+            y_init, z_init, vx_init, vy_init, vz_init, e0_init, e1_init,
+            e2_init, e3_init, w1_init, w2_init, w3_init]
+        Flight.out_of_rail_time : int, float
             Time, in seconds, in which the rocket completely leaves the
             rail.
-        Flight.outOfRailState : list
+        Flight.out_of_rail_state : list
             State vector u corresponding to state when the rocket
             completely leaves the rail.
-        Flight.outOfRailVelocity : int, float
+        Flight.out_of_rail_velocity : int, float
             Velocity, in m/s, with which the rocket completely leaves the
             rail.
-        Flight.apogeeState : array
+        Flight.apogee_state : array
             State vector u corresponding to state when the rocket's
             vertical velocity is zero in the apogee.
-        Flight.apogeeTime : int, float
+        Flight.apogee_time : int, float
             Time, in seconds, in which the rocket's vertical velocity
             reaches zero in the apogee.
-        Flight.apogeeX : int, float
+        Flight.apogee_x : int, float
             X coordinate (positive east) of the center of mass of the
             rocket when it reaches apogee.
-        Flight.apogeeY : int, float
+        Flight.apogee_y : int, float
             Y coordinate (positive north) of the center of mass of the
             rocket when it reaches apogee.
         Flight.apogee : int, float
             Z coordinate, or altitude, of the center of mass of the
             rocket when it reaches apogee.
-        Flight.xImpact : int, float
+        Flight.x_impact : int, float
             X coordinate (positive east) of the center of mass of the
             rocket when it impacts ground.
-        Flight.yImpact : int, float
+        Flight.y_impact : int, float
             Y coordinate (positive east) of the center of mass of the
             rocket when it impacts ground.
-        Flight.impactVelocity : int, float
+        Flight.impact_velocity : int, float
             Velocity magnitude of the center of mass of the rocket when
             it impacts ground.
-        Flight.impactState : array
+        Flight.impact_state : array
             State vector u corresponding to state when the rocket
             impacts the ground.
-        Flight.parachuteEvents : array
+        Flight.parachute_events : array
             List that stores parachute events triggered during flight.
-        Flight.functionEvaluations : array
+        Flight.function_evaluations : array
             List that stores number of derivative function evaluations
             during numerical integration in cumulative manner.
-        Flight.functionEvaluationsPerTimeStep : array
+        Flight.function_evaluations_per_time_step : array
             List that stores number of derivative function evaluations
             per time step during numerical integration.
-        Flight.timeSteps : array
+        Flight.time_steps : array
             List of time steps taking during numerical integration in
             seconds.
-        Flight.flightPhases : Flight.FlightPhases
+        Flight.FlightPhases : Flight.FlightPhases
             Stores and manages flight phases.
 
         Solution Secondary Attributes:
-        (Only available after Flight.postProcess has been called.)
         Atmospheric:
-        Flight.windVelocityX : Function
+        Flight.wind_velocity_x : Function
             Wind velocity X (East) experienced by the rocket as a
             function of time. Can be called or accessed as array.
-        Flight.windVelocityY : Function
+        Flight.wind_velocity_y : Function
             Wind velocity Y (North) experienced by the rocket as a
             function of time. Can be called or accessed as array.
         Flight.density : Function
             Air density experienced by the rocket as a function of
             time. Can be called or accessed as array.
         Flight.pressure : Function
             Air pressure experienced by the rocket as a function of
             time. Can be called or accessed as array.
-        Flight.dynamicViscosity : Function
+        Flight.dynamic_viscosity : Function
             Air dynamic viscosity experienced by the rocket as a function of
             time. Can be called or accessed as array.
-        Flight.speedOfSound : Function
+        Flight.speed_of_sound : Function
             Speed of Sound in air experienced by the rocket as a
             function of time. Can be called or accessed as array.
 
         Kinematics:
         Flight.ax : Function
             Rocket's X (East) acceleration as a function of time, in m/s².
             Can be called or accessed as array.
@@ -246,59 +254,59 @@
             Rocket's angular acceleration Alpha 3 as a function of time.
             Direction 3 is in the rocket's body axis and points in the
             direction of cylindrical symmetry.
             Units of rad/s². Can be called or accessed as array.
         Flight.speed : Function
             Rocket velocity magnitude in m/s relative to ground as a
             function of time. Can be called or accessed as array.
-        Flight.maxSpeed : float
+        Flight.max_speed : float
             Maximum velocity magnitude in m/s reached by the rocket
             relative to ground during flight.
-        Flight.maxSpeedTime : float
+        Flight.max_speed_time : float
             Time in seconds at which rocket reaches maximum velocity
             magnitude relative to ground.
-        Flight.horizontalSpeed : Function
+        Flight.horizontal_speed : Function
             Rocket's velocity magnitude in the horizontal (North-East)
             plane in m/s as a function of time. Can be called or
             accessed as array.
-        Flight.Acceleration : Function
+        Flight.acceleration : Function
             Rocket acceleration magnitude in m/s² relative to ground as a
             function of time. Can be called or accessed as array.
-        Flight.maxAcceleration : float
+        Flight.max_acceleration : float
             Maximum acceleration magnitude in m/s² reached by the rocket
             relative to ground during flight.
-        Flight.maxAccelerationTime : float
+        Flight.max_acceleration_time : float
             Time in seconds at which rocket reaches maximum acceleration
             magnitude relative to ground.
-        Flight.pathAngle : Function
+        Flight.path_angle : Function
             Rocket's flight path angle, or the angle that the
             rocket's velocity makes with the horizontal (North-East)
             plane. Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
-        Flight.attitudeVectorX : Function
+        Flight.attitude_vector_x : Function
             Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the X
             direction (East) as a function of time.
             Can be called or accessed as array.
-        Flight.attitudeVectorY : Function
+        Flight.attitude_vector_y : Function
             Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the Y
             direction (East) as a function of time.
             Can be called or accessed as array.
-        Flight.attitudeVectorZ : Function
+        Flight.attitude_vector_z : Function
             Rocket's attitude vector, or the vector that points
             in the rocket's axis of symmetry, component in the Z
             direction (East) as a function of time.
             Can be called or accessed as array.
-        Flight.attitudeAngle : Function
+        Flight.attitude_angle : Function
             Rocket's attitude angle, or the angle that the
             rocket's axis of symmetry makes with the horizontal (North-East)
             plane. Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
-        Flight.lateralAttitudeAngle : Function
+        Flight.lateral_attitude_angle : Function
             Rocket's lateral attitude angle, or the angle that the
             rocket's axis of symmetry makes with plane defined by
             the launch rail direction and the Z (up) axis.
             Measured in degrees and expressed as a function
             of time. Can be called or accessed as array.
         Flight.phi : Function
             Rocket's Spin Euler Angle, φ, according to the 3-2-3 rotation
@@ -354,602 +362,571 @@
         Flight.M3 : Function
             Resultant moment (torque) in rockets axis due to aerodynamic
             forces and eccentricity as a function of time. Units in N*m.
             Expressed as a function of time. Can be called or accessed
             as array.
             Direction 3 is in the rocket's body axis and points in the
             direction of cylindrical symmetry.
-        Flight.aerodynamicLift : Function
+        Flight.aerodynamic_lift : Function
             Resultant force perpendicular to rockets axis due to
             aerodynamic effects as a function of time. Units in N.
             Expressed as a function of time. Can be called or accessed
             as array.
-        Flight.aerodynamicDrag : Function
+        Flight.aerodynamic_drag : Function
             Resultant force aligned with the rockets axis due to
             aerodynamic effects as a function of time. Units in N.
             Expressed as a function of time. Can be called or accessed
             as array.
-        Flight.aerodynamicBendingMoment : Function
+        Flight.aerodynamic_bending_moment : Function
             Resultant moment perpendicular to rocket's axis due to
             aerodynamic effects as a function of time. Units in N m.
             Expressed as a function of time. Can be called or accessed
             as array.
-        Flight.aerodynamicSpinMoment : Function
+        Flight.aerodynamic_spin_moment : Function
             Resultant moment aligned with the rockets axis due to
             aerodynamic effects as a function of time. Units in N m.
             Expressed as a function of time. Can be called or accessed
             as array.
-        Flight.railButton1NormalForce : Function
+        Flight.rail_button1_normal_force : Function
             Upper rail button normal force in N as a function
             of time. Can be called or accessed as array.
-        Flight.maxRailButton1NormalForce : float
+        Flight.max_rail_button1_normal_force : float
             Maximum upper rail button normal force experienced
             during rail flight phase in N.
-        Flight.railButton1ShearForce : Function
+        Flight.rail_button1_shear_force : Function
             Upper rail button shear force in N as a function
             of time. Can be called or accessed as array.
-        Flight.maxRailButton1ShearForce : float
+        Flight.max_rail_button1_shear_force : float
             Maximum upper rail button shear force experienced
             during rail flight phase in N.
-        Flight.railButton2NormalForce : Function
+        Flight.rail_button2_normal_force : Function
             Lower rail button normal force in N as a function
             of time. Can be called or accessed as array.
-        Flight.maxRailButton2NormalForce : float
+        Flight.max_rail_button2_normal_force : float
             Maximum lower rail button normal force experienced
             during rail flight phase in N.
-        Flight.railButton2ShearForce : Function
+        Flight.rail_button2_shear_force : Function
             Lower rail button shear force in N as a function
             of time. Can be called or accessed as array.
-        Flight.maxRailButton2ShearForce : float
+        Flight.max_rail_button2_shear_force : float
             Maximum lower rail button shear force experienced
             during rail flight phase in N.
-        Flight.rotationalEnergy : Function
+        Flight.rotational_energy : Function
             Rocket's rotational kinetic energy as a function of time.
             Units in J.
-        Flight.translationalEnergy : Function
+        Flight.translational_energy : Function
             Rocket's translational kinetic energy as a function of time.
             Units in J.
-        Flight.kineticEnergy : Function
+        Flight.kinetic_energy : Function
             Rocket's total kinetic energy as a function of time.
             Units in J.
-        Flight.potentialEnergy : Function
+        Flight.potential_energy : Function
             Rocket's gravitational potential energy as a function of
             time. Units in J.
-        Flight.totalEnergy : Function
+        Flight.total_energy : Function
             Rocket's total mechanical energy as a function of time.
             Units in J.
-        Flight.thrustPower : Function
+        Flight.thrust_power : Function
             Rocket's engine thrust power output as a function
             of time in Watts. Can be called or accessed as array.
-        Flight.dragPower : Function
+        Flight.drag_power : Function
             Aerodynamic drag power output as a function
             of time in Watts. Can be called or accessed as array.
 
         Stability and Control:
-        Flight.attitudeFrequencyResponse : Function
+        Flight.attitude_frequency_response : Function
             Fourier Frequency Analysis of the rocket's attitude angle.
             Expressed as the absolute vale of the magnitude as a function
             of frequency in Hz. Can be called or accessed as array.
-        Flight.omega1FrequencyResponse : Function
+        Flight.omega1_frequency_response : Function
             Fourier Frequency Analysis of the rocket's angular velocity omega 1.
             Expressed as the absolute vale of the magnitude as a function
             of frequency in Hz. Can be called or accessed as array.
-        Flight.omega2FrequencyResponse : Function
+        Flight.omega2_frequency_response : Function
             Fourier Frequency Analysis of the rocket's angular velocity omega 2.
             Expressed as the absolute vale of the magnitude as a function
             of frequency in Hz. Can be called or accessed as array.
-        Flight.omega3FrequencyResponse : Function
+        Flight.omega3_frequency_response : Function
             Fourier Frequency Analysis of the rocket's angular velocity omega 3.
             Expressed as the absolute vale of the magnitude as a function
             of frequency in Hz. Can be called or accessed as array.
 
-        Flight.staticMargin : Function
+        Flight.static_margin : Function
             Rocket's static margin during flight in calibers.
 
         Fluid Mechanics:
-        Flight.streamVelocityX : Function
+        Flight.stream_velocity_x : Function
             Freestream velocity x (East) component, in m/s, as a function of
             time. Can be called or accessed as array.
-        Flight.streamVelocityY : Function
+        Flight.stream_velocity_y : Function
             Freestream velocity y (North) component, in m/s, as a function of
             time. Can be called or accessed as array.
-        Flight.streamVelocityZ : Function
+        Flight.stream_velocity_z : Function
             Freestream velocity z (up) component, in m/s, as a function of
             time. Can be called or accessed as array.
-        Flight.freestreamSpeed : Function
+        Flight.free_stream_speed : Function
             Freestream velocity magnitude, in m/s, as a function of time.
             Can be called or accessed as array.
-        Flight.apogeeFreestreamSpeed : float
+        Flight.apogee_freestream_speed : float
             Freestream speed of the rocket at apogee in m/s.
-        Flight.MachNumber : Function
+        Flight.mach_number : Function
             Rocket's Mach number defined as its freestream speed
             divided by the speed of sound at its altitude. Expressed
             as a function of time. Can be called or accessed as array.
-        Flight.maxMachNumber : float
+        Flight.max_mach_number : float
             Rocket's maximum Mach number experienced during flight.
-        Flight.maxMachNumberTime : float
+        Flight.max_mach_number_time : float
             Time at which the rocket experiences the maximum Mach number.
-        Flight.ReynoldsNumber : Function
+        Flight.reynolds_number : Function
             Rocket's Reynolds number, using its diameter as reference
-            length and freestreamSpeed as reference velocity. Expressed
+            length and free_stream_speed as reference velocity. Expressed
             as a function of time. Can be called or accessed as array.
-        Flight.maxReynoldsNumber : float
+        Flight.max_reynolds_number : float
             Rocket's maximum Reynolds number experienced during flight.
-        Flight.maxReynoldsNumberTime : float
+        Flight.max_reynolds_number_time : float
             Time at which the rocket experiences the maximum Reynolds number.
-        Flight.dynamicPressure : Function
+        Flight.dynamic_pressure : Function
             Dynamic pressure experienced by the rocket in Pa as a function
             of time, defined by 0.5*rho*V^2, where rho is air density and V
             is the freestream speed. Can be called or accessed as array.
-        Flight.maxDynamicPressure : float
+        Flight.max_dynamic_pressure : float
             Maximum dynamic pressure, in Pa, experienced by the rocket.
-        Flight.maxDynamicPressureTime : float
+        Flight.max_dynamic_pressure_time : float
             Time at which the rocket experiences maximum dynamic pressure.
-        Flight.totalPressure : Function
+        Flight.total_pressure : Function
             Total pressure experienced by the rocket in Pa as a function
             of time. Can be called or accessed as array.
-        Flight.maxTotalPressure : float
+        Flight.max_total_pressure : float
             Maximum total pressure, in Pa, experienced by the rocket.
-        Flight.maxTotalPressureTime : float
+        Flight.max_total_pressure_time : float
             Time at which the rocket experiences maximum total pressure.
-        Flight.angleOfAttack : Function
+        Flight.angle_of_attack : Function
             Rocket's angle of attack in degrees as a function of time.
             Defined as the minimum angle between the attitude vector and
             the freestream velocity vector. Can be called or accessed as
             array.
-
-        Fin Flutter Analysis:
-        Flight.flutterMachNumber: Function
-            The freestream velocity at which begins flutter phenomenon in
-            rocket's fins. It's expressed as a function of the air pressure
-            experienced  for the rocket. Can be called or accessed as array.
-        Flight.difference: Function
-            Difference between flutterMachNumber and machNumber, as a function of time.
-        Flight.safetyFactor: Function
-            Ratio between the flutterMachNumber and machNumber, as a function of time.
     """
 
     def __init__(
         self,
         rocket,
         environment,
+        rail_length,
         inclination=80,
         heading=90,
-        initialSolution=None,
-        terminateOnApogee=False,
-        maxTime=600,
-        maxTimeStep=np.inf,
-        minTimeStep=0,
+        initial_solution=None,
+        terminate_on_apogee=False,
+        max_time=600,
+        max_time_step=np.inf,
+        min_time_step=0,
         rtol=1e-6,
         atol=6 * [1e-3] + 4 * [1e-6] + 3 * [1e-3],
-        timeOvershoot=True,
+        time_overshoot=True,
         verbose=False,
+        name="Flight",
+        equations_of_motion="standard",
     ):
         """Run a trajectory simulation.
 
         Parameters
         ----------
         rocket : Rocket
             Rocket to simulate. See help(Rocket) for more information.
         environment : Environment
             Environment to run simulation on. See help(Environment) for
             more information.
+        rail_length : int, float
+            Length in which the rocket will be attached to the rail, only
+            moving along a fixed direction, that is, the line parallel to the
+            rail. Currently, if the an initialSolution is passed, the rail
+            length is not used.
         inclination : int, float, optional
             Rail inclination angle relative to ground, given in degrees.
             Default is 80.
         heading : int, float, optional
             Heading angle relative to north given in degrees.
             Default is 90, which points in the x direction.
-        initialSolution : array, optional
+        initial_solution : array, Flight, optional
             Initial solution array to be used. Format is
-            initialSolution = [self.tInitial,
-                                xInit, yInit, zInit,
-                                vxInit, vyInit, vzInit,
-                                e0Init, e1Init, e2Init, e3Init,
-                                w1Init, w2Init, w3Init].
-            If None, the initial solution will start with all null values,
-            except for the euler parameters which will be calculated based
-            on given values of inclination and heading. Default is None.
-        terminateOnApogee : boolean, optional
+            initialSolution = [
+                self.tInitial,
+                xInit, yInit, zInit,
+                vxInit, vyInit, vzInit,
+                e0Init, e1Init, e2Init, e3Init,
+                w1Init, w2Init, w3Init
+            ].
+            If a Flight object is used, the last state vector will be used as
+            initial solution. If None, the initial solution will start with
+            all null values, except for the euler parameters which will be
+            calculated based on given values of inclination and heading.
+            Default is None.
+        terminate_on_apogee : boolean, optional
             Whether to terminate simulation when rocket reaches apogee.
             Default is False.
-        maxTime : int, float, optional
+        max_time : int, float, optional
             Maximum time in which to simulate trajectory in seconds.
-            Using this without setting a maxTimeStep may cause unexpected
+            Using this without setting a max_time_step may cause unexpected
             errors. Default is 600.
-        maxTimeStep : int, float, optional
+        max_time_step : int, float, optional
             Maximum time step to use during integration in seconds.
             Default is 0.01.
-        minTimeStep : int, float, optional
+        min_time_step : int, float, optional
             Minimum time step to use during integration in seconds.
             Default is 0.01.
         rtol : float, array, optional
             Maximum relative error tolerance to be tolerated in the
             integration scheme. Can be given as array for each
             state space variable. Default is 1e-3.
         atol : float, optional
             Maximum absolute error tolerance to be tolerated in the
             integration scheme. Can be given as array for each
             state space variable. Default is 6*[1e-3] + 4*[1e-6] + 3*[1e-3].
-        timeOvershoot : bool, optional
+        time_overshoot : bool, optional
             If True, decouples ODE time step from parachute trigger functions
             sampling rate. The time steps can overshoot the necessary trigger
             function evaluation points and then interpolation is used to
             calculate them and feed the triggers. Can greatly improve run
             time in some cases. Default is True.
         verbose : bool, optional
             If true, verbose mode is activated. Default is False.
+        name : str, optional
+            Name of the flight. Default is "Flight".
+        equations_of_motion : str, optional
+            Type of equations of motion to use. Can be "standard" or
+            "solid_propulsion". Default is "standard". Solid propulsion is a
+            more restricted set of equations of motion that only works for
+            solid propulsion rockets. Such equations were used in RocketPy v0
+            and are kept here for backwards compatibility.
 
         Returns
         -------
         None
         """
         # Fetch helper classes and functions
         FlightPhases = self.FlightPhases
         TimeNodes = self.TimeNodes
-        timeIterator = self.timeIterator
+        time_iterator = self.time_iterator
 
         # Save rocket, parachutes, environment, maximum simulation time
         # and termination events
         self.env = environment
         self.rocket = rocket
+        self.rail_length = rail_length
+        if self.rail_length <= 0:
+            raise ValueError("Rail length must be a positive value.")
         self.parachutes = self.rocket.parachutes[:]
         self.inclination = inclination
         self.heading = heading
-        self.maxTime = maxTime
-        self.maxTimeStep = maxTimeStep
-        self.minTimeStep = minTimeStep
+        self.max_time = max_time
+        self.max_time_step = max_time_step
+        self.min_time_step = min_time_step
         self.rtol = rtol
         self.atol = atol
-        self.initialSolution = initialSolution
-        self.timeOvershoot = timeOvershoot
-        self.terminateOnApogee = terminateOnApogee
-
-        # Modifying Rail Length for a better out of rail condition
-        upperRButton = max(self.rocket.railButtons[0])
-        lowerRButton = min(self.rocket.railButtons[0])
-        nozzle = self.rocket.distanceRocketNozzle
-        self.effective1RL = self.env.rL - abs(nozzle - upperRButton)
-        self.effective2RL = self.env.rL - abs(nozzle - lowerRButton)
+        self.initial_solution = initial_solution
+        self.time_overshoot = time_overshoot
+        self.terminate_on_apogee = terminate_on_apogee
+        self.name = name
+        self.equations_of_motion = equations_of_motion
 
         # Flight initialization
-        # Initialize solution monitors
-        self.outOfRailTime = 0
-        self.outOfRailState = np.array([0])
-        self.outOfRailVelocity = 0
-        self.apogeeState = np.array([0])
-        self.apogeeTime = 0
-        self.apogeeX = 0
-        self.apogeeY = 0
-        self.apogee = 0
-        self.xImpact = 0
-        self.yImpact = 0
-        self.impactVelocity = 0
-        self.impactState = np.array([0])
-        self.parachuteEvents = []
-        self.postProcessed = False
-        # Initialize solver monitors
-        self.functionEvaluations = []
-        self.functionEvaluationsPerTimeStep = []
-        self.timeSteps = []
-        # Initialize solution state
-        self.solution = []
-        if self.initialSolution is None:
-            # Initialize time and state variables
-            self.tInitial = 0
-            xInit, yInit, zInit = 0, 0, self.env.elevation
-            vxInit, vyInit, vzInit = 0, 0, 0
-            w1Init, w2Init, w3Init = 0, 0, 0
-            # Initialize attitude
-            psiInit = -heading * (np.pi / 180)  # Precession / Heading Angle
-            thetaInit = (inclination - 90) * (np.pi / 180)  # Nutation Angle
-            e0Init = np.cos(psiInit / 2) * np.cos(thetaInit / 2)
-            e1Init = np.cos(psiInit / 2) * np.sin(thetaInit / 2)
-            e2Init = np.sin(psiInit / 2) * np.sin(thetaInit / 2)
-            e3Init = np.sin(psiInit / 2) * np.cos(thetaInit / 2)
-            # Store initial conditions
-            self.initialSolution = [
-                self.tInitial,
-                xInit,
-                yInit,
-                zInit,
-                vxInit,
-                vyInit,
-                vzInit,
-                e0Init,
-                e1Init,
-                e2Init,
-                e3Init,
-                w1Init,
-                w2Init,
-                w3Init,
-            ]
-            # Set initial derivative for rail phase
-            self.initialDerivative = self.uDotRail1
-        else:
-            # Initial solution given, ignore rail phase
-            # TODO: Check if rocket is actually out of rail. Otherwise, start at rail
-            self.outOfRailState = self.initialSolution[1:]
-            self.outOfRailTime = self.initialSolution[0]
-            self.initialDerivative = self.uDot
+        self.__init_post_process_variables()
+        self.__init_solution_monitors()
+        self.__init_equations_of_motion()
+
+        # Initialize prints and plots objects
+        self.prints = _FlightPrints(self)
+        self.plots = _FlightPlots(self)
 
-        self.tInitial = self.initialSolution[0]
-        self.solution.append(self.initialSolution)
-        self.t = self.solution[-1][0]
-        self.y = self.solution[-1][1:]
-
-        # Calculate normal and lateral surface wind
-        windU = self.env.windVelocityX(self.env.elevation)
-        windV = self.env.windVelocityY(self.env.elevation)
-        headingRad = heading * np.pi / 180
-        self.frontalSurfaceWind = windU * np.sin(headingRad) + windV * np.cos(
-            headingRad
-        )
-        self.lateralSurfaceWind = -windU * np.cos(headingRad) + windV * np.sin(
-            headingRad
-        )
+        # Initialize solver monitors
+        self.__init_solver_monitors()
 
         # Create known flight phases
-        self.flightPhases = FlightPhases()
-        self.flightPhases.addPhase(self.tInitial, self.initialDerivative, clear=False)
-        self.flightPhases.addPhase(self.maxTime)
+        self.FlightPhases = FlightPhases()
+        self.FlightPhases.add_phase(
+            self.t_initial, self.initial_derivative, clear=False
+        )
+        self.FlightPhases.add_phase(self.max_time)
 
         # Simulate flight
-        for phase_index, phase in timeIterator(self.flightPhases):
+        for phase_index, phase in time_iterator(self.FlightPhases):
             # print('\nCurrent Flight Phase List')
-            # print(self.flightPhases)
+            # print(self.FlightPhases)
             # print('\n\tCurrent Flight Phase')
             # print('\tIndex: ', phase_index, ' | Phase: ', phase)
             # Determine maximum time for this flight phase
-            phase.timeBound = self.flightPhases[phase_index + 1].t
+            phase.time_bound = self.FlightPhases[phase_index + 1].t
 
             # Evaluate callbacks
             for callback in phase.callbacks:
                 callback(self)
 
             # Create solver for this flight phase
-            self.functionEvaluations.append(0)
+            self.function_evaluations.append(0)
             phase.solver = integrate.LSODA(
                 phase.derivative,
                 t0=phase.t,
-                y0=self.y,
-                t_bound=phase.timeBound,
-                min_step=self.minTimeStep,
-                max_step=self.maxTimeStep,
+                y0=self.y_sol,
+                t_bound=phase.time_bound,
+                min_step=self.min_time_step,
+                max_step=self.max_time_step,
                 rtol=self.rtol,
                 atol=self.atol,
             )
             # print('\n\tSolver Initialization Details')
-            # print('\tInitial Time: ', phase.t)
-            # print('\tInitial State: ', self.y)
-            # print('\tTime Bound: ', phase.timeBound)
-            # print('\tMin Step: ', self.minTimeStep)
-            # print('\tMax Step: ', self.maxTimeStep)
+            # print('\t_initial Time: ', phase.t)
+            # print('\t_initial State: ', self.y_sol)
+            # print('\tTime Bound: ', phase.time_bound)
+            # print('\tMin Step: ', self.min_time_step)
+            # print('\tMax Step: ', self.max_time_step)
             # print('\tTolerances: ', self.rtol, self.atol)
 
             # Initialize phase time nodes
-            phase.timeNodes = TimeNodes()
+            phase.TimeNodes = TimeNodes()
             # Add first time node to permanent list
-            phase.timeNodes.addNode(phase.t, [], [])
+            phase.TimeNodes.add_node(phase.t, [], [])
             # Add non-overshootable parachute time nodes
-            if self.timeOvershoot is False:
-                phase.timeNodes.addParachutes(self.parachutes, phase.t, phase.timeBound)
+            if self.time_overshoot is False:
+                phase.TimeNodes.add_parachutes(
+                    self.parachutes, phase.t, phase.time_bound
+                )
             # Add lst time node to permanent list
-            phase.timeNodes.addNode(phase.timeBound, [], [])
+            phase.TimeNodes.add_node(phase.time_bound, [], [])
             # Sort time nodes
-            phase.timeNodes.sort()
+            phase.TimeNodes.sort()
             # Merge equal time nodes
-            phase.timeNodes.merge()
+            phase.TimeNodes.merge()
             # Clear triggers from first time node if necessary
             if phase.clear:
-                phase.timeNodes[0].parachutes = []
-                phase.timeNodes[0].callbacks = []
+                phase.TimeNodes[0].parachutes = []
+                phase.TimeNodes[0].callbacks = []
 
             # print('\n\tPhase Time Nodes')
-            # print('\tTime Nodes Length: ', str(len(phase.timeNodes)), ' | Time Nodes Preview: ', phase.timeNodes[0:3])
+            # print('\tTime Nodes Length: ', str(len(phase.TimeNodes)), ' | Time Nodes Preview: ', phase.TimeNodes[0:3])
 
             # Iterate through time nodes
-            for node_index, node in timeIterator(phase.timeNodes):
+            for node_index, node in time_iterator(phase.TimeNodes):
                 # print('\n\t\tCurrent Time Node')
                 # print('\t\tIndex: ', node_index, ' | Time Node: ', node)
                 # Determine time bound for this time node
-                node.timeBound = phase.timeNodes[node_index + 1].t
-                phase.solver.t_bound = node.timeBound
+                node.time_bound = phase.TimeNodes[node_index + 1].t
+                phase.solver.t_bound = node.time_bound
                 phase.solver._lsoda_solver._integrator.rwork[0] = phase.solver.t_bound
                 phase.solver._lsoda_solver._integrator.call_args[
                     4
                 ] = phase.solver._lsoda_solver._integrator.rwork
                 phase.solver.status = "running"
 
                 # Feed required parachute and discrete controller triggers
                 for callback in node.callbacks:
                     callback(self)
 
                 for parachute in node.parachutes:
                     # Calculate and save pressure signal
-                    pressure = self.env.pressure.getValueOpt(self.y[2])
-                    parachute.cleanPressureSignal.append([node.t, pressure])
+                    pressure = self.env.pressure.get_value_opt(self.y_sol[2])
+                    parachute.clean_pressure_signal.append([node.t, pressure])
                     # Calculate and save noise
                     noise = parachute.noiseFunction()
                     parachute.noiseSignal.append([node.t, noise])
                     parachute.noisyPressureSignal.append([node.t, pressure + noise])
-                    if parachute.trigger(pressure + noise, self.y):
+                    # Gets height above ground level considering noise
+                    hAGL = (
+                        self.env.pressure.find_input(
+                            pressure + noise,
+                            overshootable_node.y[2],
+                        )
+                        - self.env.elevation
+                    )
+                    if parachute.trigger(pressure + noise, hAGL, self.ySol):
                         # print('\nEVENT DETECTED')
                         # print('Parachute Triggered')
                         # print('Name: ', parachute.name, ' | Lag: ', parachute.lag)
                         # Remove parachute from flight parachutes
                         self.parachutes.remove(parachute)
                         # Create flight phase for time after detection and before inflation
-                        self.flightPhases.addPhase(
-                            node.t, phase.derivative, clear=True, index=phase_index + 1
-                        )
+                        # Must only be created if parachute has any lag
+                        i = 1
+                        if parachute.lag != 0:
+                            self.FlightPhases.add_phase(
+                                node.t,
+                                phase.derivative,
+                                clear=True,
+                                index=phase_index + i,
+                            )
+                            i += 1
                         # Create flight phase for time after inflation
                         callbacks = [
-                            lambda self, parachuteCdS=parachute.CdS: setattr(
-                                self, "parachuteCdS", parachuteCdS
+                            lambda self, parachute_CdS=parachute.cd_s: setattr(
+                                self, "parachute_CdS", parachute_CdS
                             )
                         ]
-                        self.flightPhases.addPhase(
+                        self.FlightPhases.add_phase(
                             node.t + parachute.lag,
-                            self.uDotParachute,
+                            self.u_dot_parachute,
                             callbacks,
                             clear=False,
-                            index=phase_index + 2,
+                            index=phase_index + i,
                         )
                         # Prepare to leave loops and start new flight phase
-                        phase.timeNodes.flushAfter(node_index)
-                        phase.timeNodes.addNode(self.t, [], [])
+                        phase.TimeNodes.flush_after(node_index)
+                        phase.TimeNodes.add_node(self.t, [], [])
                         phase.solver.status = "finished"
                         # Save parachute event
-                        self.parachuteEvents.append([self.t, parachute])
+                        self.parachute_events.append([self.t, parachute])
 
                 # Step through simulation
                 while phase.solver.status == "running":
                     # Step
                     phase.solver.step()
                     # Save step result
                     self.solution += [[phase.solver.t, *phase.solver.y]]
                     # Step step metrics
-                    self.functionEvaluationsPerTimeStep.append(
-                        phase.solver.nfev - self.functionEvaluations[-1]
+                    self.function_evaluations_per_time_step.append(
+                        phase.solver.nfev - self.function_evaluations[-1]
                     )
-                    self.functionEvaluations.append(phase.solver.nfev)
-                    self.timeSteps.append(phase.solver.step_size)
+                    self.function_evaluations.append(phase.solver.nfev)
+                    self.time_steps.append(phase.solver.step_size)
                     # Update time and state
                     self.t = phase.solver.t
-                    self.y = phase.solver.y
+                    self.y_sol = phase.solver.y
                     if verbose:
                         print(
                             "Current Simulation Time: {:3.4f} s".format(self.t),
                             end="\r",
                         )
                     # print('\n\t\t\tCurrent Step Details')
                     # print('\t\t\tIState: ', phase.solver._lsoda_solver._integrator.istate)
                     # print('\t\t\tTime: ', phase.solver.t)
                     # print('\t\t\tAltitude: ', phase.solver.y[2])
-                    # print('\t\t\tEvals: ', self.functionEvaluationsPerTimeStep[-1])
+                    # print('\t\t\tEvals: ', self.function_evaluations_per_time_step[-1])
 
                     # Check for first out of rail event
-                    if len(self.outOfRailState) == 1 and (
-                        self.y[0] ** 2
-                        + self.y[1] ** 2
-                        + (self.y[2] - self.env.elevation) ** 2
-                        >= self.effective1RL ** 2
+                    if len(self.out_of_rail_state) == 1 and (
+                        self.y_sol[0] ** 2
+                        + self.y_sol[1] ** 2
+                        + (self.y_sol[2] - self.env.elevation) ** 2
+                        >= self.effective_1rl**2
                     ):
                         # Rocket is out of rail
                         # Check exactly when it went out using root finding
                         # States before and after
                         # t0 -> 0
                         # print('\nEVENT DETECTED')
                         # print('Rocket is Out of Rail!')
                         # Disconsider elevation
                         self.solution[-2][3] -= self.env.elevation
                         self.solution[-1][3] -= self.env.elevation
                         # Get points
                         y0 = (
                             sum([self.solution[-2][i] ** 2 for i in [1, 2, 3]])
-                            - self.effective1RL ** 2
+                            - self.effective_1rl**2
                         )
                         yp0 = 2 * sum(
                             [
                                 self.solution[-2][i] * self.solution[-2][i + 3]
                                 for i in [1, 2, 3]
                             ]
                         )
                         t1 = self.solution[-1][0] - self.solution[-2][0]
                         y1 = (
                             sum([self.solution[-1][i] ** 2 for i in [1, 2, 3]])
-                            - self.effective1RL ** 2
+                            - self.effective_1rl**2
                         )
                         yp1 = 2 * sum(
                             [
                                 self.solution[-1][i] * self.solution[-1][i + 3]
                                 for i in [1, 2, 3]
                             ]
                         )
                         # Put elevation back
                         self.solution[-2][3] += self.env.elevation
                         self.solution[-1][3] += self.env.elevation
                         # Cubic Hermite interpolation (ax**3 + bx**2 + cx + d)
                         D = float(phase.solver.step_size)
                         d = float(y0)
                         c = float(yp0)
-                        b = float((3 * y1 - yp1 * D - 2 * c * D - 3 * d) / (D ** 2))
-                        a = float(-(2 * y1 - yp1 * D - c * D - 2 * d) / (D ** 3)) + 1e-5
+                        b = float((3 * y1 - yp1 * D - 2 * c * D - 3 * d) / (D**2))
+                        a = float(-(2 * y1 - yp1 * D - c * D - 2 * d) / (D**3)) + 1e-5
                         # Find roots
-                        d0 = b ** 2 - 3 * a * c
-                        d1 = 2 * b ** 3 - 9 * a * b * c + 27 * d * a ** 2
-                        c1 = ((d1 + (d1 ** 2 - 4 * d0 ** 3) ** (0.5)) / 2) ** (1 / 3)
+                        d0 = b**2 - 3 * a * c
+                        d1 = 2 * b**3 - 9 * a * b * c + 27 * d * a**2
+                        c1 = ((d1 + (d1**2 - 4 * d0**3) ** (0.5)) / 2) ** (1 / 3)
                         t_roots = []
                         for k in [0, 1, 2]:
-                            c2 = c1 * (-1 / 2 + 1j * (3 ** 0.5) / 2) ** k
+                            c2 = c1 * (-1 / 2 + 1j * (3**0.5) / 2) ** k
                             t_roots.append(-(1 / (3 * a)) * (b + c2 + d0 / c2))
                         # Find correct root
                         valid_t_root = []
                         for t_root in t_roots:
                             if 0 < t_root.real < t1 and abs(t_root.imag) < 0.001:
                                 valid_t_root.append(t_root.real)
                         if len(valid_t_root) > 1:
                             raise ValueError(
                                 "Multiple roots found when solving for rail exit time."
                             )
+                        elif len(valid_t_root) == 0:
+                            raise ValueError(
+                                "No valid roots found when solving for rail exit time."
+                            )
                         # Determine final state when upper button is going out of rail
                         self.t = valid_t_root[0] + self.solution[-2][0]
                         interpolator = phase.solver.dense_output()
-                        self.y = interpolator(self.t)
-                        self.solution[-1] = [self.t, *self.y]
-                        self.outOfRailTime = self.t
-                        self.outOfRailState = self.y
-                        self.outOfRailVelocity = (
-                            self.y[3] ** 2 + self.y[4] ** 2 + self.y[5] ** 2
+                        self.y_sol = interpolator(self.t)
+                        self.solution[-1] = [self.t, *self.y_sol]
+                        self.out_of_rail_time = self.t
+                        self.out_of_rail_time_index = len(self.solution) - 1
+                        self.out_of_rail_state = self.y_sol
+                        self.out_of_rail_velocity = (
+                            self.y_sol[3] ** 2 + self.y_sol[4] ** 2 + self.y_sol[5] ** 2
                         ) ** (0.5)
                         # Create new flight phase
-                        self.flightPhases.addPhase(
-                            self.t, self.uDot, index=phase_index + 1
+                        self.FlightPhases.add_phase(
+                            self.t,
+                            self.u_dot_generalized,
+                            index=phase_index + 1,
                         )
                         # Prepare to leave loops and start new flight phase
-                        phase.timeNodes.flushAfter(node_index)
-                        phase.timeNodes.addNode(self.t, [], [])
+                        phase.TimeNodes.flush_after(node_index)
+                        phase.TimeNodes.add_node(self.t, [], [])
                         phase.solver.status = "finished"
 
                     # Check for apogee event
-                    if len(self.apogeeState) == 1 and self.y[5] < 0:
+                    if len(self.apogee_state) == 1 and self.y_sol[5] < 0:
                         # print('\nPASSIVE EVENT DETECTED')
                         # print('Rocket Has Reached Apogee!')
                         # Apogee reported
                         # Assume linear vz(t) to detect when vz = 0
                         vz0 = self.solution[-2][6]
                         t0 = self.solution[-2][0]
                         vz1 = self.solution[-1][6]
                         t1 = self.solution[-1][0]
                         t_root = -(t1 - t0) * vz0 / (vz1 - vz0) + t0
                         # Fetch state at t_root
                         interpolator = phase.solver.dense_output()
-                        self.apogeeState = interpolator(t_root)
+                        self.apogee_state = interpolator(t_root)
                         # Store apogee data
-                        self.apogeeTime = t_root
-                        self.apogeeX = self.apogeeState[0]
-                        self.apogeeY = self.apogeeState[1]
-                        self.apogee = self.apogeeState[2]
-                        if self.terminateOnApogee:
+                        self.apogee_time = t_root
+                        self.apogee_x = self.apogee_state[0]
+                        self.apogee_y = self.apogee_state[1]
+                        self.apogee = self.apogee_state[2]
+                        if self.terminate_on_apogee:
                             # print('Terminate on Apogee Activated!')
                             self.t = t_root
-                            self.tFinal = self.t
-                            self.state = self.apogeeState
+                            self.t_final = self.t
+                            self.state = self.apogee_state
                             # Roll back solution
                             self.solution[-1] = [self.t, *self.state]
                             # Set last flight phase
-                            self.flightPhases.flushAfter(phase_index)
-                            self.flightPhases.addPhase(self.t)
+                            self.FlightPhases.flush_after(phase_index)
+                            self.FlightPhases.add_phase(self.t)
                             # Prepare to leave loops and start new flight phase
-                            phase.timeNodes.flushAfter(node_index)
-                            phase.timeNodes.addNode(self.t, [], [])
+                            phase.TimeNodes.flush_after(node_index)
+                            phase.TimeNodes.add_node(self.t, [], [])
                             phase.solver.status = "finished"
                     # Check for impact event
-                    if self.y[2] < self.env.elevation:
+                    if self.y_sol[2] < self.env.elevation:
                         # print('\nPASSIVE EVENT DETECTED')
                         # print('Rocket Has Reached Ground!')
                         # Impact reported
                         # Check exactly when it went out using root finding
                         # States before and after
                         # t0 -> 0
                         # Disconsider elevation
@@ -964,2413 +941,2363 @@
                         # Put elevation back
                         self.solution[-2][3] += self.env.elevation
                         self.solution[-1][3] += self.env.elevation
                         # Cubic Hermite interpolation (ax**3 + bx**2 + cx + d)
                         D = float(phase.solver.step_size)
                         d = float(y0)
                         c = float(yp0)
-                        b = float((3 * y1 - yp1 * D - 2 * c * D - 3 * d) / (D ** 2))
-                        a = float(-(2 * y1 - yp1 * D - c * D - 2 * d) / (D ** 3))
+                        b = float((3 * y1 - yp1 * D - 2 * c * D - 3 * d) / (D**2))
+                        a = float(-(2 * y1 - yp1 * D - c * D - 2 * d) / (D**3))
                         # Find roots
-                        d0 = b ** 2 - 3 * a * c
-                        d1 = 2 * b ** 3 - 9 * a * b * c + 27 * d * a ** 2
-                        c1 = ((d1 + (d1 ** 2 - 4 * d0 ** 3) ** (0.5)) / 2) ** (1 / 3)
+                        d0 = b**2 - 3 * a * c
+                        d1 = 2 * b**3 - 9 * a * b * c + 27 * d * a**2
+                        c1 = ((d1 + (d1**2 - 4 * d0**3) ** (0.5)) / 2) ** (1 / 3)
                         t_roots = []
                         for k in [0, 1, 2]:
-                            c2 = c1 * (-1 / 2 + 1j * (3 ** 0.5) / 2) ** k
+                            c2 = c1 * (-1 / 2 + 1j * (3**0.5) / 2) ** k
                             t_roots.append(-(1 / (3 * a)) * (b + c2 + d0 / c2))
                         # Find correct root
                         valid_t_root = []
                         for t_root in t_roots:
                             if 0 < t_root.real < t1 and abs(t_root.imag) < 0.001:
                                 valid_t_root.append(t_root.real)
                         if len(valid_t_root) > 1:
                             raise ValueError(
                                 "Multiple roots found when solving for impact time."
                             )
                         # Determine impact state at t_root
                         self.t = valid_t_root[0] + self.solution[-2][0]
                         interpolator = phase.solver.dense_output()
-                        self.y = interpolator(self.t)
+                        self.y_sol = interpolator(self.t)
                         # Roll back solution
-                        self.solution[-1] = [self.t, *self.y]
+                        self.solution[-1] = [self.t, *self.y_sol]
                         # Save impact state
-                        self.impactState = self.y
-                        self.xImpact = self.impactState[0]
-                        self.yImpact = self.impactState[1]
-                        self.zImpact = self.impactState[2]
-                        self.impactVelocity = self.impactState[5]
-                        self.tFinal = self.t
+                        self.impact_state = self.y_sol
+                        self.x_impact = self.impact_state[0]
+                        self.y_impact = self.impact_state[1]
+                        self.zImpact = self.impact_state[2]
+                        self.impact_velocity = self.impact_state[5]
+                        self.t_final = self.t
                         # Set last flight phase
-                        self.flightPhases.flushAfter(phase_index)
-                        self.flightPhases.addPhase(self.t)
+                        self.FlightPhases.flush_after(phase_index)
+                        self.FlightPhases.add_phase(self.t)
                         # Prepare to leave loops and start new flight phase
-                        phase.timeNodes.flushAfter(node_index)
-                        phase.timeNodes.addNode(self.t, [], [])
+                        phase.TimeNodes.flush_after(node_index)
+                        phase.TimeNodes.add_node(self.t, [], [])
                         phase.solver.status = "finished"
 
                     # List and feed overshootable time nodes
-                    if self.timeOvershoot:
+                    if self.time_overshoot:
                         # Initialize phase overshootable time nodes
-                        overshootableNodes = TimeNodes()
+                        overshootable_nodes = TimeNodes()
                         # Add overshootable parachute time nodes
-                        overshootableNodes.addParachutes(
+                        overshootable_nodes.add_parachutes(
                             self.parachutes, self.solution[-2][0], self.t
                         )
                         # Add last time node (always skipped)
-                        overshootableNodes.addNode(self.t, [], [])
-                        if len(overshootableNodes) > 1:
+                        overshootable_nodes.add_node(self.t, [], [])
+                        if len(overshootable_nodes) > 1:
                             # Sort overshootable time nodes
-                            overshootableNodes.sort()
+                            overshootable_nodes.sort()
                             # Merge equal overshootable time nodes
-                            overshootableNodes.merge()
+                            overshootable_nodes.merge()
                             # Clear if necessary
-                            if overshootableNodes[0].t == phase.t and phase.clear:
-                                overshootableNodes[0].parachutes = []
-                                overshootableNodes[0].callbacks = []
+                            if overshootable_nodes[0].t == phase.t and phase.clear:
+                                overshootable_nodes[0].parachutes = []
+                                overshootable_nodes[0].callbacks = []
                             # print('\n\t\t\t\tOvershootable Time Nodes')
                             # print('\t\t\t\tInterval: ', self.solution[-2][0], self.t)
-                            # print('\t\t\t\tOvershootable Nodes Length: ', str(len(overshootableNodes)), ' | Overshootable Nodes: ', overshootableNodes)
+                            # print('\t\t\t\tOvershootable Nodes Length: ', str(len(overshootable_nodes)), ' | Overshootable Nodes: ', overshootable_nodes)
                             # Feed overshootable time nodes trigger
                             interpolator = phase.solver.dense_output()
-                            for overshootable_index, overshootableNode in timeIterator(
-                                overshootableNodes
-                            ):
+                            for (
+                                overshootable_index,
+                                overshootable_node,
+                            ) in time_iterator(overshootable_nodes):
                                 # print('\n\t\t\t\tCurrent Overshootable Node')
-                                # print('\t\t\t\tIndex: ', overshootable_index, ' | Overshootable Node: ', overshootableNode)
+                                # print('\t\t\t\tIndex: ', overshootable_index, ' | Overshootable Node: ', overshootable_node)
                                 # Calculate state at node time
-                                overshootableNode.y = interpolator(overshootableNode.t)
+                                overshootable_node.y = interpolator(
+                                    overshootable_node.t
+                                )
                                 # Calculate and save pressure signal
-                                pressure = self.env.pressure.getValueOpt(
-                                    overshootableNode.y[2]
+                                pressure = self.env.pressure.get_value_opt(
+                                    overshootable_node.y[2]
                                 )
-                                for parachute in overshootableNode.parachutes:
+                                for parachute in overshootable_node.parachutes:
                                     # Save pressure signal
-                                    parachute.cleanPressureSignal.append(
-                                        [overshootableNode.t, pressure]
+                                    parachute.clean_pressure_signal.append(
+                                        [overshootable_node.t, pressure]
                                     )
                                     # Calculate and save noise
-                                    noise = parachute.noiseFunction()
-                                    parachute.noiseSignal.append(
-                                        [overshootableNode.t, noise]
+                                    noise = parachute.noise_function()
+                                    parachute.noise_signal.append(
+                                        [overshootable_node.t, noise]
                                     )
-                                    parachute.noisyPressureSignal.append(
-                                        [overshootableNode.t, pressure + noise]
+                                    parachute.noisy_pressure_signal.append(
+                                        [overshootable_node.t, pressure + noise]
+                                    )
+                                    # Gets height above ground level considering noise
+                                    hAGL = (
+                                        self.env.pressure.find_input(
+                                            pressure + noise,
+                                            overshootable_node.y[2],
+                                        )
+                                        - self.env.elevation
                                     )
+
                                     if parachute.trigger(
-                                        pressure + noise, overshootableNode.y
+                                        pressure + noise, hAGL, overshootable_node.y
                                     ):
                                         # print('\nEVENT DETECTED')
                                         # print('Parachute Triggered')
                                         # print('Name: ', parachute.name, ' | Lag: ', parachute.lag)
                                         # Remove parachute from flight parachutes
                                         self.parachutes.remove(parachute)
                                         # Create flight phase for time after detection and before inflation
-                                        self.flightPhases.addPhase(
-                                            overshootableNode.t,
-                                            phase.derivative,
-                                            clear=True,
-                                            index=phase_index + 1,
-                                        )
+                                        # Must only be created if parachute has any lag
+                                        i = 1
+                                        if parachute.lag != 0:
+                                            self.FlightPhases.add_phase(
+                                                overshootable_node.t,
+                                                phase.derivative,
+                                                clear=True,
+                                                index=phase_index + i,
+                                            )
+                                            i += 1
                                         # Create flight phase for time after inflation
                                         callbacks = [
-                                            lambda self, parachuteCdS=parachute.CdS: setattr(
-                                                self, "parachuteCdS", parachuteCdS
+                                            lambda self, parachute_CdS=parachute.cd_s: setattr(
+                                                self, "parachute_CdS", parachute_CdS
                                             )
                                         ]
-                                        self.flightPhases.addPhase(
-                                            overshootableNode.t + parachute.lag,
-                                            self.uDotParachute,
+                                        self.FlightPhases.add_phase(
+                                            overshootable_node.t + parachute.lag,
+                                            self.u_dot_parachute,
                                             callbacks,
                                             clear=False,
-                                            index=phase_index + 2,
+                                            index=phase_index + i,
                                         )
                                         # Rollback history
-                                        self.t = overshootableNode.t
-                                        self.y = overshootableNode.y
+                                        self.t = overshootable_node.t
+                                        self.y_sol = overshootable_node.y
                                         self.solution[-1] = [
-                                            overshootableNode.t,
-                                            *overshootableNode.y,
+                                            overshootable_node.t,
+                                            *overshootable_node.y,
                                         ]
                                         # Prepare to leave loops and start new flight phase
-                                        overshootableNodes.flushAfter(
+                                        overshootable_nodes.flush_after(
                                             overshootable_index
                                         )
-                                        phase.timeNodes.flushAfter(node_index)
-                                        phase.timeNodes.addNode(self.t, [], [])
+                                        phase.TimeNodes.flush_after(node_index)
+                                        phase.TimeNodes.add_node(self.t, [], [])
                                         phase.solver.status = "finished"
                                         # Save parachute event
-                                        self.parachuteEvents.append([self.t, parachute])
+                                        self.parachute_events.append(
+                                            [self.t, parachute]
+                                        )
 
-        self.tFinal = self.t
+        self.t_final = self.t
         if verbose:
             print("Simulation Completed at Time: {:3.4f} s".format(self.t))
 
-    def uDotRail1(self, t, u, postProcessing=False):
+    def __init_post_process_variables(self):
+        """Initialize post-process variables."""
+        # Initialize all variables calculated after initialization.
+        # Important to do so that MATLAB® can access them
+        self._drift = Function(0)
+        self._bearing = Function(0)
+        self._latitude = Function(0)
+        self._longitude = Function(0)
+
+    def __init_solution_monitors(self):
+        # Initialize solution monitors
+        self.out_of_rail_time = 0
+        self.out_of_rail_time_index = 0
+        self.out_of_rail_state = np.array([0])
+        self.out_of_rail_velocity = 0
+        self.apogee_state = np.array([0])
+        self.apogee_time = 0
+        self.apogee_x = 0
+        self.apogee_y = 0
+        self.apogee = 0
+        self.x_impact = 0
+        self.y_impact = 0
+        self.impact_velocity = 0
+        self.impact_state = np.array([0])
+        self.parachute_events = []
+        self.post_processed = False
+
+        return None
+
+    def __init_flight_state(self):
+        """Initialize flight state variables."""
+        if self.initial_solution is None:
+            # Initialize time and state variables
+            self.t_initial = 0
+            x_init, y_init, z_init = 0, 0, self.env.elevation
+            vx_init, vy_init, vz_init = 0, 0, 0
+            w1_init, w2_init, w3_init = 0, 0, 0
+            # Initialize attitude
+            psi_init = -self.heading * (np.pi / 180)  # Precession / Heading Angle
+            theta_init = (self.inclination - 90) * (np.pi / 180)  # Nutation Angle
+            e0_init = np.cos(psi_init / 2) * np.cos(theta_init / 2)
+            e1_init = np.cos(psi_init / 2) * np.sin(theta_init / 2)
+            e2_init = np.sin(psi_init / 2) * np.sin(theta_init / 2)
+            e3_init = np.sin(psi_init / 2) * np.cos(theta_init / 2)
+            # Store initial conditions
+            self.initial_solution = [
+                self.t_initial,
+                x_init,
+                y_init,
+                z_init,
+                vx_init,
+                vy_init,
+                vz_init,
+                e0_init,
+                e1_init,
+                e2_init,
+                e3_init,
+                w1_init,
+                w2_init,
+                w3_init,
+            ]
+            # Set initial derivative for rail phase
+            self.initial_derivative = self.udot_rail1
+        elif isinstance(self.initial_solution, Flight):
+            # Initialize time and state variables based on last solution of
+            # previous flight
+            self.initial_solution = self.initial_solution.solution[-1]
+            # Set unused monitors
+            self.outOfRailState = self.initialSolution[1:]
+            self.out_of_rail_time = self.initialSolution[0]
+            self.out_of_rail_time_index = 0
+            # Set initial derivative for 6-DOF flight phase
+            self.initial_derivative = self.u_dot_generalized
+        else:
+            # Initial solution given, ignore rail phase
+            # TODO: Check if rocket is actually out of rail. Otherwise, start at rail
+            self.out_of_rail_state = self.initial_solution[1:]
+            self.out_of_rail_time = self.initial_solution[0]
+            self.out_of_rail_time_index = 0
+            self.initial_derivative = self.u_dot_generalized
+
+    def __init_solver_monitors(self):
+        # Initialize solver monitors
+        self.function_evaluations = []
+        self.function_evaluations_per_time_step = []
+        self.time_steps = []
+        # Initialize solution state
+        self.solution = []
+        self.__init_flight_state()
+
+        self.t_initial = self.initial_solution[0]
+        self.solution.append(self.initial_solution)
+        self.t = self.solution[-1][0]
+        self.y_sol = self.solution[-1][1:]
+
+    def __init_equations_of_motion(self):
+        """Initialize equations of motion."""
+        if self.equations_of_motion == "solid_propulsion":
+            self.u_dot_generalized = self.u_dot
+
+    def __init_equations_of_motion(self):
+        """Initialize equations of motion."""
+        if self.equations_of_motion == "solid_propulsion":
+            self.uDotGeneralized = self.uDot
+
+    @cached_property
+    def effective_1rl(self):
+        nozzle = (
+            self.rocket.motor_position - self.rocket.center_of_dry_mass_position
+        ) * self.rocket._csys  # Kinda works for single nozzle
+        try:
+            rail_buttons = self.rocket.rail_buttons[0]
+            upper_r_button = (
+                rail_buttons.component.buttons_distance + rail_buttons.position
+            )
+        except IndexError:  # No rail buttons defined
+            upper_r_button = nozzle
+        effective_1rl = self.rail_length - abs(nozzle - upper_r_button)
+        return effective_1rl
+
+    @cached_property
+    def effective_2rl(self):
+        nozzle = (
+            self.rocket.motor_position - self.rocket.center_of_dry_mass_position
+        ) * self.rocket._csys
+        try:
+            rail_buttons = self.rocket.rail_buttons[0]
+            lower_r_button = rail_buttons.position
+        except IndexError:  # No rail buttons defined
+            lower_r_button = nozzle
+        effective_2rl = self.rail_length - abs(nozzle - lower_r_button)
+        return effective_2rl
+
+    @cached_property
+    def frontal_surface_wind(self):
+        # Surface wind magnitude in the frontal direction at the rail's elevation
+        wind_u = self.env.wind_velocity_x(self.env.elevation)
+        wind_v = self.env.wind_velocity_y(self.env.elevation)
+        heading_rad = self.heading * np.pi / 180
+        frontal_surface_wind = wind_u * np.sin(heading_rad) + wind_v * np.cos(
+            heading_rad
+        )
+        return frontal_surface_wind
+
+    @cached_property
+    def lateral_surface_wind(self):
+        # Surface wind magnitude in the lateral direction at the rail's elevation
+        wind_u = self.env.wind_velocity_x(self.env.elevation)
+        wind_v = self.env.wind_velocity_y(self.env.elevation)
+        heading_rad = self.heading * np.pi / 180
+        lateral_surface_wind = -wind_u * np.cos(heading_rad) + wind_v * np.sin(
+            heading_rad
+        )
+        return lateral_surface_wind
+
+    def udot_rail1(self, t, u, post_processing=False):
         """Calculates derivative of u state vector with respect to time
         when rocket is flying in 1 DOF motion in the rail.
 
         Parameters
         ----------
         t : float
             Time in seconds
         u : list
             State vector defined by u = [x, y, z, vx, vy, vz, e0, e1,
             e2, e3, omega1, omega2, omega3].
-        postProcessing : bool, optional
+        post_processing : bool, optional
             If True, adds flight data information directly to self
             variables such as self.attackAngle. Default is False.
 
         Return
         ------
-        uDot : list
-            State vector defined by uDot = [vx, vy, vz, ax, ay, az,
-            e0Dot, e1Dot, e2Dot, e3Dot, alpha1, alpha2, alpha3].
+        u_dot : list
+            State vector defined by u_dot = [vx, vy, vz, ax, ay, az,
+            e0dot, e1dot, e2dot, e3dot, alpha1, alpha2, alpha3].
 
         """
         # Check if post processing mode is on
-        if postProcessing:
-            # Use uDot post processing code
-            return self.uDot(t, u, True)
+        if post_processing:
+            # Use u_dot post processing code
+            return self.u_dot_generalized(t, u, True)
 
         # Retrieve integration data
         x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
 
         # Retrieve important quantities
         # Mass
-        M = self.rocket.totalMass.getValueOpt(t)
+        M = self.rocket.total_mass.get_value_opt(t)
 
         # Get freestream speed
-        freestreamSpeed = (
-            (self.env.windVelocityX.getValueOpt(z) - vx) ** 2
-            + (self.env.windVelocityY.getValueOpt(z) - vy) ** 2
+        free_stream_speed = (
+            (self.env.wind_velocity_x.get_value_opt(z) - vx) ** 2
+            + (self.env.wind_velocity_y.get_value_opt(z) - vy) ** 2
             + (vz) ** 2
         ) ** 0.5
-        freestreamMach = freestreamSpeed / self.env.speedOfSound.getValueOpt(z)
-        dragCoeff = self.rocket.powerOnDrag.getValueOpt(freestreamMach)
+        free_stream_mach = free_stream_speed / self.env.speed_of_sound.get_value_opt(z)
+        drag_coeff = self.rocket.power_on_drag.get_value_opt(free_stream_mach)
 
         # Calculate Forces
-        Thrust = self.rocket.motor.thrust.getValueOpt(t)
-        rho = self.env.density.getValueOpt(z)
-        R3 = -0.5 * rho * (freestreamSpeed ** 2) * self.rocket.area * (dragCoeff)
+        thrust = self.rocket.motor.thrust.get_value_opt(t)
+        rho = self.env.density.get_value_opt(z)
+        R3 = -0.5 * rho * (free_stream_speed**2) * self.rocket.area * (drag_coeff)
 
         # Calculate Linear acceleration
-        a3 = (R3 + Thrust) / M - (e0 ** 2 - e1 ** 2 - e2 ** 2 + e3 ** 2) * self.env.g
+        a3 = (R3 + thrust) / M - (
+            e0**2 - e1**2 - e2**2 + e3**2
+        ) * self.env.gravity(z)
         if a3 > 0:
             ax = 2 * (e1 * e3 + e0 * e2) * a3
             ay = 2 * (e2 * e3 - e0 * e1) * a3
-            az = (1 - 2 * (e1 ** 2 + e2 ** 2)) * a3
+            az = (1 - 2 * (e1**2 + e2**2)) * a3
         else:
             ax, ay, az = 0, 0, 0
 
         return [vx, vy, vz, ax, ay, az, 0, 0, 0, 0, 0, 0, 0]
 
-    def uDotRail2(self, t, u, postProcessing=False):
+    def udot_rail2(self, t, u, post_processing=False):
         """[Still not implemented] Calculates derivative of u state vector with
         respect to time when rocket is flying in 3 DOF motion in the rail.
 
         Parameters
         ----------
         t : float
             Time in seconds
         u : list
             State vector defined by u = [x, y, z, vx, vy, vz, e0, e1,
             e2, e3, omega1, omega2, omega3].
-        postProcessing : bool, optional
+        post_processing : bool, optional
             If True, adds flight data information directly to self
             variables such as self.attackAngle, by default False
 
         Returns
         -------
-        uDot : list
-            State vector defined by uDot = [vx, vy, vz, ax, ay, az,
-            e0Dot, e1Dot, e2Dot, e3Dot, alpha1, alpha2, alpha3].
+        u_dot : list
+            State vector defined by u_dot = [vx, vy, vz, ax, ay, az,
+            e0dot, e1dot, e2dot, e3dot, alpha1, alpha2, alpha3].
         """
-        # Hey! We will finish this function later, now we just can use uDot
-        return self.uDot(t, u, postProcessing=postProcessing)
+        # Hey! We will finish this function later, now we just can use u_dot
+        return self.u_dot_generalized(t, u, post_processing=post_processing)
 
-    def uDot(self, t, u, postProcessing=False):
+    def u_dot(self, t, u, post_processing=False):
         """Calculates derivative of u state vector with respect to time
         when rocket is flying in 6 DOF motion during ascent out of rail
         and descent without parachute.
 
         Parameters
         ----------
         t : float
             Time in seconds
         u : list
             State vector defined by u = [x, y, z, vx, vy, vz, e0, e1,
             e2, e3, omega1, omega2, omega3].
-        postProcessing : bool, optional
+        post_processing : bool, optional
             If True, adds flight data information directly to self
             variables such as self.attackAngle, by default False
 
         Returns
         -------
-        uDot : list
-            State vector defined by uDot = [vx, vy, vz, ax, ay, az,
-            e0Dot, e1Dot, e2Dot, e3Dot, alpha1, alpha2, alpha3].
+        u_dot : list
+            State vector defined by u_dot = [vx, vy, vz, ax, ay, az,
+            e0dot, e1dot, e2dot, e3dot, alpha1, alpha2, alpha3].
         """
 
         # Retrieve integration data
         x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
         # Determine lift force and moment
         R1, R2 = 0, 0
         M1, M2, M3 = 0, 0, 0
         # Determine current behavior
-        if t < self.rocket.motor.burnOutTime:
+        if t < self.rocket.motor.burn_out_time:
             # Motor burning
             # Retrieve important motor quantities
             # Inertias
-            Tz = self.rocket.motor.inertiaZ.getValueOpt(t)
-            Ti = self.rocket.motor.inertiaI.getValueOpt(t)
-            TzDot = self.rocket.motor.inertiaZDot.getValueOpt(t)
-            TiDot = self.rocket.motor.inertiaIDot.getValueOpt(t)
+            Tz = self.rocket.motor.I_33.get_value_opt(t)
+            Ti = self.rocket.motor.I_11.get_value_opt(t)
+            TzDot = self.rocket.motor.I_33.differentiate(t, dx=1e-6)
+            TiDot = self.rocket.motor.I_11.differentiate(t, dx=1e-6)
             # Mass
-            MtDot = self.rocket.motor.massDot.getValueOpt(t)
-            Mt = self.rocket.motor.mass.getValueOpt(t)
+            MtDot = self.rocket.motor.mass_flow_rate.get_value_opt(t)
+            Mt = self.rocket.motor.propellant_mass.get_value_opt(t)
             # Thrust
-            Thrust = self.rocket.motor.thrust.getValueOpt(t)
+            thrust = self.rocket.motor.thrust.get_value_opt(t)
             # Off center moment
-            M1 += self.rocket.thrustEccentricityX * Thrust
-            M2 -= self.rocket.thrustEccentricityY * Thrust
+            M1 += self.rocket.thrust_eccentricity_x * thrust
+            M2 -= self.rocket.thrust_eccentricity_y * thrust
         else:
             # Motor stopped
             # Retrieve important motor quantities
             # Inertias
-            Tz, Ti, TzDot, TiDot = 0, 0, 0, 0
+            Tz, Ti, Tzdot, Tidot = 0, 0, 0, 0
             # Mass
-            MtDot, Mt = 0, 0
-            # Thrust
-            Thrust = 0
+            Mtdot, Mt = 0, 0
+            # thrust
+            thrust = 0
 
         # Retrieve important quantities
         # Inertias
-        Rz = self.rocket.inertiaZ
-        Ri = self.rocket.inertiaI
+        Rz = self.rocket.dry_I_33
+        Ri = self.rocket.dry_I_11
         # Mass
-        Mr = self.rocket.mass
+        Mr = self.rocket.dry_mass
         M = Mt + Mr
         mu = (Mt * Mr) / (Mt + Mr)
         # Geometry
-        b = -self.rocket.distanceRocketPropellant
-        c = -self.rocket.distanceRocketNozzle
+        # b = -self.rocket.distance_rocket_propellant
+        b = (
+            -(
+                self.rocket.center_of_propellant_position(0)
+                - self.rocket.center_of_dry_mass_position
+            )
+            * self.rocket._csys
+        )
+        # c = -self.rocket.distance_rocket_nozzle
+        c = (
+            -(self.rocket.motor_position - self.rocket.center_of_dry_mass_position)
+            * self.rocket._csys
+        )
         a = b * Mt / M
-        rN = self.rocket.motor.nozzleRadius
+        rN = self.rocket.motor.nozzle_radius
         # Prepare transformation matrix
-        a11 = 1 - 2 * (e2 ** 2 + e3 ** 2)
+        a11 = 1 - 2 * (e2**2 + e3**2)
         a12 = 2 * (e1 * e2 - e0 * e3)
         a13 = 2 * (e1 * e3 + e0 * e2)
         a21 = 2 * (e1 * e2 + e0 * e3)
-        a22 = 1 - 2 * (e1 ** 2 + e3 ** 2)
+        a22 = 1 - 2 * (e1**2 + e3**2)
         a23 = 2 * (e2 * e3 - e0 * e1)
         a31 = 2 * (e1 * e3 - e0 * e2)
         a32 = 2 * (e2 * e3 + e0 * e1)
-        a33 = 1 - 2 * (e1 ** 2 + e2 ** 2)
+        a33 = 1 - 2 * (e1**2 + e2**2)
         # Transformation matrix: (123) -> (XYZ)
         K = [[a11, a12, a13], [a21, a22, a23], [a31, a32, a33]]
         # Transformation matrix: (XYZ) -> (123) or K transpose
         Kt = [[a11, a21, a31], [a12, a22, a32], [a13, a23, a33]]
 
         # Calculate Forces and Moments
         # Get freestream speed
-        windVelocityX = self.env.windVelocityX.getValueOpt(z)
-        windVelocityY = self.env.windVelocityY.getValueOpt(z)
-        freestreamSpeed = (
-            (windVelocityX - vx) ** 2 + (windVelocityY - vy) ** 2 + (vz) ** 2
+        wind_velocity_x = self.env.wind_velocity_x.get_value_opt(z)
+        wind_velocity_y = self.env.wind_velocity_y.get_value_opt(z)
+        free_stream_speed = (
+            (wind_velocity_x - vx) ** 2 + (wind_velocity_y - vy) ** 2 + (vz) ** 2
         ) ** 0.5
-        freestreamMach = freestreamSpeed / self.env.speedOfSound.getValueOpt(z)
+        free_stream_mach = free_stream_speed / self.env.speed_of_sound.get_value_opt(z)
 
         # Determine aerodynamics forces
         # Determine Drag Force
-        if t > self.rocket.motor.burnOutTime:
-            dragCoeff = self.rocket.powerOnDrag.getValueOpt(freestreamMach)
+        if t < self.rocket.motor.burn_out_time:
+            drag_coeff = self.rocket.power_on_drag.get_value_opt(free_stream_mach)
         else:
-            dragCoeff = self.rocket.powerOffDrag.getValueOpt(freestreamMach)
-        rho = self.env.density.getValueOpt(z)
-        R3 = -0.5 * rho * (freestreamSpeed ** 2) * self.rocket.area * (dragCoeff)
+            drag_coeff = self.rocket.power_off_drag.get_value_opt(free_stream_mach)
+        rho = self.env.density.get_value_opt(z)
+        R3 = -0.5 * rho * (free_stream_speed**2) * self.rocket.area * (drag_coeff)
+        # R3 += self.__computeDragForce(z, Vector(vx, vy, vz))
         # Off center moment
-        M1 += self.rocket.cpEccentricityY * R3
-        M2 -= self.rocket.cpEccentricityX * R3
+        M1 += self.rocket.cp_eccentricity_y * R3
+        M2 -= self.rocket.cp_eccentricity_x * R3
         # Get rocket velocity in body frame
-        vxB = a11 * vx + a21 * vy + a31 * vz
-        vyB = a12 * vx + a22 * vy + a32 * vz
-        vzB = a13 * vx + a23 * vy + a33 * vz
+        vx_b = a11 * vx + a21 * vy + a31 * vz
+        vy_b = a12 * vx + a22 * vy + a32 * vz
+        vz_b = a13 * vx + a23 * vy + a33 * vz
         # Calculate lift and moment for each component of the rocket
-        for aerodynamicSurface in self.rocket.aerodynamicSurfaces:
-            compCp = aerodynamicSurface[0][2]
+        for aero_surface, position in self.rocket.aerodynamic_surfaces:
+            comp_cp = (
+                position - self.rocket.center_of_dry_mass_position
+            ) * self.rocket._csys - aero_surface.cpz
+            surface_radius = aero_surface.rocket_radius
+            reference_area = np.pi * surface_radius**2
             # Component absolute velocity in body frame
-            compVxB = vxB + compCp * omega2
-            compVyB = vyB - compCp * omega1
-            compVzB = vzB
+            comp_vx_b = vx_b + comp_cp * omega2
+            comp_vy_b = vy_b - comp_cp * omega1
+            comp_vz_b = vz_b
             # Wind velocity at component
-            compZ = z + compCp
-            compWindVx = self.env.windVelocityX.getValueOpt(compZ)
-            compWindVy = self.env.windVelocityY.getValueOpt(compZ)
+            comp_z = z + comp_cp
+            comp_wind_vx = self.env.wind_velocity_x.get_value_opt(comp_z)
+            comp_wind_vy = self.env.wind_velocity_y.get_value_opt(comp_z)
             # Component freestream velocity in body frame
-            compWindVxB = a11 * compWindVx + a21 * compWindVy
-            compWindVyB = a12 * compWindVx + a22 * compWindVy
-            compWindVzB = a13 * compWindVx + a23 * compWindVy
-            compStreamVxB = compWindVxB - compVxB
-            compStreamVyB = compWindVyB - compVyB
-            compStreamVzB = compWindVzB - compVzB
-            compStreamSpeed = (
-                compStreamVxB ** 2 + compStreamVyB ** 2 + compStreamVzB ** 2
+            comp_wind_vx_b = a11 * comp_wind_vx + a21 * comp_wind_vy
+            comp_wind_vy_b = a12 * comp_wind_vx + a22 * comp_wind_vy
+            comp_wind_vz_b = a13 * comp_wind_vx + a23 * comp_wind_vy
+            comp_stream_vx_b = comp_wind_vx_b - comp_vx_b
+            comp_stream_vy_b = comp_wind_vy_b - comp_vy_b
+            comp_stream_vz_b = comp_wind_vz_b - comp_vz_b
+            comp_stream_speed = (
+                comp_stream_vx_b**2 + comp_stream_vy_b**2 + comp_stream_vz_b**2
             ) ** 0.5
             # Component attack angle and lift force
-            compAttackAngle = 0
-            compLift, compLiftXB, compLiftYB = 0, 0, 0
-            if compStreamVxB ** 2 + compStreamVyB ** 2 != 0:
-                # Normalize component stream velocity in body frame
-                compStreamVzBn = compStreamVzB / compStreamSpeed
-                if -1 * compStreamVzBn < 1:
-                    compAttackAngle = np.arccos(-compStreamVzBn)
-                    cLift = abs(aerodynamicSurface[1](compAttackAngle))
-                    # Component lift force magnitude
-                    compLift = (
-                        0.5 * rho * (compStreamSpeed ** 2) * self.rocket.area * cLift
+            comp_attack_angle = 0
+            comp_lift, comp_lift_xb, comp_lift_yb = 0, 0, 0
+            if comp_stream_vx_b**2 + comp_stream_vy_b**2 != 0:
+                # normalize component stream velocity in body frame
+                comp_stream_vz_bn = comp_stream_vz_b / comp_stream_speed
+                if -1 * comp_stream_vz_bn < 1:
+                    comp_attack_angle = np.arccos(-comp_stream_vz_bn)
+                    c_lift = aero_surface.cl(comp_attack_angle, free_stream_mach)
+                    # component lift force magnitude
+                    comp_lift = (
+                        0.5 * rho * (comp_stream_speed**2) * reference_area * c_lift
                     )
-                    # Component lift force components
-                    liftDirNorm = (compStreamVxB ** 2 + compStreamVyB ** 2) ** 0.5
-                    compLiftXB = compLift * (compStreamVxB / liftDirNorm)
-                    compLiftYB = compLift * (compStreamVyB / liftDirNorm)
-                    # Add to total lift force
-                    R1 += compLiftXB
-                    R2 += compLiftYB
+                    # component lift force components
+                    lift_dir_norm = (
+                        comp_stream_vx_b**2 + comp_stream_vy_b**2
+                    ) ** 0.5
+                    comp_lift_xb = comp_lift * (comp_stream_vx_b / lift_dir_norm)
+                    comp_lift_yb = comp_lift * (comp_stream_vy_b / lift_dir_norm)
+                    # add to total lift force
+                    R1 += comp_lift_xb
+                    R2 += comp_lift_yb
                     # Add to total moment
-                    M1 -= (compCp + a) * compLiftYB
-                    M2 += (compCp + a) * compLiftXB
+                    M1 -= (comp_cp + a) * comp_lift_yb
+                    M2 += (comp_cp + a) * comp_lift_xb
             # Calculates Roll Moment
-            if aerodynamicSurface[-1] == "Fins":
-                Clfdelta, Cldomega, cantAngleRad = aerodynamicSurface[2]
-                if cantAngleRad != 0:
-                    Clf = Clfdelta * cantAngleRad
-                    Cld = Cldomega * omega3 / freestreamSpeed
-                    M3 += Clf - Cld
+            try:
+                clf_delta, cld_omega, cant_angle_rad = aero_surface.roll_parameters
+                M3f = (
+                    (1 / 2 * rho * free_stream_speed**2)
+                    * reference_area
+                    * 2
+                    * surface_radius
+                    * clf_delta(free_stream_mach)
+                    * cant_angle_rad
+                )
+                M3d = (
+                    (1 / 2 * rho * free_stream_speed)
+                    * reference_area
+                    * (2 * surface_radius) ** 2
+                    * cld_omega(free_stream_mach)
+                    * omega3
+                    / 2
+                )
+                M3 += M3f - M3d
+            except AttributeError:
+                pass
         # Calculate derivatives
         # Angular acceleration
         alpha1 = (
             M1
             - (
-                omega2 * omega3 * (Rz + Tz - Ri - Ti - mu * b ** 2)
+                omega2 * omega3 * (Rz + Tz - Ri - Ti - mu * b**2)
                 + omega1
                 * (
-                    (TiDot + MtDot * (Mr - 1) * (b / M) ** 2)
-                    - MtDot * ((rN / 2) ** 2 + (c - b * mu / Mr) ** 2)
+                    (Tidot + Mtdot * (Mr - 1) * (b / M) ** 2)
+                    - Mtdot * ((rN / 2) ** 2 + (c - b * mu / Mr) ** 2)
                 )
             )
-        ) / (Ri + Ti + mu * b ** 2)
+        ) / (Ri + Ti + mu * b**2)
         alpha2 = (
             M2
             - (
-                omega1 * omega3 * (Ri + Ti + mu * b ** 2 - Rz - Tz)
+                omega1 * omega3 * (Ri + Ti + mu * b**2 - Rz - Tz)
                 + omega2
                 * (
-                    (TiDot + MtDot * (Mr - 1) * (b / M) ** 2)
-                    - MtDot * ((rN / 2) ** 2 + (c - b * mu / Mr) ** 2)
+                    (Tidot + Mtdot * (Mr - 1) * (b / M) ** 2)
+                    - Mtdot * ((rN / 2) ** 2 + (c - b * mu / Mr) ** 2)
                 )
             )
-        ) / (Ri + Ti + mu * b ** 2)
-        alpha3 = (M3 - omega3 * (TzDot - MtDot * (rN ** 2) / 2)) / (Rz + Tz)
+        ) / (Ri + Ti + mu * b**2)
+        alpha3 = (M3 - omega3 * (Tzdot - Mtdot * (rN**2) / 2)) / (Rz + Tz)
         # Euler parameters derivative
-        e0Dot = 0.5 * (-omega1 * e1 - omega2 * e2 - omega3 * e3)
-        e1Dot = 0.5 * (omega1 * e0 + omega3 * e2 - omega2 * e3)
-        e2Dot = 0.5 * (omega2 * e0 - omega3 * e1 + omega1 * e3)
-        e3Dot = 0.5 * (omega3 * e0 + omega2 * e1 - omega1 * e2)
+        e0dot = 0.5 * (-omega1 * e1 - omega2 * e2 - omega3 * e3)
+        e1dot = 0.5 * (omega1 * e0 + omega3 * e2 - omega2 * e3)
+        e2dot = 0.5 * (omega2 * e0 - omega3 * e1 + omega1 * e3)
+        e3dot = 0.5 * (omega3 * e0 + omega2 * e1 - omega1 * e2)
 
         # Linear acceleration
         L = [
-            (R1 - b * Mt * (omega2 ** 2 + omega3 ** 2) - 2 * c * MtDot * omega2) / M,
-            (R2 + b * Mt * (alpha3 + omega1 * omega2) + 2 * c * MtDot * omega1) / M,
-            (R3 - b * Mt * (alpha2 - omega1 * omega3) + Thrust) / M,
+            (R1 - b * Mt * (omega2**2 + omega3**2) - 2 * c * Mtdot * omega2) / M,
+            (R2 + b * Mt * (alpha3 + omega1 * omega2) + 2 * c * Mtdot * omega1) / M,
+            (R3 - b * Mt * (alpha2 - omega1 * omega3) + thrust) / M,
         ]
         ax, ay, az = np.dot(K, L)
-        az -= self.env.g  # Include gravity
+        az -= self.env.gravity(z)  # Include gravity
 
-        # Create uDot
-        uDot = [
+        # Create u_dot
+        u_dot = [
             vx,
             vy,
             vz,
             ax,
             ay,
             az,
-            e0Dot,
-            e1Dot,
-            e2Dot,
-            e3Dot,
+            e0dot,
+            e1dot,
+            e2dot,
+            e3dot,
             alpha1,
             alpha2,
             alpha3,
         ]
 
-        if postProcessing:
+        if post_processing:
             # Dynamics variables
-            self.R1.append([t, R1])
-            self.R2.append([t, R2])
-            self.R3.append([t, R3])
-            self.M1.append([t, M1])
-            self.M2.append([t, M2])
-            self.M3.append([t, M3])
+            self.R1_list.append([t, R1])
+            self.R2_list.append([t, R2])
+            self.R3_list.append([t, R3])
+            self.M1_list.append([t, M1])
+            self.M2_list.append([t, M2])
+            self.M3_list.append([t, M3])
             # Atmospheric Conditions
-            self.windVelocityX.append([t, self.env.windVelocityX(z)])
-            self.windVelocityY.append([t, self.env.windVelocityY(z)])
-            self.density.append([t, self.env.density(z)])
-            self.dynamicViscosity.append([t, self.env.dynamicViscosity(z)])
-            self.pressure.append([t, self.env.pressure(z)])
-            self.speedOfSound.append([t, self.env.speedOfSound(z)])
+            self.wind_velocity_x_list.append(
+                [t, self.env.wind_velocity_x.get_value_opt(z)]
+            )
+            self.wind_velocity_y_list.append(
+                [t, self.env.wind_velocity_y.get_value_opt(z)]
+            )
+            self.density_list.append([t, self.env.density.get_value_opt(z)])
+            self.dynamic_viscosity_list.append(
+                [t, self.env.dynamic_viscosity.get_value_opt(z)]
+            )
+            self.pressure_list.append([t, self.env.pressure.get_value_opt(z)])
+            self.speed_of_sound_list.append(
+                [t, self.env.speed_of_sound.get_value_opt(z)]
+            )
+
+        return u_dot
+
+    def u_dot_generalized(self, t, u, post_processing=False):
+        """Calculates derivative of u state vector with respect to time when the
+        rocket is flying in 6 DOF motion in space and significant mass variation
+        effects exist. Typical flight phases include powered ascent after launch
+        rail.
+
+        Parameters
+        ----------
+        t : float
+            Time in seconds
+        u : list
+            State vector defined by u = [x, y, z, vx, vy, vz, q0, q1,
+            q2, q3, omega1, omega2, omega3].
+        post_processing : bool, optional
+            If True, adds flight data information directly to self variables
+            such as self.attackAngle, by default False.
+
+        Returns
+        -------
+        u_dot : list
+            State vector defined by u_dot = [vx, vy, vz, ax, ay, az,
+            e0Dot, e1Dot, e2Dot, e3Dot, alpha1, alpha2, alpha3].
+        """
+        # Retrieve integration data
+        x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
+
+        # Create necessary vectors
+        # r = Vector([x, y, z])               # CDM position vector
+        v = Vector([vx, vy, vz])  # CDM velocity vector
+        e = [e0, e1, e2, e3]  # Euler parameters/quaternions
+        w = Vector([omega1, omega2, omega3])  # Angular velocity vector
+
+        # Retrieve necessary quantities
+        rho = self.env.density.get_value_opt(z)
+        total_mass = self.rocket.total_mass.get_value_opt(t)
+        total_mass_dot = self.rocket.total_mass.differentiate(t)
+        total_mass_ddot = self.rocket.total_mass.differentiate(t, order=2)
+        ## CM position vector and time derivatives relative to CDM in body frame
+        r_CM_z = (
+            -1
+            * (
+                (
+                    self.rocket.center_of_propellant_position
+                    - self.rocket.center_of_dry_mass_position
+                )
+                * self.rocket._csys
+            )
+            * self.rocket.motor.propellant_mass
+            / total_mass
+        )
+        r_CM = Vector([0, 0, r_CM_z.get_value_opt(t)])
+        r_CM_dot = Vector([0, 0, r_CM_z.differentiate(t)])
+        r_CM_ddot = Vector([0, 0, r_CM_z.differentiate(t, order=2)])
+        ## Nozzle gyration tensor
+        r_NOZ = (
+            -(self.rocket.motor_position - self.rocket.center_of_dry_mass_position)
+            * self.rocket._csys
+        )
+        S_noz_33 = 0.5 * self.rocket.motor.nozzle_radius**2
+        S_noz_11 = 0.5 * S_noz_33 + 0.25 * r_NOZ**2
+        S_noz_22 = S_noz_11
+        S_noz_12 = 0
+        S_noz_13 = 0
+        S_noz_23 = 0
+        S_nozzle = Matrix(
+            [
+                [S_noz_11, S_noz_12, S_noz_13],
+                [S_noz_12, S_noz_22, S_noz_23],
+                [S_noz_13, S_noz_23, S_noz_33],
+            ]
+        )
+        ## Inertia tensor
+        I_11 = self.rocket.I_11.get_value_opt(t)
+        I_12 = self.rocket.I_12.get_value_opt(t)
+        I_13 = self.rocket.I_13.get_value_opt(t)
+        I_22 = self.rocket.I_22.get_value_opt(t)
+        I_23 = self.rocket.I_23.get_value_opt(t)
+        I_33 = self.rocket.I_33.get_value_opt(t)
+        I = Matrix(
+            [
+                [I_11, I_12, I_13],
+                [I_12, I_22, I_23],
+                [I_13, I_23, I_33],
+            ]
+        )
+        ## Inertia tensor time derivative in the body frame
+        I_11_dot = self.rocket.I_11.differentiate(t)
+        I_12_dot = self.rocket.I_12.differentiate(t)
+        I_13_dot = self.rocket.I_13.differentiate(t)
+        I_22_dot = self.rocket.I_22.differentiate(t)
+        I_23_dot = self.rocket.I_23.differentiate(t)
+        I_33_dot = self.rocket.I_33.differentiate(t)
+        I_dot = Matrix(
+            [
+                [I_11_dot, I_12_dot, I_13_dot],
+                [I_12_dot, I_22_dot, I_23_dot],
+                [I_13_dot, I_23_dot, I_33_dot],
+            ]
+        )
+        ## Inertia tensor relative to CM
+        H = (r_CM.cross_matrix @ -r_CM.cross_matrix) * total_mass
+        I_CM = I - H
+
+        # Prepare transformation matrices
+        K = Matrix.transformation(e)
+        Kt = K.transpose
+
+        # Compute aerodynamic forces and moments
+        R1, R2, R3, M1, M2, M3 = 0, 0, 0, 0, 0, 0
+
+        ## Drag force
+        rho = self.env.density.get_value_opt(z)
+        wind_velocity_x = self.env.wind_velocity_x.get_value_opt(z)
+        wind_velocity_y = self.env.wind_velocity_y.get_value_opt(z)
+        wind_velocity = Vector([wind_velocity_x, wind_velocity_y, 0])
+        free_stream_speed = abs((wind_velocity - Vector(v)))
+        free_stream_mach = free_stream_speed / self.env.speed_of_sound.get_value_opt(z)
+        if t < self.rocket.motor.burn_out_time:
+            drag_coeff = self.rocket.power_on_drag.get_value_opt(free_stream_mach)
+        else:
+            drag_coeff = self.rocket.power_off_drag.get_value_opt(free_stream_mach)
+        R3 += -0.5 * rho * (free_stream_speed**2) * self.rocket.area * (drag_coeff)
 
-        return uDot
+        ## Off center moment
+        M1 += self.rocket.cp_eccentricity_y * R3
+        M2 -= self.rocket.cp_eccentricity_x * R3
 
-    def uDotParachute(self, t, u, postProcessing=False):
+        # Get rocket velocity in body frame
+        vB = Kt @ v
+        # Calculate lift and moment for each component of the rocket
+        for aeroSurface, position in self.rocket.aerodynamic_surfaces:
+            compCpz = (
+                position - self.rocket.center_of_dry_mass_position
+            ) * self.rocket._csys - aeroSurface.cpz
+            compCp = Vector([0, 0, compCpz])
+            surfaceRadius = aeroSurface.rocket_radius
+            referenceArea = np.pi * surfaceRadius**2
+            # Component absolute velocity in body frame
+            compVB = vB + (w ^ compCp)
+            # Wind velocity at component altitude
+            compZ = z + (K @ compCp).z
+            compWindVx = self.env.wind_velocity_x.get_value_opt(compZ)
+            compWindVy = self.env.wind_velocity_y.get_value_opt(compZ)
+            # Component freestream velocity in body frame
+            compWindVB = Kt @ Vector([compWindVx, compWindVy, 0])
+            compStreamVelocity = compWindVB - compVB
+            compStreamVxB, compStreamVyB, compStreamVzB = compStreamVelocity
+            compStreamSpeed = abs(compStreamVelocity)
+            compStreamMach = compStreamSpeed / self.env.speed_of_sound.get_value_opt(z)
+            # Component attack angle and lift force
+            compAttackAngle = 0
+            compLift, compLiftXB, compLiftYB = 0, 0, 0
+            if compStreamVxB**2 + compStreamVyB**2 != 0:
+                # Normalize component stream velocity in body frame
+                compStreamVzBn = compStreamVzB / compStreamSpeed
+                if -1 * compStreamVzBn < 1:
+                    compAttackAngle = np.arccos(-compStreamVzBn)
+                    cLift = aeroSurface.cl(compAttackAngle, compStreamMach)
+                    # Component lift force magnitude
+                    compLift = (
+                        0.5 * rho * (compStreamSpeed**2) * referenceArea * cLift
+                    )
+                    # Component lift force components
+                    liftDirNorm = (compStreamVxB**2 + compStreamVyB**2) ** 0.5
+                    compLiftXB = compLift * (compStreamVxB / liftDirNorm)
+                    compLiftYB = compLift * (compStreamVyB / liftDirNorm)
+                    # Add to total lift force
+                    R1 += compLiftXB
+                    R2 += compLiftYB
+                    # Add to total moment
+                    M1 -= (compCpz + r_CM_z.get_value_opt(t)) * compLiftYB
+                    M2 += (compCpz + r_CM_z.get_value_opt(t)) * compLiftXB
+            # Calculates Roll Moment
+            try:
+                Clfdelta, Cldomega, cantAngleRad = aeroSurface.rollParameters
+                M3f = (
+                    (1 / 2 * rho * compStreamSpeed**2)
+                    * referenceArea
+                    * 2
+                    * surfaceRadius
+                    * Clfdelta(compStreamMach)
+                    * cantAngleRad
+                )
+                M3d = (
+                    (1 / 2 * rho * compStreamSpeed)
+                    * referenceArea
+                    * (2 * surfaceRadius) ** 2
+                    * Cldomega(compStreamMach)
+                    * omega3
+                    / 2
+                )
+                M3 += M3f - M3d
+            except AttributeError:
+                pass
+        weightB = Kt @ Vector([0, 0, -total_mass * self.env.gravity(z)])
+        T00 = total_mass * r_CM
+        T03 = (
+            2 * total_mass_dot * (Vector([0, 0, r_NOZ]) - r_CM)
+            - 2 * total_mass * r_CM_dot
+        )
+        T04 = (
+            self.rocket.motor.thrust(t) * Vector([0, 0, 1])
+            - total_mass * r_CM_ddot
+            - 2 * total_mass_dot * r_CM_dot
+            + total_mass_ddot * (Vector([0, 0, r_NOZ]) - r_CM)
+        )
+        T05 = total_mass_dot * S_nozzle - I_dot
+
+        T20 = ((w ^ T00) ^ w) + (w ^ T03) + T04 + weightB + Vector([R1, R2, R3])
+
+        T21 = ((I @ w) ^ w) + T05 @ w - (weightB ^ r_CM) + Vector([M1, M2, M3])
+
+        # Angular velocity derivative
+        w_dot = I_CM.inverse @ (T21 + (T20 ^ r_CM))
+
+        # Velocity vector derivative
+        v_dot = K @ (T20 / total_mass - (r_CM ^ w_dot))
+
+        # Euler parameters derivative
+        e_dot = [
+            0.5 * (-omega1 * e1 - omega2 * e2 - omega3 * e3),
+            0.5 * (omega1 * e0 + omega3 * e2 - omega2 * e3),
+            0.5 * (omega2 * e0 - omega3 * e1 + omega1 * e3),
+            0.5 * (omega3 * e0 + omega2 * e1 - omega1 * e2),
+        ]
+
+        # Position vector derivative
+        r_dot = [vx, vy, vz]
+
+        # Create u_dot
+        u_dot = [*r_dot, *v_dot, *e_dot, *w_dot]
+
+        if post_processing:
+            # Dynamics variables
+            self.R1_list.append([t, R1])
+            self.R2_list.append([t, R2])
+            self.R3_list.append([t, R3])
+            self.M1_list.append([t, M1])
+            self.M2_list.append([t, M2])
+            self.M3_list.append([t, M3])
+            # Atmospheric Conditions
+            self.wind_velocity_x_list.append(
+                [t, self.env.wind_velocity_x.get_value_opt(z)]
+            )
+            self.wind_velocity_y_list.append(
+                [t, self.env.wind_velocity_y.get_value_opt(z)]
+            )
+            self.density_list.append([t, self.env.density.get_value_opt(z)])
+            self.dynamic_viscosity_list.append(
+                [t, self.env.dynamic_viscosity.get_value_opt(z)]
+            )
+            self.pressure_list.append([t, self.env.pressure.get_value_opt(z)])
+            self.speed_of_sound_list.append(
+                [t, self.env.speed_of_sound.get_value_opt(z)]
+            )
+
+        return u_dot
+
+    def u_dot_parachute(self, t, u, post_processing=False):
         """Calculates derivative of u state vector with respect to time
         when rocket is flying under parachute. A 3 DOF approximation is
         used.
 
         Parameters
         ----------
         t : float
             Time in seconds
         u : list
             State vector defined by u = [x, y, z, vx, vy, vz, e0, e1,
             e2, e3, omega1, omega2, omega3].
-        postProcessing : bool, optional
+        post_processing : bool, optional
             If True, adds flight data information directly to self
             variables such as self.attackAngle. Default is False.
 
         Return
         ------
-        uDot : list
-            State vector defined by uDot = [vx, vy, vz, ax, ay, az,
-            e0Dot, e1Dot, e2Dot, e3Dot, alpha1, alpha2, alpha3].
+        u_dot : list
+            State vector defined by u_dot = [vx, vy, vz, ax, ay, az,
+            e0dot, e1dot, e2dot, e3dot, alpha1, alpha2, alpha3].
 
         """
         # Parachute data
-        CdS = self.parachuteCdS
+        cd_s = self.parachute_CdS
         ka = 1
         R = 1.5
-        rho = self.env.density.getValueOpt(u[2])
+        rho = self.env.density.get_value_opt(u[2])
         to = 1.2
-        ma = ka * rho * (4 / 3) * np.pi * R ** 3
+        ma = ka * rho * (4 / 3) * np.pi * R**3
         mp = self.rocket.mass
         eta = 1
-        Rdot = (6 * R * (1 - eta) / (1.2 ** 6)) * (
-            (1 - eta) * t ** 5 + eta * (to ** 3) * (t ** 2)
+        Rdot = (6 * R * (1 - eta) / (1.2**6)) * (
+            (1 - eta) * t**5 + eta * (to**3) * (t**2)
         )
         Rdot = 0
         # Get relevant state data
         x, y, z, vx, vy, vz, e0, e1, e2, e3, omega1, omega2, omega3 = u
         # Get wind data
-        windVelocityX = self.env.windVelocityX.getValueOpt(z)
-        windVelocityY = self.env.windVelocityY.getValueOpt(z)
-        freestreamSpeed = (
-            (windVelocityX - vx) ** 2 + (windVelocityY - vy) ** 2 + (vz) ** 2
+        wind_velocity_x = self.env.wind_velocity_x.get_value_opt(z)
+        wind_velocity_y = self.env.wind_velocity_y.get_value_opt(z)
+        free_stream_speed = (
+            (wind_velocity_x - vx) ** 2 + (wind_velocity_y - vy) ** 2 + (vz) ** 2
         ) ** 0.5
-        freestreamX = vx - windVelocityX
-        freestreamY = vy - windVelocityY
-        freestreamZ = vz
+        freestream_x = vx - wind_velocity_x
+        freestream_y = vy - wind_velocity_y
+        freestream_z = vz
         # Determine drag force
         pseudoD = (
-            -0.5 * rho * CdS * freestreamSpeed - ka * rho * 4 * np.pi * (R ** 2) * Rdot
+            -0.5 * rho * cd_s * free_stream_speed
+            - ka * rho * 4 * np.pi * (R**2) * Rdot
         )
-        Dx = pseudoD * freestreamX
-        Dy = pseudoD * freestreamY
-        Dz = pseudoD * freestreamZ
+        Dx = pseudoD * freestream_x
+        Dy = pseudoD * freestream_y
+        Dz = pseudoD * freestream_z
         ax = Dx / (mp + ma)
         ay = Dy / (mp + ma)
         az = (Dz - 9.8 * mp) / (mp + ma)
 
-        if postProcessing:
+        if post_processing:
             # Dynamics variables
-            self.R1.append([t, Dx])
-            self.R2.append([t, Dy])
-            self.R3.append([t, Dz])
-            self.M1.append([t, 0])
-            self.M2.append([t, 0])
-            self.M3.append([t, 0])
+            self.R1_list.append([t, Dx])
+            self.R2_list.append([t, Dy])
+            self.R3_list.append([t, Dz])
+            self.M1_list.append([t, 0])
+            self.M2_list.append([t, 0])
+            self.M3_list.append([t, 0])
             # Atmospheric Conditions
-            self.windVelocityX.append([t, self.env.windVelocityX(z)])
-            self.windVelocityY.append([t, self.env.windVelocityY(z)])
-            self.density.append([t, self.env.density(z)])
-            self.dynamicViscosity.append([t, self.env.dynamicViscosity(z)])
-            self.pressure.append([t, self.env.pressure(z)])
-            self.speedOfSound.append([t, self.env.speedOfSound(z)])
+            self.wind_velocity_x_list.append([t, self.env.wind_velocity_x(z)])
+            self.wind_velocity_y_list.append([t, self.env.wind_velocity_y(z)])
+            self.density_list.append([t, self.env.density(z)])
+            self.dynamic_viscosity_list.append([t, self.env.dynamic_viscosity(z)])
+            self.pressure_list.append([t, self.env.pressure(z)])
+            self.speed_of_sound_list.append([t, self.env.speed_of_sound(z)])
 
         return [vx, vy, vz, ax, ay, az, 0, 0, 0, 0, 0, 0, 0]
 
-    def postProcess(self):
-        """Post-process all Flight information produced during
-        simulation. Includes the calculation of maximum values,
-        calculation of secondary values such as energy and conversion
-        of lists to Function objects to facilitate plotting.
+    @cached_property
+    def solution_array(self):
+        """Returns solution array of the rocket flight."""
+        return np.array(self.solution)
+
+    @cached_property
+    def time(self):
+        """Returns time array from solution."""
+        return self.solution_array[:, 0]
+
+    # Process first type of outputs - state vector
+    # Transform solution array into Functions
+    @funcify_method("Time (s)", "X (m)", "spline", "constant")
+    def x(self):
+        """Rocket x position as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 1]]
+
+    @funcify_method("Time (s)", "Y (m)", "spline", "constant")
+    def y(self):
+        """Rocket y position as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 2]]
+
+    @funcify_method("Time (s)", "Z (m)", "spline", "constant")
+    def z(self):
+        """Rocket z position as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 3]]
+
+    @funcify_method("Time (s)", "Vx (m/s)", "spline", "zero")
+    def vx(self):
+        """Rocket x velocity as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 4]]
+
+    @funcify_method("Time (s)", "Vy (m/s)", "spline", "zero")
+    def vy(self):
+        """Rocket y velocity as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 5]]
+
+    @funcify_method("Time (s)", "Vz (m/s)", "spline", "zero")
+    def vz(self):
+        """Rocket z velocity as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 6]]
+
+    @funcify_method("Time (s)", "e0", "spline", "constant")
+    def e0(self):
+        """Rocket quaternion e0 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 7]]
+
+    @funcify_method("Time (s)", "e1", "spline", "constant")
+    def e1(self):
+        """Rocket quaternion e1 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 8]]
+
+    @funcify_method("Time (s)", "e2", "spline", "constant")
+    def e2(self):
+        """Rocket quaternion e2 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 9]]
+
+    @funcify_method("Time (s)", "e3", "spline", "constant")
+    def e3(self):
+        """Rocket quaternion e3 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 10]]
+
+    @funcify_method("Time (s)", "ω1 (rad/s)", "spline", "zero")
+    def w1(self):
+        """Rocket angular velocity ω1 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 11]]
+
+    @funcify_method("Time (s)", "ω2 (rad/s)", "spline", "zero")
+    def w2(self):
+        """Rocket angular velocity ω2 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 12]]
+
+    @funcify_method("Time (s)", "ω3 (rad/s)", "spline", "zero")
+    def w3(self):
+        """Rocket angular velocity ω3 as a rocketpy.Function of time."""
+        return self.solution_array[:, [0, 13]]
+
+    # Process second type of outputs - accelerations components
+    @funcify_method("Time (s)", "Ax (m/s²)", "spline", "zero")
+    def ax(self):
+        """Rocket x acceleration as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[0]
+
+    @funcify_method("Time (s)", "Ay (m/s²)", "spline", "zero")
+    def ay(self):
+        """Rocket y acceleration as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[1]
+
+    @funcify_method("Time (s)", "Az (m/s²)", "spline", "zero")
+    def az(self):
+        """Rocket z acceleration as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[2]
+
+    @funcify_method("Time (s)", "α1 (rad/s²)", "spline", "zero")
+    def alpha1(self):
+        """Rocket angular acceleration α1 as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[3]
+
+    @funcify_method("Time (s)", "α2 (rad/s²)", "spline", "zero")
+    def alpha2(self):
+        """Rocket angular acceleration α2 as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[4]
+
+    @funcify_method("Time (s)", "α3 (rad/s²)", "spline", "zero")
+    def alpha3(self):
+        """Rocket angular acceleration α3 as a rocketpy.Function of time."""
+        return self.retrieve_acceleration_arrays[5]
+
+    # Process third type of outputs - Temporary values
+    @funcify_method("Time (s)", "R1 (N)", "spline", "zero")
+    def R1(self):
+        """Aerodynamic force along the first axis that is perpendicular to the
+        rocket's axis of symmetry as a rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[0]
+
+    @funcify_method("Time (s)", "R2 (N)", "spline", "zero")
+    def R2(self):
+        """Aerodynamic force along the second axis that is perpendicular to the
+        rocket's axis of symmetry as a rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[1]
+
+    @funcify_method("Time (s)", "R3 (N)", "spline", "zero")
+    def R3(self):
+        """Aerodynamic force along the rocket's axis of symmetry as a
+        rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[2]
+
+    @funcify_method("Time (s)", "M1 (Nm)", "spline", "zero")
+    def M1(self):
+        """Aerodynamic bending moment in the same direction as the axis that is
+        perpendicular to the rocket's axis of symmetry as a rocketpy.Function of
+        time.
+        """
+        return self.retrieve_temporary_values_arrays[3]
+
+    @funcify_method("Time (s)", "M2 (Nm)", "spline", "zero")
+    def M2(self):
+        """Aerodynamic bending moment in the same direction as the axis that is
+        perpendicular to the rocket's axis of symmetry as a rocketpy.Function
+        of time."""
+        return self.retrieve_temporary_values_arrays[4]
+
+    @funcify_method("Time (s)", "M3 (Nm)", "spline", "zero")
+    def M3(self):
+        """Aerodynamic bending moment in the same direction as the rocket's
+        axis of symmetry as a rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[5]
+
+    @funcify_method("Time (s)", "Pressure (Pa)", "spline", "constant")
+    def pressure(self):
+        """Air pressure felt by the rocket as a rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[6]
+
+    @funcify_method("Time (s)", "Density (kg/m³)", "spline", "constant")
+    def density(self):
+        """Air density felt by the rocket as a rocketpy.Function of time."""
+        return self.retrieve_temporary_values_arrays[7]
+
+    @funcify_method("Time (s)", "Dynamic Viscosity (Pa s)", "spline", "constant")
+    def dynamic_viscosity(self):
+        """Air dynamic viscosity felt by the rocket as a rocketpy.Function of
+        time."""
+        return self.retrieve_temporary_values_arrays[8]
+
+    @funcify_method("Time (s)", "Speed of Sound (m/s)", "spline", "constant")
+    def speed_of_sound(self):
+        """Speed of sound in the air felt by the rocket as a rocketpy.Function
+        of time."""
+        return self.retrieve_temporary_values_arrays[9]
+
+    @funcify_method("Time (s)", "Wind Velocity X (East) (m/s)", "spline", "constant")
+    def wind_velocity_x(self):
+        """Wind velocity in the X direction (east) as a rocketpy.Function of
+        time."""
+        return self.retrieve_temporary_values_arrays[10]
+
+    @funcify_method("Time (s)", "Wind Velocity Y (North) (m/s)", "spline", "constant")
+    def wind_velocity_y(self):
+        """Wind velocity in the y direction (north) as a rocketpy.Function of
+        time."""
+        return self.retrieve_temporary_values_arrays[11]
+
+    # Process fourth type of output - values calculated from previous outputs
+
+    # Kinematics functions and values
+    # Velocity Magnitude
+    @funcify_method("Time (s)", "Speed - Velocity Magnitude (m/s)")
+    def speed(self):
+        """Rocket speed, or velocity magnitude, as a rocketpy.Function of time."""
+        return (self.vx**2 + self.vy**2 + self.vz**2) ** 0.5
+
+    @cached_property
+    def max_speed_time(self):
+        """Time at which the rocket reaches its maximum speed."""
+        max_speed_time_index = np.argmax(self.speed.get_source()[:, 1])
+        return self.speed[max_speed_time_index, 0]
+
+    @cached_property
+    def max_speed(self):
+        """Maximum speed reached by the rocket."""
+        return self.speed(self.max_speed_time)
+
+    # Accelerations
+    @funcify_method("Time (s)", "acceleration Magnitude (m/s²)")
+    def acceleration(self):
+        """Rocket acceleration magnitude as a rocketpy.Function of time."""
+        return (self.ax**2 + self.ay**2 + self.az**2) ** 0.5
+
+    @cached_property
+    def max_acceleration(self):
+        """Maximum acceleration reached by the rocket."""
+        max_acceleration_time_index = np.argmax(self.acceleration[:, 1])
+        return self.acceleration[max_acceleration_time_index, 1]
+
+    @cached_property
+    def max_acceleration_time(self):
+        """Time at which the rocket reaches its maximum acceleration."""
+        max_acceleration_time_index = np.argmax(self.acceleration[:, 1])
+        return self.acceleration[max_acceleration_time_index, 0]
+
+    @funcify_method("Time (s)", "Horizontal Speed (m/s)")
+    def horizontal_speed(self):
+        """Rocket horizontal speed as a rocketpy.Function of time."""
+        return (self.vx**2 + self.vy**2) ** 0.5
+
+    # Path Angle
+    @funcify_method("Time (s)", "Path Angle (°)", "spline", "constant")
+    def path_angle(self):
+        """Rocket path angle as a rocketpy.Function of time."""
+        path_angle = (180 / np.pi) * np.arctan2(
+            self.vz[:, 1], self.horizontal_speed[:, 1]
+        )
+        return np.column_stack([self.time, path_angle])
+
+    # Attitude Angle
+    @funcify_method("Time (s)", "Attitude Vector X Component")
+    def attitude_vector_x(self):
+        """Rocket attitude vector X component as a rocketpy.Function of time."""
+        return 2 * (self.e1 * self.e3 + self.e0 * self.e2)  # a13
+
+    @funcify_method("Time (s)", "Attitude Vector Y Component")
+    def attitude_vector_y(self):
+        """Rocket attitude vector Y component as a rocketpy.Function of time."""
+        return 2 * (self.e2 * self.e3 - self.e0 * self.e1)  # a23
+
+    @funcify_method("Time (s)", "Attitude Vector Z Component")
+    def attitude_vector_z(self):
+        """Rocket attitude vector Z component as a rocketpy.Function of time."""
+        return 1 - 2 * (self.e1**2 + self.e2**2)  # a33
+
+    @funcify_method("Time (s)", "Attitude Angle (°)")
+    def attitude_angle(self):
+        """Rocket attitude angle as a rocketpy.Function of time."""
+        horizontal_attitude_proj = (
+            self.attitude_vector_x**2 + self.attitude_vector_y**2
+        ) ** 0.5
+        attitude_angle = (180 / np.pi) * np.arctan2(
+            self.attitude_vector_z[:, 1], horizontal_attitude_proj[:, 1]
+        )
+        attitude_angle = np.column_stack([self.time, attitude_angle])
+        return attitude_angle
+
+    # Lateral Attitude Angle
+    @funcify_method("Time (s)", "Lateral Attitude Angle (°)")
+    def lateral_attitude_angle(self):
+        """Rocket lateral attitude angle as a rocketpy.Function of time."""
+        lateral_vector_angle = (np.pi / 180) * (self.heading - 90)
+        lateral_vector_x = np.sin(lateral_vector_angle)
+        lateral_vector_y = np.cos(lateral_vector_angle)
+        attitude_lateral_proj = (
+            lateral_vector_x * self.attitude_vector_x[:, 1]
+            + lateral_vector_y * self.attitude_vector_y[:, 1]
+        )
+        attitude_lateral_proj_x = attitude_lateral_proj * lateral_vector_x
+        attitude_lateral_proj_y = attitude_lateral_proj * lateral_vector_y
+        attitude_lateral_plane_proj_x = (
+            self.attitude_vector_x[:, 1] - attitude_lateral_proj_x
+        )
+        attitude_lateral_plane_proj_y = (
+            self.attitude_vector_y[:, 1] - attitude_lateral_proj_y
+        )
+        attitude_lateral_plane_proj_z = self.attitude_vector_z[:, 1]
+        attitude_lateral_plane_proj = (
+            attitude_lateral_plane_proj_x**2
+            + attitude_lateral_plane_proj_y**2
+            + attitude_lateral_plane_proj_z**2
+        ) ** 0.5
+        lateral_attitude_angle = (180 / np.pi) * np.arctan2(
+            attitude_lateral_proj, attitude_lateral_plane_proj
+        )
+        lateral_attitude_angle = np.column_stack([self.time, lateral_attitude_angle])
+        return lateral_attitude_angle
+
+    # Euler Angles
+    @funcify_method("Time (s)", "Precession Angle - ψ (°)", "spline", "constant")
+    def psi(self):
+        """Precession angle as a rocketpy.Function of time."""
+        psi = (180 / np.pi) * (
+            np.arctan2(self.e3[:, 1], self.e0[:, 1])
+            + np.arctan2(-self.e2[:, 1], -self.e1[:, 1])
+        )  # Precession angle
+        psi = np.column_stack([self.time, psi])  # Precession angle
+        return psi
+
+    @funcify_method("Time (s)", "Spin Angle - φ (°)", "spline", "constant")
+    def phi(self):
+        """Spin angle as a rocketpy.Function of time."""
+        phi = (180 / np.pi) * (
+            np.arctan2(self.e3[:, 1], self.e0[:, 1])
+            - np.arctan2(-self.e2[:, 1], -self.e1[:, 1])
+        )  # Spin angle
+        phi = np.column_stack([self.time, phi])  # Spin angle
+        return phi
+
+    @funcify_method("Time (s)", "Nutation Angle - θ (°)", "spline", "constant")
+    def theta(self):
+        """Nutation angle as a rocketpy.Function of time."""
+        theta = (
+            (180 / np.pi)
+            * 2
+            * np.arcsin(-((self.e1[:, 1] ** 2 + self.e2[:, 1] ** 2) ** 0.5))
+        )  # Nutation angle
+        theta = np.column_stack([self.time, theta])  # Nutation angle
+        return theta
+
+    # Fluid Mechanics variables
+    # Freestream Velocity
+    @funcify_method("Time (s)", "Freestream Velocity X (m/s)", "spline", "constant")
+    def stream_velocity_x(self):
+        """Freestream velocity X component as a rocketpy.Function of time."""
+        stream_velocity_x = np.column_stack(
+            (self.time, self.wind_velocity_x[:, 1] - self.vx[:, 1])
+        )
+        return stream_velocity_x
+
+    @funcify_method("Time (s)", "Freestream Velocity Y (m/s)", "spline", "constant")
+    def stream_velocity_y(self):
+        """Freestream velocity Y component as a rocketpy.Function of time."""
+        stream_velocity_y = np.column_stack(
+            (self.time, self.wind_velocity_y[:, 1] - self.vy[:, 1])
+        )
+        return stream_velocity_y
+
+    @funcify_method("Time (s)", "Freestream Velocity Z (m/s)", "spline", "constant")
+    def stream_velocity_z(self, interpolation="spline", extrapolation="natural"):
+        """Freestream velocity Z component as a rocketpy.Function of time."""
+        stream_velocity_z = np.column_stack((self.time, -self.vz[:, 1]))
+        return stream_velocity_z
+
+    @funcify_method("Time (s)", "Freestream Speed (m/s)", "spline", "constant")
+    def free_stream_speed(self):
+        """Freestream speed as a rocketpy.Function of time."""
+        free_stream_speed = (
+            self.stream_velocity_x**2
+            + self.stream_velocity_y**2
+            + self.stream_velocity_z**2
+        ) ** 0.5
+        return free_stream_speed.get_source()
+
+    # Apogee Freestream speed
+    @cached_property
+    def apogee_freestream_speed(self):
+        """Freestream speed at apogee in m/s."""
+        return self.free_stream_speed(self.apogee_time)
+
+    # Mach Number
+    @funcify_method("Time (s)", "Mach Number", "spline", "zero")
+    def mach_number(self):
+        """Mach number as a rocketpy.Function of time."""
+        return self.free_stream_speed / self.speed_of_sound
+
+    @cached_property
+    def max_mach_number_time(self):
+        """Time of maximum Mach number."""
+        max_mach_number_time_index = np.argmax(self.mach_number[:, 1])
+        return self.mach_number[max_mach_number_time_index, 0]
+
+    @cached_property
+    def max_mach_number(self):
+        """Maximum Mach number."""
+        return self.mach_number(self.max_mach_number_time)
+
+    # Reynolds Number
+    @funcify_method("Time (s)", "Reynolds Number", "spline", "zero")
+    def reynolds_number(self):
+        """Reynolds number as a rocketpy.Function of time."""
+        return (self.density * self.free_stream_speed / self.dynamic_viscosity) * (
+            2 * self.rocket.radius
+        )
+
+    @cached_property
+    def max_reynolds_number_time(self):
+        """Time of maximum Reynolds number."""
+        max_reynolds_number_time_index = np.argmax(self.reynolds_number[:, 1])
+        return self.reynolds_number[max_reynolds_number_time_index, 0]
+
+    @cached_property
+    def max_reynolds_number(self):
+        """Maximum Reynolds number."""
+        return self.reynolds_number(self.max_reynolds_number_time)
+
+    # Dynamic Pressure
+    @funcify_method("Time (s)", "Dynamic Pressure (Pa)", "spline", "zero")
+    def dynamic_pressure(self):
+        """Dynamic pressure as a rocketpy.Function of time."""
+        return 0.5 * self.density * self.free_stream_speed**2
+
+    @cached_property
+    def max_dynamic_pressure_time(self):
+        """Time of maximum dynamic pressure."""
+        max_dynamic_pressure_time_index = np.argmax(self.dynamic_pressure[:, 1])
+        return self.dynamic_pressure[max_dynamic_pressure_time_index, 0]
+
+    @cached_property
+    def max_dynamic_pressure(self):
+        """Maximum dynamic pressure."""
+        return self.dynamic_pressure(self.max_dynamic_pressure_time)
+
+    # Total Pressure
+    @funcify_method("Time (s)", "Total Pressure (Pa)", "spline", "zero")
+    def total_pressure(self):
+        return self.pressure * (1 + 0.2 * self.mach_number**2) ** (3.5)
+
+    @cached_property
+    def max_total_pressure_time(self):
+        """Time of maximum total pressure."""
+        max_total_pressure_time_index = np.argmax(self.total_pressure[:, 1])
+        return self.total_pressure[max_total_pressure_time_index, 0]
+
+    @cached_property
+    def max_total_pressure(self):
+        """Maximum total pressure."""
+        return self.total_pressure(self.max_total_pressure_time)
+
+    # Dynamics functions and variables
+
+    #  Aerodynamic Lift and Drag
+    @funcify_method("Time (s)", "Aerodynamic Lift Force (N)", "spline", "zero")
+    def aerodynamic_lift(self):
+        """Aerodynamic lift force as a rocketpy.Function of time."""
+        return (self.R1**2 + self.R2**2) ** 0.5
+
+    @funcify_method("Time (s)", "Aerodynamic Drag Force (N)", "spline", "zero")
+    def aerodynamic_drag(self):
+        """Aerodynamic drag force as a rocketpy.Function of time."""
+        return -1 * self.R3
+
+    @funcify_method("Time (s)", "Aerodynamic Bending Moment (Nm)", "spline", "zero")
+    def aerodynamic_bending_moment(self):
+        """Aerodynamic bending moment as a rocketpy.Function of time."""
+        return (self.M1**2 + self.M2**2) ** 0.5
+
+    @funcify_method("Time (s)", "Aerodynamic Spin Moment (Nm)", "spline", "zero")
+    def aerodynamic_spin_moment(self):
+        """Aerodynamic spin moment as a rocketpy.Function of time."""
+        return self.M3
+
+    # Energy
+    # Kinetic Energy
+    @funcify_method("Time (s)", "Rotational Kinetic Energy (J)")
+    def rotational_energy(self):
+        # b = -self.rocket.distanceRocketPropellant
+        b = (
+            -(self.rocket.motor_position - self.rocket.center_of_dry_mass_position)
+            * self.rocket._csys
+        )
+        mu = self.rocket.reduced_mass
+        Rz = self.rocket.dry_I_33
+        Ri = self.rocket.dry_I_11
+        Tz = self.rocket.motor.I_33
+        Ti = self.rocket.motor.I_11
+        I1, I2, I3 = (Ri + Ti + mu * b**2), (Ri + Ti + mu * b**2), (Rz + Tz)
+        # Redefine I1, I2 and I3 time grid to allow for efficient Function algebra
+        I1.set_discrete_based_on_model(self.w1)
+        I2.set_discrete_based_on_model(self.w1)
+        I3.set_discrete_based_on_model(self.w1)
+        rotational_energy = 0.5 * (
+            I1 * self.w1**2 + I2 * self.w2**2 + I3 * self.w3**2
+        )
+        rotational_energy.set_discrete_based_on_model(self.w1)
+        return rotational_energy
+
+    @funcify_method("Time (s)", "Translational Kinetic Energy (J)", "spline", "zero")
+    def translational_energy(self):
+        """Translational kinetic energy as a rocketpy.Function of time."""
+        # Redefine total_mass time grid to allow for efficient Function algebra
+        total_mass = deepcopy(self.rocket.total_mass)
+        total_mass.set_discrete_based_on_model(self.vz)
+        translational_energy = (
+            0.5 * total_mass * (self.vx**2 + self.vy**2 + self.vz**2)
+        )
+        return translational_energy
+
+    @funcify_method("Time (s)", "Kinetic Energy (J)", "spline", "zero")
+    def kinetic_energy(self):
+        """Total kinetic energy as a rocketpy.Function of time."""
+        return self.rotational_energy + self.translational_energy
+
+    # Potential Energy
+    @funcify_method("Time (s)", "Potential Energy (J)", "spline", "constant")
+    def potential_energy(self):
+        """Potential energy as a rocketpy.Function of time in relation to sea
+        level."""
+        # Constants
+        GM = 3.986004418e14
+        # Redefine total_mass time grid to allow for efficient Function algebra
+        total_mass = deepcopy(self.rocket.total_mass)
+        total_mass.set_discrete_based_on_model(self.z)
+        potential_energy = (
+            GM
+            * total_mass
+            * (1 / (self.z + self.env.earth_radius) - 1 / self.env.earth_radius)
+        )
+        return potential_energy
+
+    # Total Mechanical Energy
+    @funcify_method("Time (s)", "Mechanical Energy (J)", "spline", "constant")
+    def total_energy(self):
+        """Total mechanical energy as a rocketpy.Function of time."""
+        return self.kinetic_energy + self.potential_energy
+
+    # thrust Power
+    @funcify_method("Time (s)", "thrust Power (W)", "spline", "zero")
+    def thrust_power(self):
+        """thrust power as a rocketpy.Function of time."""
+        thrust = deepcopy(self.rocket.motor.thrust)
+        thrust = thrust.set_discrete_based_on_model(self.speed)
+        thrust_power = thrust * self.speed
+        return thrust_power
+
+    # Drag Power
+    @funcify_method("Time (s)", "Drag Power (W)", "spline", "zero")
+    def drag_power(self):
+        """Drag power as a rocketpy.Function of time."""
+        drag_power = self.R3 * self.speed
+        drag_power.set_outputs("Drag Power (W)")
+        return drag_power
+
+    # Angle of Attack
+    @funcify_method("Time (s)", "Angle of Attack (°)", "spline", "constant")
+    def angle_of_attack(self):
+        """Angle of attack of the rocket with respect to the freestream
+        velocity vector."""
+        dotProduct = [
+            -self.attitude_vector_x.get_value_opt(i)
+            * self.stream_velocity_x.get_value_opt(i)
+            - self.attitude_vector_y.get_value_opt(i)
+            * self.stream_velocity_y.get_value_opt(i)
+            - self.attitude_vector_z.get_value_opt(i)
+            * self.stream_velocity_z.get_value_opt(i)
+            for i in self.time
+        ]
+        # Define freestream speed list
+        free_stream_speed = [self.free_stream_speed(i) for i in self.time]
+        free_stream_speed = np.nan_to_num(free_stream_speed)
+
+        # Normalize dot product
+        dot_product_normalized = [
+            i / j if j > 1e-6 else 0 for i, j in zip(dotProduct, free_stream_speed)
+        ]
+        dot_product_normalized = np.nan_to_num(dot_product_normalized)
+        dot_product_normalized = np.clip(dot_product_normalized, -1, 1)
+
+        # Calculate angle of attack and convert to degrees
+        angle_of_attack = np.rad2deg(np.arccos(dot_product_normalized))
+        angle_of_attack = np.column_stack([self.time, angle_of_attack])
+
+        return angle_of_attack
+
+    # Frequency response and stability variables
+    @funcify_method("Frequency (Hz)", "ω1 Fourier Amplitude", "spline", "zero")
+    def omega1_frequency_response(self):
+        """Angular velocity 1 frequency response as a rocketpy.Function of frequency,
+        as the rocket leaves the launch rail for 5 seconds of flight."""
+        return self.w1.to_frequency_domain(
+            self.out_of_rail_time, self.out_of_rail_time + 5, 100
+        )
+
+    @funcify_method("Frequency (Hz)", "ω2 Fourier Amplitude", "spline", "zero")
+    def omega2_frequency_response(self):
+        """Angular velocity 2 frequency response as a rocketpy.Function of frequency,
+        as the rocket leaves the launch rail for 5 seconds of flight."""
+        return self.w2.to_frequency_domain(
+            self.out_of_rail_time, self.out_of_rail_time + 5, 100
+        )
+
+    @funcify_method("Frequency (Hz)", "ω3 Fourier Amplitude", "spline", "zero")
+    def omega3_frequency_response(self):
+        """Angular velocity 3 frequency response as a rocketpy.Function of frequency,
+        as the rocket leaves the launch rail for 5 seconds of flight."""
+        return self.w3.to_frequency_domain(
+            self.out_of_rail_time, self.out_of_rail_time + 5, 100
+        )
+
+    @funcify_method(
+        "Frequency (Hz)", "Attitude Angle Fourier Amplitude", "spline", "zero"
+    )
+    def attitude_frequency_response(self):
+        """Attitude frequency response as a rocketpy.Function of frequency, as the
+        rocket leaves the launch rail for 5 seconds of flight."""
+        return self.attitude_angle.to_frequency_domain(
+            lower=self.out_of_rail_time,
+            upper=self.out_of_rail_time + 5,
+            sampling_frequency=100,
+        )
+
+    @cached_property
+    def static_margin(self):
+        """Static margin of the rocket."""
+        return self.rocket.static_margin
+
+    # Rail Button Forces
+    @funcify_method("Time (s)", "Upper Rail Button Normal Force (N)", "spline", "zero")
+    def rail_button1_normal_force(self):
+        """Upper rail button normal force as a rocketpy.Function of time. If
+        there's no rail button defined, the function returns a null Function."""
+        return self.__calculate_rail_button_forces[0]
+
+    @funcify_method("Time (s)", "Upper Rail Button Shear Force (N)", "spline", "zero")
+    def rail_button1_shear_force(self):
+        """Upper rail button shear force as a rocketpy.Function of time. If
+        there's no rail button defined, the function returns a null Function."""
+        return self.__calculate_rail_button_forces[1]
+
+    @funcify_method("Time (s)", "Lower Rail Button Normal Force (N)", "spline", "zero")
+    def rail_button2_normal_force(self):
+        """Lower rail button normal force as a rocketpy.Function of time. If
+        there's no rail button defined, the function returns a null Function."""
+        return self.__calculate_rail_button_forces[2]
+
+    @funcify_method("Time (s)", "Lower Rail Button Shear Force (N)", "spline", "zero")
+    def rail_button2_shear_force(self):
+        """Lower rail button shear force as a rocketpy.Function of time. If
+        there's no rail button defined, the function returns a null Function."""
+        return self.__calculate_rail_button_forces[3]
+
+    @property
+    def max_rail_button1_normal_force(self):
+        """Maximum upper rail button normal force, in Newtons."""
+        return self.rail_button1_normal_force.max
+
+    @property
+    def max_rail_button1_shear_force(self):
+        """Maximum upper rail button shear force, in Newtons."""
+        return self.rail_button1_shear_force.max
+
+    @property
+    def max_rail_button2_normal_force(self):
+        """Maximum lower rail button normal force, in Newtons."""
+        return self.rail_button2_normal_force.max
+
+    @property
+    def max_rail_button2_shear_force(self):
+        """Maximum lower rail button shear force, in Newtons."""
+        return self.rail_button2_shear_force.max
+
+    @funcify_method(
+        "Time (s)", "Horizontal Distance to Launch Point (m)", "spline", "constant"
+    )
+    def drift(self):
+        """Rocket horizontal distance to tha launch point, in meters, as a
+        rocketpy.Function of time."""
+        return np.column_stack(
+            (self.time, (self.x[:, 1] ** 2 + self.y[:, 1] ** 2) ** 0.5)
+        )
+
+        return drift
+
+    @funcify_method("Time (s)", "Bearing (°)", "spline", "constant")
+    def bearing(self):
+        """Rocket bearing compass, in degrees, as a rocketpy.Function of time."""
+        x, y = self.x[:, 1], self.y[:, 1]
+        bearing = (2 * np.pi - np.arctan2(-x, y)) * (180 / np.pi)
+        return np.column_stack((self.time, bearing))
+
+    @funcify_method("Time (s)", "Latitude (°)", "linear", "constant")
+    def latitude(self):
+        """Rocket latitude coordinate, in degrees, as a rocketpy.Function of time."""
+        lat1 = np.deg2rad(self.env.latitude)  # Launch lat point converted to radians
+
+        # Applies the haversine equation to find final lat/lon coordinates
+        latitude = np.rad2deg(
+            np.arcsin(
+                np.sin(lat1) * np.cos(self.drift[:, 1] / self.env.earth_radius)
+                + np.cos(lat1)
+                * np.sin(self.drift[:, 1] / self.env.earth_radius)
+                * np.cos(np.deg2rad(self.bearing[:, 1]))
+            )
+        )
+        return np.column_stack((self.time, latitude))
+
+    @funcify_method("Time (s)", "Longitude (°)", "linear", "constant")
+    def longitude(self):
+        """Rocket longitude coordinate, in degrees, as a rocketpy.Function of time."""
+        lat1 = np.deg2rad(self.env.latitude)  # Launch lat point converted to radians
+        lon1 = np.deg2rad(self.env.longitude)  # Launch lon point converted to radians
+
+        # Applies the haversine equation to find final lat/lon coordinates
+        longitude = np.rad2deg(
+            lon1
+            + np.arctan2(
+                np.sin(np.deg2rad(self.bearing[:, 1]))
+                * np.sin(self.drift[:, 1] / self.env.earth_radius)
+                * np.cos(lat1),
+                np.cos(self.drift[:, 1] / self.env.earth_radius)
+                - np.sin(lat1) * np.sin(np.deg2rad(self.latitude[:, 1])),
+            )
+        )
+
+        return np.column_stack((self.time, longitude))
+
+    @cached_property
+    def retrieve_acceleration_arrays(self):
+        """Retrieve acceleration arrays from the integration scheme
 
         Parameters
         ----------
-        None
 
-        Return
-        ------
-        None
+        Returns
+        -------
+        ax: list
+            acceleration in x direction
+        ay: list
+            acceleration in y direction
+        az: list
+            acceleration in z direction
+        alpha1: list
+            angular acceleration in x direction
+        alpha2: list
+            angular acceleration in y direction
+        alpha3: list
+            angular acceleration in z direction
         """
-        # Process first type of outputs - state vector
-        # Transform solution array into Functions
-        sol = np.array(self.solution)
-        self.x = Function(
-            sol[:, [0, 1]], "Time (s)", "X (m)", "spline", extrapolation="natural"
-        )
-        self.y = Function(
-            sol[:, [0, 2]], "Time (s)", "Y (m)", "spline", extrapolation="natural"
-        )
-        self.z = Function(
-            sol[:, [0, 3]], "Time (s)", "Z (m)", "spline", extrapolation="natural"
-        )
-        self.vx = Function(
-            sol[:, [0, 4]], "Time (s)", "Vx (m/s)", "spline", extrapolation="natural"
-        )
-        self.vy = Function(
-            sol[:, [0, 5]], "Time (s)", "Vy (m/s)", "spline", extrapolation="natural"
-        )
-        self.vz = Function(
-            sol[:, [0, 6]], "Time (s)", "Vz (m/s)", "spline", extrapolation="natural"
-        )
-        self.e0 = Function(
-            sol[:, [0, 7]], "Time (s)", "e0", "spline", extrapolation="natural"
-        )
-        self.e1 = Function(
-            sol[:, [0, 8]], "Time (s)", "e1", "spline", extrapolation="natural"
-        )
-        self.e2 = Function(
-            sol[:, [0, 9]], "Time (s)", "e2", "spline", extrapolation="natural"
-        )
-        self.e3 = Function(
-            sol[:, [0, 10]], "Time (s)", "e3", "spline", extrapolation="natural"
-        )
-        self.w1 = Function(
-            sol[:, [0, 11]], "Time (s)", "ω1 (rad/s)", "spline", extrapolation="natural"
-        )
-        self.w2 = Function(
-            sol[:, [0, 12]], "Time (s)", "ω2 (rad/s)", "spline", extrapolation="natural"
-        )
-        self.w3 = Function(
-            sol[:, [0, 13]], "Time (s)", "ω3 (rad/s)", "spline", extrapolation="natural"
-        )
-
-        # Process second type of outputs - accelerations
         # Initialize acceleration arrays
-        self.ax, self.ay, self.az = [], [], []
-        self.alpha1, self.alpha2, self.alpha3 = [], [], []
+        ax, ay, az = [[0, 0]], [[0, 0]], [[0, 0]]
+        alpha1, alpha2, alpha3 = [[0, 0]], [[0, 0]], [[0, 0]]
         # Go through each time step and calculate accelerations
         # Get flight phases
-        for phase_index, phase in self.timeIterator(self.flightPhases):
-            initTime = phase.t
-            finalTime = self.flightPhases[phase_index + 1].t
-            currentDerivative = phase.derivative
+        for phase_index, phase in self.time_iterator(self.FlightPhases):
+            init_time = phase.t
+            final_time = self.FlightPhases[phase_index + 1].t
+            current_derivative = phase.derivative
             # Call callback functions
             for callback in phase.callbacks:
                 callback(self)
             # Loop through time steps in flight phase
             for step in self.solution:  # Can be optimized
-                if initTime < step[0] <= finalTime:
+                if init_time < step[0] <= final_time:
                     # Get derivatives
-                    uDot = currentDerivative(step[0], step[1:])
+                    u_dot = current_derivative(step[0], step[1:])
                     # Get accelerations
-                    ax, ay, az = uDot[3:6]
-                    alpha1, alpha2, alpha3 = uDot[10:]
+                    ax_value, ay_value, az_value = u_dot[3:6]
+                    alpha1_value, alpha2_value, alpha3_value = u_dot[10:]
                     # Save accelerations
-                    self.ax.append([step[0], ax])
-                    self.ay.append([step[0], ay])
-                    self.az.append([step[0], az])
-                    self.alpha1.append([step[0], alpha1])
-                    self.alpha2.append([step[0], alpha2])
-                    self.alpha3.append([step[0], alpha3])
-        # Convert accelerations to functions
-        self.ax = Function(self.ax, "Time (s)", "Ax (m/s2)", "spline")
-        self.ay = Function(self.ay, "Time (s)", "Ay (m/s2)", "spline")
-        self.az = Function(self.az, "Time (s)", "Az (m/s2)", "spline")
-        self.alpha1 = Function(self.alpha1, "Time (s)", "α1 (rad/s2)", "spline")
-        self.alpha2 = Function(self.alpha2, "Time (s)", "α2 (rad/s2)", "spline")
-        self.alpha3 = Function(self.alpha3, "Time (s)", "α3 (rad/s2)", "spline")
+                    ax.append([step[0], ax_value])
+                    ay.append([step[0], ay_value])
+                    az.append([step[0], az_value])
+                    alpha1.append([step[0], alpha1_value])
+                    alpha2.append([step[0], alpha2_value])
+                    alpha3.append([step[0], alpha3_value])
+
+        return ax, ay, az, alpha1, alpha2, alpha3
+
+    @cached_property
+    def retrieve_temporary_values_arrays(self):
+        """Retrieve temporary values arrays from the integration scheme.
+        Currently, the following temporary values are retrieved:
+            - R1
+            - R2
+            - R3
+            - M1
+            - M2
+            - M3
+            - pressure
+            - density
+            - dynamic_viscosity
+            - speed_of_sound
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.R1_list: list
+            R1 values.
+        self.R2_list: list
+            R2 values.
+        self.R3_list: list
+            R3 values are the aerodynamic force values in the rocket's axis
+            direction.
+        self.M1_list: list
+            M1 values.
+        self.M2_list: list
+            Aerodynamic bending moment in e2 direction at each time step.
+        self.M3_list: list
+            Aerodynamic bending moment in e3 direction at each time step.
+        self.pressure_list: list
+            Air pressure at each time step.
+        self.density_list: list
+            Air density at each time step.
+        self.dynamic_viscosity_list: list
+            Dynamic viscosity at each time step.
+        self.speed_of_sound_list: list
+            Speed of sound at each time step.
+        self.wind_velocity_x_list: list
+            Wind velocity in x direction at each time step.
+        self.wind_velocity_y_list: list
+            Wind velocity in y direction at each time step.
+        """
 
-        # Process third type of outputs - temporary values calculated during integration
         # Initialize force and atmospheric arrays
-        self.R1, self.R2, self.R3, self.M1, self.M2, self.M3 = [], [], [], [], [], []
-        self.pressure, self.density, self.dynamicViscosity, self.speedOfSound = (
-            [],
-            [],
-            [],
-            [],
-        )
-        self.windVelocityX, self.windVelocityY = [], []
+        self.R1_list = []
+        self.R2_list = []
+        self.R3_list = []
+        self.M1_list = []
+        self.M2_list = []
+        self.M3_list = []
+        self.pressure_list = []
+        self.density_list = []
+        self.dynamic_viscosity_list = []
+        self.speed_of_sound_list = []
+        self.wind_velocity_x_list = []
+        self.wind_velocity_y_list = []
+
         # Go through each time step and calculate forces and atmospheric values
         # Get flight phases
-        for phase_index, phase in self.timeIterator(self.flightPhases):
-            initTime = phase.t
-            finalTime = self.flightPhases[phase_index + 1].t
-            currentDerivative = phase.derivative
+        for phase_index, phase in self.time_iterator(self.FlightPhases):
+            init_time = phase.t
+            final_time = self.FlightPhases[phase_index + 1].t
+            current_derivative = phase.derivative
             # Call callback functions
             for callback in phase.callbacks:
                 callback(self)
             # Loop through time steps in flight phase
             for step in self.solution:  # Can be optimized
-                if initTime < step[0] <= finalTime or (initTime == 0 and step[0] == 0):
+                if init_time < step[0] <= final_time or (
+                    init_time == self.t_initial and step[0] == self.t_initial
+                ):
                     # Call derivatives in post processing mode
-                    uDot = currentDerivative(step[0], step[1:], postProcessing=True)
-        # Convert forces and atmospheric arrays to functions
-        self.R1 = Function(self.R1, "Time (s)", "R1 (N)", "spline")
-        self.R2 = Function(self.R2, "Time (s)", "R2 (N)", "spline")
-        self.R3 = Function(self.R3, "Time (s)", "R3 (N)", "spline")
-        self.M1 = Function(self.M1, "Time (s)", "M1 (Nm)", "spline")
-        self.M2 = Function(self.M2, "Time (s)", "M2 (Nm)", "spline")
-        self.M3 = Function(self.M3, "Time (s)", "M3 (Nm)", "spline")
-        self.windVelocityX = Function(
-            self.windVelocityX, "Time (s)", "Wind Velocity X (East) (m/s)", "spline"
-        )
-        self.windVelocityY = Function(
-            self.windVelocityY, "Time (s)", "Wind Velocity Y (North) (m/s)", "spline"
-        )
-        self.density = Function(self.density, "Time (s)", "Density (kg/m³)", "spline")
-        self.pressure = Function(self.pressure, "Time (s)", "Pressure (Pa)", "spline")
-        self.dynamicViscosity = Function(
-            self.dynamicViscosity, "Time (s)", "Dynamic Viscosity (Pa s)", "spline"
-        )
-        self.speedOfSound = Function(
-            self.speedOfSound, "Time (s)", "Speed of Sound (m/s)", "spline"
-        )
-
-        # Process fourth type of output - values calculated from previous outputs
-
-        # Kinematics functions and values
-        # Velocity Magnitude
-        self.speed = (self.vx ** 2 + self.vy ** 2 + self.vz ** 2) ** 0.5
-        self.speed.setOutputs("Speed - Velocity Magnitude (m/s)")
-        maxSpeedTimeIndex = np.argmax(self.speed[:, 1])
-        self.maxSpeed = self.speed[maxSpeedTimeIndex, 1]
-        self.maxSpeedTime = self.speed[maxSpeedTimeIndex, 0]
-        # Acceleration
-        self.acceleration = (self.ax ** 2 + self.ay ** 2 + self.az ** 2) ** 0.5
-        self.acceleration.setOutputs("Acceleration Magnitude (m/s²)")
-        maxAccelerationTimeIndex = np.argmax(self.acceleration[:, 1])
-        self.maxAcceleration = self.acceleration[maxAccelerationTimeIndex, 1]
-        self.maxAccelerationTime = self.acceleration[maxAccelerationTimeIndex, 0]
-        # Path Angle
-        self.horizontalSpeed = (self.vx ** 2 + self.vy ** 2) ** 0.5
-        pathAngle = (180 / np.pi) * np.arctan2(
-            self.vz[:, 1], self.horizontalSpeed[:, 1]
-        )
-        pathAngle = np.column_stack([self.vz[:, 0], pathAngle])
-        self.pathAngle = Function(pathAngle, "Time (s)", "Path Angle (°)")
-        # Attitude Angle
-        self.attitudeVectorX = 2 * (self.e1 * self.e3 + self.e0 * self.e2)  # a13
-        self.attitudeVectorY = 2 * (self.e2 * self.e3 - self.e0 * self.e1)  # a23
-        self.attitudeVectorZ = 1 - 2 * (self.e1 ** 2 + self.e2 ** 2)  # a33
-        horizontalAttitudeProj = (
-            self.attitudeVectorX ** 2 + self.attitudeVectorY ** 2
-        ) ** 0.5
-        attitudeAngle = (180 / np.pi) * np.arctan2(
-            self.attitudeVectorZ[:, 1], horizontalAttitudeProj[:, 1]
-        )
-        attitudeAngle = np.column_stack([self.attitudeVectorZ[:, 0], attitudeAngle])
-        self.attitudeAngle = Function(attitudeAngle, "Time (s)", "Attitude Angle (°)")
-        # Lateral Attitude Angle
-        lateralVectorAngle = (np.pi / 180) * (self.heading - 90)
-        lateralVectorX = np.sin(lateralVectorAngle)
-        lateralVectorY = np.cos(lateralVectorAngle)
-        attitudeLateralProj = (
-            lateralVectorX * self.attitudeVectorX[:, 1]
-            + lateralVectorY * self.attitudeVectorY[:, 1]
-        )
-        attitudeLateralProjX = attitudeLateralProj * lateralVectorX
-        attitudeLateralProjY = attitudeLateralProj * lateralVectorY
-        attitudeLateralPlaneProjX = self.attitudeVectorX[:, 1] - attitudeLateralProjX
-        attitudeLateralPlaneProjY = self.attitudeVectorY[:, 1] - attitudeLateralProjY
-        attitudeLateralPlaneProjZ = self.attitudeVectorZ[:, 1]
-        attitudeLateralPlaneProj = (
-            attitudeLateralPlaneProjX ** 2
-            + attitudeLateralPlaneProjY ** 2
-            + attitudeLateralPlaneProjZ ** 2
-        ) ** 0.5
-        lateralAttitudeAngle = (180 / np.pi) * np.arctan2(
-            attitudeLateralProj, attitudeLateralPlaneProj
-        )
-        lateralAttitudeAngle = np.column_stack(
-            [self.attitudeVectorZ[:, 0], lateralAttitudeAngle]
-        )
-        self.lateralAttitudeAngle = Function(
-            lateralAttitudeAngle, "Time (s)", "Lateral Attitude Angle (°)"
-        )
-        # Euler Angles
-        psi = (180 / np.pi) * (
-            np.arctan2(self.e3[:, 1], self.e0[:, 1])
-            + np.arctan2(-self.e2[:, 1], -self.e1[:, 1])
-        )  # Precession angle
-        psi = np.column_stack([self.e1[:, 0], psi])  # Precession angle
-        self.psi = Function(psi, "Time (s)", "Precession Angle - ψ (°)")
+                    u_dot = current_derivative(step[0], step[1:], post_processing=True)
 
-        phi = (180 / np.pi) * (
-            np.arctan2(self.e3[:, 1], self.e0[:, 1])
-            - np.arctan2(-self.e2[:, 1], -self.e1[:, 1])
-        )  # Spin angle
-        phi = np.column_stack([self.e1[:, 0], phi])  # Spin angle
-        self.phi = Function(phi, "Time (s)", "Spin Angle - φ (°)")
+        temporary_values = [
+            self.R1_list,
+            self.R2_list,
+            self.R3_list,
+            self.M1_list,
+            self.M2_list,
+            self.M3_list,
+            self.pressure_list,
+            self.density_list,
+            self.dynamic_viscosity_list,
+            self.speed_of_sound_list,
+            self.wind_velocity_x_list,
+            self.wind_velocity_y_list,
+        ]
 
-        theta = (
-            (180 / np.pi)
-            * 2
-            * np.arcsin(-((self.e1[:, 1] ** 2 + self.e2[:, 1] ** 2) ** 0.5))
-        )  # Nutation angle
-        theta = np.column_stack([self.e1[:, 0], theta])  # Nutation angle
-        self.theta = Function(theta, "Time (s)", "Nutation Angle - θ (°)")
+        return temporary_values
 
-        # Dynamics functions and variables
-        # Rail Button Forces
-        alpha = self.rocket.railButtons.angularPosition * (
-            np.pi / 180
-        )  # Rail buttons angular position
-        D1 = self.rocket.railButtons.distanceToCM[
-            0
-        ]  # Distance from Rail Button 1 (upper) to CM
-        D2 = self.rocket.railButtons.distanceToCM[
-            1
-        ]  # Distance from Rail Button 2 (lower) to CM
-        F11 = (self.R1 * D2 - self.M2) / (
-            D1 + D2
-        )  # Rail Button 1 force in the 1 direction
-        F12 = (self.R2 * D2 + self.M1) / (
-            D1 + D2
-        )  # Rail Button 1 force in the 2 direction
-        F21 = (self.R1 * D1 + self.M2) / (
-            D1 + D2
-        )  # Rail Button 2 force in the 1 direction
-        F22 = (self.R2 * D1 - self.M1) / (
-            D1 + D2
-        )  # Rail Button 2 force in the 2 direction
-        outOfRailTimeIndex = np.searchsorted(
-            F11[:, 0], self.outOfRailTime
-        )  # Find out of rail time index
-        # F11 = F11[:outOfRailTimeIndex + 1, :] # Limit force calculation to when rocket is in rail
-        # F12 = F12[:outOfRailTimeIndex + 1, :] # Limit force calculation to when rocket is in rail
-        # F21 = F21[:outOfRailTimeIndex + 1, :] # Limit force calculation to when rocket is in rail
-        # F22 = F22[:outOfRailTimeIndex + 1, :] # Limit force calculation to when rocket is in rail
-        self.railButton1NormalForce = F11 * np.cos(alpha) + F12 * np.sin(alpha)
-        self.railButton1NormalForce.setOutputs("Upper Rail Button Normal Force (N)")
-        self.railButton1ShearForce = F11 * -np.sin(alpha) + F12 * np.cos(alpha)
-        self.railButton1ShearForce.setOutputs("Upper Rail Button Shear Force (N)")
-        self.railButton2NormalForce = F21 * np.cos(alpha) + F22 * np.sin(alpha)
-        self.railButton2NormalForce.setOutputs("Lower Rail Button Normal Force (N)")
-        self.railButton2ShearForce = F21 * -np.sin(alpha) + F22 * np.cos(alpha)
-        self.railButton2ShearForce.setOutputs("Lower Rail Button Shear Force (N)")
-        # Rail Button Maximum Forces
-        if outOfRailTimeIndex == 0:
-            self.maxRailButton1NormalForce = 0
-            self.maxRailButton1ShearForce = 0
-            self.maxRailButton2NormalForce = 0
-            self.maxRailButton2ShearForce = 0
-        else:
-            self.maxRailButton1NormalForce = np.amax(
-                self.railButton1NormalForce[:outOfRailTimeIndex]
-            )
-            self.maxRailButton1ShearForce = np.amax(
-                self.railButton1ShearForce[:outOfRailTimeIndex]
-            )
-            self.maxRailButton2NormalForce = np.amax(
-                self.railButton2NormalForce[:outOfRailTimeIndex]
-            )
-            self.maxRailButton2ShearForce = np.amax(
-                self.railButton2ShearForce[:outOfRailTimeIndex]
-            )
-        # Aerodynamic Lift and Drag
-        self.aerodynamicLift = (self.R1 ** 2 + self.R2 ** 2) ** 0.5
-        self.aerodynamicLift.setOutputs("Aerodynamic Lift Force (N)")
-        self.aerodynamicDrag = -1 * self.R3
-        self.aerodynamicDrag.setOutputs("Aerodynamic Drag Force (N)")
-        self.aerodynamicBendingMoment = (self.M1 ** 2 + self.M2 ** 2) ** 0.5
-        self.aerodynamicBendingMoment.setOutputs("Aerodynamic Bending Moment (N m)")
-        self.aerodynamicSpinMoment = self.M3
-        self.aerodynamicSpinMoment.setOutputs("Aerodynamic Spin Moment (N m)")
-        # Energy
-        b = -self.rocket.distanceRocketPropellant
-        totalMass = self.rocket.totalMass
-        mu = self.rocket.reducedMass
-        Rz = self.rocket.inertiaZ
-        Ri = self.rocket.inertiaI
-        Tz = self.rocket.motor.inertiaZ
-        Ti = self.rocket.motor.inertiaI
-        I1, I2, I3 = (Ri + Ti + mu * b ** 2), (Ri + Ti + mu * b ** 2), (Rz + Tz)
-        # Redefine I1, I2 and I3 grid
-        grid = self.vx[:, 0]
-        I1 = Function(np.column_stack([grid, I1(grid)]), "Time (s)")
-        I2 = Function(np.column_stack([grid, I2(grid)]), "Time (s)")
-        I3 = Function(np.column_stack([grid, I3(grid)]), "Time (s)")
-        # Redefine total mass grid
-        totalMass = Function(np.column_stack([grid, totalMass(grid)]), "Time (s)")
-        # Redefine thrust grid
-        thrust = Function(
-            np.column_stack([grid, self.rocket.motor.thrust(grid)]), "Time (s)"
-        )
-        # Get some nicknames
-        vx, vy, vz = self.vx, self.vy, self.vz
-        w1, w2, w3 = self.w1, self.w2, self.w3
-        # Kinetic Energy
-        self.rotationalEnergy = 0.5 * (I1 * w1 ** 2 + I2 * w2 ** 2 + I3 * w3 ** 2)
-        self.rotationalEnergy.setOutputs("Rotational Kinetic Energy (J)")
-        self.translationalEnergy = 0.5 * totalMass * (vx ** 2 + vy ** 2 + vz ** 2)
-        self.translationalEnergy.setOutputs("Translational Kinetic Energy (J)")
-        self.kineticEnergy = self.rotationalEnergy + self.translationalEnergy
-        self.kineticEnergy.setOutputs("Kinetic Energy (J)")
-        # Potential Energy
-        self.potentialEnergy = totalMass * self.env.g * self.z
-        self.potentialEnergy.setInputs("Time (s)")
-        # Total Mechanical Energy
-        self.totalEnergy = self.kineticEnergy + self.potentialEnergy
-        self.totalEnergy.setOutputs("Total Mechanical Energy (J)")
-        # Thrust Power
-        self.thrustPower = thrust * self.speed
-        self.thrustPower.setOutputs("Thrust Power (W)")
-        # Drag Power
-        self.dragPower = self.R3 * self.speed
-        self.dragPower.setOutputs("Drag Power (W)")
-
-        # Stability and Control variables
-        # Angular velocities frequency response - Fourier Analysis
-        # Omega 1 - w1
-        Fs = 100.0
-        # sampling rate
-        Ts = 1.0 / Fs
-        # sampling interval
-        t = np.arange(1, self.tFinal, Ts)  # time vector
-        y = self.w1(t)
-        y -= np.mean(y)
-        n = len(y)  # length of the signal
-        k = np.arange(n)
-        T = n / Fs
-        frq = k / T  # two sides frequency range
-        frq = frq[range(n // 2)]  # one side frequency range
-        Y = np.fft.fft(y) / n  # fft computing and normalization
-        Y = Y[range(n // 2)]
-        omega1FrequencyResponse = np.column_stack([frq, abs(Y)])
-        self.omega1FrequencyResponse = Function(
-            omega1FrequencyResponse, "Frequency (Hz)", "Omega 1 Angle Fourier Amplitude"
-        )
-        # Omega 2 - w2
-        Fs = 100.0
-        # sampling rate
-        Ts = 1.0 / Fs
-        # sampling interval
-        t = np.arange(1, self.tFinal, Ts)  # time vector
-        y = self.w2(t)
-        y -= np.mean(y)
-        n = len(y)  # length of the signal
-        k = np.arange(n)
-        T = n / Fs
-        frq = k / T  # two sides frequency range
-        frq = frq[range(n // 2)]  # one side frequency range
-        Y = np.fft.fft(y) / n  # fft computing and normalization
-        Y = Y[range(n // 2)]
-        omega2FrequencyResponse = np.column_stack([frq, abs(Y)])
-        self.omega2FrequencyResponse = Function(
-            omega2FrequencyResponse, "Frequency (Hz)", "Omega 2 Angle Fourier Amplitude"
-        )
-        # Omega 3 - w3
-        Fs = 100.0
-        # sampling rate
-        Ts = 1.0 / Fs
-        # sampling interval
-        t = np.arange(1, self.tFinal, Ts)  # time vector
-        y = self.w3(t)
-        y -= np.mean(y)
-        n = len(y)  # length of the signal
-        k = np.arange(n)
-        T = n / Fs
-        frq = k / T  # two sides frequency range
-        frq = frq[range(n // 2)]  # one side frequency range
-        Y = np.fft.fft(y) / n  # fft computing and normalization
-        Y = Y[range(n // 2)]
-        omega3FrequencyResponse = np.column_stack([frq, abs(Y)])
-        self.omega3FrequencyResponse = Function(
-            omega3FrequencyResponse, "Frequency (Hz)", "Omega 3 Angle Fourier Amplitude"
-        )
-        # Attitude Frequency Response
-        Fs = 100.0
-        # sampling rate
-        Ts = 1.0 / Fs
-        # sampling interval
-        t = np.arange(1, self.tFinal, Ts)  # time vector
-        y = self.attitudeAngle(t)
-        y -= np.mean(y)
-        n = len(y)  # length of the signal
-        k = np.arange(n)
-        T = n / Fs
-        frq = k / T  # two sides frequency range
-        frq = frq[range(n // 2)]  # one side frequency range
-        Y = np.fft.fft(y) / n  # fft computing and normalization
-        Y = Y[range(n // 2)]
-        attitudeFrequencyResponse = np.column_stack([frq, abs(Y)])
-        self.attitudeFrequencyResponse = Function(
-            attitudeFrequencyResponse,
-            "Frequency (Hz)",
-            "Attitude Angle Fourier Amplitude",
-        )
-        # Static Margin
-        self.staticMargin = self.rocket.staticMargin
-
-        # Fluid Mechanics variables
-        # Freestream Velocity
-        self.streamVelocityX = self.windVelocityX - self.vx
-        self.streamVelocityX.setOutputs("Freestream Velocity X (m/s)")
-        self.streamVelocityY = self.windVelocityY - self.vy
-        self.streamVelocityY.setOutputs("Freestream Velocity Y (m/s)")
-        self.streamVelocityZ = -1 * self.vz
-        self.streamVelocityZ.setOutputs("Freestream Velocity Z (m/s)")
-        self.freestreamSpeed = (
-            self.streamVelocityX ** 2
-            + self.streamVelocityY ** 2
-            + self.streamVelocityZ ** 2
-        ) ** 0.5
-        self.freestreamSpeed.setOutputs("Freestream Speed (m/s)")
-        # Apogee Freestream speed
-        self.apogeeFreestreamSpeed = self.freestreamSpeed(self.apogeeTime)
-        # Mach Number
-        self.MachNumber = self.freestreamSpeed / self.speedOfSound
-        self.MachNumber.setOutputs("Mach Number")
-        maxMachNumberTimeIndex = np.argmax(self.MachNumber[:, 1])
-        self.maxMachNumberTime = self.MachNumber[maxMachNumberTimeIndex, 0]
-        self.maxMachNumber = self.MachNumber[maxMachNumberTimeIndex, 1]
-        # Reynolds Number
-        self.ReynoldsNumber = (
-            self.density * self.freestreamSpeed / self.dynamicViscosity
-        ) * (2 * self.rocket.radius)
-        self.ReynoldsNumber.setOutputs("Reynolds Number")
-        maxReynoldsNumberTimeIndex = np.argmax(self.ReynoldsNumber[:, 1])
-        self.maxReynoldsNumberTime = self.ReynoldsNumber[maxReynoldsNumberTimeIndex, 0]
-        self.maxReynoldsNumber = self.ReynoldsNumber[maxReynoldsNumberTimeIndex, 1]
-        # Dynamic Pressure
-        self.dynamicPressure = 0.5 * self.density * self.freestreamSpeed ** 2
-        self.dynamicPressure.setOutputs("Dynamic Pressure (Pa)")
-        maxDynamicPressureTimeIndex = np.argmax(self.dynamicPressure[:, 1])
-        self.maxDynamicPressureTime = self.dynamicPressure[
-            maxDynamicPressureTimeIndex, 0
-        ]
-        self.maxDynamicPressure = self.dynamicPressure[maxDynamicPressureTimeIndex, 1]
-        # Total Pressure
-        self.totalPressure = self.pressure * (1 + 0.2 * self.MachNumber ** 2) ** (3.5)
-        self.totalPressure.setOutputs("Total Pressure (Pa)")
-        maxtotalPressureTimeIndex = np.argmax(self.totalPressure[:, 1])
-        self.maxtotalPressureTime = self.totalPressure[maxtotalPressureTimeIndex, 0]
-        self.maxtotalPressure = self.totalPressure[maxDynamicPressureTimeIndex, 1]
-        # Angle of Attack
-        angleOfAttack = []
-        for i in range(len(self.attitudeVectorX[:, 1])):
-            dotProduct = -(
-                self.attitudeVectorX[i, 1] * self.streamVelocityX[i, 1]
-                + self.attitudeVectorY[i, 1] * self.streamVelocityY[i, 1]
-                + self.attitudeVectorZ[i, 1] * self.streamVelocityZ[i, 1]
-            )
-            if self.freestreamSpeed[i, 1] < 1e-6:
-                angleOfAttack.append([self.freestreamSpeed[i, 0], 0])
-            else:
-                dotProductNormalized = dotProduct / self.freestreamSpeed[i, 1]
-                dotProductNormalized = (
-                    1 if dotProductNormalized > 1 else dotProductNormalized
-                )
-                dotProductNormalized = (
-                    -1 if dotProductNormalized < -1 else dotProductNormalized
-                )
-                angleOfAttack.append(
-                    [
-                        self.freestreamSpeed[i, 0],
-                        (180 / np.pi) * np.arccos(dotProductNormalized),
-                    ]
-                )
-        self.angleOfAttack = Function(
-            angleOfAttack, "Time (s)", "Angle Of Attack (°)", "linear"
-        )
+    @cached_property
+    def __calculate_rail_button_forces(self):
+        """Calculate the forces applied to the rail buttons while rocket is still
+        on the launch rail. It will return 0 if no rail buttons are defined.
 
-        # Post process other quantities
+        Returns
+        -------
+        F11: Function
+            Rail Button 1 force in the 1 direction
+        F12: Function
+            Rail Button 1 force in the 2 direction
+        F21: Function
+            Rail Button 2 force in the 1 direction
+        F22: Function
+            Rail Button 2 force in the 2 direction
+        """
+        # First check for no rail phase or rail buttons
+        nullForce = []
+        if self.out_of_rail_time_index == 0:  # No rail phase, no rail button forces
+            warnings.warn(
+                "Trying to calculate rail button forces without a rail phase defined."
+                + "The rail button forces will be set to zero."
+            )
+            return nullForce, nullForce, nullForce, nullForce
+        if len(self.rocket.rail_buttons) == 0:
+            warnings.warn(
+                "Trying to calculate rail button forces without rail buttons defined."
+                + "The rail button forces will be set to zero."
+            )
+            return nullForce, nullForce, nullForce, nullForce
+
+        # Distance from Rail Button 1 (upper) to CM
+        rail_buttons_tuple = self.rocket.rail_buttons[0]
+        upper_button_position = (
+            rail_buttons_tuple.component.buttons_distance + rail_buttons_tuple.position
+        )
+        lower_button_position = rail_buttons_tuple.position
+        angular_position_rad = (
+            rail_buttons_tuple.component.angular_position * np.pi / 180
+        )
+        D1 = (
+            upper_button_position - self.rocket.center_of_dry_mass_position
+        ) * self.rocket._csys
+        # Distance from Rail Button 2 (lower) to CM
+        D2 = (
+            lower_button_position - self.rocket.center_of_dry_mass_position
+        ) * self.rocket._csys
+        F11 = (self.R1 * D2 - self.M2) / (D1 + D2)
+        F11.set_outputs("Upper button force direction 1 (m)")
+        F12 = (self.R2 * D2 + self.M1) / (D1 + D2)
+        F12.set_outputs("Upper button force direction 2 (m)")
+        F21 = (self.R1 * D1 + self.M2) / (D1 + D2)
+        F21.set_outputs("Lower button force direction 1 (m)")
+        F22 = (self.R2 * D1 - self.M1) / (D1 + D2)
+        F22.set_outputs("Lower button force direction 2 (m)")
+
+        model = Function(
+            F11.get_source()[: self.out_of_rail_time_index + 1, :],
+            interpolation=F11.__interpolation__,
+        )
+
+        # Limit force calculation to when rocket is in rail
+        F11.set_discrete_based_on_model(model)
+        F12.set_discrete_based_on_model(model)
+        F21.set_discrete_based_on_model(model)
+        F22.set_discrete_based_on_model(model)
+
+        rail_button1_normal_force = F11 * np.cos(angular_position_rad) + F12 * np.sin(
+            angular_position_rad
+        )
+        rail_button1_shear_force = F11 * -np.sin(angular_position_rad) + F12 * np.cos(
+            angular_position_rad
+        )
+        rail_button2_normal_force = F21 * np.cos(angular_position_rad) + F22 * np.sin(
+            angular_position_rad
+        )
+        rail_button2_shear_force = F21 * -np.sin(angular_position_rad) + F22 * np.cos(
+            angular_position_rad
+        )
+
+        return (
+            rail_button1_normal_force,
+            rail_button1_shear_force,
+            rail_button2_normal_force,
+            rail_button2_shear_force,
+        )
+
+    def _calculate_pressure_signal(self):
+        """Calculate the pressure signal from the pressure sensor.
+        It creates a SignalFunction attribute in the parachute object.
+        Parachute works as a subclass of Rocket class.
 
+        Returns
+        -------
+        None
+        """
         # Transform parachute sensor feed into functions
         for parachute in self.rocket.parachutes:
-            parachute.cleanPressureSignalFunction = Function(
-                parachute.cleanPressureSignal,
+            parachute.clean_pressure_signal_function = Function(
+                parachute.clean_pressure_signal,
                 "Time (s)",
                 "Pressure - Without Noise (Pa)",
                 "linear",
             )
-            parachute.noisyPressureSignalFunction = Function(
-                parachute.noisyPressureSignal,
+            parachute.noisy_pressure_signal_function = Function(
+                parachute.noisy_pressure_signal,
                 "Time (s)",
                 "Pressure - With Noise (Pa)",
                 "linear",
             )
-            parachute.noiseSignalFunction = Function(
-                parachute.noiseSignal, "Time (s)", "Pressure Noise (Pa)", "linear"
+            parachute.noise_signal_function = Function(
+                parachute.noise_signal, "Time (s)", "Pressure Noise (Pa)", "linear"
             )
 
-        # Register post processing
-        self.postProcessed = True
-
         return None
 
-    def info(self):
-        """Prints out a summary of the data available about the Flight.
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of out of rail time
-        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
-        outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
-        )
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
-        else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        # Print surface wind conditions
-        print("Surface Wind Conditions\n")
-        print("Frontal Surface Wind Speed: {:.2f} m/s".format(self.frontalSurfaceWind))
-        print("Lateral Surface Wind Speed: {:.2f} m/s".format(self.lateralSurfaceWind))
-
-        # Print out of rail conditions
-        print("\n\n Rail Departure State\n")
-        print("Rail Departure Time: {:.3f} s".format(self.outOfRailTime))
-        print("Rail Departure Velocity: {:.3f} m/s".format(self.outOfRailVelocity))
-        print(
-            "Rail Departure Static Margin: {:.3f} c".format(
-                self.staticMargin(self.outOfRailTime)
-            )
-        )
-        print(
-            "Rail Departure Angle of Attack: {:.3f}°".format(
-                self.angleOfAttack(self.outOfRailTime)
-            )
-        )
-        print(
-            "Rail Departure Thrust-Weight Ratio: {:.3f}".format(
-                self.rocket.thrustToWeight(self.outOfRailTime)
-            )
-        )
-        print(
-            "Rail Departure Reynolds Number: {:.3e}".format(
-                self.ReynoldsNumber(self.outOfRailTime)
-            )
-        )
-
-        # Print burnOut conditions
-        print("\n\nBurnOut State\n")
-        print("BurnOut time: {:.3f} s".format(self.rocket.motor.burnOutTime))
-        print(
-            "Altitude at burnOut: {:.3f} m (AGL)".format(
-                self.z(self.rocket.motor.burnOutTime) - self.env.elevation
-            )
-        )
-        print(
-            "Rocket velocity at burnOut: {:.3f} m/s".format(
-                self.speed(self.rocket.motor.burnOutTime)
-            )
-        )
-        print(
-            "Freestream velocity at burnOut: {:.3f} m/s".format(
-                (
-                    self.streamVelocityX(self.rocket.motor.burnOutTime) ** 2
-                    + self.streamVelocityY(self.rocket.motor.burnOutTime) ** 2
-                    + self.streamVelocityZ(self.rocket.motor.burnOutTime) ** 2
-                )
-                ** 0.5
-            )
-        )
-        print(
-            "Mach Number at burnOut: {:.3f}".format(
-                self.MachNumber(self.rocket.motor.burnOutTime)
-            )
-        )
-        print(
-            "Kinetic energy at burnOut: {:.3e} J".format(
-                self.kineticEnergy(self.rocket.motor.burnOutTime)
-            )
-        )
-
-        # Print apogee conditions
-        print("\n\nApogee\n")
-        print(
-            "Apogee Altitude: {:.3f} m (ASL) | {:.3f} m (AGL)".format(
-                self.apogee, self.apogee - self.env.elevation
-            )
-        )
-        print("Apogee Time: {:.3f} s".format(self.apogeeTime))
-        print("Apogee Freestream Speed: {:.3f} m/s".format(self.apogeeFreestreamSpeed))
-
-        # Print events registered
-        print("\n\nEvents\n")
-        if len(self.parachuteEvents) == 0:
-            print("No Parachute Events Were Triggered.")
-        for event in self.parachuteEvents:
-            triggerTime = event[0]
-            parachute = event[1]
-            openTime = triggerTime + parachute.lag
-            velocity = self.freestreamSpeed(openTime)
-            altitude = self.z(openTime)
-            name = parachute.name.title()
-            print(name + " Ejection Triggered at: {:.3f} s".format(triggerTime))
-            print(name + " Parachute Inflated at: {:.3f} s".format(openTime))
-            print(
-                name
-                + " Parachute Inflated with Freestream Speed of: {:.3f} m/s".format(
-                    velocity
-                )
-            )
-            print(
-                name
-                + " Parachute Inflated at Height of: {:.3f} m (AGL)".format(
-                    altitude - self.env.elevation
-                )
-            )
-
-        # Print impact conditions
-        if len(self.impactState) != 0:
-            print("\n\nImpact\n")
-            print("X Impact: {:.3f} m".format(self.xImpact))
-            print("Y Impact: {:.3f} m".format(self.yImpact))
-            print("Time of Impact: {:.3f} s".format(self.tFinal))
-            print("Velocity at Impact: {:.3f} m/s".format(self.impactVelocity))
-        elif self.terminateOnApogee is False:
-            print("\n\nEnd of Simulation\n")
-            print("Time: {:.3f} s".format(self.solution[-1][0]))
-            print("Altitude: {:.3f} m".format(self.solution[-1][3]))
-
-        # Print maximum values
-        print("\n\nMaximum Values\n")
-        print(
-            "Maximum Speed: {:.3f} m/s at {:.2f} s".format(
-                self.maxSpeed, self.maxSpeedTime
-            )
-        )
-        print(
-            "Maximum Mach Number: {:.3f} Mach at {:.2f} s".format(
-                self.maxMachNumber, self.maxMachNumberTime
-            )
-        )
-        print(
-            "Maximum Reynolds Number: {:.3e} at {:.2f} s".format(
-                self.maxReynoldsNumber, self.maxReynoldsNumberTime
-            )
-        )
-        print(
-            "Maximum Dynamic Pressure: {:.3e} Pa at {:.2f} s".format(
-                self.maxDynamicPressure, self.maxDynamicPressureTime
-            )
-        )
-        print(
-            "Maximum Acceleration: {:.3f} m/s² at {:.2f} s".format(
-                self.maxAcceleration, self.maxAccelerationTime
-            )
-        )
-        print(
-            "Maximum Gs: {:.3f} g at {:.2f} s".format(
-                self.maxAcceleration / self.env.g, self.maxAccelerationTime
-            )
-        )
-        print(
-            "Maximum Upper Rail Button Normal Force: {:.3f} N".format(
-                self.maxRailButton1NormalForce
-            )
-        )
-        print(
-            "Maximum Upper Rail Button Shear Force: {:.3f} N".format(
-                self.maxRailButton1ShearForce
-            )
-        )
-        print(
-            "Maximum Lower Rail Button Normal Force: {:.3f} N".format(
-                self.maxRailButton2NormalForce
-            )
-        )
-        print(
-            "Maximum Lower Rail Button Shear Force: {:.3f} N".format(
-                self.maxRailButton2ShearForce
-            )
-        )
-
-        return None
+    def post_process(self, interpolation="spline", extrapolation="natural"):
+        """Post-process all Flight information produced during
+        simulation. Includes the calculation of maximum values,
+        calculation of secondary values such as energy and conversion
+        of lists to Function objects to facilitate plotting.
 
-    def printInitialConditionsData(self):
-        """Prints all initial conditions data available about the flight
+        * This method is deprecated and is only kept here for backwards
+        compatibility. * All attributes that need to be post processed are
+        computed just in time.
 
         Parameters
         ----------
         None
 
         Return
         ------
         None
         """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
+        # Register post processing
+        self.post_processed = True
 
-        print(
-            "Position - x: {:.2f} m | y: {:.2f} m | z: {:.2f} m".format(
-                self.x(0), self.y(0), self.z(0)
-            )
-        )
-        print(
-            "Velocity - Vx: {:.2f} m/s | Vy: {:.2f} m/s | Vz: {:.2f} m/s".format(
-                self.vx(0), self.vy(0), self.vz(0)
-            )
-        )
-        print(
-            "Attitude - e0: {:.3f} | e1: {:.3f} | e2: {:.3f} | e3: {:.3f}".format(
-                self.e0(0), self.e1(0), self.e2(0), self.e3(0)
-            )
-        )
-        print(
-            "Euler Angles - Spin φ : {:.2f}° | Nutation θ: {:.2f}° | Precession ψ: {:.2f}°".format(
-                self.phi(0), self.theta(0), self.psi(0)
-            )
-        )
-        print(
-            "Angular Velocity - ω1: {:.2f} rad/s | ω2: {:.2f} rad/s| ω3: {:.2f} rad/s".format(
-                self.w1(0), self.w2(0), self.w3(0)
-            )
-        )
         return None
 
-    def printNumericalIntegrationSettings(self):
-        """Prints out the Numerical Integration settings
+    def info(self):
+        """Prints out a summary of the data available about the Flight.
 
         Parameters
         ----------
         None
 
         Return
         ------
         None
         """
-        print("Maximum Allowed Flight Time: {:f} s".format(self.maxTime))
-        print("Maximum Allowed Time Step: {:f} s".format(self.maxTimeStep))
-        print("Minimum Allowed Time Step: {:e} s".format(self.minTimeStep))
-        print("Relative Error Tolerance: ", self.rtol)
-        print("Absolute Error Tolerance: ", self.atol)
-        print("Allow Event Overshoot: ", self.timeOvershoot)
-        print("Terminate Simulation on Apogee: ", self.terminateOnApogee)
-        print("Number of Time Steps Used: ", len(self.timeSteps))
-        print(
-            "Number of Derivative Functions Evaluation: ",
-            sum(self.functionEvaluationsPerTimeStep),
-        )
-        print(
-            "Average Function Evaluations per Time Step: {:3f}".format(
-                sum(self.functionEvaluationsPerTimeStep) / len(self.timeSteps)
-            )
-        )
-
+        self.prints.all()
         return None
 
-    def calculateStallWindVelocity(self, stallAngle):
+    def calculate_stall_wind_velocity(self, stall_angle):
         """Function to calculate the maximum wind velocity before the angle of
         attack exceeds a desired angle, at the instant of departing rail launch.
         Can be helpful if you know the exact stall angle of all aerodynamics
         surfaces.
 
         Parameters
         ----------
-        stallAngle : float
+        stall_angle : float
             Angle, in degrees, for which you would like to know the maximum wind
             speed before the angle of attack exceeds it
         Return
         ------
         None
         """
-        vF = self.outOfRailVelocity
+        vF = self.out_of_rail_velocity
 
         # Convert angle to radians
-        theta = self.inclination * np.pi / 180
-        stallAngle = stallAngle * np.pi / 180
+        theta = self.inclination * 3.14159265359 / 180
+        stall_angle = stall_angle * 3.14159265359 / 180
 
-        c = (math.cos(stallAngle) ** 2 - math.cos(theta) ** 2) / math.sin(
-            stallAngle
+        c = (math.cos(stall_angle) ** 2 - math.cos(theta) ** 2) / math.sin(
+            stall_angle
         ) ** 2
         wV = (
             2 * vF * math.cos(theta) / c
             + (
-                4 * vF * vF * math.cos(theta) * math.cos(theta) / (c ** 2)
+                4 * vF * vF * math.cos(theta) * math.cos(theta) / (c**2)
                 + 4 * 1 * vF * vF / c
             )
             ** 0.5
         ) / 2
 
-        # Convert stallAngle to degrees
-        stallAngle = stallAngle * 180 / np.pi
+        # Convert stall_angle to degrees
+        stall_angle = stall_angle * 180 / np.pi
         print(
             "Maximum wind velocity at Rail Departure time before angle of attack exceeds {:.3f}°: {:.3f} m/s".format(
-                stallAngle, wV
+                stall_angle, wV
             )
         )
 
         return None
 
-    def plot3dTrajectory(self):
-        """Plot a 3D graph of the trajectory
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get max and min x and y
-        maxZ = max(self.z[:, 1] - self.env.elevation)
-        maxX = max(self.x[:, 1])
-        minX = min(self.x[:, 1])
-        maxY = max(self.y[:, 1])
-        minY = min(self.y[:, 1])
-        maxXY = max(maxX, maxY)
-        minXY = min(minX, minY)
-
-        # Create figure
-        fig1 = plt.figure(figsize=(9, 9))
-        ax1 = plt.subplot(111, projection="3d")
-        ax1.plot(self.x[:, 1], self.y[:, 1], zs=0, zdir="z", linestyle="--")
-        ax1.plot(
-            self.x[:, 1],
-            self.z[:, 1] - self.env.elevation,
-            zs=minXY,
-            zdir="y",
-            linestyle="--",
-        )
-        ax1.plot(
-            self.y[:, 1],
-            self.z[:, 1] - self.env.elevation,
-            zs=minXY,
-            zdir="x",
-            linestyle="--",
-        )
-        ax1.plot(
-            self.x[:, 1], self.y[:, 1], self.z[:, 1] - self.env.elevation, linewidth="2"
-        )
-        ax1.scatter(0, 0, 0)
-        ax1.set_xlabel("X - East (m)")
-        ax1.set_ylabel("Y - North (m)")
-        ax1.set_zlabel("Z - Altitude Above Ground Level (m)")
-        ax1.set_title("Flight Trajectory")
-        ax1.set_zlim3d([0, maxZ])
-        ax1.set_ylim3d([minXY, maxXY])
-        ax1.set_xlim3d([minXY, maxXY])
-        ax1.view_init(15, 45)
-        plt.show()
+    def export_pressures(self, file_name, time_step):
+        """Exports the pressure experienced by the rocket during the flight to
+        an external file, the '.csv' format is recommended, as the columns will
+        be separated by commas. It can handle flights with or without
+        parachutes, although it is not possible to get a noisy pressure signal
+        if no parachute is added.
 
-        return None
+        If a parachute is added, the file will contain 3 columns: time in
+        seconds, clean pressure in Pascals and noisy pressure in Pascals.
+        For flights without parachutes, the third column will be discarded
 
-    def plotLinearKinematicsData(self):
-        """Prints out all Kinematics graphs available about the Flight
+        This function was created especially for the 'Projeto Jupiter'
+        Electronics Subsystems team and aims to help in configuring
+        micro-controllers.
 
         Parameters
         ----------
-        None
+        file_name : string
+            The final file name,
+        time_step : float
+            Time step desired for the final file
 
         Return
         ------
         None
         """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Velocity and acceleration plots
-        fig2 = plt.figure(figsize=(9, 12))
-
-        ax1 = plt.subplot(414)
-        ax1.plot(self.vx[:, 0], self.vx[:, 1], color="#ff7f0e")
-        ax1.set_xlim(0, self.tFinal)
-        ax1.set_title("Velocity X | Acceleration X")
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Velocity X (m/s)", color="#ff7f0e")
-        ax1.tick_params("y", colors="#ff7f0e")
-        ax1.grid(True)
-
-        ax1up = ax1.twinx()
-        ax1up.plot(self.ax[:, 0], self.ax[:, 1], color="#1f77b4")
-        ax1up.set_ylabel("Acceleration X (m/s²)", color="#1f77b4")
-        ax1up.tick_params("y", colors="#1f77b4")
-
-        ax2 = plt.subplot(413)
-        ax2.plot(self.vy[:, 0], self.vy[:, 1], color="#ff7f0e")
-        ax2.set_xlim(0, self.tFinal)
-        ax2.set_title("Velocity Y | Acceleration Y")
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Velocity Y (m/s)", color="#ff7f0e")
-        ax2.tick_params("y", colors="#ff7f0e")
-        ax2.grid(True)
-
-        ax2up = ax2.twinx()
-        ax2up.plot(self.ay[:, 0], self.ay[:, 1], color="#1f77b4")
-        ax2up.set_ylabel("Acceleration Y (m/s²)", color="#1f77b4")
-        ax2up.tick_params("y", colors="#1f77b4")
-
-        ax3 = plt.subplot(412)
-        ax3.plot(self.vz[:, 0], self.vz[:, 1], color="#ff7f0e")
-        ax3.set_xlim(0, self.tFinal)
-        ax3.set_title("Velocity Z | Acceleration Z")
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Velocity Z (m/s)", color="#ff7f0e")
-        ax3.tick_params("y", colors="#ff7f0e")
-        ax3.grid(True)
-
-        ax3up = ax3.twinx()
-        ax3up.plot(self.az[:, 0], self.az[:, 1], color="#1f77b4")
-        ax3up.set_ylabel("Acceleration Z (m/s²)", color="#1f77b4")
-        ax3up.tick_params("y", colors="#1f77b4")
-
-        ax4 = plt.subplot(411)
-        ax4.plot(self.speed[:, 0], self.speed[:, 1], color="#ff7f0e")
-        ax4.set_xlim(0, self.tFinal)
-        ax4.set_title("Velocity Magnitude | Acceleration Magnitude")
-        ax4.set_xlabel("Time (s)")
-        ax4.set_ylabel("Velocity (m/s)", color="#ff7f0e")
-        ax4.tick_params("y", colors="#ff7f0e")
-        ax4.grid(True)
-
-        ax4up = ax4.twinx()
-        ax4up.plot(self.acceleration[:, 0], self.acceleration[:, 1], color="#1f77b4")
-        ax4up.set_ylabel("Acceleration (m/s²)", color="#1f77b4")
-        ax4up.tick_params("y", colors="#1f77b4")
 
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-        return None
+        time_points = np.arange(0, self.t_final, time_step)
 
-    def plotAttitudeData(self):
-        """Prints out all Angular position graphs available about the Flight
+        # Create the file
+        file = open(file_name, "w")
 
-        Parameters
-        ----------
-        None
+        if len(self.rocket.parachutes) == 0:
+            pressure = self.env.pressure(self.z(time_points))
+            for i in range(0, time_points.size, 1):
+                file.write("{:f}, {:.5f}\n".format(time_points[i], pressure[i]))
 
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
         else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        # Angular position plots
-        fig3 = plt.figure(figsize=(9, 12))
-
-        ax1 = plt.subplot(411)
-        ax1.plot(self.e0[:, 0], self.e0[:, 1], label="$e_0$")
-        ax1.plot(self.e1[:, 0], self.e1[:, 1], label="$e_1$")
-        ax1.plot(self.e2[:, 0], self.e2[:, 1], label="$e_2$")
-        ax1.plot(self.e3[:, 0], self.e3[:, 1], label="$e_3$")
-        ax1.set_xlim(0, eventTime)
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Euler Parameters")
-        ax1.set_title("Euler Parameters")
-        ax1.legend()
-        ax1.grid(True)
-
-        ax2 = plt.subplot(412)
-        ax2.plot(self.psi[:, 0], self.psi[:, 1])
-        ax2.set_xlim(0, eventTime)
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("ψ (°)")
-        ax2.set_title("Euler Precession Angle")
-        ax2.grid(True)
-
-        ax3 = plt.subplot(413)
-        ax3.plot(self.theta[:, 0], self.theta[:, 1], label="θ - Nutation")
-        ax3.set_xlim(0, eventTime)
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("θ (°)")
-        ax3.set_title("Euler Nutation Angle")
-        ax3.grid(True)
-
-        ax4 = plt.subplot(414)
-        ax4.plot(self.phi[:, 0], self.phi[:, 1], label="φ - Spin")
-        ax4.set_xlim(0, eventTime)
-        ax4.set_xlabel("Time (s)")
-        ax4.set_ylabel("φ (°)")
-        ax4.set_title("Euler Spin Angle")
-        ax4.grid(True)
+            for parachute in self.rocket.parachutes:
+                for i in range(0, time_points.size, 1):
+                    pCl = Function(
+                        parachute.clean_pressure_signal,
+                        "Time (s)",
+                        "Pressure - Without Noise (Pa)",
+                        "linear",
+                    )(time_points[i])
+                    pNs = Function(
+                        parachute.noisy_pressure_signal,
+                        "Time (s)",
+                        "Pressure - With Noise (Pa)",
+                        "linear",
+                    )(time_points[i])
+                    file.write(
+                        "{:f}, {:.5f}, {:.5f}\n".format(time_points[i], pCl, pNs)
+                    )
+                # We need to save only 1 parachute data
+                pass
 
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
+        file.close()
 
         return None
 
-    def plotFlightPathAngleData(self):
-        """Prints out Flight path and Rocket Attitude angle graphs available
-        about the Flight
+    def export_data(self, file_name, *variables, time_step=None):
+        """Exports flight data to a comma separated value file (.csv).
+
+        Data is exported in columns, with the first column representing time
+        steps. The first line of the file is a header line, specifying the
+        meaning of each column and its units.
 
         Parameters
         ----------
-        None
+        file_name : string
+            The file name or path of the exported file. Example: flight_data.csv
+            Do not use forbidden characters, such as '/' in Linux/Unix and
+            '<, >, :, ", /, \\, | ?, *' in Windows.
+        variables : strings, optional
+            Names of the data variables which shall be exported. Must be Flight
+            class attributes which are instances of the Function class. Usage
+            example: test_flight.export_data('test.csv', 'z', 'angle_of_attack',
+            'mach_number').
+        time_step : float, optional
+            Time step desired for the data. If None, all integration time steps
+            will be exported. Otherwise, linear interpolation is carried out to
+            calculate values at the desired time steps. Example: 0.001.
+        """
+
+        # Fast evaluation for the most basic scenario
+        if time_step is None and len(variables) == 0:
+            np.savetxt(
+                file_name,
+                self.solution,
+                fmt="%.6f",
+                delimiter=",",
+                header=""
+                "Time (s),"
+                "X (m),"
+                "Y (m),"
+                "Z (m),"
+                "E0,"
+                "E1,"
+                "E2,"
+                "E3,"
+                "W1 (rad/s),"
+                "W2 (rad/s),"
+                "W3 (rad/s)",
+            )
+            return
+
+        # Not so fast evaluation for general case
+        if variables is None:
+            variables = [
+                "x",
+                "y",
+                "z",
+                "vx",
+                "vy",
+                "vz",
+                "e0",
+                "e1",
+                "e2",
+                "e3",
+                "w1",
+                "w2",
+                "w3",
+            ]
 
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
+        if time_step is None:
+            time_points = self.time
         else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        # Path, Attitude and Lateral Attitude Angle
-        # Angular position plots
-        fig5 = plt.figure(figsize=(9, 6))
-
-        ax1 = plt.subplot(211)
-        ax1.plot(self.pathAngle[:, 0], self.pathAngle[:, 1], label="Flight Path Angle")
-        ax1.plot(
-            self.attitudeAngle[:, 0],
-            self.attitudeAngle[:, 1],
-            label="Rocket Attitude Angle",
-        )
-        ax1.set_xlim(0, eventTime)
-        ax1.legend()
-        ax1.grid(True)
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Angle (°)")
-        ax1.set_title("Flight Path and Attitude Angle")
-
-        ax2 = plt.subplot(212)
-        ax2.plot(self.lateralAttitudeAngle[:, 0], self.lateralAttitudeAngle[:, 1])
-        ax2.set_xlim(0, eventTime)
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Lateral Attitude Angle (°)")
-        ax2.set_title("Lateral Attitude Angle")
-        ax2.grid(True)
+            time_points = np.arange(self.t_initial, self.t_final, time_step)
 
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        return None
+        exported_matrix = [time_points]
+        exported_header = "Time (s)"
 
-    def plotAngularKinematicsData(self):
-        """Prints out all Angular velocity and acceleration graphs available
-        about the Flight
+        # Loop through variables, get points and names (for the header)
+        for variable in variables:
+            if variable in self.__dict__.keys():
+                variable_function = self.__dict__[variable]
+            # Deal with decorated Flight methods
+            else:
+                try:
+                    obj = getattr(self.__class__, variable)
+                    variable_function = obj.__get__(self, self.__class__)
+                except AttributeError:
+                    raise AttributeError(
+                        "Variable '{}' not found in Flight class".format(variable)
+                    )
+            variable_points = variable_function(time_points)
+            exported_matrix += [variable_points]
+            exported_header += ", " + variable_function.__outputs__[0]
 
-        Parameters
-        ----------
-        None
+        exported_matrix = np.array(exported_matrix).T  # Fix matrix orientation
 
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
-        else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        # Angular velocity and acceleration plots
-        fig4 = plt.figure(figsize=(9, 9))
-        ax1 = plt.subplot(311)
-        ax1.plot(self.w1[:, 0], self.w1[:, 1], color="#ff7f0e")
-        ax1.set_xlim(0, eventTime)
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Angular Velocity - ${\omega_1}$ (rad/s)", color="#ff7f0e")
-        ax1.set_title(
-            "Angular Velocity ${\omega_1}$ | Angular Acceleration ${\\alpha_1}$"
-        )
-        ax1.tick_params("y", colors="#ff7f0e")
-        ax1.grid(True)
-
-        ax1up = ax1.twinx()
-        ax1up.plot(self.alpha1[:, 0], self.alpha1[:, 1], color="#1f77b4")
-        ax1up.set_ylabel(
-            "Angular Acceleration - ${\\alpha_1}$ (rad/s²)", color="#1f77b4"
-        )
-        ax1up.tick_params("y", colors="#1f77b4")
-
-        ax2 = plt.subplot(312)
-        ax2.plot(self.w2[:, 0], self.w2[:, 1], color="#ff7f0e")
-        ax2.set_xlim(0, eventTime)
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Angular Velocity - ${\omega_2}$ (rad/s)", color="#ff7f0e")
-        ax2.set_title(
-            "Angular Velocity ${\omega_2}$ | Angular Acceleration ${\\alpha_2}$"
-        )
-        ax2.tick_params("y", colors="#ff7f0e")
-        ax2.grid(True)
-
-        ax2up = ax2.twinx()
-        ax2up.plot(self.alpha2[:, 0], self.alpha2[:, 1], color="#1f77b4")
-        ax2up.set_ylabel(
-            "Angular Acceleration - ${\\alpha_2}$ (rad/s²)", color="#1f77b4"
-        )
-        ax2up.tick_params("y", colors="#1f77b4")
-
-        ax3 = plt.subplot(313)
-        ax3.plot(self.w3[:, 0], self.w3[:, 1], color="#ff7f0e")
-        ax3.set_xlim(0, eventTime)
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Angular Velocity - ${\omega_3}$ (rad/s)", color="#ff7f0e")
-        ax3.set_title(
-            "Angular Velocity ${\omega_3}$ | Angular Acceleration ${\\alpha_3}$"
-        )
-        ax3.tick_params("y", colors="#ff7f0e")
-        ax3.grid(True)
-
-        ax3up = ax3.twinx()
-        ax3up.plot(self.alpha3[:, 0], self.alpha3[:, 1], color="#1f77b4")
-        ax3up.set_ylabel(
-            "Angular Acceleration - ${\\alpha_3}$ (rad/s²)", color="#1f77b4"
+        np.savetxt(
+            file_name,
+            exported_matrix,
+            fmt="%.6f",
+            delimiter=",",
+            header=exported_header,
+            encoding="utf-8",
         )
-        ax3up.tick_params("y", colors="#1f77b4")
 
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
+        return
 
-        return None
-
-    def plotTrajectoryForceData(self):
-        """Prints out all Forces and Moments graphs available about the Flight
+    def export_kml(
+        self,
+        file_name="trajectory.kml",
+        time_step=None,
+        extrude=True,
+        color="641400F0",
+        altitude_mode="absolute",
+    ):
+        """Exports flight data to a .kml file, which can be opened with Google
+        Earth to display the rocket's trajectory.
 
         Parameters
         ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of out of rail time
-        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
-        outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
-        )
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
-        else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        # Rail Button Forces
-        fig6 = plt.figure(figsize=(9, 6))
-
-        ax1 = plt.subplot(211)
-        ax1.plot(
-            self.railButton1NormalForce[:outOfRailTimeIndex, 0],
-            self.railButton1NormalForce[:outOfRailTimeIndex, 1],
-            label="Upper Rail Button",
-        )
-        ax1.plot(
-            self.railButton2NormalForce[:outOfRailTimeIndex, 0],
-            self.railButton2NormalForce[:outOfRailTimeIndex, 1],
-            label="Lower Rail Button",
-        )
-        ax1.set_xlim(0, self.outOfRailTime if self.outOfRailTime > 0 else self.tFinal)
-        ax1.legend()
-        ax1.grid(True)
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Normal Force (N)")
-        ax1.set_title("Rail Buttons Normal Force")
-
-        ax2 = plt.subplot(212)
-        ax2.plot(
-            self.railButton1ShearForce[:outOfRailTimeIndex, 0],
-            self.railButton1ShearForce[:outOfRailTimeIndex, 1],
-            label="Upper Rail Button",
-        )
-        ax2.plot(
-            self.railButton2ShearForce[:outOfRailTimeIndex, 0],
-            self.railButton2ShearForce[:outOfRailTimeIndex, 1],
-            label="Lower Rail Button",
-        )
-        ax2.set_xlim(0, self.outOfRailTime if self.outOfRailTime > 0 else self.tFinal)
-        ax2.legend()
-        ax2.grid(True)
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Shear Force (N)")
-        ax2.set_title("Rail Buttons Shear Force")
-
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        # Aerodynamic force and moment plots
-        fig7 = plt.figure(figsize=(9, 12))
-
-        ax1 = plt.subplot(411)
-        ax1.plot(
-            self.aerodynamicLift[:eventTimeIndex, 0],
-            self.aerodynamicLift[:eventTimeIndex, 1],
-            label="Resultant",
-        )
-        ax1.plot(self.R1[:eventTimeIndex, 0], self.R1[:eventTimeIndex, 1], label="R1")
-        ax1.plot(self.R2[:eventTimeIndex, 0], self.R2[:eventTimeIndex, 1], label="R2")
-        ax1.set_xlim(0, eventTime)
-        ax1.legend()
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Lift Force (N)")
-        ax1.set_title("Aerodynamic Lift Resultant Force")
-        ax1.grid()
-
-        ax2 = plt.subplot(412)
-        ax2.plot(
-            self.aerodynamicDrag[:eventTimeIndex, 0],
-            self.aerodynamicDrag[:eventTimeIndex, 1],
-        )
-        ax2.set_xlim(0, eventTime)
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Drag Force (N)")
-        ax2.set_title("Aerodynamic Drag Force")
-        ax2.grid()
-
-        ax3 = plt.subplot(413)
-        ax3.plot(
-            self.aerodynamicBendingMoment[:eventTimeIndex, 0],
-            self.aerodynamicBendingMoment[:eventTimeIndex, 1],
-            label="Resultant",
-        )
-        ax3.plot(self.M1[:eventTimeIndex, 0], self.M1[:eventTimeIndex, 1], label="M1")
-        ax3.plot(self.M2[:eventTimeIndex, 0], self.M2[:eventTimeIndex, 1], label="M2")
-        ax3.set_xlim(0, eventTime)
-        ax3.legend()
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Bending Moment (N m)")
-        ax3.set_title("Aerodynamic Bending Resultant Moment")
-        ax3.grid()
-
-        ax4 = plt.subplot(414)
-        ax4.plot(
-            self.aerodynamicSpinMoment[:eventTimeIndex, 0],
-            self.aerodynamicSpinMoment[:eventTimeIndex, 1],
-        )
-        ax4.set_xlim(0, eventTime)
-        ax4.set_xlabel("Time (s)")
-        ax4.set_ylabel("Spin Moment (N m)")
-        ax4.set_title("Aerodynamic Spin Moment")
-        ax4.grid()
-
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        return None
-
-    def plotEnergyData(self):
-        """Prints out all Energy components graphs available about the Flight
-
+        file_name : string
+            The file name or path of the exported file. Example: flight_data.csv
+            Do not use forbidden characters, such as '/' in Linux/Unix and
+            '<, >, :, ", /, \\, | ?, *' in Windows.
+        time_step : float, optional
+            Time step desired for the data. If None, all integration time steps
+            will be exported. Otherwise, linear interpolation is carried out to
+            calculate values at the desired time steps. Example: 0.001.
+        extrude: bool, optional
+            To be used if you want to project the path over ground by using an
+            extruded polygon. In case False only the linestring containing the
+            flight path will be created. Default is True.
+        color : str, optional
+            Color of your trajectory path, need to be used in specific kml
+            format. Refer to http://www.zonums.com/gmaps/kml_color/ for more
+            info.
+        altitude_mode: str
+            Select elevation values format to be used on the kml file. Use
+            'relativetoground' if you want use Above Ground Level elevation, or
+            'absolute' if you want to parse elevation using Above Sea Level.
+            Default is 'relativetoground'. Only works properly if the ground
+            level is flat. Change to 'absolute' if the terrain is to irregular
+            or contains mountains.
         Returns
         -------
         None
         """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of out of rail time
-        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
-        outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
-        )
-
-        # Get index of time before parachute event
-        if len(self.parachuteEvents) > 0:
-            eventTime = self.parachuteEvents[0][0] + self.parachuteEvents[0][1].lag
-            eventTimeIndex = np.nonzero(self.x[:, 0] == eventTime)[0][0]
-        else:
-            eventTime = self.tFinal
-            eventTimeIndex = -1
-
-        fig8 = plt.figure(figsize=(9, 9))
-
-        ax1 = plt.subplot(411)
-        ax1.plot(
-            self.kineticEnergy[:, 0], self.kineticEnergy[:, 1], label="Kinetic Energy"
-        )
-        ax1.plot(
-            self.rotationalEnergy[:, 0],
-            self.rotationalEnergy[:, 1],
-            label="Rotational Energy",
-        )
-        ax1.plot(
-            self.translationalEnergy[:, 0],
-            self.translationalEnergy[:, 1],
-            label="Translational Energy",
-        )
-        ax1.set_xlim(0, self.apogeeTime if self.apogeeTime != 0.0 else self.tFinal)
-        ax1.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax1.set_title("Kinetic Energy Components")
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Energy (J)")
-
-        ax1.legend()
-        ax1.grid()
-
-        ax2 = plt.subplot(412)
-        ax2.plot(self.totalEnergy[:, 0], self.totalEnergy[:, 1], label="Total Energy")
-        ax2.plot(
-            self.kineticEnergy[:, 0], self.kineticEnergy[:, 1], label="Kinetic Energy"
-        )
-        ax2.plot(
-            self.potentialEnergy[:, 0],
-            self.potentialEnergy[:, 1],
-            label="Potential Energy",
-        )
-        ax2.set_xlim(0, self.apogeeTime if self.apogeeTime != 0.0 else self.tFinal)
-        ax2.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax2.set_title("Total Mechanical Energy Components")
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Energy (J)")
-        ax2.legend()
-        ax2.grid()
-
-        ax3 = plt.subplot(413)
-        ax3.plot(self.thrustPower[:, 0], self.thrustPower[:, 1], label="|Thrust Power|")
-        ax3.set_xlim(0, self.rocket.motor.burnOutTime)
-        ax3.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax3.set_title("Thrust Absolute Power")
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Power (W)")
-        ax3.legend()
-        ax3.grid()
-
-        ax4 = plt.subplot(414)
-        ax4.plot(self.dragPower[:, 0], -self.dragPower[:, 1], label="|Drag Power|")
-        ax4.set_xlim(0, self.apogeeTime if self.apogeeTime != 0.0 else self.tFinal)
-        ax3.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax4.set_title("Drag Absolute Power")
-        ax4.set_xlabel("Time (s)")
-        ax4.set_ylabel("Power (W)")
-        ax4.legend()
-        ax4.grid()
-
-        plt.subplots_adjust(hspace=1)
-        plt.show()
-
-        return None
-
-    def plotFluidMechanicsData(self):
-        """Prints out a summary of the Fluid Mechanics graphs available about
-        the Flight
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Get index of out of rail time
-        outOfRailTimeIndexes = np.nonzero(self.x[:, 0] == self.outOfRailTime)
-        outOfRailTimeIndex = (
-            -1 if len(outOfRailTimeIndexes) == 0 else outOfRailTimeIndexes[0][0]
-        )
-
-        # Trajectory Fluid Mechanics Plots
-        fig10 = plt.figure(figsize=(9, 12))
-
-        ax1 = plt.subplot(411)
-        ax1.plot(self.MachNumber[:, 0], self.MachNumber[:, 1])
-        ax1.set_xlim(0, self.tFinal)
-        ax1.set_title("Mach Number")
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Mach Number")
-        ax1.grid()
-
-        ax2 = plt.subplot(412)
-        ax2.plot(self.ReynoldsNumber[:, 0], self.ReynoldsNumber[:, 1])
-        ax2.set_xlim(0, self.tFinal)
-        ax2.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax2.set_title("Reynolds Number")
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Reynolds Number")
-        ax2.grid()
-
-        ax3 = plt.subplot(413)
-        ax3.plot(
-            self.dynamicPressure[:, 0],
-            self.dynamicPressure[:, 1],
-            label="Dynamic Pressure",
-        )
-        ax3.plot(
-            self.totalPressure[:, 0], self.totalPressure[:, 1], label="Total Pressure"
-        )
-        ax3.plot(self.pressure[:, 0], self.pressure[:, 1], label="Static Pressure")
-        ax3.set_xlim(0, self.tFinal)
-        ax3.legend()
-        ax3.ticklabel_format(style="sci", axis="y", scilimits=(0, 0))
-        ax3.set_title("Total and Dynamic Pressure")
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Pressure (Pa)")
-        ax3.grid()
-
-        ax4 = plt.subplot(414)
-        ax4.plot(self.angleOfAttack[:, 0], self.angleOfAttack[:, 1])
-        ax4.set_xlim(
-            self.outOfRailTime, 10 * self.outOfRailTime + 1
-        )  # +1 Prevents problem when self.outOfRailTime=0
-        ax4.set_ylim(0, self.angleOfAttack(self.outOfRailTime))
-        ax4.set_title("Angle of Attack")
-        ax4.set_xlabel("Time (s)")
-        ax4.set_ylabel("Angle of Attack (°)")
-        ax4.grid()
-
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        return None
-
-    def calculateFinFlutterAnalysis(self, finThickness, shearModulus):
-        """Calculate, create and plot the Fin Flutter velocity, based on the
-        pressure profile provided by Atmospheric model selected. It considers the
-        Flutter Boundary Equation that is based on a calculation published in
-        NACA Technical Paper 4197.
-        Be careful, these results are only estimates of a real problem and may
-        not be useful for fins made from non-isotropic materials. These results
-        should not be used as a way to fully prove the safety of any rocket’s fins.
-        IMPORTANT: This function works if only a single set of fins is added
-
-        Parameters
-        ----------
-        finThickness : float
-            The fin thickness, in meters
-        shearModulus : float
-            Shear Modulus of fins' material, must be given in Pascal
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        s = (self.rocket.tipChord + self.rocket.rootChord) * self.rocket.span / 2
-        ar = self.rocket.span * self.rocket.span / s
-        la = self.rocket.tipChord / self.rocket.rootChord
-
-        # Calculate the Fin Flutter Mach Number
-        self.flutterMachNumber = (
-            (shearModulus * 2 * (ar + 2) * (finThickness / self.rocket.rootChord) ** 3)
-            / (1.337 * (ar ** 3) * (la + 1) * self.pressure)
-        ) ** 0.5
-
-        # Calculate difference between Fin Flutter Mach Number and the Rocket Speed
-        self.difference = self.flutterMachNumber - self.MachNumber
-
-        # Calculate a safety factor for flutter
-        self.safetyFactor = self.flutterMachNumber / self.MachNumber
-
-        # Calculate the minimun Fin Flutter Mach Number and Velocity
-        # Calculate the time and height of minimun Fin Flutter Mach Number
-        minflutterMachNumberTimeIndex = np.argmin(self.flutterMachNumber[:, 1])
-        minflutterMachNumber = self.flutterMachNumber[minflutterMachNumberTimeIndex, 1]
-        minMFTime = self.flutterMachNumber[minflutterMachNumberTimeIndex, 0]
-        minMFHeight = self.z(minMFTime) - self.env.elevation
-        minMFVelocity = minflutterMachNumber * self.env.speedOfSound(minMFHeight)
-
-        # Calculate minimum difference between Fin Flutter Mach Number and the Rocket Speed
-        # Calculate the time and height of the difference ...
-        minDifferenceTimeIndex = np.argmin(self.difference[:, 1])
-        minDif = self.difference[minDifferenceTimeIndex, 1]
-        minDifTime = self.difference[minDifferenceTimeIndex, 0]
-        minDifHeight = self.z(minDifTime) - self.env.elevation
-        minDifVelocity = minDif * self.env.speedOfSound(minDifHeight)
-
-        # Calculate the minimun Fin Flutter Safety factor
-        # Calculate the time and height of minimun Fin Flutter Safety factor
-        minSFTimeIndex = np.argmin(self.safetyFactor[:, 1])
-        minSF = self.safetyFactor[minSFTimeIndex, 1]
-        minSFTime = self.safetyFactor[minSFTimeIndex, 0]
-        minSFHeight = self.z(minSFTime) - self.env.elevation
-
-        # Print fin's geometric parameters
-        print("Fin's geometric parameters")
-        print("Surface area (S): {:.4f} m2".format(s))
-        print("Aspect ratio (AR): {:.3f}".format(ar))
-        print("TipChord/RootChord = \u03BB = {:.3f}".format(la))
-        print("Fin Thickness: {:.5f} m".format(finThickness))
-
-        # Print fin's material properties
-        print("\n\nFin's material properties")
-        print("Shear Modulus (G): {:.3e} Pa".format(shearModulus))
-
-        # Print a summary of the Fin Flutter Analysis
-        print("\n\nFin Flutter Analysis")
-        print(
-            "Minimum Fin Flutter Velocity: {:.3f} m/s at {:.2f} s".format(
-                minMFVelocity, minMFTime
-            )
-        )
-        print("Minimum Fin Flutter Mach Number: {:.3f} ".format(minflutterMachNumber))
-        # print(
-        #    "Altitude of minimum Fin Flutter Velocity: {:.3f} m (AGL)".format(
-        #        minMFHeight
-        #    )
-        # )
-        print(
-            "Minimum of (Fin Flutter Mach Number - Rocket Speed): {:.3f} m/s at {:.2f} s".format(
-                minDifVelocity, minDifTime
-            )
-        )
-        print(
-            "Minimum of (Fin Flutter Mach Number - Rocket Speed): {:.3f} Mach at {:.2f} s".format(
-                minDif, minDifTime
-            )
-        )
-        # print(
-        #    "Altitude of minimum (Fin Flutter Mach Number - Rocket Speed): {:.3f} m (AGL)".format(
-        #        minDifHeight
-        #    )
-        # )
-        print(
-            "Minimum Fin Flutter Safety Factor: {:.3f} at {:.2f} s".format(
-                minSF, minSFTime
-            )
-        )
-        print(
-            "Altitude of minimum Fin Flutter Safety Factor: {:.3f} m (AGL)\n\n".format(
-                minSFHeight
-            )
-        )
-
-        # Create plots
-        fig12 = plt.figure(figsize=(6, 9))
-        ax1 = plt.subplot(311)
-        ax1.plot()
-        ax1.plot(
-            self.flutterMachNumber[:, 0],
-            self.flutterMachNumber[:, 1],
-            label="Fin flutter Mach Number",
-        )
-        ax1.plot(
-            self.MachNumber[:, 0],
-            self.MachNumber[:, 1],
-            label="Rocket Freestream Speed",
-        )
-        ax1.set_xlim(0, self.apogeeTime if self.apogeeTime != 0.0 else self.tFinal)
-        ax1.set_title("Fin Flutter Mach Number x Time(s)")
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Mach")
-        ax1.legend()
-        ax1.grid(True)
-
-        ax2 = plt.subplot(312)
-        ax2.plot(self.difference[:, 0], self.difference[:, 1])
-        ax2.set_xlim(0, self.apogeeTime if self.apogeeTime != 0.0 else self.tFinal)
-        ax2.set_title("Mach flutter - Freestream velocity")
-        ax2.set_xlabel("Time (s)")
-        ax2.set_ylabel("Mach")
-        ax2.grid()
-
-        ax3 = plt.subplot(313)
-        ax3.plot(self.safetyFactor[:, 0], self.safetyFactor[:, 1])
-        ax3.set_xlim(self.outOfRailTime, self.apogeeTime)
-        ax3.set_ylim(0, 6)
-        ax3.set_title("Fin Flutter Safety Factor")
-        ax3.set_xlabel("Time (s)")
-        ax3.set_ylabel("Safety Factor")
-        ax3.grid()
-
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        return None
-
-    def plotStabilityAndControlData(self):
-        """Prints out Rocket Stability and Control parameters graphs available
-        about the Flight
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        fig9 = plt.figure(figsize=(9, 6))
-
-        ax1 = plt.subplot(211)
-        ax1.plot(self.staticMargin[:, 0], self.staticMargin[:, 1])
-        ax1.set_xlim(0, self.staticMargin[:, 0][-1])
-        ax1.set_title("Static Margin")
-        ax1.set_xlabel("Time (s)")
-        ax1.set_ylabel("Static Margin (c)")
-        ax1.grid()
-
-        ax2 = plt.subplot(212)
-        maxAttitude = max(self.attitudeFrequencyResponse[:, 1])
-        maxAttitude = maxAttitude if maxAttitude != 0 else 1
-        ax2.plot(
-            self.attitudeFrequencyResponse[:, 0],
-            self.attitudeFrequencyResponse[:, 1] / maxAttitude,
-            label="Attitude Angle",
-        )
-        maxOmega1 = max(self.omega1FrequencyResponse[:, 1])
-        maxOmega1 = maxOmega1 if maxOmega1 != 0 else 1
-        ax2.plot(
-            self.omega1FrequencyResponse[:, 0],
-            self.omega1FrequencyResponse[:, 1] / maxOmega1,
-            label="$\omega_1$",
-        )
-        maxOmega2 = max(self.omega2FrequencyResponse[:, 1])
-        maxOmega2 = maxOmega2 if maxOmega2 != 0 else 1
-        ax2.plot(
-            self.omega2FrequencyResponse[:, 0],
-            self.omega2FrequencyResponse[:, 1] / maxOmega2,
-            label="$\omega_2$",
-        )
-        maxOmega3 = max(self.omega3FrequencyResponse[:, 1])
-        maxOmega3 = maxOmega3 if maxOmega3 != 0 else 1
-        ax2.plot(
-            self.omega3FrequencyResponse[:, 0],
-            self.omega3FrequencyResponse[:, 1] / maxOmega3,
-            label="$\omega_3$",
-        )
-        ax2.set_title("Frequency Response")
-        ax2.set_xlabel("Frequency (Hz)")
-        ax2.set_ylabel("Amplitude Magnitude Normalized")
-        ax2.set_xlim(0, 5)
-        ax2.legend()
-        ax2.grid()
-
-        plt.subplots_adjust(hspace=0.5)
-        plt.show()
-
-        return None
-
-    def plotPressureSignals(self):
-        """Prints out all Parachute Trigger Pressure Signals.
-        This function can be called also for plot pressure data for flights
-        without Parachutes, in this case the Pressure Signals will be simply
-        the pressure provided by the atmosphericModel, at Flight z positions.
-        This means that no noise will be considered if at least one parachute
-        has not been added.
-
-        This function aims to help the engineer to visually check if there
-        are anomalies with the Flight Simulation.
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        if len(self.rocket.parachutes) == 0:
-            plt.figure()
-            ax1 = plt.subplot(111)
-            ax1.plot(self.z[:, 0], self.env.pressure(self.z[:, 1]))
-            ax1.set_title("Pressure at Rocket's Altitude")
-            ax1.set_xlabel("Time (s)")
-            ax1.set_ylabel("Pressure (Pa)")
-            ax1.set_xlim(0, self.tFinal)
-            ax1.grid()
-
-            plt.show()
-
-        else:
-            for parachute in self.rocket.parachutes:
-                print("Parachute: ", parachute.name)
-                parachute.noiseSignalFunction()
-                parachute.noisyPressureSignalFunction()
-                parachute.cleanPressureSignalFunction()
-
-        return None
-
-    def exportPressures(self, fileName, timeStep):
-        """Exports the pressure experienced by the rocket during the flight to
-        an external file, the '.csv' format is recommended, as the columns will
-        be separated by commas. It can handle flights with or without parachutes,
-        although it is not possible to get a noisy pressure signal if no
-        parachute is added.
-
-        If a parachute is added, the file will contain 3 columns: time in seconds,
-        clean pressure in Pascals and noisy pressure in Pascals. For flights without
-        parachutes, the third column will be discarded
-
-        This function was created especially for the Projeto Jupiter Electronics
-        Subsystems team and aims to help in configuring microcontrollers.
-
-        Parameters
-        ----------
-        fileName : string
-            The final file name,
-        timeStep : float
-            Time step desired for the final file
-
-        Return
-        ------
-        None
-        """
-        if self.postProcessed is False:
-            self.postProcess()
-
-        timePoints = np.arange(0, self.tFinal, timeStep)
-
-        # Create the file
-        file = open(fileName, "w")
-
-        if len(self.rocket.parachutes) == 0:
-            pressure = self.env.pressure(self.z(timePoints))
-            for i in range(0, timePoints.size, 1):
-                file.write("{:f}, {:.5f}\n".format(timePoints[i], pressure[i]))
-
+        # Define time points vector
+        if time_step is None:
+            time_points = self.time
         else:
-            for parachute in self.rocket.parachutes:
-                for i in range(0, timePoints.size, 1):
-                    pCl = parachute.cleanPressureSignalFunction(timePoints[i])
-                    pNs = parachute.noisyPressureSignalFunction(timePoints[i])
-                    file.write("{:f}, {:.5f}, {:.5f}\n".format(timePoints[i], pCl, pNs))
-                # We need to save only 1 parachute data
-                pass
-
-        file.close()
+            time_points = np.arange(self.t_initial, self.t_final + time_step, time_step)
+        # Open kml file with simplekml library
+        kml = simplekml.Kml(open=1)
+        trajectory = kml.newlinestring(name="Rocket Trajectory - Powered by RocketPy")
+        coords = []
+        if altitude_mode == "relativetoground":
+            # In this mode the elevation data will be the Above Ground Level
+            # elevation. Only works properly if the ground level is similar to
+            # a plane, i.e. it might not work well if the terrain has mountains
+            for t in time_points:
+                coords.append(
+                    (
+                        self.longitude(t),
+                        self.latitude(t),
+                        self.z(t) - self.env.elevation,
+                    )
+                )
+            trajectory.coords = coords
+            trajectory.altitudemode = simplekml.AltitudeMode.relativetoground
+        else:  # altitude_mode == 'absolute'
+            # In this case the elevation data will be the Above Sea Level elevation
+            # Ensure you use the correct value on self.env.elevation, otherwise
+            # the trajectory path can be offset from ground
+            for t in time_points:
+                coords.append((self.longitude(t), self.latitude(t), self.z(t)))
+            trajectory.coords = coords
+            trajectory.altitudemode = simplekml.AltitudeMode.absolute
+        # Modify style of trajectory linestring
+        trajectory.style.linestyle.color = color
+        trajectory.style.polystyle.color = color
+        if extrude:
+            trajectory.extrude = 1
+        # Save the KML
+        kml.save(file_name)
+        print("File ", file_name, " saved with success!")
 
         return None
 
-    def allInfo(self):
+    def all_info(self):
         """Prints out all data and graphs available about the Flight.
 
         Parameters
         ----------
         None
 
         Return
         ------
         None
         """
-        # Post-process results
-        if self.postProcessed is False:
-            self.postProcess()
-
-        # Print initial conditions
-        print("Initial Conditions\n")
-        self.printInitialConditionsData()
-
-        # Print launch rail orientation
-        print("\n\nLaunch Rail Orientation\n")
-        print("Launch Rail Inclination: {:.2f}°".format(self.inclination))
-        print("Launch Rail Heading: {:.2f}°\n\n".format(self.heading))
 
         # Print a summary of data about the flight
         self.info()
 
-        print("\n\nNumerical Integration Information\n")
-        self.printNumericalIntegrationSettings()
-
-        print("\n\nTrajectory 3d Plot\n")
-        self.plot3dTrajectory()
-
-        print("\n\nTrajectory Kinematic Plots\n")
-        self.plotLinearKinematicsData()
-
-        print("\n\nAngular Position Plots\n")
-        self.plotFlightPathAngleData()
-
-        print("\n\nPath, Attitude and Lateral Attitude Angle plots\n")
-        self.plotAttitudeData()
-
-        print("\n\nTrajectory Angular Velocity and Acceleration Plots\n")
-        self.plotAngularKinematicsData()
-
-        print("\n\nTrajectory Force Plots\n")
-        self.plotTrajectoryForceData()
-
-        print("\n\nTrajectory Energy Plots\n")
-        self.plotEnergyData()
-
-        print("\n\nTrajectory Fluid Mechanics Plots\n")
-        self.plotFluidMechanicsData()
-
-        print("\n\nTrajectory Stability and Control Plots\n")
-        self.plotStabilityAndControlData()
+        self.plots.all()
 
         return None
 
     def animate(self, start=0, stop=None, fps=12, speed=4, elev=None, azim=None):
         """Plays an animation of the flight. Not implemented yet. Only
         kinda works outside notebook.
         """
         # Set up stopping time
-        stop = self.tFinal if stop is None else stop
+        stop = self.t_final if stop is None else stop
         # Speed = 4 makes it almost real time - matplotlib is way to slow
         # Set up graph
         fig = plt.figure(figsize=(18, 15))
         axes = fig.gca(projection="3d")
         # Initialize time
-        timeRange = np.linspace(start, stop, fps * (stop - start))
+        time_range = np.linspace(start, stop, fps * (stop - start))
         # Initialize first frame
         axes.set_title("Trajectory and Velocity Animation")
         axes.set_xlabel("X (m)")
         axes.set_ylabel("Y (m)")
         axes.set_zlabel("Z (m)")
         axes.view_init(elev, azim)
         R = axes.quiver(0, 0, 0, 0, 0, 0, color="r", label="Rocket")
         V = axes.quiver(0, 0, 0, 0, 0, 0, color="g", label="Velocity")
         W = axes.quiver(0, 0, 0, 0, 0, 0, color="b", label="Wind")
         S = axes.quiver(0, 0, 0, 0, 0, 0, color="black", label="Freestream")
         axes.legend()
         # Animate
-        for t in timeRange:
+        for t in time_range:
             R.remove()
             V.remove()
             W.remove()
             S.remove()
             # Calculate rocket position
             Rx, Ry, Rz = self.x(t), self.y(t), self.z(t)
             Ru = 1 * (2 * (self.e1(t) * self.e3(t) + self.e0(t) * self.e2(t)))
@@ -3378,20 +3305,20 @@
             Rw = 1 * (1 - 2 * (self.e1(t) ** 2 + self.e2(t) ** 2))
             # Calculate rocket Mach number
             Vx = self.vx(t) / 340.40
             Vy = self.vy(t) / 340.40
             Vz = self.vz(t) / 340.40
             # Calculate wind Mach Number
             z = self.z(t)
-            Wx = self.env.windVelocityX(z) / 20
-            Wy = self.env.windVelocityY(z) / 20
+            Wx = self.env.wind_velocity_x(z) / 20
+            Wy = self.env.wind_velocity_y(z) / 20
             # Calculate freestream Mach Number
-            Sx = self.streamVelocityX(t) / 340.40
-            Sy = self.streamVelocityY(t) / 340.40
-            Sz = self.streamVelocityZ(t) / 340.40
+            Sx = self.stream_velocity_x(t) / 340.40
+            Sy = self.stream_velocity_y(t) / 340.40
+            Sz = self.stream_velocity_z(t) / 340.40
             # Plot Quivers
             R = axes.quiver(Rx, Ry, Rz, Ru, Rv, Rw, color="r")
             V = axes.quiver(Rx, Ry, Rz, -Vx, -Vy, -Vz, color="g")
             W = axes.quiver(Rx - Vx, Ry - Vy, Rz - Vz, Wx, Wy, 0, color="b")
             S = axes.quiver(Rx, Ry, Rz, Sx, Sy, Sz, color="black")
             # Adjust axis
             axes.set_xlim(Rx - 1, Rx + 1)
@@ -3399,15 +3326,15 @@
             axes.set_zlim(Rz - 1, Rz + 1)
             # plt.pause(1/(fps*speed))
             try:
                 plt.pause(1 / (fps * speed))
             except:
                 time.sleep(1 / (fps * speed))
 
-    def timeIterator(self, nodeList):
+    def time_iterator(self, nodeList):
         i = 0
         while i < len(nodeList) - 1:
             yield i, nodeList[i]
             i += 1
 
     class FlightPhases:
         def __init__(self, init_list=[]):
@@ -3418,89 +3345,103 @@
 
         def __len__(self):
             return len(self.list)
 
         def __repr__(self):
             return str(self.list)
 
-        def add(self, flightPhase, index=None):
+        def add(self, flight_phase, index=None):
             # Handle first phase
             if len(self.list) == 0:
-                self.list.append(flightPhase)
+                self.list.append(flight_phase)
             # Handle appending to last position
             elif index is None:
                 # Check if new flight phase respects time
-                previousPhase = self.list[-1]
-                if flightPhase.t > previousPhase.t:
+                previous_phase = self.list[-1]
+                if flight_phase.t > previous_phase.t:
                     # All good! Add phase.
-                    self.list.append(flightPhase)
-                elif flightPhase.t == previousPhase.t:
+                    self.list.append(flight_phase)
+                elif flight_phase.t == previous_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting together with the one preceding it."
+                        "WARNING: Trying to add a flight phase starting "
+                        + "together with the one preceding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    flightPhase.t += 1e-7
-                    self.add(flightPhase)
-                elif flightPhase.t < previousPhase.t:
+                    flight_phase.t += 1e-7
+                    self.add(flight_phase)
+                elif flight_phase.t < previous_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting before the one preceding it."
+                        "WARNING: Trying to add a flight phase starting before "
+                        + "the one preceding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    self.add(flightPhase, -2)
+                    print("Or by having a negative parachute lag.")
+                    self.add(flight_phase, -2)
             # Handle inserting into intermediary position
             else:
                 # Check if new flight phase respects time
-                nextPhase = self.list[index]
-                previousPhase = self.list[index - 1]
-                if previousPhase.t < flightPhase.t < nextPhase.t:
+                next_phase = self.list[index]
+                previous_phase = self.list[index - 1]
+                if previous_phase.t < flight_phase.t < next_phase.t:
                     # All good! Add phase.
-                    self.list.insert(index, flightPhase)
-                elif flightPhase.t < previousPhase.t:
+                    self.list.insert(index, flight_phase)
+                elif flight_phase.t < previous_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting before the one preceding it."
+                        "WARNING: Trying to add a flight phase starting before "
+                        + "the one preceding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    self.add(flightPhase, index - 1)
-                elif flightPhase.t == previousPhase.t:
+                    print("Or by having a negative parachute lag.")
+                    self.add(flight_phase, index - 1)
+                elif flight_phase.t == previous_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting together with the one preceding it."
+                        "WARNING: Trying to add a flight phase starting "
+                        + "together with the one preceding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    flightPhase.t += 1e-7
-                    self.add(flightPhase, index)
-                elif flightPhase.t == nextPhase.t:
+                    flight_phase.t += 1e-7
+                    self.add(flight_phase, index)
+                elif flight_phase.t == next_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting together with the one proceding it."
+                        "WARNING: Trying to add a flight phase starting "
+                        + "together with the one proceeding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    flightPhase.t += 1e-7
-                    self.add(flightPhase, index + 1)
-                elif flightPhase.t > nextPhase.t:
+                    flight_phase.t += 1e-7
+                    self.add(flight_phase, index + 1)
+                elif flight_phase.t > next_phase.t:
                     print(
-                        "WARNING: Trying to add a flight phase starting after the one proceding it."
+                        "WARNING: Trying to add a flight phase starting after "
+                        + "the one proceeding it."
                     )
                     print(
-                        "This may be caused by more than when parachute being triggered simultaneously."
+                        "This may be caused by more than when parachute being "
+                        + "triggered simultaneously."
                     )
-                    self.add(flightPhase, index + 1)
+                    self.add(flight_phase, index + 1)
 
-        def addPhase(self, t, derivatives=None, callback=[], clear=True, index=None):
+        def add_phase(self, t, derivatives=None, callback=[], clear=True, index=None):
             self.add(self.FlightPhase(t, derivatives, callback, clear), index)
 
-        def flushAfter(self, index):
+        def flush_after(self, index):
             del self.list[index + 1 :]
 
         class FlightPhase:
             def __init__(self, t, derivative=None, callbacks=[], clear=True):
                 self.t = t
                 self.derivative = derivative
                 self.callbacks = callbacks[:]
@@ -3529,22 +3470,22 @@
 
         def __repr__(self):
             return str(self.list)
 
         def add(self, timeNode):
             self.list.append(timeNode)
 
-        def addNode(self, t, parachutes, callbacks):
+        def add_node(self, t, parachutes, callbacks):
             self.list.append(self.TimeNode(t, parachutes, callbacks))
 
-        def addParachutes(self, parachutes, t_init, t_end):
+        def add_parachutes(self, parachutes, t_init, t_end):
             # Iterate over parachutes
             for parachute in parachutes:
                 # Calculate start of sampling time nodes
-                pcDt = 1 / parachute.samplingRate
+                pcDt = 1 / parachute.sampling_rate
                 parachute_node_list = [
                     self.TimeNode(i * pcDt, [parachute], [])
                     for i in range(
                         math.ceil(t_init / pcDt), math.floor(t_end / pcDt) + 1
                     )
                 ]
                 self.list += parachute_node_list
@@ -3564,15 +3505,15 @@
                     self.tmp_list[-1].callbacks += node.callbacks
                 # Add new node to tmp list if there is none with the same time
                 else:
                     self.tmp_list.append(node)
             # Save tmp list to permanent
             self.list = self.tmp_list
 
-        def flushAfter(self, index):
+        def flush_after(self, index):
             del self.list[index + 1 :]
 
         class TimeNode:
             def __init__(self, t, parachutes, callbacks):
                 self.t = t
                 self.parachutes = parachutes
                 self.callbacks = callbacks
```

### Comparing `rocketpy-0.9.9/rocketpy/Function.py` & `rocketpy-1.0.0a1/rocketpy/Function.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # -*- coding: utf-8 -*-
 
 __author__ = "Giovani Hidalgo Ceotto, Lucas Kierulff Balabram"
-__copyright__ = "Copyright 20XX, Projeto Jupiter"
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __license__ = "MIT"
 
-import re
-import math
-import bisect
-import warnings
-import time
-from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
+from inspect import signature
+from pathlib import Path
+
+try:
+    from functools import cached_property
+except ImportError:
+    from .tools import cached_property
 
-import numpy as np
-from scipy import integrate
-from scipy import linalg
 import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
+import numpy as np
+from scipy import integrate, linalg, optimize
 
 
 class Function:
     """Class converts a python function or a data sequence into an object
     which can be handled more naturally, enabling easy interpolation,
-    extrapolation, ploting and algebra.
+    extrapolation, plotting and algebra.
     """
 
     def __init__(
         self,
         source,
         inputs=["Scalar"],
         outputs=["Scalar"],
         interpolation=None,
         extrapolation=None,
+        title=None,
     ):
         """Convert source into a Function, to be used more naturally.
         Set inputs, outputs, domain dimension, interpolation and extrapolation
         method, and process the source.
 
         Parameters
         ----------
@@ -56,378 +53,435 @@
             this parameter must be given for correct operation.
         outputs : string, sequence of strings, optional
             The name of the outputs of the function. Will be used for
             representation and graphing (axis names). Scalar is default.
         interpolation : string, optional
             Interpolation method to be used if source type is ndarray.
             For 1-D functions, linear, polynomial, akima and spline are
-            supported. For N-D functions, only shepard is suporrted.
+            supported. For N-D functions, only shepard is supported.
             Default for 1-D functions is spline.
         extrapolation : string, optional
             Extrapolation method to be used if source type is ndarray.
             Options are 'natural', which keeps interpolation, 'constant',
             which returns the value of the function at the edge of the interval,
             and 'zero', which returns zero for all points outside of source
             range. Default for 1-D functions is constant.
+        title : string, optional
+            Title to be displayed in the plots' figures. If none, the title will
+            be constructed using the inputs and outputs arguments in the form
+            of  "{inputs} x {outputs}".
 
         Returns
         -------
         None
         """
         # Set input and output
-        self.setInputs(inputs)
-        self.setOutputs(outputs)
+        self.set_inputs(inputs)
+        self.set_outputs(outputs)
         # Save interpolation method
         self.__interpolation__ = interpolation
         self.__extrapolation__ = extrapolation
         # Initialize last_interval
         self.last_interval = 0
         # Set source
-        self.setSource(source)
+        self.set_source(source)
+        #  Set function title
+        self.set_title(title)
+
         # Return
         return None
 
     # Define all set methods
-    def setInputs(self, inputs):
+    def set_inputs(self, inputs):
         """Set the name and number of the incoming arguments of the Function.
 
         Parameters
         ----------
         inputs : string, sequence of strings
             The name of the parameters (inputs) of the Function.
 
         Returns
         -------
         self : Function
         """
         self.__inputs__ = [inputs] if isinstance(inputs, str) else list(inputs)
-        self.__domDim__ = len(self.__inputs__)
+        self.__dom_dim__ = len(self.__inputs__)
         return self
 
-    def setOutputs(self, outputs):
+    def set_outputs(self, outputs):
         """Set the name and number of the output of the Function.
 
         Parameters
         ----------
         outputs : string, sequence of strings
             The name of the output of the function. Example: Distance (m).
 
         Returns
         -------
         self : Function
         """
         self.__outputs__ = [outputs] if isinstance(outputs, str) else list(outputs)
-        self.__imgDim__ = len(self.__outputs__)
+        self.__img_dim__ = len(self.__outputs__)
         return self
 
-    def setSource(self, source):
+    def set_source(self, source):
         """Set the source which defines the output of the function giving a
         certain input.
 
         Parameters
         ----------
-        source : function, scalar, ndarray, string
+        source : function, scalar, ndarray, string, Function
             The actual function. If type is function, it will be called for
             evaluation. If type is int or float, it will be treated as a
             constant function. If ndarray, its points will be used for
             interpolation. An ndarray should be as [(x0, y0, z0), (x1, y1, z1),
             (x2, y2, z2), ...] where x0 and y0 are inputs and z0 is output. If
             string, imports file named by the string and treats it as csv.
             The file is converted into ndarray and should not have headers.
+            If the source is a Function, its source will be copied and another
+            Function will be created following the new inputs and outputs.
 
         Returns
         -------
         self : Function
         """
-        # Import CSV if source is a string and convert values to ndarray
-        if isinstance(source, str):
+        # If the source is a Function
+        if isinstance(source, Function):
+            source = source.get_source()
+        # Import CSV if source is a string or Path and convert values to ndarray
+        if isinstance(source, (str, Path)):
             # Read file and check for headers
             f = open(source, "r")
-            firstLine = f.readline()
+            first_line = f.readline()
             # If headers are found...
-            if firstLine[0] in ['"', "'"]:
+            if first_line[0] in ['"', "'"]:
                 # Headers available
-                firstLine = firstLine.replace('"', " ").replace("'", " ")
-                firstLine = firstLine.split(" , ")
-                self.setInputs(firstLine[0])
-                self.setOutputs(firstLine[1:])
+                first_line = first_line.replace('"', " ").replace("'", " ")
+                first_line = first_line.split(" , ")
+                self.set_inputs(first_line[0])
+                self.set_outputs(first_line[1:])
                 source = np.loadtxt(source, delimiter=",", skiprows=1, dtype=float)
             # if headers are not found
             else:
                 source = np.loadtxt(source, delimiter=",", dtype=float)
         # Convert to ndarray if source is a list
         if isinstance(source, (list, tuple)):
             source = np.array(source, dtype=np.float64)
         # Convert number source into vectorized lambda function
         if isinstance(source, (int, float)):
             temp = 1 * source
-            source = lambda x: 0 * x + temp
+
+            def source(x):
+                return temp
+
         # Handle callable source or number source
         if callable(source):
             # Set source
             self.source = source
-            # Set geValueOpt2
-            self.getValueOpt = source
+            # Set get_value_opt
+            self.get_value_opt = source
             # Set arguments name and domain dimensions
             parameters = signature(source).parameters
-            self.__domDim__ = len(parameters)
-            if self.__inputs__ == ["Time (s)"]:
+            self.__dom_dim__ = len(parameters)
+            if self.__inputs__ == ["Scalar"]:
                 self.__inputs__ = list(parameters)
             # Set interpolation and extrapolation
             self.__interpolation__ = None
             self.__extrapolation__ = None
         # Handle ndarray source
         else:
             # Check to see if dimensions match incoming data set
             newTotalDim = len(source[0, :])
-            oldTotalDim = self.__domDim__ + self.__imgDim__
+            oldTotalDim = self.__dom_dim__ + self.__img_dim__
             dV = self.__inputs__ == ["Scalar"] and self.__outputs__ == ["Scalar"]
             # If they don't, update default values or throw error
             if newTotalDim != oldTotalDim:
                 if dV:
                     # Update dimensions and inputs
-                    self.__domDim__ = newTotalDim - 1
-                    self.__inputs__ = self.__domDim__ * self.__inputs__
+                    self.__dom_dim__ = newTotalDim - 1
+                    self.__inputs__ = self.__dom_dim__ * self.__inputs__
                 else:
                     # User has made a mistake inputting inputs and outputs
                     print("Error in input and output dimensions!")
                     return None
             # Do things if domDim is 1
-            if self.__domDim__ == 1:
+            if self.__dom_dim__ == 1:
                 source = source[source[:, 0].argsort()]
+
+                self.x_array = source[:, 0]
+                self.xinitial, self.xfinal = self.x_array[0], self.x_array[-1]
+
+                self.y_array = source[:, 1]
+                self.y_initial, self.y_final = self.y_array[0], self.y_array[-1]
+
                 # Finally set data source as source
                 self.source = source
+                # Update extrapolation method
+                if self.__extrapolation__ is None:
+                    self.set_extrapolation()
                 # Set default interpolation for point source if it hasn't
                 if self.__interpolation__ is None:
-                    self.setInterpolation()
+                    self.set_interpolation()
                 else:
                     # Updates interpolation coefficients
-                    self.setInterpolation(self.__interpolation__)
+                    self.set_interpolation(self.__interpolation__)
             # Do things if function is multivariate
             else:
+                self.x_array = source[:, 0]
+                self.xinitial, self.xfinal = self.x_array[0], self.x_array[-1]
+
+                self.y_array = source[:, 1]
+                self.y_initial, self.y_final = self.y_array[0], self.y_array[-1]
+
+                self.z_array = source[:, 2]
+                self.z_initial, self.z_final = self.z_array[0], self.z_array[-1]
+
                 # Finally set data source as source
                 self.source = source
                 if self.__interpolation__ is None:
-                    self.setInterpolation("shepard")
-            # Update extrapolation method
-            if self.__extrapolation__ is None:
-                self.setExtrapolation()
+                    self.set_interpolation("shepard")
         # Return self
         return self
 
-    def setInterpolation(self, method="spline"):
+    @cached_property
+    def min(self):
+        """Get the minimum value of the Function y_array.
+        Raises an error if the Function is lambda based.
+
+        Returns
+        -------
+        minimum: float.
+        """
+        return self.y_array.min()
+
+    @cached_property
+    def max(self):
+        """Get the maximum value of the Function y_array.
+        Raises an error if the Function is lambda based.
+
+        Returns
+        -------
+        maximum: float.
+        """
+        return self.y_array.max()
+
+    def set_interpolation(self, method="spline"):
         """Set interpolation method and process data is method requires.
 
         Parameters
         ----------
         method : string, optional
             Interpolation method to be used if source type is ndarray.
             For 1-D functions, linear, polynomial, akima and spline is
-            supported. For N-D functions, only shepard is suporrted.
+            supported. For N-D functions, only shepard is supported.
             Default is 'spline'.
 
         Returns
         -------
         self : Function
         """
         # Set interpolation method
         self.__interpolation__ = method
         # Spline, akima and polynomial need data processing
         # Shepard, and linear do not
         if method == "spline":
-            self.__interpolateSpline__()
+            self.__interpolate_spline__()
         elif method == "polynomial":
-            self.__interpolatePolynomial__()
+            self.__interpolate_polynomial__()
         elif method == "akima":
-            self.__interpolateAkima__()
+            self.__interpolate_akima__()
 
-        # Set geValueOpt
-        self.setGetValueOpt()
+        # Set get_value_opt
+        self.set_get_value_opt()
 
         # Returns self
         return self
 
-    def setExtrapolation(self, method="constant"):
+    def set_extrapolation(self, method="constant"):
         """Set extrapolation behavior of data set.
 
         Parameters
         ----------
         extrapolation : string, optional
             Extrapolation method to be used if source type is ndarray.
             Options are 'natural', which keeps interpolation, 'constant',
             which returns the value of the function at the edge of the interval,
             and 'zero', which returns zero for all points outside of source
-            range. Default is 'zero'.
+            range. Default is 'constant'.
 
         Returns
         -------
         self : Function
         """
         # Set extrapolation method
         self.__extrapolation__ = method
         # Return self
         return self
 
-    def setGetValueOpt(self):
+    def set_get_value_opt(self):
         """Crates a method that evaluates interpolations rather quickly
         when compared to other options available, such as just calling
-        the object instance or calling self.getValue directly. See
-        Function.getValueOpt for documentation.
+        the object instance or calling self.get_value directly. See
+        Function.get_value_opt for documentation.
 
         Returns
         -------
         self : Function
         """
         # Retrieve general info
-        xData = self.source[:, 0]
-        yData = self.source[:, 1]
-        xmin, xmax = xData[0], xData[-1]
+        x_data = self.x_array
+        y_data = self.y_array
+        x_min, x_max = self.xinitial, self.xfinal
         if self.__extrapolation__ == "zero":
             extrapolation = 0  # Extrapolation is zero
         elif self.__extrapolation__ == "natural":
             extrapolation = 1  # Extrapolation is natural
-        else:
+        elif self.__extrapolation__ == "constant":
             extrapolation = 2  # Extrapolation is constant
+        else:
+            raise ValueError(f"Invalid extrapolation type {self.__extrapolation__}")
 
         # Crete method to interpolate this info for each interpolation type
         if self.__interpolation__ == "spline":
-            coeffs = self.__splineCoefficients__
+            coeffs = self.__spline_coefficients__
 
-            def getValueOpt(x):
-                xInterval = np.searchsorted(xData, x)
+            def get_value_opt(x):
+                x_interval = np.searchsorted(x_data, x)
                 # Interval found... interpolate... or extrapolate
-                if xmin <= x <= xmax:
+                if x_min <= x <= x_max:
                     # Interpolate
-                    xInterval = xInterval if xInterval != 0 else 1
-                    a = coeffs[:, xInterval - 1]
-                    x = x - xData[xInterval - 1]
-                    y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    x_interval = x_interval if x_interval != 0 else 1
+                    a = coeffs[:, x_interval - 1]
+                    x = x - x_data[x_interval - 1]
+                    y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:
                     # Extrapolate
                     if extrapolation == 0:  # Extrapolation == zero
                         y = 0
                     elif extrapolation == 1:  # Extrapolation == natural
-                        a = coeffs[:, 0] if x < xmin else coeffs[:, -1]
-                        x = x - xData[0] if x < xmin else x - xData[-2]
-                        y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                        a = coeffs[:, 0] if x < x_min else coeffs[:, -1]
+                        x = x - x_data[0] if x < x_min else x - x_data[-2]
+                        y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                     else:  # Extrapolation is set to constant
-                        y = yData[0] if x < xmin else yData[-1]
+                        y = y_data[0] if x < x_min else y_data[-1]
                 return y
 
-            self.getValueOpt = getValueOpt
+            self.get_value_opt = get_value_opt
 
         elif self.__interpolation__ == "linear":
 
-            def getValueOpt(x):
-                xInterval = np.searchsorted(xData, x)
+            def get_value_opt(x):
+                x_interval = np.searchsorted(x_data, x)
                 # Interval found... interpolate... or extrapolate
-                if xmin <= x <= xmax:
+                if x_min <= x <= x_max:
                     # Interpolate
-                    dx = float(xData[xInterval] - xData[xInterval - 1])
-                    dy = float(yData[xInterval] - yData[xInterval - 1])
-                    y = (x - xData[xInterval - 1]) * (dy / dx) + yData[xInterval - 1]
+                    dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                    dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                    y = (x - x_data[x_interval - 1]) * (dy / dx) + y_data[
+                        x_interval - 1
+                    ]
                 else:
                     # Extrapolate
                     if extrapolation == 0:  # Extrapolation == zero
                         y = 0
                     elif extrapolation == 1:  # Extrapolation == natural
-                        xInterval = 1 if x < xmin else -1
-                        dx = float(xData[xInterval] - xData[xInterval - 1])
-                        dy = float(yData[xInterval] - yData[xInterval - 1])
-                        y = (x - xData[xInterval - 1]) * (dy / dx) + yData[
-                            xInterval - 1
+                        x_interval = 1 if x < x_min else -1
+                        dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                        dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                        y = (x - x_data[x_interval - 1]) * (dy / dx) + y_data[
+                            x_interval - 1
                         ]
                     else:  # Extrapolation is set to constant
-                        y = yData[0] if x < xmin else yData[-1]
+                        y = y_data[0] if x < x_min else y_data[-1]
                 return y
 
-            self.getValueOpt = getValueOpt
+            self.get_value_opt = get_value_opt
 
         elif self.__interpolation__ == "akima":
-            coeffs = np.array(self.__akimaCoefficients__)
+            coeffs = np.array(self.__akima_coefficients__)
 
-            def getValueOpt(x):
-                xInterval = np.searchsorted(xData, x)
+            def get_value_opt(x):
+                x_interval = np.searchsorted(x_data, x)
                 # Interval found... interpolate... or extrapolate
-                if xmin <= x <= xmax:
+                if x_min <= x <= x_max:
                     # Interpolate
-                    xInterval = xInterval if xInterval != 0 else 1
-                    a = coeffs[4 * xInterval - 4 : 4 * xInterval]
-                    y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    x_interval = x_interval if x_interval != 0 else 1
+                    a = coeffs[4 * x_interval - 4 : 4 * x_interval]
+                    y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:
                     # Extrapolate
                     if extrapolation == 0:  # Extrapolation == zero
                         y = 0
                     elif extrapolation == 1:  # Extrapolation == natural
-                        a = coeffs[:4] if x < xmin else coeffs[-4:]
-                        y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                        a = coeffs[:4] if x < x_min else coeffs[-4:]
+                        y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                     else:  # Extrapolation is set to constant
-                        y = yData[0] if x < xmin else yData[-1]
+                        y = y_data[0] if x < x_min else y_data[-1]
                 return y
 
-            self.getValueOpt = getValueOpt
+            self.get_value_opt = get_value_opt
 
         elif self.__interpolation__ == "polynomial":
-            coeffs = self.__polynomialCoefficients__
+            coeffs = self.__polynomial_coefficients__
 
-            def getValueOpt(x):
+            def get_value_opt(x):
                 # Interpolate... or extrapolate
-                if xmin <= x <= xmax:
+                if x_min <= x <= x_max:
                     # Interpolate
                     y = 0
                     for i in range(len(coeffs)):
-                        y += coeffs[i] * (x ** i)
+                        y += coeffs[i] * (x**i)
                 else:
                     # Extrapolate
                     if extrapolation == 0:  # Extrapolation == zero
                         y = 0
                     elif extrapolation == 1:  # Extrapolation == natural
                         y = 0
                         for i in range(len(coeffs)):
-                            y += coeffs[i] * (x ** i)
+                            y += coeffs[i] * (x**i)
                     else:  # Extrapolation is set to constant
-                        y = yData[0] if x < xmin else yData[-1]
+                        y = y_data[0] if x < x_min else y_data[-1]
                 return y
 
-            self.getValueOpt = getValueOpt
+            self.get_value_opt = get_value_opt
 
         elif self.__interpolation__ == "shepard":
-            xData = self.source[:, 0:-1]  # Support for N-Dimensions
-            len_yData = len(yData)  # A little speed up
+            x_data = self.source[:, 0:-1]  # Support for N-Dimensions
+            len_y_data = len(y_data)  # A little speed up
 
-            def getValueOpt(*args):
+            def get_value_opt(*args):
                 x = np.array([[float(x) for x in list(args)]])
-                numeratorSum = 0
-                denominatorSum = 0
-                for i in range(len_yData):
-                    sub = xData[i] - x
+                numerator_sum = 0
+                denominator_sum = 0
+                for i in range(len_y_data):
+                    sub = x_data[i] - x
                     distance = np.linalg.norm(sub)
                     if distance == 0:
-                        numeratorSum = yData[i]
-                        denominatorSum = 1
+                        numerator_sum = y_data[i]
+                        denominator_sum = 1
                         break
                     else:
                         weight = distance ** (-3)
-                        numeratorSum = numeratorSum + yData[i] * weight
-                        denominatorSum = denominatorSum + weight
-                return numeratorSum / denominatorSum
+                        numerator_sum = numerator_sum + y_data[i] * weight
+                        denominator_sum = denominator_sum + weight
+                return numerator_sum / denominator_sum
 
-            self.getValueOpt = getValueOpt
+            self.get_value_opt = get_value_opt
 
         # Returns self
         return self
 
-    def setDiscrete(
+    def set_discrete(
         self,
         lower=0,
         upper=10,
         samples=200,
         interpolation="spline",
         extrapolation="constant",
-        oneByOne=True,
+        one_by_one=True,
     ):
         """This method transforms function defined Functions into list
         defined Functions. It evaluates the function at certain points
         (sampling range) and stores the results in a list, which is converted
         into a Function and then returned. The original Function object is
         replaced by the new one.
 
@@ -437,85 +491,256 @@
             Value where sampling range will start. Default is 0.
         upper : scalar, optional
             Value where sampling range will end. Default is 10.
         samples : int, optional
             Number of samples to be taken from inside range. Default is 200.
         interpolation : string
             Interpolation method to be used if source type is ndarray.
-            For 1-D functions, linear, polynomail, akima and spline is
-            supported. For N-D functions, only shepard is suporrted.
+            For 1-D functions, linear, polynomial, akima and spline is
+            supported. For N-D functions, only shepard is supported.
             Default is 'spline'.
         extrapolation : string, optional
             Extrapolation method to be used if source type is ndarray.
             Options are 'natural', which keeps interpolation, 'constant',
             which returns the value of the function at the edge of the interval,
             and 'zero', which returns zero for all points outside of source
             range. Default is 'constant'.
-        oneByOne : boolean, optional
+        one_by_one : boolean, optional
             If True, evaluate Function in each sample point separately. If
             False, evaluates Function in vectorized form. Default is True.
 
         Returns
         -------
         self : Function
         """
-        if self.__domDim__ == 1:
-            Xs = np.linspace(lower, upper, samples)
-            Ys = self.getValue(Xs.tolist()) if oneByOne else self.getValue(Xs)
-            self.source = np.concatenate(([Xs], [Ys])).transpose()
-            self.setInterpolation(interpolation)
-            self.setExtrapolation(extrapolation)
-        elif self.__domDim__ == 2:
+        if self.__dom_dim__ == 1:
+            xs = np.linspace(lower, upper, samples)
+            ys = self.get_value(xs.tolist()) if one_by_one else self.get_value(xs)
+            self.set_source(np.concatenate(([xs], [ys])).transpose())
+            self.set_interpolation(interpolation)
+            self.set_extrapolation(extrapolation)
+        elif self.__dom_dim__ == 2:
             lower = 2 * [lower] if isinstance(lower, (int, float)) else lower
             upper = 2 * [upper] if isinstance(upper, (int, float)) else upper
             sam = 2 * [samples] if isinstance(samples, (int, float)) else samples
             # Create nodes to evaluate function
-            Xs = np.linspace(lower[0], upper[0], sam[0])
-            Ys = np.linspace(lower[1], upper[1], sam[1])
-            Xs, Ys = np.meshgrid(Xs, Ys)
-            Xs, Ys = Xs.flatten(), Ys.flatten()
-            mesh = [[Xs[i], Ys[i]] for i in range(len(Xs))]
+            xs = np.linspace(lower[0], upper[0], sam[0])
+            ys = np.linspace(lower[1], upper[1], sam[1])
+            xs, ys = np.meshgrid(xs, ys)
+            xs, ys = xs.flatten(), ys.flatten()
+            mesh = [[xs[i], ys[i]] for i in range(len(xs))]
             # Evaluate function at all mesh nodes and convert it to matrix
-            Zs = np.array(self.getValue(mesh))
-            self.source = np.concatenate(([Xs], [Ys], [Zs])).transpose()
+            Zs = np.array(self.get_value(mesh))
+            self.set_source(np.concatenate(([xs], [ys], [Zs])).transpose())
             self.__interpolation__ = "shepard"
         return self
 
+    def set_discrete_based_on_model(
+        self, model_function, one_by_one=True, keep_self=True
+    ):
+        """This method transforms the domain of Function instance into a list of
+        discrete points based on the domain of a model Function instance. It does so by
+        retrieving the domain, domain name, interpolation method and extrapolation
+        method of the model Function instance. It then evaluates the original Function
+        instance in all points of the retrieved domain to generate the list of discrete
+        points that will be used for interpolation when this Function is called.
+
+        Parameters
+        ----------
+        model_function : Function
+            Function object that will be used to define the sampling points,
+            interpolation method and extrapolation method.
+            Must be a Function whose source attribute is a list (i.e. a list based
+            Function instance).
+            Must have the same domain dimension as the Function to be discretized.
+
+        one_by_one : boolean, optional
+            If True, evaluate Function in each sample point separately. If
+            False, evaluates Function in vectorized form. Default is True.
+
+        keepSelf : boolean, optional
+            If True, the original Function interpolation and extrapolation methods
+            will be kept. If False, those are substituted by the ones from the model
+            Function. Default is True.
+
+        Returns
+        -------
+        self : Function
+
+        See also
+        --------
+        Function.set_discrete
+
+        Examples
+        --------
+        This method is particularly useful when algebraic operations are carried out
+        using Function instances defined by different discretized domains (same range,
+        but different mesh size). Once an algebraic operation is done, it will not
+        directly be applied between the list of discrete points of the two Function
+        instances. Instead, the result will be a Function instance defined by a callable
+        that calls both Function instances and performs the operation. This makes the
+        evaluation of the resulting Function inefficient, due to extra function calling
+        overhead and multiple interpolations being carried out.
+
+        >>> from rocketpy import Function
+        >>> f = Function([(0, 0), (1, 1), (2, 4), (3, 9), (4, 16)])
+        >>> g = Function([(0, 0), (2, 2), (4, 4)])
+        >>> h = f * g
+        >>> type(h.source)
+        <class 'function'>
+
+        Therefore, it is good practice to make sure both Function instances are defined
+        by the same domain, i.e. by the same list of mesh points. This way, the
+        algebraic operation will be carried out directly between the lists of discrete
+        points, generating a new Function instance defined by this result. When it is
+        evaluated, there are no extra function calling overheads neither multiple
+        interpolations.
+
+        >>> g.set_discrete_based_on_model(f)
+        'Function from R1 to R1 : (Scalar) → (Scalar)'
+        >>> h = f * g
+        >>> h.source
+        array([[ 0.,  0.],
+               [ 1.,  1.],
+               [ 2.,  8.],
+               [ 3., 27.],
+               [ 4., 64.]])
+
+        Notes
+        -----
+        1. This method performs in place replacement of the original Function object
+        source.
+
+        2. This method is similar to set_discrete, but it uses the domain of a model
+        Function to define the domain of the new Function instance.
+        """
+        if not isinstance(model_function.source, np.ndarray):
+            raise TypeError("model_function must be a list based Function.")
+        if model_function.__dom_dim__ != self.__dom_dim__:
+            raise ValueError("model_function must have the same domain dimension.")
+
+        if self.__dom_dim__ == 1:
+            xs = model_function.source[:, 0]
+            ys = self.get_value(xs.tolist()) if one_by_one else self.get_value(xs)
+            self.set_source(np.concatenate(([xs], [ys])).transpose())
+        elif self.__dom_dim__ == 2:
+            # Create nodes to evaluate function
+            xs = model_function.source[:, 0]
+            ys = model_function.source[:, 1]
+            xs, ys = np.meshgrid(xs, ys)
+            xs, ys = xs.flatten(), ys.flatten()
+            mesh = [[xs[i], ys[i]] for i in range(len(xs))]
+            # Evaluate function at all mesh nodes and convert it to matrix
+            Zs = np.array(self.get_value(mesh))
+            self.set_source(np.concatenate(([xs], [ys], [Zs])).transpose())
+
+        interp = (
+            self.__interpolation__ if keep_self else model_function.__interpolation__
+        )
+        extrap = (
+            self.__extrapolation__ if keep_self else model_function.__extrapolation__
+        )
+
+        self.set_interpolation(interp)
+        self.set_extrapolation(extrap)
+
+        return self
+
+    def reset(
+        self,
+        inputs=None,
+        outputs=None,
+        interpolation=None,
+        extrapolation=None,
+        title=None,
+    ):
+        """This method allows the user to reset the inputs, outputs, interpolation
+        and extrapolation settings of a Function object, all at once, without
+        having to call each of the corresponding methods.
+
+        Parameters
+        ----------
+        inputs : string, sequence of strings, optional
+            List of input variable names. If None, the original inputs are kept.
+            See Function.set_inputs for more information.
+        outputs : string, sequence of strings, optional
+            List of output variable names. If None, the original outputs are kept.
+            See Function.set_outputs for more information.
+        interpolation : string, optional
+            Interpolation method to be used if source type is ndarray.
+            See Function.set_interpolation for more information.
+        extrapolation : string, optional
+            Extrapolation method to be used if source type is ndarray.
+            See Function.set_extrapolation for more information.
+
+        Examples
+        --------
+        A simple use case is to reset the inputs and outputs of a Function object
+        that has been defined by algebraic manipulation of other Function objects.
+
+        >>> from rocketpy import Function
+        >>> v = Function(lambda t: (9.8*t**2)/2, inputs='t', outputs='v')
+        >>> mass = 10 # Mass
+        >>> kinetic_energy = mass * v**2 / 2
+        >>> v.get_inputs(), v.get_outputs()
+        (['t'], ['v'])
+        >>> kinetic_energy
+        'Function from R1 to R1 : (x) → (Scalar)'
+        >>> kinetic_energy.reset(inputs='t', outputs='Kinetic Energy');
+        'Function from R1 to R1 : (t) → (Kinetic Energy)'
+
+        Returns
+        -------
+        self : Function
+        """
+        if inputs is not None:
+            self.set_inputs(inputs)
+        if outputs is not None:
+            self.set_outputs(outputs)
+        if interpolation is not None and interpolation != self.__interpolation__:
+            self.set_interpolation(interpolation)
+        if extrapolation is not None and extrapolation != self.__extrapolation__:
+            self.set_extrapolation(extrapolation)
+
+        self.set_title(title)
+
+        return self
+
     # Define all get methods
-    def getInputs(self):
+    def get_inputs(self):
         "Return tuple of inputs of the function."
         return self.__inputs__
 
-    def getOutputs(self):
+    def get_outputs(self):
         "Return tuple of outputs of the function."
         return self.__outputs__
 
-    def getSource(self):
+    def get_source(self):
         "Return source list or function of the Function."
         return self.source
 
-    def getImageDim(self):
+    def get_image_dim(self):
         "Return int describing dimension of the image space of the function."
-        return self.__imgDim__
+        return self.__img_dim__
 
-    def getDomainDim(self):
+    def get_domain_dim(self):
         "Return int describing dimension of the domain space of the function."
-        return self.__domDim__
+        return self.__dom_dim__
 
-    def getInterpolationMethod(self):
+    def get_interpolation_method(self):
         "Return string describing interpolation method used."
         return self.__interpolation__
 
-    def getExtrapolationMethod(self):
+    def get_extrapolation_method(self):
         "Return string describing extrapolation method used."
         return self.__extrapolation__
 
-    def getValue(self, *args):
+    def get_value(self, *args):
         """This method returns the value of the Function at the specified
-        point. See Function.getValueOpt for a faster, but limited,
+        point. See Function.get_value_opt for a faster, but limited,
         implementation.
 
         Parameters
         ----------
         args : scalar, list
             Value where the Function is to be evaluated. If the Function is
             1-D, only one argument is expected, which may be an int, a float
@@ -542,135 +767,139 @@
         # Returns value for shepard interpolation
         elif self.__interpolation__ == "shepard":
             if isinstance(args[0], (list, tuple)):
                 x = list(args[0])
             else:
                 x = [[float(x) for x in list(args)]]
             ans = x
-            xData = self.source[:, 0:-1]
-            yData = self.source[:, -1]
+            x_data = self.source[:, 0:-1]
+            y_data = self.source[:, -1]
             for i in range(len(x)):
-                numeratorSum = 0
-                denominatorSum = 0
-                for o in range(len(yData)):
-                    sub = xData[o] - x[i]
+                numerator_sum = 0
+                denominator_sum = 0
+                for o in range(len(y_data)):
+                    sub = x_data[o] - x[i]
                     distance = (sub.dot(sub)) ** (0.5)
-                    # print(xData[o], x[i], distance)
+                    # print(x_data[o], x[i], distance)
                     if distance == 0:
-                        numeratorSum = yData[o]
-                        denominatorSum = 1
+                        numerator_sum = y_data[o]
+                        denominator_sum = 1
                         break
                     else:
                         weight = distance ** (-3)
-                        numeratorSum = numeratorSum + yData[o] * weight
-                        denominatorSum = denominatorSum + weight
-                ans[i] = numeratorSum / denominatorSum
+                        numerator_sum = numerator_sum + y_data[o] * weight
+                        denominator_sum = denominator_sum + weight
+                ans[i] = numerator_sum / denominator_sum
             return ans if len(ans) > 1 else ans[0]
         # Returns value for polynomial interpolation function type
         elif self.__interpolation__ == "polynomial":
             if isinstance(args[0], (int, float)):
                 args = [list(args)]
             x = np.array(args[0])
-            xData = self.source[:, 0]
-            yData = self.source[:, 1]
-            xmin, xmax = xData[0], xData[-1]
-            coeffs = self.__polynomialCoefficients__
+            x_data = self.x_array
+            y_data = self.y_array
+            x_min, x_max = self.xinitial, self.xfinal
+            coeffs = self.__polynomial_coefficients__
             A = np.zeros((len(args[0]), coeffs.shape[0]))
             for i in range(coeffs.shape[0]):
-                A[:, i] = x ** i
+                A[:, i] = x**i
             ans = A.dot(coeffs).tolist()
             for i in range(len(x)):
-                if not (xmin <= x[i] <= xmax):
+                if not (x_min <= x[i] <= x_max):
                     if self.__extrapolation__ == "constant":
-                        ans[i] = yData[0] if x[i] < xmin else yData[-1]
+                        ans[i] = y_data[0] if x[i] < x_min else y_data[-1]
                     elif self.__extrapolation__ == "zero":
                         ans[i] = 0
             return ans if len(ans) > 1 else ans[0]
         # Returns value for spline, akima or linear interpolation function type
         elif self.__interpolation__ in ["spline", "akima", "linear"]:
-            if isinstance(args[0], (int, float, complex)):
+            if isinstance(args[0], (int, float, complex, np.integer)):
                 args = [list(args)]
             x = [arg for arg in args[0]]
-            xData = self.source[:, 0]
-            yData = self.source[:, 1]
-            xIntervals = np.searchsorted(xData, x)
-            xmin, xmax = xData[0], xData[-1]
+            x_data = self.x_array
+            y_data = self.y_array
+            x_intervals = np.searchsorted(x_data, x)
+            x_min, x_max = self.xinitial, self.xfinal
             if self.__interpolation__ == "spline":
-                coeffs = self.__splineCoefficients__
+                coeffs = self.__spline_coefficients__
                 for i in range(len(x)):
-                    if x[i] == xmin or x[i] == xmax:
-                        x[i] = yData[xIntervals[i]]
-                    elif xmin < x[i] < xmax or (self.__extrapolation__ == "natural"):
-                        if not xmin < x[i] < xmax:
-                            a = coeffs[:, 0] if x[i] < xmin else coeffs[:, -1]
-                            x[i] = x[i] - xData[0] if x[i] < xmin else x[i] - xData[-2]
+                    if x[i] == x_min or x[i] == x_max:
+                        x[i] = y_data[x_intervals[i]]
+                    elif x_min < x[i] < x_max or (self.__extrapolation__ == "natural"):
+                        if not x_min < x[i] < x_max:
+                            a = coeffs[:, 0] if x[i] < x_min else coeffs[:, -1]
+                            x[i] = (
+                                x[i] - x_data[0] if x[i] < x_min else x[i] - x_data[-2]
+                            )
                         else:
-                            a = coeffs[:, xIntervals[i] - 1]
-                            x[i] = x[i] - xData[xIntervals[i] - 1]
+                            a = coeffs[:, x_intervals[i] - 1]
+                            x[i] = x[i] - x_data[x_intervals[i] - 1]
                         x[i] = a[3] * x[i] ** 3 + a[2] * x[i] ** 2 + a[1] * x[i] + a[0]
                     else:
                         # Extrapolate
                         if self.__extrapolation__ == "zero":
                             x[i] = 0
                         else:  # Extrapolation is set to constant
-                            x[i] = yData[0] if x[i] < xmin else yData[-1]
+                            x[i] = y_data[0] if x[i] < x_min else y_data[-1]
             elif self.__interpolation__ == "linear":
                 for i in range(len(x)):
                     # Interval found... interpolate... or extrapolate
-                    inter = xIntervals[i]
-                    if xmin <= x[i] <= xmax:
+                    inter = x_intervals[i]
+                    if x_min <= x[i] <= x_max:
                         # Interpolate
-                        dx = float(xData[inter] - xData[inter - 1])
-                        dy = float(yData[inter] - yData[inter - 1])
-                        x[i] = (x[i] - xData[inter - 1]) * (dy / dx) + yData[inter - 1]
+                        dx = float(x_data[inter] - x_data[inter - 1])
+                        dy = float(y_data[inter] - y_data[inter - 1])
+                        x[i] = (x[i] - x_data[inter - 1]) * (dy / dx) + y_data[
+                            inter - 1
+                        ]
                     else:
                         # Extrapolate
                         if self.__extrapolation__ == "zero":  # Extrapolation == zero
                             x[i] = 0
                         elif (
                             self.__extrapolation__ == "natural"
                         ):  # Extrapolation == natural
-                            inter = 1 if x[i] < xmin else -1
-                            dx = float(xData[inter] - xData[inter - 1])
-                            dy = float(yData[inter] - yData[inter - 1])
-                            x[i] = (x[i] - xData[inter - 1]) * (dy / dx) + yData[
+                            inter = 1 if x[i] < x_min else -1
+                            dx = float(x_data[inter] - x_data[inter - 1])
+                            dy = float(y_data[inter] - y_data[inter - 1])
+                            x[i] = (x[i] - x_data[inter - 1]) * (dy / dx) + y_data[
                                 inter - 1
                             ]
                         else:  # Extrapolation is set to constant
-                            x[i] = yData[0] if x[i] < xmin else yData[-1]
+                            x[i] = y_data[0] if x[i] < x_min else y_data[-1]
             else:
-                coeffs = self.__akimaCoefficients__
+                coeffs = self.__akima_coefficients__
                 for i in range(len(x)):
-                    if x[i] == xmin or x[i] == xmax:
-                        x[i] = yData[xIntervals[i]]
-                    elif xmin < x[i] < xmax or (self.__extrapolation__ == "natural"):
-                        if not (xmin < x[i] < xmax):
-                            a = coeffs[:4] if x[i] < xmin else coeffs[-4:]
+                    if x[i] == x_min or x[i] == x_max:
+                        x[i] = y_data[x_intervals[i]]
+                    elif x_min < x[i] < x_max or (self.__extrapolation__ == "natural"):
+                        if not (x_min < x[i] < x_max):
+                            a = coeffs[:4] if x[i] < x_min else coeffs[-4:]
                         else:
-                            a = coeffs[4 * xIntervals[i] - 4 : 4 * xIntervals[i]]
+                            a = coeffs[4 * x_intervals[i] - 4 : 4 * x_intervals[i]]
                         x[i] = a[3] * x[i] ** 3 + a[2] * x[i] ** 2 + a[1] * x[i] + a[0]
                     else:
                         # Extrapolate
                         if self.__extrapolation__ == "zero":
                             x[i] = 0
                         else:  # Extrapolation is set to constant
-                            x[i] = yData[0] if x[i] < xmin else yData[-1]
+                            x[i] = y_data[0] if x[i] < x_min else y_data[-1]
             if isinstance(args[0], np.ndarray):
                 return np.array(x)
             else:
                 return x if len(x) > 1 else x[0]
 
-    def getValueOpt_deprecated(self, *args):
+    def get_value_opt_deprecated(self, *args):
         """THE CODE BELOW IS HERE FOR DOCUMENTATION PURPOSES ONLY. IT WAS
         REPLACED FOR ALL INSTANCES BY THE FUNCTION.SETGETVALUEOPT METHOD.
 
         This method returns the value of the Function at the specified
-        point in a limited but optimized manner. See Function.getValue for an
+        point in a limited but optimized manner. See Function.get_value for an
         implementation which allows more kinds of inputs.
-        This method optimizes the Function.getValue method by only
+        This method optimizes the Function.get_value method by only
         implementing function evaluations of single inputs, i.e., it is not
         vectorized. Furthermore, it actually implements a different method
         for each interpolation type, eliminating some if statements.
         Currently supports callables and spline, linear, akima, polynomial and
         shepard interpolated Function objects.
 
         Parameters
@@ -687,138 +916,142 @@
         """
         # Callables
         if callable(self.source):
             return self.source(*args)
 
         # Interpolated Function
         # Retrieve general info
-        xData = self.source[:, 0]
-        yData = self.source[:, 1]
-        xmin, xmax = xData[0], xData[-1]
+        x_data = self.x_array
+        y_data = self.y_array
+        x_min, x_max = self.xinitial, self.xfinal
         if self.__extrapolation__ == "zero":
             extrapolation = 0  # Extrapolation is zero
         elif self.__extrapolation__ == "natural":
             extrapolation = 1  # Extrapolation is natural
-        else:
+        elif self.__extrapolation__ == "constant":
             extrapolation = 2  # Extrapolation is constant
+        else:
+            raise ValueError(f"Invalid extrapolation type {self.__extrapolation__}")
 
         # Interpolate this info for each interpolation type
         # Spline
         if self.__interpolation__ == "spline":
             x = args[0]
-            coeffs = self.__splineCoefficients__
-            xInterval = np.searchsorted(xData, x)
+            coeffs = self.__spline_coefficients__
+            x_interval = np.searchsorted(x_data, x)
             # Interval found... interpolate... or extrapolate
-            if xmin <= x <= xmax:
+            if x_min <= x <= x_max:
                 # Interpolate
-                xInterval = xInterval if xInterval != 0 else 1
-                a = coeffs[:, xInterval - 1]
-                x = x - xData[xInterval - 1]
-                y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                x_interval = x_interval if x_interval != 0 else 1
+                a = coeffs[:, x_interval - 1]
+                x = x - x_data[x_interval - 1]
+                y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
             else:
                 # Extrapolate
                 if extrapolation == 0:  # Extrapolation == zero
                     y = 0
                 elif extrapolation == 1:  # Extrapolation == natural
-                    a = coeffs[:, 0] if x < xmin else coeffs[:, -1]
-                    x = x - xData[0] if x < xmin else x - xData[-2]
-                    y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    a = coeffs[:, 0] if x < x_min else coeffs[:, -1]
+                    x = x - x_data[0] if x < x_min else x - x_data[-2]
+                    y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:  # Extrapolation is set to constant
-                    y = yData[0] if x < xmin else yData[-1]
+                    y = y_data[0] if x < x_min else y_data[-1]
             return y
         # Linear
         elif self.__interpolation__ == "linear":
             x = args[0]
-            xInterval = np.searchsorted(xData, x)
+            x_interval = np.searchsorted(x_data, x)
             # Interval found... interpolate... or extrapolate
-            if xmin <= x <= xmax:
+            if x_min <= x <= x_max:
                 # Interpolate
-                dx = float(xData[xInterval] - xData[xInterval - 1])
-                dy = float(yData[xInterval] - yData[xInterval - 1])
-                y = (x - xData[xInterval - 1]) * (dy / dx) + yData[xInterval - 1]
+                dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                y = (x - x_data[x_interval - 1]) * (dy / dx) + y_data[x_interval - 1]
             else:
                 # Extrapolate
                 if extrapolation == 0:  # Extrapolation == zero
                     y = 0
                 elif extrapolation == 1:  # Extrapolation == natural
-                    xInterval = 1 if x < xmin else -1
-                    dx = float(xData[xInterval] - xData[xInterval - 1])
-                    dy = float(yData[xInterval] - yData[xInterval - 1])
-                    y = (x - xData[xInterval - 1]) * (dy / dx) + yData[xInterval - 1]
+                    x_interval = 1 if x < x_min else -1
+                    dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                    dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                    y = (x - x_data[x_interval - 1]) * (dy / dx) + y_data[
+                        x_interval - 1
+                    ]
                 else:  # Extrapolation is set to constant
-                    y = yData[0] if x < xmin else yData[-1]
+                    y = y_data[0] if x < x_min else y_data[-1]
             return y
         # Akima
         elif self.__interpolation__ == "akima":
             x = args[0]
-            coeffs = np.array(self.__akimaCoefficients__)
-            xInterval = np.searchsorted(xData, x)
+            coeffs = np.array(self.__akima_coefficients__)
+            x_interval = np.searchsorted(x_data, x)
             # Interval found... interpolate... or extrapolate
-            if xmin <= x <= xmax:
+            if x_min <= x <= x_max:
                 # Interpolate
-                xInterval = xInterval if xInterval != 0 else 1
-                a = coeffs[4 * xInterval - 4 : 4 * xInterval]
-                y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                x_interval = x_interval if x_interval != 0 else 1
+                a = coeffs[4 * x_interval - 4 : 4 * x_interval]
+                y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
             else:
                 # Extrapolate
                 if extrapolation == 0:  # Extrapolation == zero
                     y = 0
                 elif extrapolation == 1:  # Extrapolation == natural
-                    a = coeffs[:4] if x < xmin else coeffs[-4:]
-                    y = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    a = coeffs[:4] if x < x_min else coeffs[-4:]
+                    y = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:  # Extrapolation is set to constant
-                    y = yData[0] if x < xmin else yData[-1]
+                    y = y_data[0] if x < x_min else y_data[-1]
             return y
-        # Polynominal
+        # Polynomial
         elif self.__interpolation__ == "polynomial":
             x = args[0]
-            coeffs = self.__polynomialCoefficients__
+            coeffs = self.__polynomial_coefficients__
             # Interpolate... or extrapolate
-            if xmin <= x <= xmax:
+            if x_min <= x <= x_max:
                 # Interpolate
                 y = 0
                 for i in range(len(coeffs)):
-                    y += coeffs[i] * (x ** i)
+                    y += coeffs[i] * (x**i)
             else:
                 # Extrapolate
                 if extrapolation == 0:  # Extrapolation == zero
                     y = 0
                 elif extrapolation == 1:  # Extrapolation == natural
                     y = 0
                     for i in range(len(coeffs)):
-                        y += coeffs[i] * (x ** i)
+                        y += coeffs[i] * (x**i)
                 else:  # Extrapolation is set to constant
-                    y = yData[0] if x < xmin else yData[-1]
+                    y = y_data[0] if x < x_min else y_data[-1]
             return y
         # Shepard
         elif self.__interpolation__ == "shepard":
-            xData = self.source[:, 0:-1]  # Support for N-Dimensions
-            len_yData = len(yData)  # A little speed up
+            x_data = self.source[:, 0:-1]  # Support for N-Dimensions
+            len_y_data = len(y_data)  # A little speed up
             x = np.array([[float(x) for x in list(args)]])
-            numeratorSum = 0
-            denominatorSum = 0
-            for i in range(len_yData):
-                sub = xData[i] - x
+            numerator_sum = 0
+            denominator_sum = 0
+            for i in range(len_y_data):
+                sub = x_data[i] - x
                 distance = np.linalg.norm(sub)
                 if distance == 0:
-                    numeratorSum = yData[i]
-                    denominatorSum = 1
+                    numerator_sum = y_data[i]
+                    denominator_sum = 1
                     break
                 else:
                     weight = distance ** (-3)
-                    numeratorSum = numeratorSum + yData[i] * weight
-                    denominatorSum = denominatorSum + weight
-            return numeratorSum / denominatorSum
+                    numerator_sum = numerator_sum + y_data[i] * weight
+                    denominator_sum = denominator_sum + weight
+            return numerator_sum / denominator_sum
 
-    def getValueOpt2(self, *args):
-        """DEPRECATED!! - See Function.getValueOpt for new version.
+    def get_value_opt2(self, *args):
+        """DEPRECATED!! - See Function.get_value_opt for new version.
         This method returns the value of the Function at the specified
-        point in a limited but optimized manner. See Function.getValue for an
+        point in a limited but optimized manner. See Function.get_value for an
         implementation which allows more kinds of inputs.
-        This method optimizes the Function.getValue method by only
+        This method optimizes the Function.get_value method by only
         implementing function evaluations of single inputs, i.e., it is not
         vectorized. Furthermore, it actually implements a different method
         for each interpolation type, eliminating some if statements.
         Finally, it uses Numba to compile the methods, which further optimizes
         the implementation.
         The code below is here for documentation purposes only. It is
         overwritten for all instances by the Function.setGetValuteOpt2 method.
@@ -837,79 +1070,81 @@
         """
         # Returns value for function function type
         if callable(self.source):
             return self.source(*args)
         # Returns value for spline, akima or linear interpolation function type
         elif self.__interpolation__ in ["spline", "akima", "linear"]:
             x = args[0]
-            xData = self.source[:, 0]
-            yData = self.source[:, 1]
+            x_data = self.x_array
+            y_data = self.y_array
             # Hunt in intervals near the last interval which was used.
-            xInterval = self.last_interval
-            if xData[xInterval - 1] <= x <= xData[xInterval]:
+            x_interval = self.last_interval
+            if x_data[x_interval - 1] <= x <= x_data[x_interval]:
                 pass
             else:
-                xInterval = np.searchsorted(xData, x)
-                self.last_interval = xInterval if xInterval < len(xData) else 0
+                x_interval = np.searchsorted(x_data, x)
+                self.last_interval = x_interval if x_interval < len(x_data) else 0
             # Interval found... keep going
-            xmin, xmax = xData[0], xData[-1]
+            x_min, x_max = self.xinitial, self.xfinal
             if self.__interpolation__ == "spline":
-                coeffs = self.__splineCoefficients__
-                if x == xmin or x == xmax:
-                    x = yData[xInterval]
-                elif xmin < x < xmax or (self.__extrapolation__ == "natural"):
-                    if not xmin < x < xmax:
-                        a = coeffs[:, 0] if x < xmin else coeffs[:, -1]
-                        x = x - xData[0] if x < xmin else x - xData[-2]
+                coeffs = self.__spline_coefficients__
+                if x == x_min or x == x_max:
+                    x = y_data[x_interval]
+                elif x_min < x < x_max or (self.__extrapolation__ == "natural"):
+                    if not x_min < x < x_max:
+                        a = coeffs[:, 0] if x < x_min else coeffs[:, -1]
+                        x = x - x_data[0] if x < x_min else x - x_data[-2]
                     else:
-                        a = coeffs[:, xInterval - 1]
-                        x = x - xData[xInterval - 1]
-                    x = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                        a = coeffs[:, x_interval - 1]
+                        x = x - x_data[x_interval - 1]
+                    x = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:
                     # Extrapolate
                     if self.__extrapolation__ == "zero":
                         x = 0
                     else:  # Extrapolation is set to constant
-                        x = yData[0] if x < xmin else yData[-1]
+                        x = y_data[0] if x < x_min else y_data[-1]
             elif self.__interpolation__ == "linear":
-                if x == xmin or x == xmax:
-                    x = yData[xInterval]
-                elif xmin < x < xmax or (self.__extrapolation__ == "natural"):
-                    dx = float(xData[xInterval] - xData[xInterval - 1])
-                    dy = float(yData[xInterval] - yData[xInterval - 1])
-                    x = (x - xData[xInterval - 1]) * (dy / dx) + yData[xInterval - 1]
+                if x == x_min or x == x_max:
+                    x = y_data[x_interval]
+                elif x_min < x < x_max or (self.__extrapolation__ == "natural"):
+                    dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                    dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                    x = (x - x_data[x_interval - 1]) * (dy / dx) + y_data[
+                        x_interval - 1
+                    ]
                 elif self.__extrapolation__ == "natural":
-                    y0 = yData[0] if x < xmin else yData[-1]
-                    xInterval = 1 if x < xmin else -1
-                    dx = float(xData[xInterval] - xData[xInterval - 1])
-                    dy = float(yData[xInterval] - yData[xInterval - 1])
-                    x = (x - xData[xInterval - 1]) * (dy / dx) + y0
+                    y0 = y_data[0] if x < x_min else y_data[-1]
+                    x_interval = 1 if x < x_min else -1
+                    dx = float(x_data[x_interval] - x_data[x_interval - 1])
+                    dy = float(y_data[x_interval] - y_data[x_interval - 1])
+                    x = (x - x_data[x_interval - 1]) * (dy / dx) + y0
                 else:
                     # Extrapolate
                     if self.__extrapolation__ == "zero":
                         x = 0
                     else:  # Extrapolation is set to constant
-                        x = yData[0] if x < xmin else yData[-1]
+                        x = y_data[0] if x < x_min else y_data[-1]
             else:
                 if self.__interpolation__ == "akima":
-                    coeffs = self.__akimaCoefficients__
-                if x == xmin or x == xmax:
-                    x = yData[xInterval]
-                elif xmin < x < xmax:
-                    a = coeffs[4 * xInterval - 4 : 4 * xInterval]
-                    x = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    coeffs = self.__akima_coefficients__
+                if x == x_min or x == x_max:
+                    x = y_data[x_interval]
+                elif x_min < x < x_max:
+                    a = coeffs[4 * x_interval - 4 : 4 * x_interval]
+                    x = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 elif self.__extrapolation__ == "natural":
-                    a = coeffs[:4] if x < xmin else coeffs[-4:]
-                    x = a[3] * x ** 3 + a[2] * x ** 2 + a[1] * x + a[0]
+                    a = coeffs[:4] if x < x_min else coeffs[-4:]
+                    x = a[3] * x**3 + a[2] * x**2 + a[1] * x + a[0]
                 else:
                     # Extrapolate
                     if self.__extrapolation__ == "zero":
                         x = 0
                     else:  # Extrapolation is set to constant
-                        x = yData[0] if x < xmin else yData[-1]
+                        x = y_data[0] if x < x_min else y_data[-1]
             return x
 
     def __getitem__(self, args):
         """Returns item of the Function source. If the source is not an array,
         an error will result.
 
         Parameters
@@ -931,14 +1166,79 @@
         Returns
         -------
         len(self.source) : int
             Length of Function.source.
         """
         return len(self.source)
 
+    def __bool__(self):
+        """Returns true if self exists. This is to avoid getting into __len__
+        method in boolean statements.
+
+        Returns
+        -------
+        bool : bool
+            Always True.
+        """
+        return True
+
+    # Define all conversion methods
+    def to_frequency_domain(self, lower, upper, sampling_frequency, remove_dc=True):
+        """Performs the conversion of the Function to the Frequency Domain and returns
+        the result. This is done by taking the Fourier transform of the Function.
+        The resulting frequency domain is symmetric, i.e., the negative frequencies are
+        included as well.
+
+        Parameters
+        ----------
+        lower : float
+            Lower bound of the time range.
+        upper : float
+            Upper bound of the time range.
+        sampling_frequency : float
+            Sampling frequency at which to perform the Fourier transform.
+        remove_dc : bool, optional
+            If True, the DC component is removed from the Fourier transform.
+
+        Returns
+        -------
+        Function
+            The Function in the frequency domain.
+
+        Examples
+        --------
+        >>> from rocketpy import Function
+        >>> import numpy as np
+        >>> main_frequency = 10 # Hz
+        >>> time = np.linspace(0, 10, 1000)
+        >>> signal = np.sin(2 * np.pi * main_frequency * time)
+        >>> time_domain = Function(np.array([time, signal]).T)
+        >>> frequency_domain = time_domain.to_frequency_domain(lower=0, upper=10, sampling_frequency=100)
+        >>> peak_frequencies_index = np.where(frequency_domain[:, 1] > 0.001)
+        >>> peak_frequencies = frequency_domain[peak_frequencies_index, 0]
+        >>> print(peak_frequencies)
+        [[-10.  10.]]
+        """
+        # Get the time domain data
+        sampling_time_step = 1.0 / sampling_frequency
+        sampling_range = np.arange(lower, upper, sampling_time_step)
+        number_of_samples = len(sampling_range)
+        sampled_points = self(sampling_range)
+        if remove_dc:
+            sampled_points -= np.mean(sampled_points)
+        fourier_amplitude = np.abs(np.fft.fft(sampled_points) / (number_of_samples / 2))
+        fourier_frequencies = np.fft.fftfreq(number_of_samples, sampling_time_step)
+        return Function(
+            source=np.array([fourier_frequencies, fourier_amplitude]).T,
+            inputs="Frequency (Hz)",
+            outputs="Amplitude",
+            interpolation="linear",
+            extrapolation="zero",
+        )
+
     # Define all presentation methods
     def __call__(self, *args):
         """Plot the Function if no argument is given. If an
         argument is given, return the value of the function at the desired
         point.
 
         Parameters
@@ -954,95 +1254,113 @@
         Returns
         -------
         ans : None, scalar, list
         """
         if len(args) == 0:
             return self.plot()
         else:
-            return self.getValue(*args)
+            return self.get_value(*args)
 
     def __str__(self):
         "Return a string representation of the Function"
-        return (
+        return str(
             "Function from R"
-            + str(self.__domDim__)
+            + str(self.__dom_dim__)
             + " to R"
-            + str(self.__imgDim__)
+            + str(self.__img_dim__)
             + " : ("
             + ", ".join(self.__inputs__)
             + ") → ("
             + ", ".join(self.__outputs__)
             + ")"
         )
 
     def __repr__(self):
         "Return a string representation of the Function"
-        return (
+        return repr(
             "Function from R"
-            + str(self.__domDim__)
+            + str(self.__dom_dim__)
             + " to R"
-            + str(self.__imgDim__)
+            + str(self.__img_dim__)
             + " : ("
             + ", ".join(self.__inputs__)
             + ") → ("
             + ", ".join(self.__outputs__)
             + ")"
         )
 
+    def set_title(self, title):
+        if title:
+            self.title = title
+        else:
+            if self.__dom_dim__ == 1:
+                self.title = (
+                    self.__outputs__[0].title() + " x " + self.__inputs__[0].title()
+                )
+            elif self.__dom_dim__ == 2:
+                self.title = (
+                    self.__outputs__[0].title()
+                    + " x "
+                    + self.__inputs__[0].title()
+                    + " x "
+                    + self.__inputs__[1].title()
+                )
+
     def plot(self, *args, **kwargs):
         """Call Function.plot1D if Function is 1-Dimensional or call
         Function.plot2D if Function is 2-Dimensional and forward arguments
         and key-word arguments."""
         if isinstance(self, list):
             # Compare multiple plots
-            Function.comparePlots(self)
+            Function.compare_plots(self)
         else:
-            if self.__domDim__ == 1:
+            if self.__dom_dim__ == 1:
                 self.plot1D(*args, **kwargs)
-            elif self.__domDim__ == 2:
+            elif self.__dom_dim__ == 2:
                 self.plot2D(*args, **kwargs)
             else:
                 print("Error: Only functions with 1D or 2D domains are plottable!")
 
     def plot1D(
         self,
         lower=None,
         upper=None,
         samples=1000,
-        forceData=False,
-        forcePoints=False,
-        returnObject=False,
+        force_data=False,
+        force_points=False,
+        return_object=False,
+        equal_axis=False,
     ):
         """Plot 1-Dimensional Function, from a lower limit to an upper limit,
         by sampling the Function several times in the interval. The title of
         the graph is given by the name of the axes, which are taken from
         the Function`s input and output names.
 
         Parameters
         ----------
         lower : scalar, optional
             The lower limit of the interval in which the function is to be
-            ploted. The default value for function type Functions is 0. By
+            plotted. The default value for function type Functions is 0. By
             contrast, if the Function is given by a dataset, the default
             value is the start of the dataset.
         upper : scalar, optional
             The upper limit of the interval in which the function is to be
-            ploted. The default value for function type Functions is 10. By
+            plotted. The default value for function type Functions is 10. By
             contrast, if the Function is given by a dataset, the default
             value is the end of the dataset.
         samples : int, optional
             The number of samples in which the function will be evaluated for
             plotting it, which draws lines between each evaluated point.
             The default value is 1000.
-        forceData : Boolean, optional
-            If Function is given by an interpolated dataset, setting forceData
+        force_data : Boolean, optional
+            If Function is given by an interpolated dataset, setting force_data
             to True will plot all points, as a scatter, in the dataset.
             Default value is False.
-        forcePoints : Boolean, optional
-            Setting forcePoints to True will plot all points, as a scatter, in
+        force_points : Boolean, optional
+            Setting force_points to True will plot all points, as a scatter, in
             which the Function was evaluated in the dataset. Default value is
             False.
 
         Returns
         -------
         None
         """
@@ -1051,213 +1369,209 @@
         ax = fig.axes
         if callable(self.source):
             # Determine boundaries
             lower = 0 if lower is None else lower
             upper = 10 if upper is None else upper
         else:
             # Determine boundaries
-            xData = self.source[:, 0]
-            xmin, xmax = xData[0], xData[-1]
-            lower = xmin if lower is None else lower
-            upper = xmax if upper is None else upper
-            # Plot data points if forceData = True
-            tooLow = True if xmin >= lower else False
-            tooHigh = True if xmax <= upper else False
-            loInd = 0 if tooLow else np.where(xData >= lower)[0][0]
-            upInd = len(xData) - 1 if tooHigh else np.where(xData <= upper)[0][0]
-            points = self.source[loInd : (upInd + 1), :].T.tolist()
-            if forceData:
+            x_data = self.x_array
+            x_min, x_max = self.xinitial, self.xfinal
+            lower = x_min if lower is None else lower
+            upper = x_max if upper is None else upper
+            # Plot data points if force_data = True
+            too_low = True if x_min >= lower else False
+            too_high = True if x_max <= upper else False
+            lo_ind = 0 if too_low else np.where(x_data >= lower)[0][0]
+            up_ind = len(x_data) - 1 if too_high else np.where(x_data <= upper)[0][0]
+            points = self.source[lo_ind : (up_ind + 1), :].T.tolist()
+            if force_data:
                 plt.scatter(points[0], points[1], marker="o")
         # Calculate function at mesh nodes
         x = np.linspace(lower, upper, samples)
-        y = self.getValue(x.tolist())
+        y = self.get_value(x.tolist())
         # Plots function
-        if forcePoints:
+        if force_points:
             plt.scatter(x, y, marker="o")
+        if equal_axis:
+            plt.axis("equal")
         plt.plot(x, y)
         # Turn on grid and set title and axis
         plt.grid(True)
-        plt.title(self.__outputs__[0].title() + " x " + self.__inputs__[0].title())
+        plt.title(self.title)
         plt.xlabel(self.__inputs__[0].title())
         plt.ylabel(self.__outputs__[0].title())
         plt.show()
-        if returnObject:
+        if return_object:
             return fig, ax
 
     def plot2D(
         self,
         lower=None,
         upper=None,
         samples=[30, 30],
-        forceData=True,
-        dispType="surface",
+        force_data=True,
+        disp_type="surface",
     ):
         """Plot 2-Dimensional Function, from a lower limit to an upper limit,
         by sampling the Function several times in the interval. The title of
         the graph is given by the name of the axis, which are taken from
         the Function`s inputs and output names.
 
         Parameters
         ----------
         lower : scalar, array of int or float, optional
             The lower limits of the interval in which the function is to be
-            ploted, which can be an int or float, which is repeated for both
+            plotted, which can be an int or float, which is repeated for both
             axis, or an array specifying the limit for each axis. The default
             value for function type Functions is 0. By contrast, if the
             Function is given by a dataset, the default value is the start of
             the dataset for each axis.
         upper : scalar, array of int or float, optional
             The upper limits of the interval in which the function is to be
-            ploted, which can be an int or float, which is repeated for both
+            plotted, which can be an int or float, which is repeated for both
             axis, or an array specifying the limit for each axis. The default
             value for function type Functions is 0. By contrast, if the
             Function is given by a dataset, the default value is the end of
             the dataset for each axis.
         samples : int, array of int, optional
             The number of samples in which the function will be evaluated for
             plotting it, which draws lines between each evaluated point.
             The default value is 30 for each axis.
-        forceData : Boolean, optional
-            If Function is given by an interpolated dataset, setting forceData
+        force_data : Boolean, optional
+            If Function is given by an interpolated dataset, setting force_data
             to True will plot all points, as a scatter, in the dataset.
             Default value is False.
-        dispType : string, optional
+        disp_type : string, optional
             Display type of plotted graph, which can be surface, wireframe,
             contour, or contourf. Default value is surface.
 
         Returns
         -------
         None
         """
         # Prepare plot
         figure = plt.figure()
-        axes = figure.gca(projection="3d")
+        axes = figure.add_subplot(111, projection="3d")
         # Define a mesh and f values at mesh nodes for plotting
         if callable(self.source):
             # Determine boundaries
             lower = [0, 0] if lower is None else lower
             lower = 2 * [lower] if isinstance(lower, (int, float)) else lower
             upper = [10, 10] if upper is None else upper
             upper = 2 * [upper] if isinstance(upper, (int, float)) else upper
         else:
             # Determine boundaries
-            xData = self.source[:, 0]
-            yData = self.source[:, 1]
-            xMin, xMax = xData.min(), xData.max()
-            yMin, yMax = yData.min(), yData.max()
-            lower = [xMin, yMin] if lower is None else lower
+            x_data = self.x_array
+            y_data = self.y_array
+            x_min, x_max = x_data.min(), x_data.max()
+            y_min, y_max = y_data.min(), y_data.max()
+            lower = [x_min, y_min] if lower is None else lower
             lower = 2 * [lower] if isinstance(lower, (int, float)) else lower
-            upper = [xMax, yMax] if upper is None else upper
+            upper = [x_max, y_max] if upper is None else upper
             upper = 2 * [upper] if isinstance(upper, (int, float)) else upper
-            # Plot data points if forceData = True
-            if forceData:
-                axes.scatter(xData, yData, self.source[:, -1])
+            # Plot data points if force_data = True
+            if force_data:
+                axes.scatter(x_data, y_data, self.source[:, -1])
         # Create nodes to evaluate function
         x = np.linspace(lower[0], upper[0], samples[0])
         y = np.linspace(lower[1], upper[1], samples[1])
-        meshX, meshY = np.meshgrid(x, y)
-        meshXFlat, meshYFlat = meshX.flatten(), meshY.flatten()
-        mesh = [[meshXFlat[i], meshYFlat[i]] for i in range(len(meshXFlat))]
+        mesh_x, mesh_y = np.meshgrid(x, y)
+        mesh_x_flat, mesh_y_flat = mesh_x.flatten(), mesh_y.flatten()
+        mesh = [[mesh_x_flat[i], mesh_y_flat[i]] for i in range(len(mesh_x_flat))]
         # Evaluate function at all mesh nodes and convert it to matrix
-        z = np.array(self.getValue(mesh)).reshape(meshX.shape)
+        z = np.array(self.get_value(mesh)).reshape(mesh_x.shape)
         # Plot function
-        if dispType == "surface":
+        if disp_type == "surface":
             surf = axes.plot_surface(
-                meshX,
-                meshY,
+                mesh_x,
+                mesh_y,
                 z,
                 rstride=1,
                 cstride=1,
                 # cmap=cm.coolwarm,
                 linewidth=0,
                 alpha=0.6,
             )
             figure.colorbar(surf)
-        elif dispType == "wireframe":
-            axes.plot_wireframe(meshX, meshY, z, rstride=1, cstride=1)
-        elif dispType == "contour":
+        elif disp_type == "wireframe":
+            axes.plot_wireframe(mesh_x, mesh_y, z, rstride=1, cstride=1)
+        elif disp_type == "contour":
             figure.clf()
-            CS = plt.contour(meshX, meshY, z)
+            CS = plt.contour(mesh_x, mesh_y, z)
             plt.clabel(CS, inline=1, fontsize=10)
-        elif dispType == "contourf":
+        elif disp_type == "contourf":
             figure.clf()
-            CS = plt.contour(meshX, meshY, z)
-            plt.contourf(meshX, meshY, z)
+            CS = plt.contour(mesh_x, mesh_y, z)
+            plt.contourf(mesh_x, mesh_y, z)
             plt.clabel(CS, inline=1, fontsize=10)
-        # axes.contourf(meshX, meshY, z, zdir='x', offset=xMin, cmap=cm.coolwarm)
-        # axes.contourf(meshX, meshY, z, zdir='y', offset=yMax, cmap=cm.coolwarm)
-        plt.title(
-            self.__outputs__[0].title()
-            + " x "
-            + self.__inputs__[0].title()
-            + " x "
-            + self.__inputs__[1].title()
-        )
+        # axes.contourf(mesh_x, mesh_y, z, zdir='x', offset=x_min, cmap=cm.coolwarm)
+        # axes.contourf(mesh_x, mesh_y, z, zdir='y', offset=y_max, cmap=cm.coolwarm)
+        plt.title(self.title)
         axes.set_xlabel(self.__inputs__[0].title())
         axes.set_ylabel(self.__inputs__[1].title())
         axes.set_zlabel(self.__outputs__[0].title())
         plt.show()
 
     @staticmethod
-    def comparePlots(
+    def compare_plots(
         plot_list,
         lower=None,
         upper=None,
         samples=1000,
         title="",
         xlabel="",
         ylabel="",
-        forceData=False,
-        forcePoints=False,
-        returnObject=False,
+        force_data=False,
+        force_points=False,
+        return_object=False,
     ):
         """Plots N 1-Dimensional Functions in the same plot, from a lower
         limit to an upper limit, by sampling the Functions several times in
         the interval.
 
         Parameters
         ----------
         plot_list : list
             List of Functions or list of tuples in the format (Function,
             label), where label is a string which will be displayed in the
             legend.
         lower : scalar, optional
             The lower limit of the interval in which the Functions are to be
-            ploted. The default value for function type Functions is 0. By
+            plotted. The default value for function type Functions is 0. By
             contrast, if the Functions given are defined by a dataset, the
             default value is the lowest value of the datasets.
         upper : scalar, optional
             The upper limit of the interval in which the Functions are to be
-            ploted. The default value for function type Functions is 10. By
+            plotted. The default value for function type Functions is 10. By
             contrast, if the Functions given are defined by a dataset, the
             default value is the highest value of the datasets.
         samples : int, optional
             The number of samples in which the functions will be evaluated for
             plotting it, which draws lines between each evaluated point.
             The default value is 1000.
         title : string, optional
             Title of the plot. Default value is an empty string.
         xlabel : string, optional
             X-axis label. Default value is an empty string.
         ylabel : string, optional
             Y-axis label. Default value is an empty string.
-        forceData : Boolean, optional
-            If Function is given by an interpolated dataset, setting forceData
+        force_data : Boolean, optional
+            If Function is given by an interpolated dataset, setting force_data
             to True will plot all points, as a scatter, in the dataset.
             Default value is False.
-        forcePoints : Boolean, optional
-            Setting forcePoints to True will plot all points, as a scatter, in
+        force_points : Boolean, optional
+            Setting force_points to True will plot all points, as a scatter, in
             which the Function was evaluated to plot it. Default value is
             False.
 
         Returns
         -------
         None
         """
-        noRangeSpecified = True if lower is None and upper is None else False
+        no_range_specified = True if lower is None and upper is None else False
         # Convert to list of tuples if list of Function was given
         plots = []
         for plot in plot_list:
             if isinstance(plot, (tuple, list)):
                 plots.append(plot)
             else:
                 plots.append((plot, ""))
@@ -1274,98 +1588,98 @@
 
         # Define a mesh and y values at mesh nodes for plotting
         if lower is None:
             lower = 0
             for plot in plots:
                 if not callable(plot[0].source):
                     # Determine boundaries
-                    xmin = plot[0].source[0, 0]
-                    lower = xmin if xmin < lower else lower
+                    x_min = plot[0].source[0, 0]
+                    lower = x_min if x_min < lower else lower
         if upper is None:
             upper = 10
             for plot in plots:
                 if not callable(plot[0].source):
                     # Determine boundaries
-                    xmax = plot[0].source[-1, 0]
-                    upper = xmax if xmax > upper else upper
+                    x_max = plot[0].source[-1, 0]
+                    upper = x_max if x_max > upper else upper
         x = np.linspace(lower, upper, samples)
 
         # Iterate to plot all plots
         for plot in plots:
             # Deal with discrete data sets when no range is given
-            if noRangeSpecified and not callable(plot[0].source):
+            if no_range_specified and not callable(plot[0].source):
                 ax.plot(plot[0][:, 0], plot[0][:, 1], label=plot[1])
-                if forcePoints:
+                if force_points:
                     ax.scatter(plot[0][:, 0], plot[0][:, 1], marker="o")
             else:
                 # Calculate function at mesh nodes
-                y = plot[0].getValue(x.tolist())
+                y = plot[0].get_value(x.tolist())
                 # Plots function
                 ax.plot(x, y, label=plot[1])
-                if forcePoints:
+                if force_points:
                     ax.scatter(x, y, marker="o")
 
         # Plot data points if specified
-        if forceData:
+        if force_data:
             for plot in plots:
                 if not callable(plot[0].source):
-                    xData = plot[0].source[:, 0]
-                    xmin, xmax = xData[0], xData[-1]
-                    tooLow = True if xmin >= lower else False
-                    tooHigh = True if xmax <= upper else False
-                    loInd = 0 if tooLow else np.where(xData >= lower)[0][0]
-                    upInd = (
-                        len(xData) - 1 if tooHigh else np.where(xData <= upper)[0][0]
+                    x_data = plot[0].source[:, 0]
+                    x_min, x_max = x_data[0], x_data[-1]
+                    too_low = True if x_min >= lower else False
+                    too_high = True if x_max <= upper else False
+                    lo_ind = 0 if too_low else np.where(x_data >= lower)[0][0]
+                    up_ind = (
+                        len(x_data) - 1 if too_high else np.where(x_data <= upper)[0][0]
                     )
-                    points = plot[0].source[loInd : (upInd + 1), :].T.tolist()
+                    points = plot[0].source[lo_ind : (up_ind + 1), :].T.tolist()
                     ax.scatter(points[0], points[1], marker="o")
 
         # Setup legend
         ax.legend(loc="best", shadow=True)
 
         # Turn on grid and set title and axis
         plt.grid(True)
         plt.title(title)
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
 
         # Show plot
         plt.show()
 
-        if returnObject:
+        if return_object:
             return fig, ax
 
     # Define all interpolation methods
-    def __interpolatePolynomial__(self):
+    def __interpolate_polynomial__(self):
         """Calculate polynomail coefficients that fit the data exactly."""
         # Find the degree of the polynomial interpolation
         degree = self.source.shape[0] - 1
         # Get x and y values for all supplied points.
-        x = self.source[:, 0]
-        y = self.source[:, 1]
+        x = self.x_array
+        y = self.y_array
         # Check if interpolation requires large numbers
         if np.amax(x) ** degree > 1e308:
             print(
                 "Polynomial interpolation of too many points can't be done."
                 " Once the degree is too high, numbers get too large."
                 " The process becomes inefficient. Using spline instead."
             )
-            return self.setInterpolation("spline")
+            return self.set_interpolation("spline")
         # Create coefficient matrix1
         A = np.zeros((degree + 1, degree + 1))
         for i in range(degree + 1):
-            A[:, i] = x ** i
+            A[:, i] = x**i
         # Solve the system and store the resultant coefficients
-        self.__polynomialCoefficients__ = np.linalg.solve(A, y)
+        self.__polynomial_coefficients__ = np.linalg.solve(A, y)
 
-    def __interpolateSpline__(self):
+    def __interpolate_spline__(self):
         """Calculate natural spline coefficients that fit the data exactly."""
         # Get x and y values for all supplied points
-        x = self.source[:, 0]
-        y = self.source[:, 1]
+        x = self.x_array
+        y = self.y_array
         mdim = len(x)
         h = [x[i + 1] - x[i] for i in range(0, mdim - 1)]
         # Initialize the matrix
         Ab = np.zeros((3, mdim))
         # Construct the Ab banded matrix and B vector
         Ab[1, 0] = 1  # A[0, 0] = 1
         B = [0]
@@ -1381,21 +1695,21 @@
         # Calculate other coefficients
         b = [
             ((y[i + 1] - y[i]) / h[i] - h[i] * (2 * c[i] + c[i + 1]) / 3)
             for i in range(0, mdim - 1)
         ]
         d = [(c[i + 1] - c[i]) / (3 * h[i]) for i in range(0, mdim - 1)]
         # Store coefficients
-        self.__splineCoefficients__ = np.array([y[0:-1], b, c[0:-1], d])
+        self.__spline_coefficients__ = np.array([y[0:-1], b, c[0:-1], d])
 
-    def __interpolateAkima__(self):
+    def __interpolate_akima__(self):
         """Calculate akima spline coefficients that fit the data exactly"""
         # Get x and y values for all supplied points
-        x = self.source[:, 0]
-        y = self.source[:, 1]
+        x = self.x_array
+        y = self.y_array
         # Estimate derivatives at each point
         d = [0] * len(x)
         d[0] = (y[1] - y[0]) / (x[1] - x[0])
         d[-1] = (y[-1] - y[-2]) / (x[-1] - x[-2])
         for i in range(1, len(x) - 1):
             w1, w2 = (x[i] - x[i - 1]), (x[i + 1] - x[i])
             d1, d2 = ((y[i] - y[i - 1]) / w1), ((y[i + 1] - y[i]) / w2)
@@ -1404,18 +1718,18 @@
         coeffs = [0] * 4 * (len(x) - 1)
         for i in range(len(x) - 1):
             xl, xr = x[i], x[i + 1]
             yl, yr = y[i], y[i + 1]
             dl, dr = d[i], d[i + 1]
             A = np.array(
                 [
-                    [1, xl, xl ** 2, xl ** 3],
-                    [1, xr, xr ** 2, xr ** 3],
-                    [0, 1, 2 * xl, 3 * xl ** 2],
-                    [0, 1, 2 * xr, 3 * xr ** 2],
+                    [1, xl, xl**2, xl**3],
+                    [1, xr, xr**2, xr**3],
+                    [0, 1, 2 * xl, 3 * xl**2],
+                    [0, 1, 2 * xr, 3 * xr**2],
                 ]
             )
             Y = np.array([yl, yr, dl, dr]).T
             coeffs[4 * i : 4 * i + 4] = np.linalg.solve(A, Y)
             """For some reason this doesn't always work!
             coeffs[4*i] = (dr*xl**2*xr*(-xl + xr) + dl*xl*xr**2*(-xl + xr) +
                            3*xl*xr**2*yl - xr**3*yl + xl**3*yr -
@@ -1424,287 +1738,384 @@
                              xr*(dl*(-2*xl**2 + xl*xr + xr**2) +
                              6*xl*(yl - yr)))/(xl-xr)**3
             coeffs[4*i+2] = (-dl*(xl**2 + xl*xr - 2*xr**2) +
                              dr*(-2*xl**2 + xl*xr + xr**2) +
                              3*(xl + xr)*(yl - yr))/(xl-xr)**3
             coeffs[4*i+3] = (dl*(xl - xr) + dr*(xl - xr) -
                              2*yl + 2*yr)/(xl-xr)**3"""
-        self.__akimaCoefficients__ = coeffs
+        self.__akima_coefficients__ = coeffs
+
+    def __neg__(self):
+        """Negates the Function object. The result has the same effect as
+        multiplying the Function by -1.
+
+        Returns
+        -------
+        Function
+            The negated Function object.
+        """
+        if isinstance(self.source, np.ndarray):
+            neg_source = np.column_stack((self.x_array, -self.y_array))
+            return Function(
+                neg_source,
+                self.__inputs__,
+                self.__outputs__,
+                self.__interpolation__,
+                self.__extrapolation__,
+            )
+        else:
+            return Function(
+                lambda x: -self.source(x),
+                self.__inputs__,
+                self.__outputs__,
+                self.__interpolation__,
+                self.__extrapolation__,
+            )
+
+    def __ge__(self, other):
+        """Greater than or equal to comparison operator. It can be used to
+        compare a Function object with a scalar or another Function object.
+        This has the same effect as comparing numpy arrays.
+
+        Note that it only works for Functions if at least one of them is
+        defined by a set of points so that the bounds of the domain can be
+        set.
+        If both are defined by a set of points, they must have the same
+        discretization.
+
+        Parameters
+        ----------
+        other : scalar or Function
+
+        Returns
+        -------
+        numpy.ndarray of bool
+            The result of the comparison one by one.
+        """
+        otherIsFunction = isinstance(other, Function)
+
+        if isinstance(self.source, np.ndarray):
+            if otherIsFunction:
+                try:
+                    return self.y_array >= other.y_array
+                except AttributeError:
+                    # Other is lambda based Function
+                    return self.y_array >= other(self.x_array)
+                except ValueError:
+                    raise ValueError(
+                        "Comparison not supported between instances of the "
+                        "Function class with different domain discretization."
+                    )
+            else:
+                # Other is not a Function
+                try:
+                    return self.y_array >= other
+                except TypeError:
+                    raise TypeError(
+                        "Comparison not supported between instances of "
+                        f"'Function' and '{type(other)}'."
+                    )
+        else:
+            # self is lambda based Function
+            if otherIsFunction:
+                try:
+                    return self(other.x_array) >= other.y_array
+                except AttributeError:
+                    raise TypeError(
+                        "Comparison not supported between two instances of "
+                        "the Function class with callable sources."
+                    )
+
+    def __le__(self, other):
+        """Less than or equal to comparison operator. It can be used to
+        compare a Function object with a scalar or another Function object.
+        This has the same effect as comparing numpy arrays.
+
+        Note that it only works for Functions if at least one of them is
+        defined by a set of points so that the bounds of the domain can be
+        set.
+        If both are defined by a set of points, they must have the same
+        discretization.
+
+        Parameters
+        ----------
+        other : scalar or Function
+
+        Returns
+        -------
+        numpy.ndarray of bool
+            The result of the comparison one by one.
+        """
+        otherIsFunction = isinstance(other, Function)
+
+        if isinstance(self.source, np.ndarray):
+            if otherIsFunction:
+                try:
+                    return self.y_array <= other.y_array
+                except AttributeError:
+                    # Other is lambda based Function
+                    return self.y_array <= other(self.x_array)
+                except ValueError:
+                    raise ValueError("Operands should have the same discretization.")
+            else:
+                # Other is not a Function
+                try:
+                    return self.y_array <= other
+                except TypeError:
+                    raise TypeError(
+                        "Comparison not supported between instances of "
+                        f"'Function' and '{type(other)}'."
+                    )
+        else:
+            # self is lambda based Function
+            if otherIsFunction:
+                try:
+                    return self(other.x_array) <= other.y_array
+                except AttributeError:
+                    raise TypeError(
+                        "Comparison not supported between two instances of "
+                        "the Function class with callable sources."
+                    )
+
+    def __gt__(self, other):
+        """Greater than comparison operator. It can be used to compare a
+        Function object with a scalar or another Function object. This has
+        the same effect as comparing numpy arrays.
+
+        Note that it only works for Functions if at least one of them is
+        defined by a set of points so that the bounds of the domain can be
+        set.
+        If both are defined by a set of points, they must have the same
+        discretization.
+
+        Parameters
+        ----------
+        other : scalar or Function
+
+        Returns
+        -------
+        numpy.ndarray of bool
+            The result of the comparison one by one.
+        """
+        return ~self.__le__(other)
+
+    def __lt__(self, other):
+        """Less than comparison operator. It can be used to compare a
+        Function object with a scalar or another Function object. This has
+        the same effect as comparing numpy arrays.
+
+        Note that it only works for Functions if at least one of them is
+        defined by a set of points so that the bounds of the domain can be
+        set.
+        If both are defined by a set of points, they must have the same
+        discretization.
+
+        Parameters
+        ----------
+        other : scalar or Function
+
+        Returns
+        -------
+        numpy.ndarray of bool
+            The result of the comparison one by one.
+        """
+        return ~self.__ge__(other)
 
     # Define all possible algebraic operations
-    def __truediv__(self, other):
-        """Devides a Function object and returns a new Function object
-        which gives the result of the division. Only implemented for 1D
-        domains.
+    def __add__(self, other):
+        """Sums a Function object and 'other', returns a new Function
+        object which gives the result of the sum. Only implemented for
+        1D domains.
 
         Parameters
         ----------
         other : Function, int, float, callable
-            What self will be divided by. If other and self are Function
-            objects which are based on interpolation, have the exact same
-            domain (are defined in the same grid points), have the same
-            interpolation method and have the same input name, then a
-            special implementation is used. This implementation is faster,
-            however behavior between grid points is only interpolated,
-            not calculated as it would be.
+            What self will be added to. If other and self are Function
+            objects which are based on a list of points, have the exact same
+            domain (are defined in the same grid points) and have the same
+            dimension, then a special implementation is used.
+            This implementation is faster, however behavior between grid
+            points is only interpolated, not calculated as it would be;
+            the resultant Function has the same interpolation as self.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of self(x)/other(x).
+            A Function object which gives the result of self(x)+other(x).
         """
         # If other is Function try...
         try:
             # Check if Function objects source is array or callable
-            # Check if Function objects have same interpolation and domain
+            # Check if Function objects have the same domain discretization
             if (
                 isinstance(other.source, np.ndarray)
                 and isinstance(self.source, np.ndarray)
-                and self.__interpolation__ == other.__interpolation__
-                and self.__inputs__ == other.__inputs__
-                and np.any(self.source[:, 0] - other.source[:, 0]) == False
+                and self.__dom_dim__ == other.__dom_dim__
+                and np.array_equal(self.x_array, other.x_array)
             ):
                 # Operate on grid values
-                Ys = self.source[:, 1] / other.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
+                ys = self.y_array + other.y_array
+                xs = self.x_array
+                source = np.concatenate(([xs], [ys])).transpose()
                 # Retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
-                outputs = self.__outputs__[0] + "/" + other.__outputs__[0]
+                outputs = self.__outputs__[0] + " + " + other.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (self.getValueOpt2(x) / other(x)))
+                return Function(lambda x: (self.get_value(x) + other(x)))
         # If other is Float except...
-        except:
+        except AttributeError:
             if isinstance(other, (float, int, complex)):
                 # Check if Function object source is array or callable
                 if isinstance(self.source, np.ndarray):
                     # Operate on grid values
-                    Ys = self.source[:, 1] / other
-                    Xs = self.source[:, 0]
-                    source = np.concatenate(([Xs], [Ys])).transpose()
+                    ys = self.y_array + other
+                    xs = self.x_array
+                    source = np.concatenate(([xs], [ys])).transpose()
                     # Retrieve inputs, outputs and interpolation
                     inputs = self.__inputs__[:]
-                    outputs = self.__outputs__[0] + "/" + str(other)
+                    outputs = self.__outputs__[0] + " + " + str(other)
                     outputs = "(" + outputs + ")"
                     interpolation = self.__interpolation__
                     # Create new Function object
                     return Function(source, inputs, outputs, interpolation)
                 else:
-                    return Function(lambda x: (self.getValueOpt2(x) / other))
+                    return Function(lambda x: (self.get_value(x) + other))
             # Or if it is just a callable
             elif callable(other):
-                return Function(lambda x: (self.getValueOpt2(x) / other(x)))
+                return Function(lambda x: (self.get_value(x) + other(x)))
 
-    def __rtruediv__(self, other):
-        """Devides 'other' by a Function object and returns a new Function
-        object which gives the result of the division. Only implemented for
+    def __radd__(self, other):
+        """Sums 'other' and a Function object and returns a new Function
+        object which gives the result of the sum. Only implemented for
         1D domains.
 
         Parameters
         ----------
         other : int, float, callable
-            What self will divide.
+            What self will be added to.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of other(x)/self(x).
+            A Function object which gives the result of other(x)/+self(x).
         """
-        # Check if Function object source is array and other is float
-        if isinstance(other, (float, int, complex)):
-            if isinstance(self.source, np.ndarray):
-                # Operate on grid values
-                Ys = other / self.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
-                # Retrieve inputs, outputs and interpolation
-                inputs = self.__inputs__[:]
-                outputs = str(other) + "/" + self.__outputs__[0]
-                outputs = "(" + outputs + ")"
-                interpolation = self.__interpolation__
-                # Create new Function object
-                return Function(source, inputs, outputs, interpolation)
-            else:
-                return Function(lambda x: (other / self.getValueOpt2(x)))
-        # Or if it is just a callable
-        elif callable(other):
-            return Function(lambda x: (other(x) / self.getValueOpt2(x)))
+        return self + other
 
-    def __pow__(self, other):
-        """Raises a Function object to the power of 'other' and
-        returns a new Function object which gives the result. Only
-        implemented for 1D domains.
+    def __sub__(self, other):
+        """Subtracts from a Function object and returns a new Function object
+        which gives the result of the subtraction. Only implemented for 1D
+        domains.
 
         Parameters
         ----------
         other : Function, int, float, callable
-            What self will be raised to. If other and self are Function
-            objects which are based on interpolation, have the exact same
-            domain (are defined in the same grid points), have the same
-            interpolation method and have the same input name, then a
-            special implementation is used. This implementation is faster,
-            however behavior between grid points is only interpolated,
-            not calculated as it would be.
+            What self will be subtracted by. If other and self are Function
+            objects which are based on a list of points, have the exact same
+            domain (are defined in the same grid points) and have the same
+            dimension, then a special implementation is used.
+            This implementation is faster, however behavior between grid
+            points is only interpolated, not calculated as it would be;
+            the resultant Function has the same interpolation as self.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of self(x)**other(x).
+            A Function object which gives the result of self(x)-other(x).
         """
-        # If other is Function try...
         try:
-            # Check if Function objects source is array or callable
-            # Check if Function objects have same interpolation and domain
-            if (
-                isinstance(other.source, np.ndarray)
-                and isinstance(self.source, np.ndarray)
-                and self.__interpolation__ == other.__interpolation__
-                and self.__inputs__ == other.__inputs__
-                and np.any(self.source[:, 0] - other.source[:, 0]) == False
-            ):
-                # Operate on grid values
-                Ys = self.source[:, 1] ** other.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
-                # Retrieve inputs, outputs and interpolation
-                inputs = self.__inputs__[:]
-                outputs = self.__outputs__[0] + "**" + other.__outputs__[0]
-                outputs = "(" + outputs + ")"
-                interpolation = self.__interpolation__
-                # Create new Function object
-                return Function(source, inputs, outputs, interpolation)
-            else:
-                return Function(lambda x: (self.getValueOpt2(x) ** other(x)))
-        # If other is Float except...
-        except:
-            if isinstance(other, (float, int, complex)):
-                # Check if Function object source is array or callable
-                if isinstance(self.source, np.ndarray):
-                    # Operate on grid values
-                    Ys = self.source[:, 1] ** other
-                    Xs = self.source[:, 0]
-                    source = np.concatenate(([Xs], [Ys])).transpose()
-                    # Retrieve inputs, outputs and interpolation
-                    inputs = self.__inputs__[:]
-                    outputs = self.__outputs__[0] + "**" + str(other)
-                    outputs = "(" + outputs + ")"
-                    interpolation = self.__interpolation__
-                    # Create new Function object
-                    return Function(source, inputs, outputs, interpolation)
-                else:
-                    return Function(lambda x: (self.getValue(x) ** other))
-            # Or if it is just a callable
-            elif callable(other):
-                return Function(lambda x: (self.getValue(x) ** other(x)))
+            return self + (-other)
+        except TypeError:
+            return Function(lambda x: (self.get_value(x) - other(x)))
 
-    def __rpow__(self, other):
-        """Raises 'other' to the power of a Function object and returns
-        a new Function object which gives the result. Only implemented
-        for 1D domains.
+    def __rsub__(self, other):
+        """Subtracts a Function object from 'other' and returns a new Function
+        object which gives the result of the subtraction. Only implemented for
+        1D domains.
 
         Parameters
         ----------
         other : int, float, callable
-            What self will exponentiate.
+            What self will subtract from.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of other(x)**self(x).
+            A Function object which gives the result of other(x)-self(x).
         """
-        # Check if Function object source is array and other is float
-        if isinstance(other, (float, int, complex)):
-            if isinstance(self.source, np.ndarray):
-                # Operate on grid values
-                Ys = other ** self.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
-                # Retrieve inputs, outputs and interpolation
-                inputs = self.__inputs__[:]
-                outputs = str(other) + "**" + self.__outputs__[0]
-                outputs = "(" + outputs + ")"
-                interpolation = self.__interpolation__
-                # Create new Function object
-                return Function(source, inputs, outputs, interpolation)
-            else:
-                return Function(lambda x: (other ** self.getValue(x)))
-        # Or if it is just a callable
-        elif callable(other):
-            return Function(lambda x: (other(x) ** self.getValue(x)))
+        return other + (-self)
 
     def __mul__(self, other):
         """Multiplies a Function object and returns a new Function object
         which gives the result of the multiplication. Only implemented for 1D
         domains.
 
         Parameters
         ----------
         other : Function, int, float, callable
             What self will be multiplied by. If other and self are Function
-            objects which are based on interpolation, have the exact same
-            domain (are defined in the same grid points), have the same
-            interpolation method and have the same input name, then a
-            special implementation is used. This implementation is faster,
-            however behavior between grid points is only interpolated,
-            not calculated as it would be.
+            objects which are based on a list of points, have the exact same
+            domain (are defined in the same grid points) and have the same
+            dimension, then a special implementation is used.
+            This implementation is faster, however behavior between grid
+            points is only interpolated, not calculated as it would be;
+            the resultant Function has the same interpolation as self.
 
         Returns
         -------
         result : Function
             A Function object which gives the result of self(x)*other(x).
         """
         # If other is Function try...
         try:
             # Check if Function objects source is array or callable
-            # Check if Function objects have same interpolation and domain
+            # Check if Function objects have the same domain discretization
             if (
                 isinstance(other.source, np.ndarray)
                 and isinstance(self.source, np.ndarray)
-                and self.__interpolation__ == other.__interpolation__
-                and self.__inputs__ == other.__inputs__
-                and np.any(self.source[:, 0] - other.source[:, 0]) == False
+                and self.__dom_dim__ == other.__dom_dim__
+                and np.array_equal(self.x_array, other.x_array)
             ):
                 # Operate on grid values
-                Ys = self.source[:, 1] * other.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
+                ys = self.y_array * other.y_array
+                xs = self.x_array
+                source = np.concatenate(([xs], [ys])).transpose()
                 # Retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
                 outputs = self.__outputs__[0] + "*" + other.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (self.getValue(x) * other(x)))
+                return Function(lambda x: (self.get_value(x) * other(x)))
         # If other is Float except...
-        except:
+        except AttributeError:
             if isinstance(other, (float, int, complex)):
                 # Check if Function object source is array or callable
                 if isinstance(self.source, np.ndarray):
                     # Operate on grid values
-                    Ys = self.source[:, 1] * other
-                    Xs = self.source[:, 0]
-                    source = np.concatenate(([Xs], [Ys])).transpose()
+                    ys = self.y_array * other
+                    xs = self.x_array
+                    source = np.concatenate(([xs], [ys])).transpose()
                     # Retrieve inputs, outputs and interpolation
                     inputs = self.__inputs__[:]
                     outputs = self.__outputs__[0] + "*" + str(other)
                     outputs = "(" + outputs + ")"
                     interpolation = self.__interpolation__
                     # Create new Function object
                     return Function(source, inputs, outputs, interpolation)
                 else:
-                    return Function(lambda x: (self.getValue(x) * other))
+                    return Function(lambda x: (self.get_value(x) * other))
             # Or if it is just a callable
             elif callable(other):
-                return Function(lambda x: (self.getValue(x) * other(x)))
+                return Function(lambda x: (self.get_value(x) * other(x)))
 
     def __rmul__(self, other):
         """Multiplies 'other' by a Function object and returns a new Function
         object which gives the result of the multiplication. Only implemented for
         1D domains.
 
         Parameters
@@ -1713,237 +2124,237 @@
             What self will be multiplied by.
 
         Returns
         -------
         result : Function
             A Function object which gives the result of other(x)*self(x).
         """
-        # Check if Function object source is array and other is float
-        if isinstance(other, (float, int, complex)):
-            if isinstance(self.source, np.ndarray):
-                # Operate on grid values
-                Ys = other * self.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
-                # Retrieve inputs, outputs and interpolation
-                inputs = self.__inputs__[:]
-                outputs = str(other) + "*" + self.__outputs__[0]
-                outputs = "(" + outputs + ")"
-                interpolation = self.__interpolation__
-                # Create new Function object
-                return Function(source, inputs, outputs, interpolation)
-            else:
-                return Function(lambda x: (other * self.getValue(x)))
-        # Or if it is just a callable
-        elif callable(other):
-            return Function(lambda x: (other(x) * self.getValue(x)))
+        return self * other
 
-    def __add__(self, other):
-        """Sums a Function object and 'other', returns a new Function
-        object which gives the result of the sum. Only implemented for
-        1D domains.
+    def __truediv__(self, other):
+        """Divides a Function object and returns a new Function object
+        which gives the result of the division. Only implemented for 1D
+        domains.
 
         Parameters
         ----------
         other : Function, int, float, callable
-            What self will be added to. If other and self are Function
-            objects which are based on interpolation, have the exact same
-            domain (are defined in the same grid points), have the same
-            interpolation method and have the same input name, then a
-            special implementation is used. This implementation is faster,
-            however behavior between grid points is only interpolated,
-            not calculated as it would be.
+            What self will be divided by. If other and self are Function
+            objects which are based on a list of points, have the exact same
+            domain (are defined in the same grid points) and have the same
+            dimension, then a special implementation is used.
+            This implementation is faster, however behavior between grid
+            points is only interpolated, not calculated as it would be;
+            the resultant Function has the same interpolation as self.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of self(x)+other(x).
+            A Function object which gives the result of self(x)/other(x).
         """
         # If other is Function try...
         try:
             # Check if Function objects source is array or callable
-            # Check if Function objects have same interpolation and domain
+            # Check if Function objects have the same domain discretization
             if (
                 isinstance(other.source, np.ndarray)
                 and isinstance(self.source, np.ndarray)
-                and self.__interpolation__ == other.__interpolation__
-                and self.__inputs__ == other.__inputs__
-                and np.any(self.source[:, 0] - other.source[:, 0]) == False
+                and self.__dom_dim__ == other.__dom_dim__
+                and np.array_equal(self.x_array, other.x_array)
             ):
-                # Operate on grid values
-                Ys = self.source[:, 1] + other.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
-                # Retrieve inputs, outputs and interpolation
+                # operate on grid values
+                with np.errstate(divide="ignore", invalid="ignore"):
+                    ys = self.source[:, 1] / other.source[:, 1]
+                    ys = np.nan_to_num(ys)
+                xs = self.source[:, 0]
+                source = np.concatenate(([xs], [ys])).transpose()
+                # retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
-                outputs = self.__outputs__[0] + " + " + other.__outputs__[0]
+                outputs = self.__outputs__[0] + "/" + other.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (self.getValue(x) + other(x)))
+                return Function(lambda x: (self.get_value_opt(x) / other(x)))
         # If other is Float except...
-        except:
+        except AttributeError:
             if isinstance(other, (float, int, complex)):
                 # Check if Function object source is array or callable
                 if isinstance(self.source, np.ndarray):
                     # Operate on grid values
-                    Ys = self.source[:, 1] + other
-                    Xs = self.source[:, 0]
-                    source = np.concatenate(([Xs], [Ys])).transpose()
+                    ys = self.y_array / other
+                    xs = self.x_array
+                    source = np.concatenate(([xs], [ys])).transpose()
                     # Retrieve inputs, outputs and interpolation
                     inputs = self.__inputs__[:]
-                    outputs = self.__outputs__[0] + " + " + str(other)
+                    outputs = self.__outputs__[0] + "/" + str(other)
                     outputs = "(" + outputs + ")"
                     interpolation = self.__interpolation__
                     # Create new Function object
                     return Function(source, inputs, outputs, interpolation)
                 else:
-                    return Function(lambda x: (self.getValue(x) + other))
+                    return Function(lambda x: (self.get_value_opt(x) / other))
             # Or if it is just a callable
             elif callable(other):
-                return Function(lambda x: (self.getValue(x) + other(x)))
+                return Function(lambda x: (self.get_value_opt(x) / other(x)))
 
-    def __radd__(self, other):
-        """Sums 'other' and a Function object and returns a new Function
-        object which gives the result of the sum. Only implemented for
+    def __rtruediv__(self, other):
+        """Divides 'other' by a Function object and returns a new Function
+        object which gives the result of the division. Only implemented for
         1D domains.
 
         Parameters
         ----------
         other : int, float, callable
-            What self will be added to.
+            What self will divide.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of other(x)/+self(x).
+            A Function object which gives the result of other(x)/self(x).
         """
         # Check if Function object source is array and other is float
         if isinstance(other, (float, int, complex)):
             if isinstance(self.source, np.ndarray):
                 # Operate on grid values
-                Ys = other + self.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
+                ys = other / self.y_array
+                xs = self.x_array
+                source = np.concatenate(([xs], [ys])).transpose()
                 # Retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
-                outputs = str(other) + " + " + self.__outputs__[0]
+                outputs = str(other) + "/" + self.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (other + self.getValue(x)))
+                return Function(lambda x: (other / self.get_value_opt(x)))
         # Or if it is just a callable
         elif callable(other):
-            return Function(lambda x: (other(x) + self.getValue(x)))
+            return Function(lambda x: (other(x) / self.get_value_opt(x)))
 
-    def __sub__(self, other):
-        """Subtracts from a Function object and returns a new Function object
-        which gives the result of the subtraction. Only implemented for 1D
-        domains.
+    def __pow__(self, other):
+        """Raises a Function object to the power of 'other' and
+        returns a new Function object which gives the result. Only
+        implemented for 1D domains.
 
         Parameters
         ----------
         other : Function, int, float, callable
-            What self will be subtracted by. If other and self are Function
-            objects which are based on interpolation, have the exact same
-            domain (are defined in the same grid points), have the same
-            interpolation method and have the same input name, then a
-            special implementation is used. This implementation is faster,
-            however behavior between grid points is only interpolated,
-            not calculated as it would be.
+            What self will be raised to. If other and self are Function
+            objects which are based on a list of points, have the exact same
+            domain (are defined in the same grid points) and have the same
+            dimension, then a special implementation is used.
+            This implementation is faster, however behavior between grid
+            points is only interpolated, not calculated as it would be;
+            the resultant Function has the same interpolation as self.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of self(x)-other(x).
+            A Function object which gives the result of self(x)**other(x).
         """
         # If other is Function try...
         try:
             # Check if Function objects source is array or callable
-            # Check if Function objects have same interpolation and domain
+            # Check if Function objects have the same domain discretization
             if (
                 isinstance(other.source, np.ndarray)
                 and isinstance(self.source, np.ndarray)
-                and self.__interpolation__ == other.__interpolation__
-                and self.__inputs__ == other.__inputs__
-                and np.any(self.source[:, 0] - other.source[:, 0]) == False
+                and self.__dom_dim__ == other.__dom_dim__
+                and np.any(self.x_array - other.x_array) == False
+                and np.array_equal(self.x_array, other.x_array)
             ):
                 # Operate on grid values
-                Ys = self.source[:, 1] - other.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
+                ys = self.y_array**other.y_array
+                xs = self.x_array
+                source = np.concatenate(([xs], [ys])).transpose()
                 # Retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
-                outputs = self.__outputs__[0] + " - " + other.__outputs__[0]
+                outputs = self.__outputs__[0] + "**" + other.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (self.getValue(x) * other(x)))
+                return Function(lambda x: (self.get_value_opt(x) ** other(x)))
         # If other is Float except...
-        except:
+        except AttributeError:
             if isinstance(other, (float, int, complex)):
                 # Check if Function object source is array or callable
                 if isinstance(self.source, np.ndarray):
                     # Operate on grid values
-                    Ys = self.source[:, 1] - other
-                    Xs = self.source[:, 0]
-                    source = np.concatenate(([Xs], [Ys])).transpose()
+                    ys = self.y_array**other
+                    xs = self.x_array
+                    source = np.concatenate(([xs], [ys])).transpose()
                     # Retrieve inputs, outputs and interpolation
                     inputs = self.__inputs__[:]
-                    outputs = self.__outputs__[0] + " - " + str(other)
+                    outputs = self.__outputs__[0] + "**" + str(other)
                     outputs = "(" + outputs + ")"
                     interpolation = self.__interpolation__
                     # Create new Function object
                     return Function(source, inputs, outputs, interpolation)
                 else:
-                    return Function(lambda x: (self.getValue(x) - other))
+                    return Function(lambda x: (self.get_value(x) ** other))
             # Or if it is just a callable
             elif callable(other):
-                return Function(lambda x: (self.getValue(x) - other(x)))
+                return Function(lambda x: (self.get_value(x) ** other(x)))
 
-    def __rsub__(self, other):
-        """Subtracts a Function object from 'other' and returns a new Function
-        object which gives the result of the subtraction. Only implemented for
-        1D domains.
+    def __rpow__(self, other):
+        """Raises 'other' to the power of a Function object and returns
+        a new Function object which gives the result. Only implemented
+        for 1D domains.
 
         Parameters
         ----------
         other : int, float, callable
-            What self will subtract from.
+            What self will exponentiate.
 
         Returns
         -------
         result : Function
-            A Function object which gives the result of other(x)-self(x).
+            A Function object which gives the result of other(x)**self(x).
         """
         # Check if Function object source is array and other is float
         if isinstance(other, (float, int, complex)):
             if isinstance(self.source, np.ndarray):
                 # Operate on grid values
-                Ys = other - self.source[:, 1]
-                Xs = self.source[:, 0]
-                source = np.concatenate(([Xs], [Ys])).transpose()
+                ys = other**self.y_array
+                xs = self.x_array
+                source = np.concatenate(([xs], [ys])).transpose()
                 # Retrieve inputs, outputs and interpolation
                 inputs = self.__inputs__[:]
-                outputs = str(other) + " - " + self.__outputs__[0]
+                outputs = str(other) + "**" + self.__outputs__[0]
                 outputs = "(" + outputs + ")"
                 interpolation = self.__interpolation__
                 # Create new Function object
                 return Function(source, inputs, outputs, interpolation)
             else:
-                return Function(lambda x: (other - self.getValue(x)))
+                return Function(lambda x: (other ** self.get_value(x)))
         # Or if it is just a callable
         elif callable(other):
-            return Function(lambda x: (other(x) - self.getValue(x)))
+            return Function(lambda x: (other(x) ** self.get_value(x)))
+
+    def __matmul__(self, other):
+        """Operator @ as an alias for composition. Therefore, this
+        method is a shorthand for self.compose(other). See self.compose
+        for more information.
+
+        Parameters
+        ----------
+        other : Function
+            Function object to be composed with self.
+
+        Returns
+        -------
+        result : Function
+            A Function object which gives the result of self(other(x)).
+        """
+        return self.compose(other)
 
     def integral(self, a, b, numerical=False):
         """Evaluate a definite integral of a 1-D Function in the interval
         from a to b.
 
         Parameters
         ----------
@@ -1959,81 +2370,718 @@
             unavailable, calculate numerically anyways.
 
         Returns
         -------
         ans : float
             Evaluated integral.
         """
+        # Guarantee a < b
+        integration_sign = np.sign(b - a)
+        if integration_sign == -1:
+            a, b = b, a
+        # Different implementations depending on interpolation
         if self.__interpolation__ == "spline" and numerical is False:
-            # Integrate using spline coefficients
-            xData = self.source[:, 0]
-            yData = self.source[:, 1]
-            coeffs = self.__splineCoefficients__
+            x_data = self.x_array
+            y_data = self.y_array
+            coeffs = self.__spline_coefficients__
             ans = 0
             # Check to see if interval starts before point data
-            if a < xData[0]:
+            if a < x_data[0]:
                 if self.__extrapolation__ == "constant":
-                    ans += yData[0] * (xData[0] - a)
+                    ans += y_data[0] * (min(x_data[0], b) - a)
                 elif self.__extrapolation__ == "natural":
                     c = coeffs[:, 0]
-                    subB = a - xData[0]  # subA = 0
+                    sub_b = a - x_data[0]
+                    sub_a = min(b, x_data[0]) - x_data[0]
+                    ans += (
+                        (c[3] * sub_a**4) / 4
+                        + (c[2] * sub_a**3 / 3)
+                        + (c[1] * sub_a**2 / 2)
+                        + c[0] * sub_a
+                    )
                     ans -= (
-                        (c[3] * subB ** 4) / 4
-                        + (c[2] * subB ** 3 / 3)
-                        + (c[1] * subB ** 2 / 2)
-                        + c[0] * subB
+                        (c[3] * sub_b**4) / 4
+                        + (c[2] * sub_b**3 / 3)
+                        + (c[1] * sub_b**2 / 2)
+                        + c[0] * sub_b
                     )
                 else:
                     # self.__extrapolation__ = 'zero'
                     pass
-            # Integrate in subintervals between Xs of given data up to b
-            i = 0
-            while i < len(xData) - 1 and xData[i] < b:
-                if b < xData[i + 1]:
-                    subB = b - xData[i]  # subA = 0
+
+            # Integrate in subintervals between xs of given data up to b
+            i = max(np.searchsorted(x_data, a, side="left") - 1, 0)
+            while i < len(x_data) - 1 and x_data[i] < b:
+                if x_data[i] <= a <= x_data[i + 1] and x_data[i] <= b <= x_data[i + 1]:
+                    sub_a = a - x_data[i]
+                    sub_b = b - x_data[i]
+                elif x_data[i] <= a <= x_data[i + 1]:
+                    sub_a = a - x_data[i]
+                    sub_b = x_data[i + 1] - x_data[i]
+                elif b <= x_data[i + 1]:
+                    sub_a = 0
+                    sub_b = b - x_data[i]
                 else:
-                    subB = xData[i + 1] - xData[i]  # subA = 0
+                    sub_a = 0
+                    sub_b = x_data[i + 1] - x_data[i]
                 c = coeffs[:, i]
-                subB = xData[i + 1] - xData[i]  # subA = 0
                 ans += (
-                    (c[3] * subB ** 4) / 4
-                    + (c[2] * subB ** 3 / 3)
-                    + (c[1] * subB ** 2 / 2)
-                    + c[0] * subB
+                    (c[3] * sub_b**4) / 4
+                    + (c[2] * sub_b**3 / 3)
+                    + (c[1] * sub_b**2 / 2)
+                    + c[0] * sub_b
+                )
+                ans -= (
+                    (c[3] * sub_a**4) / 4
+                    + (c[2] * sub_a**3 / 3)
+                    + (c[1] * sub_a**2 / 2)
+                    + c[0] * sub_a
                 )
                 i += 1
             # Check to see if interval ends after point data
-            if b > xData[-1]:
+            if b > x_data[-1]:
                 if self.__extrapolation__ == "constant":
-                    ans += yData[-1] * (b - xData[-1])
+                    ans += y_data[-1] * (b - max(x_data[-1], a))
                 elif self.__extrapolation__ == "natural":
                     c = coeffs[:, -1]
-                    subA = xData[-1] - xData[-2]
-                    subB = b - xData[-2]
+                    sub_a = max(x_data[-1], a) - x_data[-2]
+                    sub_b = b - x_data[-2]
                     ans -= (
-                        (c[3] * subA ** 4) / 4
-                        + (c[2] * subA ** 3 / 3)
-                        + (c[1] * subA ** 2 / 2)
-                        + c[0] * subA
+                        (c[3] * sub_a**4) / 4
+                        + (c[2] * sub_a**3 / 3)
+                        + (c[1] * sub_a**2 / 2)
+                        + c[0] * sub_a
                     )
                     ans += (
-                        (c[3] * subB ** 4) / 4
-                        + (c[2] * subB ** 3 / 3)
-                        + (c[1] * subB ** 2 / 2)
-                        + c[0] * subB
+                        (c[3] * sub_b**4) / 4
+                        + (c[2] * sub_b**3 / 3)
+                        + (c[1] * sub_b**2 / 2)
+                        + c[0] * sub_b
                     )
                 else:
                     # self.__extrapolation__ = 'zero'
                     pass
         elif self.__interpolation__ == "linear" and numerical is False:
-            return np.trapz(self.source[:, 1], x=self.source[:, 0])
+            # Integrate from a to b using np.trapz
+            x_data = self.x_array
+            y_data = self.y_array
+            # Get data in interval
+            x_integration_data = x_data[(x_data >= a) & (x_data <= b)]
+            y_integration_data = y_data[(x_data >= a) & (x_data <= b)]
+            # Add integration limits to data
+            if self.__extrapolation__ == "zero":
+                if a >= x_data[0]:
+                    x_integration_data = np.concatenate(([a], x_integration_data))
+                    y_integration_data = np.concatenate(([self(a)], y_integration_data))
+                if b <= x_data[-1]:
+                    x_integration_data = np.concatenate((x_integration_data, [b]))
+                    y_integration_data = np.concatenate((y_integration_data, [self(b)]))
+            else:
+                x_integration_data = np.concatenate(([a], x_integration_data))
+                y_integration_data = np.concatenate(([self(a)], y_integration_data))
+                x_integration_data = np.concatenate((x_integration_data, [b]))
+                y_integration_data = np.concatenate((y_integration_data, [self(b)]))
+            # Integrate using np.trapz
+            ans = np.trapz(y_integration_data, x_integration_data)
         else:
             # Integrate numerically
-            ans, _ = integrate.quad(self, a, b, epsabs=0.1, limit=10000)
-        return ans
+            ans, _ = integrate.quad(self, a, b, epsabs=0.001, limit=10000)
+        return integration_sign * ans
+
+    def differentiate(self, x, dx=1e-6, order=1):
+        """Differentiate a Function object at a given point.
+
+        Parameters
+        ----------
+        x : float
+            Point at which to differentiate.
+        dx : float
+            Step size to use for numerical differentiation.
+        order : int
+            Order of differentiation.
+
+        Returns
+        -------
+        ans : float
+            Evaluated derivative.
+        """
+        if order == 1:
+            return (self.get_value(x + dx) - self.get_value(x - dx)) / (2 * dx)
+        elif order == 2:
+            return (
+                self.get_value(x + dx) - 2 * self.get_value(x) + self.get_value(x - dx)
+            ) / dx**2
+
+    def identityFunction(self):
+        """Returns a Function object that correspond to the identity mapping,
+        i.e. f(x) = x.
+        If the Function object is defined on an array, the identity Function
+        follows the same discretization, and has linear interpolation and
+        extrapolation.
+        If the Function is defined by a lambda, the identity Function is the
+        identity map 'lambda x: x'.
+
+        Returns
+        -------
+        result : Function
+            A Function object that corresponds to the identity mapping.
+        """
+
+        # Check if Function object source is array
+        if isinstance(self.source, np.ndarray):
+            return Function(
+                np.column_stack((self.x_array, self.x_array)),
+                inputs=self.__inputs__,
+                outputs=f"identity of {self.__outputs__}",
+                interpolation="linear",
+                extrapolation="natural",
+            )
+        else:
+            return Function(
+                lambda x: x,
+                inputs=self.__inputs__,
+                outputs=f"identity of {self.__outputs__}",
+            )
+
+    def derivativeFunction(self):
+        """Returns a Function object which gives the derivative of the Function object.
+
+        Returns
+        -------
+        result : Function
+            A Function object which gives the derivative of self.
+        """
+        # Check if Function object source is array
+        if isinstance(self.source, np.ndarray):
+            # Operate on grid values
+            ys = np.diff(self.y_array) / np.diff(self.x_array)
+            xs = self.source[:-1, 0] + np.diff(self.x_array) / 2
+            source = np.column_stack((xs, ys))
+            # Retrieve inputs, outputs and interpolation
+            inputs = self.__inputs__[:]
+            outputs = f"d({self.__outputs__[0]})/d({inputs[0]})"
+        else:
+            source = lambda x: self.differentiate(x)
+            inputs = self.__inputs__[:]
+            outputs = f"d({self.__outputs__[0]})/d({inputs[0]})"
+
+        # Create new Function object
+        return Function(source, inputs, outputs, self.__interpolation__)
+
+    def integral_function(self, lower=None, upper=None, datapoints=100):
+        """Returns a Function object representing the integral of the Function
+        object.
+
+        Parameters
+        ----------
+        lower : scalar, optional
+            The lower limit of the interval in which the function is to be
+            evaluated at. If the Function is given by a dataset, the default
+            value is the start of the dataset.
+        upper : scalar, optional
+            The upper limit of the interval in which the function is to be
+            evaluated at. If the Function is given by a dataset, the default
+            value is the end of the dataset.
+        datapoints : int, optional
+            The number of points in which the integral will be evaluated for
+            plotting it, which draws lines between each evaluated point.
+            The default value is 100.
+
+        Returns
+        -------
+        result : Function
+            The integral of the Function object.
+        """
+        if isinstance(self.source, np.ndarray):
+            lower = self.source[0, 0] if lower is None else lower
+            upper = self.source[-1, 0] if upper is None else upper
+            x_data = np.linspace(lower, upper, datapoints)
+            y_data = np.zeros(datapoints)
+            for i in range(datapoints):
+                y_data[i] = self.integral(lower, x_data[i])
+            return Function(
+                np.column_stack((x_data, y_data)),
+                inputs=self.__inputs__,
+                outputs=[o + " Integral" for o in self.__outputs__],
+            )
+        else:
+            lower = 0 if lower is None else lower
+            return Function(
+                lambda x: self.integral(lower, x),
+                inputs=self.__inputs__,
+                outputs=[o + " Integral" for o in self.__outputs__],
+            )
+
+    def isbijective(self):
+        """Checks whether the Function is bijective. Only applicable to
+        Functions whose source is a list of points, raises an error otherwise.
+
+        Returns
+        -------
+        result : bool
+            True if the Function is bijective, False otherwise.
+        """
+        if isinstance(self.source, np.ndarray):
+            x_data_distinct = set(self.x_array)
+            y_data_distinct = set(self.y_array)
+            distinct_map = set(zip(x_data_distinct, y_data_distinct))
+            return len(distinct_map) == len(x_data_distinct) == len(y_data_distinct)
+        else:
+            raise TypeError(
+                "Only Functions whose source is a list of points can be "
+                "checked for bijectivity."
+            )
+
+    def is_strictly_bijective(self):
+        """Checks whether the Function is "strictly" bijective.
+        Only applicable to Functions whose source is a list of points,
+        raises an error otherwise.
+
+        Notes
+        -----
+        By "strictly" bijective, this implementation considers the
+        list-of-points-defined Function bijective between each consecutive pair
+        of points. Therefore, the Function may be flagged as not bijective even
+        if the mapping between the set of points which define the Function is
+        bijective.
+
+        Returns
+        -------
+        result : bool
+            True if the Function is "strictly" bijective, False otherwise.
+
+        Examples
+        --------
+        >>> f = Function([[0, 0], [1, 1], [2, 4]])
+        >>> f.isbijective()
+        True
+        >>> f.is_strictly_bijective()
+        True
+
+        >>> f = Function([[-1, 1], [0, 0], [1, 1], [2, 4]])
+        >>> f.isbijective()
+        False
+        >>> f.is_strictly_bijective()
+        False
+
+        A Function which is not "strictly" bijective, but is bijective, can be
+        constructed as x^2 defined at -1, 0 and 2.
+
+        >>> f = Function([[-1, 1], [0, 0], [2, 4]])
+        >>> f.isbijective()
+        True
+        >>> f.is_strictly_bijective()
+        False
+        """
+        if isinstance(self.source, np.ndarray):
+            # Assuming domain is sorted, range must also be
+            y_data = self.y_array
+            # Both ascending and descending order means Function is bijective
+            y_data_diff = np.diff(y_data)
+            return np.all(y_data_diff >= 0) or np.all(y_data_diff <= 0)
+        else:
+            raise TypeError(
+                "Only Functions whose source is a list of points can be "
+                "checked for bijectivity."
+            )
+
+    def inverse_function(self, approx_func=None, tol=1e-4):
+        """
+        Returns the inverse of the Function. The inverse function of F is a
+        function that undoes the operation of F. The inverse of F exists if
+        and only if F is bijective. Makes the domain the range and the range
+        the domain.
+
+        If the Function is given by a list of points, its bijectivity is
+        checked and an error is raised if it is not bijective.
+        If the Function is given by a function, its bijection is not
+        checked and may lead to innacuracies outside of its bijective region.
+
+        Parameters
+        ----------
+        approx_func : callable, optional
+            A function that approximates the inverse of the Function. This
+            function is used to find the starting guesses for the inverse
+            root finding algorithm. This is better used when the inverse
+            in complex but has a simple approximation or when the root
+            finding algorithm performs poorly due to default start point.
+            The default is None in which case the starting point is zero.
+
+        tol : float, optional
+            The tolerance for the inverse root finding algorithm. The default
+            is 1e-4.
+
+        Returns
+        -------
+        result : Function
+            A Function whose domain and range have been inverted.
+        """
+        if isinstance(self.source, np.ndarray):
+            if self.is_strictly_bijective():
+                # Swap the columns
+                source = np.flip(self.source, axis=1)
+            else:
+                raise ValueError(
+                    "Function is not bijective, so it does not have an inverse."
+                )
+        else:
+            if approx_func is not None:
+                source = lambda x: self.find_input(x, start=approx_func(x), tol=tol)
+            else:
+                source = lambda x: self.find_input(x, start=0, tol=tol)
+        return Function(
+            source,
+            inputs=self.__outputs__,
+            outputs=self.__inputs__,
+            interpolation=self.__interpolation__,
+        )
+
+    def find_input(self, val, start, tol=1e-4):
+        """
+        Finds the optimal input for a given output.
+
+        Parameters
+        ----------
+        val : int, float
+            The value of the output.
+        start : int, float
+            Initial guess of the output.
+        tol : int, float
+            Tolerance for termination.
+
+        Returns
+        -------
+        result : ndarray
+            The value of the input which gives the output closest to val.
+        """
+        return optimize.root(
+            lambda x: self.get_value(x) - val,
+            start,
+            tol=tol,
+        ).x[0]
+
+    def average(self, lower, upper):
+        """
+        Returns the average of the function.
+
+        Parameters
+        ----------
+        lower : float
+            Lower point of the region that the average will be calculated at.
+        upper : float
+            Upper point of the region that the average will be calculated at.
+
+        Returns
+        -------
+        result : float
+            The average of the function.
+        """
+        return self.integral(lower, upper) / (upper - lower)
+
+    def average_function(self, lower=None):
+        """
+        Returns a Function object representing the average of the Function
+        object.
+
+        Parameters
+        ----------
+        lower : float
+            Lower limit of the new domain. Only required if the Function's
+            source is a callable instead of a list of points.
+
+        Returns
+        -------
+        result : Function
+            The average of the Function object.
+        """
+        if isinstance(self.source, np.ndarray):
+            if lower is None:
+                lower = self.source[0, 0]
+            upper = self.source[-1, 0]
+            x_data = np.linspace(lower, upper, 100)
+            y_data = np.zeros(100)
+            y_data[0] = self.source[:, 1][0]
+            for i in range(1, 100):
+                y_data[i] = self.average(lower, x_data[i])
+            return Function(
+                np.concatenate(([x_data], [y_data])).transpose(),
+                inputs=self.__inputs__,
+                outputs=[o + " Average" for o in self.__outputs__],
+            )
+        else:
+            if lower is None:
+                lower = 0
+            return Function(
+                lambda x: self.average(lower, x),
+                inputs=self.__inputs__,
+                outputs=[o + " Average" for o in self.__outputs__],
+            )
+
+    def compose(self, func, extrapolate=False):
+        """
+        Returns a Function object which is the result of inputting a function
+        into a function (i.e. f(g(x))). The domain will become the domain of
+        the input function and the range will become the range of the original
+        function.
+
+        Parameters
+        ----------
+        func : Function
+            The function to be inputted into the function.
+
+        extrapolate : bool, optional
+            Whether or not to extrapolate the function if the input function's
+            range is outside of the original function's domain. The default is
+            False.
+
+        Returns
+        -------
+        result : Function
+            The result of inputting the function into the function.
+        """
+        # Check if the input is a function
+        if not isinstance(func, Function):
+            raise TypeError("Input must be a Function object.")
+
+        if isinstance(self.source, np.ndarray) and isinstance(func.source, np.ndarray):
+            # Perform bounds check for composition
+            if not extrapolate:
+                if func.min < self.xinitial and func.max > self.xfinal:
+                    raise ValueError(
+                        f"Input Function image {func.min, func.max} must be within "
+                        f"the domain of the Function {self.xinitial, self.xfinal}."
+                    )
+
+            return Function(
+                np.concatenate(([func.x_array], [self(func.y_array)])).T,
+                inputs=func.__inputs__,
+                outputs=self.__outputs__,
+                interpolation=self.__interpolation__,
+                extrapolation=self.__extrapolation__,
+            )
+        else:
+            return Function(
+                lambda x: self(func(x)),
+                inputs=func.__inputs__,
+                outputs=self.__outputs__,
+                interpolation=self.__interpolation__,
+                extrapolation=self.__extrapolation__,
+            )
+
+
+class PiecewiseFunction(Function):
+    def __new__(
+        cls,
+        source,
+        inputs=["Scalar"],
+        outputs=["Scalar"],
+        interpolation="spline",
+        extrapolation=None,
+        datapoints=100,
+    ):
+        """
+        Creates a piecewise function from a dictionary of functions. The keys of
+        the dictionary must be tuples that represent the domain of the function.
+        The domains must be disjoint. The piecewise function will be evaluated
+        at datapoints points to create Function object.
+
+        Parameters
+        ----------
+        source: dictionary
+            A dictionary of Function objects, where the keys are the domains.
+        inputs : list
+            A list of strings that represent the inputs of the function.
+        outputs: list
+            A list of strings that represent the outputs of the function.
+        interpolation: str
+            The type of interpolation to use. The default value is 'akima'.
+        extrapolation: str
+            The type of extrapolation to use. The default value is None.
+        datapoints: int
+            The number of points in which the piecewise function will be
+            evaluated to create a base function. The default value is 100.
+        """
+        # Check if source is a dictionary
+        if not isinstance(source, dict):
+            raise TypeError("source must be a dictionary")
+        # Check if all keys are tuples
+        for key in source.keys():
+            if not isinstance(key, tuple):
+                raise TypeError("keys of source must be tuples")
+        # Check if all domains are disjoint
+        for key1 in source.keys():
+            for key2 in source.keys():
+                if key1 != key2:
+                    if key1[0] < key2[1] and key1[1] > key2[0]:
+                        raise ValueError("domains must be disjoint")
+
+        # Crate Function
+        def calc_output(func, inputs):
+            o = np.zeros(len(inputs))
+            for j in range(len(inputs)):
+                o[j] = func.get_value(inputs[j])
+            return o
+
+        inputData = []
+        outputData = []
+        for key in sorted(source.keys()):
+            i = np.linspace(key[0], key[1], datapoints)
+            i = i[~np.in1d(i, inputData)]
+            inputData = np.concatenate((inputData, i))
+
+            f = Function(source[key])
+            outputData = np.concatenate((outputData, calc_output(f, i)))
+
+        return Function(
+            np.concatenate(([inputData], [outputData])).T,
+            inputs=inputs,
+            outputs=outputs,
+            interpolation=interpolation,
+            extrapolation=extrapolation,
+        )
+
+
+def funcify_method(*args, **kwargs):
+    """Decorator factory to wrap methods as Function objects and save them as
+    cached properties.
+
+    Parameters
+    ----------
+    *args : list
+        Positional arguments to be passed to rocketpy.Function.
+    **kwargs : dict
+        Keyword arguments to be passed to rocketpy.Function.
+
+    Returns
+    -------
+    decorator : function
+        Decorator function to wrap callables as Function objects.
+
+    Examples
+    --------
+    There are 3 types of methods that this decorator supports:
+
+    1. Method which returns a valid rocketpy.Function source argument.
+
+    >>> from rocketpy.Function import funcify_method
+    >>> class Example():
+    ...     @funcify_method(inputs=['x'], outputs=['y'])
+    ...     def f(self):
+    ...         return lambda x: x**2
+    >>> example = Example()
+    >>> example.f
+    'Function from R1 to R1 : (x) → (y)'
+
+    Normal algebra can be performed afterwards:
+
+    >>> g = 2*example.f + 3
+    >>> g(2)
+    11
+
+    2. Method which returns a rocketpy.Function instance. An interesting use is
+    to reset input and output names after algebraic operations.
+
+    >>> class Example():
+    ...     @funcify_method(inputs=['x'], outputs=['x**3'])
+    ...     def cube(self):
+    ...         f = Function(lambda x: x**2)
+    ...         g = Function(lambda x: x**5)
+    ...         return g / f
+    >>> example = Example()
+    >>> example.cube
+    'Function from R1 to R1 : (x) → (x**3)'
+
+    3. Method which is itself a valid rocketpy.Function source argument.
+
+    >>> class Example():
+    ...     @funcify_method('x', 'f(x)')
+    ...     def f(self, x):
+    ...         return x**2
+    >>> example = Example()
+    >>> example.f
+    'Function from R1 to R1 : (x) → (f(x))'
+
+    In order to reset the cache, just delete de attribute from the instance:
+
+    >>> del example.f
+
+    Once it is requested again, it will be re-created as a new Function object:
+
+    >>> example.f
+    'Function from R1 to R1 : (x) → (f(x))'
+    """
+    func = None
+    if len(args) == 1 and callable(args[0]):
+        func = args[0]
+        args = []
+
+    class funcify_method_decorator:
+        def __init__(self, func):
+            self.func = func
+            self.attrname = None
+            self.__doc__ = func.__doc__
+
+        def __set_name__(self, owner, name):
+            self.attrname = name
+
+        def __get__(self, instance, owner=None):
+            if instance is None:
+                return self
+            cache = instance.__dict__
+            try:
+                # If cache is ready, return it
+                val = cache[self.attrname]
+            except KeyError:
+                # If cache is not ready, create it
+                try:
+                    # Handle methods which return Function instances
+                    val = self.func(instance).reset(*args, **kwargs)
+                except AttributeError:
+                    # Handle methods which return a valid source
+                    source = self.func(instance)
+                    val = Function(source, *args, **kwargs)
+                except TypeError:
+                    # Handle methods which are the source themselves
+                    source = lambda *_: self.func(instance, *_)
+                    val = Function(source, *args, **kwargs)
+                except Exception:
+                    raise Exception(
+                        "Could not create Function object from method "
+                        f"{self.func.__name__}."
+                    )
+
+                val.__doc__ = self.__doc__
+                val.__cached__ = True
+                cache[self.attrname] = val
+            return val
+
+    if func:
+        return funcify_method_decorator(func)
+    else:
+        return funcify_method_decorator
+
+
+def reset_funcified_methods(instance):
+    """Resets all the funcified methods of the instance. It does so by
+    deleting the current Functions, which will make the interperter redefine
+    them when they are called. This is useful when the instance has changed
+    and the methods need to be recalculated.
+
+    Parameters
+    ----------
+    instance : object
+        The instance of the class whose funcified methods will be recalculated.
+        The class must have a mutable __dict__ attribute.
+
+    Return
+    ------
+    None
+    """
+    for key in list(instance.__dict__):
+        if hasattr(instance.__dict__[key], "__cached__"):
+            instance.__dict__.pop(key)
+
+
+if __name__ == "__main__":
+    import doctest
 
-    # Not implemented
-    def differentiate(self, x, dx=1e-6):
-        return (self.getValue(x + dx) - self.getValue(x - dx)) / (2 * dx)
-        # h = (10)**-300
-        # z = x + h*1j
-        # return self(z).imag/h
+    doctest.testmod()
```

### Comparing `rocketpy-0.9.9/rocketpy/Rocket.py` & `rocketpy-1.0.0a1/rocketpy/Rocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,739 +1,1034 @@
 # -*- coding: utf-8 -*-
 
-__author__ = "Giovani Hidalgo Ceotto, Franz Masatoshi Yuri"
-__copyright__ = "Copyright 20XX, Projeto Jupiter"
+__author__ = "Giovani Hidalgo Ceotto, Franz Masatoshi Yuri, Mateus Stano Junqueira, Kaleb Ramos Wanderley, Calebe Gomes Teles, Matheus Doretto"
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __license__ = "MIT"
 
-import re
-import math
-import bisect
 import warnings
-import time
-from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
 
 import numpy as np
-from scipy import integrate
-from scipy import linalg
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
-from numpy import genfromtxt
 
-from .Function import Function
+from .AeroSurface import (
+    EllipticalFins,
+    Fins,
+    NoseCone,
+    RailButtons,
+    Tail,
+    TrapezoidalFins,
+)
+from .Components import Components
+from .Function import Function, funcify_method
+from .motors.Motor import EmptyMotor
+from .Parachute import Parachute
+from .plots.rocket_plots import _RocketPlots
+from .prints.rocket_prints import _RocketPrints
 
 
 class Rocket:
 
-    """Keeps all rocket and parachute information.
+    """Keeps rocket information.
 
     Attributes
     ----------
         Geometrical attributes:
         Rocket.radius : float
             Rocket's largest radius in meters.
         Rocket.area : float
             Rocket's circular cross section largest frontal area in squared
             meters.
-        Rocket.distanceRocketNozzle : float
-            Distance between rocket's center of mass, without propellant,
-            to the exit face of the nozzle, in meters. Always positive.
-        Rocket.distanceRocketPropellant : float
-            Distance between rocket's center of mass, without propellant,
-            to the center of mass of propellant, in meters. Always positive.
+        Rocket.center_of_dry_mass_position : float
+            Position, in m, of the rocket's center of dry mass (i.e. center of
+            mass without propellant) relative to the rocket's coordinate system.
+            See `Rocket.coordinate_system_orientation` for more information
+            regarding the rocket's coordinate system.
+        Rocket.coordinate_system_orientation : string
+            String defining the orientation of the rocket's coordinate system.
+            The coordinate system is defined by the rocket's axis of symmetry.
+            The system's origin may be placed anywhere along such axis, such as
+            in the nozzle or in the nose cone, and must be kept the same for all
+            other positions specified. If "tail_to_nose", the coordinate system
+            is defined with the rocket's axis of symmetry pointing from the
+            rocket's tail to the rocket's nose cone. If "nose_to_tail", the
+            coordinate system is defined with the rocket's axis of symmetry
+            pointing from the rocket's nose cone to the rocket's tail.
 
         Mass and Inertia attributes:
         Rocket.mass : float
             Rocket's mass without propellant in kg.
-        Rocket.inertiaI : float
-            Rocket's moment of inertia, without propellant, with respect to
-            to an axis perpendicular to the rocket's axis of cylindrical
-            symmetry, in kg*m^2.
-        Rocket.inertiaZ : float
-            Rocket's moment of inertia, without propellant, with respect to
-            the rocket's axis of cylindrical symmetry, in kg*m^2.
-        Rocket.centerOfMass : Function
-            Distance of the rocket's center of mass, including propellant,
-            to rocket's center of mass without propellant, in meters.
-            Expressed as a function of time.
-        Rocket.reducedMass : Function
+        Rocket.center_of_mass : Function
+            Position of the rocket's center of mass, including propellant, relative
+            to the user defined rocket reference system.
+            See `Rocket.coordinate_system_orientation` for more information regarding the
+            coordinate system.
+            Expressed in meters as a function of time.
+        Rocket.reduced_mass : Function
             Function of time expressing the reduced mass of the rocket,
             defined as the product of the propellant mass and the mass
             of the rocket without propellant, divided by the sum of the
             propellant mass and the rocket mass.
-        Rocket.totalMass : Function
+        Rocket.total_mass : Function
             Function of time expressing the total mass of the rocket,
             defined as the sum of the propellant mass and the rocket
             mass without propellant.
-        Rocket.thrustToWeight : Function
+        Rocket.thrust_to_weight : Function
             Function of time expressing the motor thrust force divided by rocket
             weight. The gravitational acceleration is assumed as 9.80665 m/s^2.
 
         Eccentricity attributes:
-        Rocket.cpEccentricityX : float
+        Rocket.cp_eccentricity_x : float
             Center of pressure position relative to center of mass in the x
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.cpEccentricityY : float
+        Rocket.cp_eccentricity_y : float
             Center of pressure position relative to center of mass in the y
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.thrustEccentricityY : float
+        Rocket.thrust_eccentricity_y : float
             Thrust vector position relative to center of mass in the y
             axis, perpendicular to axis of cylindrical symmetry, in meters.
-        Rocket.thrustEccentricityX : float
+        Rocket.thrust_eccentricity_x : float
             Thrust vector position relative to center of mass in the x
             axis, perpendicular to axis of cylindrical symmetry, in meters.
 
-        Parachute attributes:
-        Rocket.parachutes : list
-            List of parachutes of the rocket.
-            Each parachute has the following attributes:
-            name : string
-                Parachute name, such as drogue and main. Has no impact in
-                simulation, as it is only used to display data in a more
-                organized matter.
-            CdS : float
-                Drag coefficient times reference area for parachute. It is
-                used to compute the drag force exerted on the parachute by
-                the equation F = ((1/2)*rho*V^2)*CdS, that is, the drag
-                force is the dynamic pressure computed on the parachute
-                times its CdS coefficient. Has units of area and must be
-                given in squared meters.
-            trigger : function
-                Function which defines if the parachute ejection system is
-                to be triggered. It must take as input the freestream
-                pressure in pascal and the state vector of the simulation,
-                which is defined by [x, y, z, vx, vy, vz, e0, e1, e2, e3, wx, wy, wz].
-                It will be called according to the sampling rate given next.
-                It should return True if the parachute ejection system is
-                to be triggered and False otherwise.
-            samplingRate : float, optional
-                Sampling rate in which the trigger function works. It is used to
-                simulate the refresh rate of onboard sensors such as barometers.
-                Default value is 100. Value must be given in hertz.
-            lag : float, optional
-                Time between the parachute ejection system is triggered and the
-                parachute is fully opened. During this time, the simulation will
-                consider the rocket as flying without a parachute. Default value
-                is 0. Must be given in seconds.
-            noise : tuple, list, optional
-                List in the format (mean, standard deviation, time-correlation).
-                The values are used to add noise to the pressure signal which is
-                passed to the trigger function. Default value is (0, 0, 0). Units
-                are in pascal.
-            noiseSignal : list
-                List of (t, noise signal) corresponding to signal passed to
-                trigger function. Completed after running a simulation.
-            noisyPressureSignal : list
-                List of (t, noisy pressure signal) that is passed to the
-                trigger function. Completed after running a simulation.
-            cleanPressureSignal : list
-                List of (t, clean pressure signal) corresponding to signal passed to
-                trigger function. Completed after running a simulation.
-            noiseSignalFunction : Function
-                Function of noiseSignal.
-            noisyPressureSignalFunction : Function
-                Function of noisyPressureSignal.
-            cleanPressureSignalFunction : Function
-                Function of cleanPressureSignal.
-
         Aerodynamic attributes
-        Rocket.aerodynamicSurfaces : list
-            List of aerodynamic surfaces of the rocket.
-        Rocket.staticMargin : float
+        Rocket.aerodynamic_surfaces : list
+            Collection of aerodynamic surfaces of the rocket. Holds Nose cones,
+            Fin sets, and Tails.
+        Rocket.cp_position : float
+            Rocket's center of pressure position relative to the user defined rocket
+            reference system. See `Rocket.coordinate_system_orientation` for more information
+            regarding the reference system.
+            Expressed in meters.
+        Rocket.static_margin : float
             Float value corresponding to rocket static margin when
             loaded with propellant in units of rocket diameter or
             calibers.
-        Rocket.powerOffDrag : Function
+        Rocket.power_off_drag : Function
             Rocket's drag coefficient as a function of Mach number when the
             motor is off.
-        Rocket.powerOnDrag : Function
+        Rocket.power_on_drag : Function
             Rocket's drag coefficient as a function of Mach number when the
             motor is on.
+        Rocket.rail_buttons : RailButtons
+            RailButtons object containing the rail buttons information.
 
         Motor attributes:
         Rocket.motor : Motor
             Rocket's motor. See Motor class for more details.
+        Rocket.motor_position : float
+            Position, in m, of the motor's nozzle exit area relative to the user defined
+            rocket coordinate system. See `Rocket.coordinate_system_orientation` for more
+            information regarding the rocket's coordinate system.
+        Rocket.center_of_propellant_position : Function
+            Position of the propellant's center of mass relative to the user defined
+            rocket reference system. See `Rocket.coordinate_system_orientation` for more
+            information regarding the rocket's coordinate system.
+            Expressed in meters as a function of time.
     """
 
     def __init__(
         self,
-        motor,
-        mass,
-        inertiaI,
-        inertiaZ,
         radius,
-        distanceRocketNozzle,
-        distanceRocketPropellant,
-        powerOffDrag,
-        powerOnDrag,
+        mass,
+        inertia,
+        power_off_drag,
+        power_on_drag,
+        center_of_mass_without_motor,
+        coordinate_system_orientation="tail_to_nose",
     ):
         """Initializes Rocket class, process inertial, geometrical and
         aerodynamic parameters.
 
         Parameters
         ----------
-        motor : Motor
-            Motor used in the rocket. See Motor class for more information.
-        mass : int, float
-            Unloaded rocket total mass (without propelant) in kg.
-        inertiaI : int, float
-            Unloaded rocket lateral (perpendicular to axis of symmetry)
-            moment of inertia (without propelant) in kg m^2.
-        inertiaZ : int, float
-            Unloaded rocket axial moment of inertia (without propelant)
-            in kg m^2.
         radius : int, float
-            Rocket biggest outer radius in meters.
-        distanceRocketNozzle : int, float
-            Distance from rocket's unloaded center of mass to nozzle outlet,
-            in meters. Generally negative, meaning a negative position in the
-            z axis which has an origin in the rocket's center of mass (without
-            propellant) and points towards the nose cone.
-        distanceRocketPropellant : int, float
-            Distance from rocket's unloaded center of mass to propellant
-            center of mass, in meters. Generally negative, meaning a negative
-            position in the z axis which has an origin in the rocket's center
-            of mass (with out propellant) and points towards the nose cone.
-        powerOffDrag : int, float, callable, string, array
+            Rocket largest outer radius in meters.
+        mass : int, float
+            Rocket total mass without motor in kg.
+        inertia : tuple, list
+            Tuple or list containing the rocket's dry mass inertia tensor
+            components, in kg*m^2.
+            Assuming e_3 is the rocket's axis of symmetry, e_1 and e_2 are
+            orthogonal and form a plane perpendicular to e_3, the dry mass
+            inertia tensor components must be given in the following order:
+            (I_11, I_22, I_33, I_12, I_13, I_23), where I_ij is the
+            component of the inertia tensor in the direction of e_i x e_j.
+            Alternatively, the inertia tensor can be given as (I_11, I_22, I_33),
+            where I_12 = I_13 = I_23 = 0.
+        power_off_drag : int, float, callable, string, array
             Rocket's drag coefficient when the motor is off. Can be given as an
             entry to the Function class. See help(Function) for more
             information. If int or float is given, it is assumed constant. If
             callable, string or array is given, it must be a function of Mach
             number only.
-        powerOnDrag : int, float, callable, string, array
+        power_on_drag : int, float, callable, string, array
             Rocket's drag coefficient when the motor is on. Can be given as an
             entry to the Function class. See help(Function) for more
             information. If int or float is given, it is assumed constant. If
             callable, string or array is given, it must be a function of Mach
             number only.
+        center_of_mass_without_motor : int, float
+            Position, in m, of the rocket's center of mass without motor
+            relative to the rocket's coordinate system. Default is 0, which
+            means the center of dry mass is chosen as the origin, to comply
+            with the legacy behavior of versions 0.X.Y.
+            See `Rocket.coordinate_system_orientation` for more information
+            regarding the rocket's coordinate system.
+        coordinate_system_orientation : string, optional
+            String defining the orientation of the rocket's coordinate system. The
+            coordinate system is defined by the rocket's axis of symmetry. The system's
+            origin may be placed anywhere along such axis, such as in the nozzle or in
+            the nose cone, and must be kept the same for all other positions specified.
+            The two options available are: "tail_to_nose" and "nose_to_tail". The first
+            defines the coordinate system with the rocket's axis of symmetry pointing
+            from the rocket's tail to the rocket's nose cone. The second option defines
+            the coordinate system with the rocket's axis of symmetry pointing from the
+            rocket's nose cone to the rocket's tail. Default is "tail_to_nose".
 
         Returns
         -------
         None
         """
+        # Define coordinate system orientation
+        self.coordinate_system_orientation = coordinate_system_orientation
+        if coordinate_system_orientation == "tail_to_nose":
+            self._csys = 1
+        elif coordinate_system_orientation == "nose_to_tail":
+            self._csys = -1
+        else:
+            raise TypeError(
+                "Invalid coordinate system orientation. Please choose between "
+                + '"tail_to_nose" and "nose_to_tail".'
+            )
+
         # Define rocket inertia attributes in SI units
         self.mass = mass
-        self.inertiaI = inertiaI
-        self.inertiaZ = inertiaZ
-        self.centerOfMass = distanceRocketPropellant * motor.mass / (mass + motor.mass)
+        inertia = (*inertia, 0, 0, 0) if len(inertia) == 3 else inertia
+        self.I_11_without_motor = inertia[0]
+        self.I_22_without_motor = inertia[1]
+        self.I_33_without_motor = inertia[2]
+        self.I_12_without_motor = inertia[3]
+        self.I_13_without_motor = inertia[4]
+        self.I_23_without_motor = inertia[5]
 
         # Define rocket geometrical parameters in SI units
+        self.center_of_mass_without_motor = center_of_mass_without_motor
         self.radius = radius
-        self.area = np.pi * self.radius ** 2
-
-        # Center of mass distance to points of interest
-        self.distanceRocketNozzle = distanceRocketNozzle
-        self.distanceRocketPropellant = distanceRocketPropellant
+        self.area = np.pi * self.radius**2
 
         # Eccentricity data initialization
-        self.cpEccentricityX = 0
-        self.cpEccentricityY = 0
-        self.thrustEccentricityY = 0
-        self.thrustEccentricityX = 0
+        self.cp_eccentricity_x = 0
+        self.cp_eccentricity_y = 0
+        self.thrust_eccentricity_y = 0
+        self.thrust_eccentricity_x = 0
 
         # Parachute data initialization
         self.parachutes = []
 
-        # Rail button data initialization
-        self.railButtons = None
-
         # Aerodynamic data initialization
-        self.aerodynamicSurfaces = []
-        self.cpPosition = 0
-        self.staticMargin = Function(
+        self.aerodynamic_surfaces = Components()
+
+        # Rail buttons data initialization
+        self.rail_buttons = Components()
+
+        self.cp_position = 0
+        self.static_margin = Function(
             lambda x: 0, inputs="Time (s)", outputs="Static Margin (c)"
         )
 
         # Define aerodynamic drag coefficients
-        self.powerOffDrag = Function(
-            powerOffDrag,
+        self.power_off_drag = Function(
+            power_off_drag,
             "Mach Number",
             "Drag Coefficient with Power Off",
-            "spline",
+            "linear",
             "constant",
         )
-        self.powerOnDrag = Function(
-            powerOnDrag,
+        self.power_on_drag = Function(
+            power_on_drag,
             "Mach Number",
             "Drag Coefficient with Power On",
-            "spline",
+            "linear",
             "constant",
         )
+        self.cp_position = 0  # Set by self.evaluate_static_margin()
 
-        # Define motor to be used
-        self.motor = motor
+        # Create a, possibly, temporary empty motor
+        # self.motors = Components()  # currently unused since only one motor is supported
+        self.add_motor(motor=EmptyMotor(), position=0)
 
         # Important dynamic inertial quantities
-        self.reducedMass = None
-        self.totalMass = None
-
-        # Calculate dynamic inertial quantities
-        self.evaluateReducedMass()
-        self.evaluateTotalMass()
-        self.thrustToWeight = self.motor.thrust / (9.80665 * self.totalMass)
-        self.thrustToWeight.setInputs("Time (s)")
-        self.thrustToWeight.setOutputs("Thrust/Weight")
+        self.center_of_mass = None
+        self.reduced_mass = None
+        self.total_mass = None
+        self.dry_mass = None
+
+        # calculate dynamic inertial quantities
+        self.evaluate_dry_mass()
+        self.evaluate_total_mass()
+        self.evaluate_center_of_dry_mass()
+        self.evaluate_center_of_mass()
+        self.evaluate_reduced_mass()
+        self.evaluate_thrust_to_weight()
 
         # Evaluate static margin (even though no aerodynamic surfaces are present yet)
-        self.evaluateStaticMargin()
+        self.evaluate_static_margin()
+
+        # Initialize plots and prints object
+        self.prints = _RocketPrints(self)
+        self.plots = _RocketPlots(self)
 
         return None
 
-    def evaluateReducedMass(self):
-        """Calculates and returns the rocket's total reduced mass. The
-        reduced mass is defined as the product of the propellant mass
-        and the mass of the rocket without propellant, divided by the
-        sum of the propellant mass and the rocket mass. The function
-        returns an object of the Function class and is defined as a
-        function of time.
+    @property
+    def nosecones(self):
+        return self.aerodynamic_surfaces.get_by_type(NoseCone)
+
+    @property
+    def fins(self):
+        return self.aerodynamic_surfaces.get_by_type(Fins)
+
+    @property
+    def tails(self):
+        return self.aerodynamic_surfaces.get_by_type(Tail)
+
+    def evaluate_total_mass(self):
+        """Calculates and returns the rocket's total mass. The total
+        mass is defined as the sum of the motor mass with propellant and the
+        rocket mass without propellant. The function returns an object
+        of the Function class and is defined as a function of time.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        self.reducedMass : Function
-            Function of time expressing the reduced mass of the rocket,
-            defined as the product of the propellant mass and the mass
-            of the rocket without propellant, divided by the sum of the
-            propellant mass and the rocket mass.
+        self.total_mass : rocketpy.Function
+            Function of time expressing the total mass of the rocket,
+            defined as the sum of the propellant mass and the rocket
+            mass without propellant.
         """
         # Make sure there is a motor associated with the rocket
         if self.motor is None:
             print("Please associate this rocket with a motor!")
             return False
 
-        # Retrieve propellant mass as a function of time
-        motorMass = self.motor.mass
-
-        # Retrieve constant rocket mass without propellant
-        mass = self.mass
-
-        # Calculate reduced mass
-        self.reducedMass = motorMass * mass / (motorMass + mass)
-        self.reducedMass.setOutputs("Reduced Mass (kg)")
+        # Calculate total mass by summing up propellant and dry mass
+        self.total_mass = self.mass + self.motor.total_mass
+        self.total_mass.set_outputs("Total Mass (Rocket + Propellant) (kg)")
 
-        # Return reduced mass
-        return self.reducedMass
+        # Return total mass
+        return self.total_mass
 
-    def evaluateTotalMass(self):
-        """Calculates and returns the rocket's total mass. The total
-        mass is defined as the sum of the propellant mass and the
-        rocket mass without propellant. The function returns an object
+    def evaluate_dry_mass(self):
+        """Calculates and returns the rocket's dry mass. The dry
+        mass is defined as the sum of the motor's dry mass and the
+        rocket mass without motor. The function returns an object
         of the Function class and is defined as a function of time.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        self.totalMass : Function
+        self.total_mass : rocketpy.Function
             Function of time expressing the total mass of the rocket,
             defined as the sum of the propellant mass and the rocket
             mass without propellant.
         """
         # Make sure there is a motor associated with the rocket
         if self.motor is None:
             print("Please associate this rocket with a motor!")
             return False
 
-        # Calculate total mass by summing up propellant and dry mass
-        self.totalMass = self.mass + self.motor.mass
-        self.totalMass.setOutputs("Total Mass (Rocket + Propellant) (kg)")
+        # Calculate total dry mass: motor (without propellant) + rocket
+        self.dry_mass = self.mass + self.motor.dry_mass
 
         # Return total mass
-        return self.totalMass
+        return self.dry_mass
+
+    def evaluate_center_of_mass(self):
+        """Evaluates rocket center of mass position relative to user defined rocket
+        reference system.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.center_of_mass : rocketpy.Function
+            Function of time expressing the rocket's center of mass position relative to
+            user defined rocket reference system.
+            See `Rocket.coordinate_system_orientation` for more information.
+        """
+        # Compute center of mass position
+        self.center_of_mass = (
+            self.center_of_mass_without_motor * self.mass
+            + self.motor_center_of_mass_position * self.motor.total_mass
+        ) / self.total_mass
+        self.center_of_mass.set_inputs("Time (s)")
+        self.center_of_mass.set_outputs("Center of Mass Position (m)")
+
+        return self.center_of_mass
+
+    def evaluate_center_of_dry_mass(self):
+        """Evaluates rocket center dry of mass (i.e. without propellant)
+        position relative to user defined rocket reference system.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.center_of_dry_mass : int, float
+            Rocket's center of dry mass position relative to user defined rocket
+            reference system. See `Rocket.coordinate_system_orientation` for more
+            information.
+        """
+        # Compute center of mass position
+        self.center_of_dry_mass_position = (
+            self.center_of_mass_without_motor * self.mass
+            + self.motor_center_of_dry_mass_position * self.motor.dry_mass
+        ) / self.dry_mass
+
+        return self.center_of_dry_mass_position
 
-    def evaluateStaticMargin(self):
+    def evaluate_reduced_mass(self):
+        """Calculates and returns the rocket's total reduced mass. The
+        reduced mass is defined as the product of the propellant mass
+        and the mass of the rocket without propellant, divided by the
+        sum of the propellant mass and the rocket mass. The function
+        returns an object of the Function class and is defined as a
+        function of time.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.reduced_mass : Function
+            Function of time expressing the reduced mass of the rocket,
+            defined as the product of the propellant mass and the mass
+            of the rocket without propellant, divided by the sum of the
+            propellant mass and the rocket mass.
+        """
+        # Make sure there is a motor associated with the rocket
+        if self.motor is None:
+            print("Please associate this rocket with a motor!")
+            return False
+
+        # Retrieve propellant mass as a function of time
+        motor_mass = self.motor.propellant_mass
+
+        # retrieve constant rocket mass without propellant
+        mass = self.dry_mass
+
+        # calculate reduced mass
+        self.reduced_mass = motor_mass * mass / (motor_mass + mass)
+        self.reduced_mass.set_outputs("Reduced Mass (kg)")
+
+        # Return reduced mass
+        return self.reduced_mass
+
+    def evaluate_thrust_to_weight(self):
+        """Evaluates thrust to weight as a Function of time.
+
+        Uses g = 9.80665 m/s² as nominal gravity for weight calculation.
+
+        Returns
+        -------
+        None
+        """
+        self.thrust_to_weight = self.motor.thrust / (9.80665 * self.total_mass)
+        self.thrust_to_weight.set_inputs("Time (s)")
+        self.thrust_to_weight.set_outputs("Thrust/Weight")
+
+    def evaluate_static_margin(self):
         """Calculates and returns the rocket's static margin when
         loaded with propellant. The static margin is saved and returned
-        in units of rocket diameter or calibers.
+        in units of rocket diameter or calibers. This function also calculates
+        the rocket center of pressure and total lift coefficients.
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        self.staticMargin : float
+        self.static_margin : float
             Float value corresponding to rocket static margin when
             loaded with propellant in units of rocket diameter or
             calibers.
         """
-        # Initialize total lift coefficient derivative and center of pressure
-        self.totalLiftCoeffDer = 0
-        self.cpPosition = 0
+        # Initialize total lift coefficient derivative and center of pressure position
+        self.total_lift_coeff_der = 0
+        self.cp_position = 0
 
         # Calculate total lift coefficient derivative and center of pressure
-        if len(self.aerodynamicSurfaces) > 0:
-            for aerodynamicSurface in self.aerodynamicSurfaces:
-                self.totalLiftCoeffDer += aerodynamicSurface[1].differentiate(
-                    x=1e-2, dx=1e-3
-                )
-                self.cpPosition += (
-                    aerodynamicSurface[1].differentiate(x=1e-2, dx=1e-3)
-                    * aerodynamicSurface[0][2]
+        if len(self.aerodynamic_surfaces) > 0:
+            for aero_surface, position in self.aerodynamic_surfaces:
+                self.total_lift_coeff_der += aero_surface.clalpha(0)
+                self.cp_position += aero_surface.clalpha(0) * (
+                    position - self._csys * aero_surface.cpz
                 )
-            self.cpPosition /= self.totalLiftCoeffDer
+            self.cp_position /= self.total_lift_coeff_der
 
         # Calculate static margin
-        self.staticMargin = (self.centerOfMass - self.cpPosition) / (2 * self.radius)
-        self.staticMargin.setInputs("Time (s)")
-        self.staticMargin.setOutputs("Static Margin (c)")
-        self.staticMargin.setDiscrete(
-            lower=0, upper=self.motor.burnOutTime, samples=200
+        self.static_margin = (self.center_of_mass - self.cp_position) / (
+            2 * self.radius
         )
+        self.static_margin *= (
+            self._csys
+        )  # Change sign if coordinate system is upside down
+        self.static_margin.set_inputs("Time (s)")
+        self.static_margin.set_outputs("Static Margin (c)")
+        self.static_margin.set_discrete(
+            lower=0, upper=self.motor.burn_out_time, samples=200
+        )
+        return None
 
-        # Return self
-        return self
+    def evaluate_dry_inertias(self):
+        """Calculates and returns the rocket's dry inertias relative to
+        the rocket's center of mass. The inertias are saved and returned
+        in units of kg*m².
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.dry_I_11 : float
+            Float value corresponding to rocket inertia tensor 11
+            component, which corresponds to the inertia relative to the
+            e_1 axis, centered at the instantaneous center of mass.
+        self.dry_I_22 : float
+            Float value corresponding to rocket inertia tensor 22
+            component, which corresponds to the inertia relative to the
+            e_2 axis, centered at the instantaneous center of mass.
+        self.dry_I_33 : float
+            Float value corresponding to rocket inertia tensor 33
+            component, which corresponds to the inertia relative to the
+            e_3 axis, centered at the instantaneous center of mass.
+        self.dry_I_12 : float
+            Float value corresponding to rocket inertia tensor 12
+            component, which corresponds to the inertia relative to the
+            e_1 and e_2 axes, centered at the instantaneous center of mass.
+        self.dry_I_13 : float
+            Float value corresponding to rocket inertia tensor 13
+            component, which corresponds to the inertia relative to the
+            e_1 and e_3 axes, centered at the instantaneous center of mass.
+        self.dry_I_23 : float
+            Float value corresponding to rocket inertia tensor 23
+            component, which corresponds to the inertia relative to the
+            e_2 and e_3 axes, centered at the instantaneous center of mass.
+
+        Notes
+        -----
+        The e_1 and e_2 directions are assumed to be the directions
+        perpendicular to the rocket axial direction.
+        The e_3 direction is assumed to be the direction parallel to the axis
+        of symmetry of the rocket.
+        RocketPy follows the definition of the inertia tensor as in [1], which
+        includes the minus sign for all products of inertia.
+
+        References
+        ----------
+        .. [1] https://en.wikipedia.org/wiki/Moment_of_inertia#Inertia_tensor
+        """
+        # Compute axes distances
+        noMCM_to_CDM = (
+            self.center_of_mass_without_motor - self.center_of_dry_mass_position
+        )
+        motorCDM_to_CDM = (
+            self.motor_center_of_dry_mass_position - self.center_of_dry_mass_position
+        )
+
+        # Compute dry inertias
+        self.dry_I_11 = (
+            self.I_11_without_motor
+            + self.mass * noMCM_to_CDM**2
+            + self.motor.dry_I_11
+            + self.motor.dry_mass * motorCDM_to_CDM**2
+        )
+        self.dry_I_22 = (
+            self.I_22_without_motor
+            + self.mass * noMCM_to_CDM**2
+            + self.motor.dry_I_22
+            + self.motor.dry_mass * motorCDM_to_CDM**2
+        )
+        self.dry_I_33 = self.I_33_without_motor + self.motor.dry_I_33
+        self.dry_I_12 = self.I_12_without_motor + self.motor.dry_I_12
+        self.dry_I_13 = self.I_13_without_motor + self.motor.dry_I_13
+        self.dry_I_23 = self.I_23_without_motor + self.motor.dry_I_23
+
+        # Return inertias
+        return (
+            self.dry_I_11,
+            self.dry_I_22,
+            self.dry_I_33,
+            self.dry_I_12,
+            self.dry_I_13,
+            self.dry_I_23,
+        )
+
+    def evaluate_inertias(self):
+        """Calculates and returns the rocket's inertias relative to
+        the rocket's center of mass. The inertias are saved and returned
+        in units of kg*m².
 
-    def addTail(self, topRadius, bottomRadius, length, distanceToCM):
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.I_11 : float
+            Float value corresponding to rocket inertia tensor 11
+            component, which corresponds to the inertia relative to the
+            e_1 axis, centered at the instantaneous center of mass.
+        self.I_22 : float
+            Float value corresponding to rocket inertia tensor 22
+            component, which corresponds to the inertia relative to the
+            e_2 axis, centered at the instantaneous center of mass.
+        self.I_33 : float
+            Float value corresponding to rocket inertia tensor 33
+            component, which corresponds to the inertia relative to the
+            e_3 axis, centered at the instantaneous center of mass.
+
+        Notes
+        -----
+        The e_1 and e_2 directions are assumed to be the directions
+        perpendicular to the rocket axial direction.
+        The e_3 direction is assumed to be the direction parallel to the axis
+        of symmetry of the rocket.
+        RocketPy follows the definition of the inertia tensor as in [1], which
+        includes the minus sign for all products of inertia.
+
+        References
+        ----------
+        .. [1] https://en.wikipedia.org/wiki/Moment_of_inertia#Inertia_tensor
+        """
+        # Get masses
+        prop_mass = self.motor.propellant_mass  # Propellant mass as a function of time
+        dry_mass = self.dry_mass  # Constant rocket dry mass without propellant
+
+        # Compute axes distances
+        CM_to_CDM = self.center_of_mass - self.center_of_dry_mass_position
+        CM_to_CPM = self.center_of_mass - self.center_of_propellant_position
+
+        # Compute inertias
+        self.I_11 = (
+            self.dry_I_11
+            + self.motor.I_11
+            + dry_mass * CM_to_CDM**2
+            + prop_mass * CM_to_CPM**2
+        )
+        self.I_22 = (
+            self.dry_I_22
+            + self.motor.I_22
+            + dry_mass * CM_to_CDM**2
+            + prop_mass * CM_to_CPM**2
+        )
+        self.I_33 = self.dry_I_33 + self.motor.I_33
+        self.I_12 = self.dry_I_12 + self.motor.I_12
+        self.I_13 = self.dry_I_13 + self.motor.I_13
+        self.I_23 = self.dry_I_23 + self.motor.I_23
+
+        # Return inertias
+        return (
+            self.I_11,
+            self.I_22,
+            self.I_33,
+            self.I_12,
+            self.I_13,
+            self.I_23,
+        )
+
+    def evaluate_nozzle_gyration_tensor(self):
+        pass
+
+    def add_motor(self, motor, position):
+        """Adds a motor to the rocket.
+
+        Parameters
+        ----------
+        motor : Motor, SolidMotor, HybridMotor, EmptyMotor
+            Motor to be added to the rocket. See Motor class for more
+            information.
+        position : int, float
+            Position, in m, of the motor's nozzle exit area relative to the user
+            defined rocket coordinate system.
+            See `Rocket.coordinate_system_orientation` for more information
+            regarding the rocket's coordinate system.
+
+        Returns
+        -------
+        None
+        """
+        if hasattr(self, "motor") and not isinstance(self.motor, EmptyMotor):
+            print(
+                "Only one motor per rocket is currently supported. "
+                + "Overwriting previous motor."
+            )
+        self.motor = motor
+        self.motor_position = position
+        _ = self._csys * self.motor._csys
+        self.center_of_propellant_position = (
+            self.motor.center_of_propellant_mass - self.motor.nozzle_position
+        ) * _ + self.motor_position
+        self.motor_center_of_mass_position = (
+            self.motor.center_of_mass - self.motor.nozzle_position
+        ) * _ + self.motor_position
+        self.motor_center_of_dry_mass_position = (
+            self.motor.center_of_dry_mass - self.motor.nozzle_position
+        ) * _ + self.motor_position
+        self.evaluate_dry_mass()
+        self.evaluate_total_mass()
+        self.evaluate_center_of_dry_mass()
+        self.evaluate_center_of_mass()
+        self.evaluate_dry_inertias()
+        self.evaluate_inertias()
+        self.evaluate_reduced_mass()
+        self.evaluate_thrust_to_weight()
+        self.evaluate_static_margin()
+        return None
+
+    def add_surfaces(self, surfaces, positions):
+        """Adds one or more aerodynamic surfaces to the rocket. The aerodynamic
+        surface must be an instance of a class that inherits from the
+        AeroSurface (e.g. NoseCone, TrapezoidalFins, etc.)
+
+        Parameters
+        ----------
+        surfaces : list, AeroSurface, NoseCone, TrapezoidalFins, EllipticalFins, Tail
+            Aerodynamic surface to be added to the rocket. Can be a list of
+            AeroSurface if more than one surface is to be added.
+            See AeroSurface class for more information.
+        positions : int, float, list
+            Position, in m, of the aerodynamic surface's center of pressure
+            relative to the user defined rocket coordinate system.
+            See `Rocket.coordinate_system_orientation` for more information
+            regarding the rocket's coordinate system.
+            If a list is passed, it will correspond to the position of each item
+            in the surfaces list.
+            For NoseCone type, position is relative to the nose cone tip.
+            For Fins type, position is relative to the point belonging to
+            the root chord which is highest in the rocket coordinate system.
+            For Tail type, position is relative to the point belonging to the
+            tail which is highest in the rocket coordinate system.
+
+        Returns
+        -------
+        None
+        """
+        try:
+            for surface, position in zip(surfaces, positions):
+                self.aerodynamic_surfaces.add(surface, position)
+        except TypeError:
+            self.aerodynamic_surfaces.add(surfaces, positions)
+
+        self.evaluate_static_margin()
+        return None
+
+    def add_tail(
+        self, top_radius, bottom_radius, length, position, radius=None, name="Tail"
+    ):
         """Create a new tail or rocket diameter change, storing its
-        parameters as part of the aerodynamicSurfaces list. Its
+        parameters as part of the aerodynamic_surfaces list. Its
         parameters are the axial position along the rocket and its
         derivative of the coefficient of lift in respect to angle of
         attack.
 
         Parameters
         ----------
-        topRadius : int, float
+        top_radius : int, float
             Tail top radius in meters, considering positive direction
             from center of mass to nose cone.
-        bottomRadius : int, float
+        bottom_radius : int, float
             Tail bottom radius in meters, considering positive direction
             from center of mass to nose cone.
         length : int, float
             Tail length or height in meters. Must be a positive value.
-        distanceToCM : int, float
-            Tail position relative to rocket unloaded center of mass,
-            considering positive direction from center of mass to nose
-            cone. Consider the point belonging to the tail which is
-            closest to the unloaded center of mass to calculate
-            distance.
+        position : int, float
+            Tail position relative to the rocket's coordinate system.
+            By tail position, understand the point belonging to the tail which is
+            highest in the rocket coordinate system (i.e. generally the point closest
+            to the nose cone).
+            See `Rocket.coordinate_system_orientation` for more information.
 
         Returns
         -------
-        cldata : Function
-            Object of the Function class. Contains tail's lift data.
-        self : Rocket
-            Object of the Rocket class.
+        tail : Tail
+            Tail object created.
         """
-        # Calculate ratio between top and bottom radius
-        r = topRadius / bottomRadius
-
-        # Retrieve reference radius
-        rref = self.radius
 
-        # Calculate cp position relative to cm
-        if distanceToCM < 0:
-            cpz = distanceToCM - (length / 3) * (1 + (1 - r) / (1 - r ** 2))
-        else:
-            cpz = distanceToCM + (length / 3) * (1 + (1 - r) / (1 - r ** 2))
-
-        # Calculate clalpha
-        clalpha = -2 * (1 - r ** (-2)) * (topRadius / rref) ** 2
-        cldata = Function(
-            lambda x: clalpha * x,
-            "Alpha (rad)",
-            "Cl",
-            interpolation="linear",
-            extrapolation="natural",
-        )
+        # Modify reference radius if not provided
+        radius = self.radius if radius is None else radius
 
-        # Store values as new aerodynamic surface
-        tail = [(0, 0, cpz), cldata, "Tail"]
-        self.aerodynamicSurfaces.append(tail)
+        # Create new tail as an object of the Tail class
+        tail = Tail(top_radius, bottom_radius, length, radius, name)
 
-        # Refresh static margin calculation
-        self.evaluateStaticMargin()
+        # Add tail to aerodynamic surfaces
+        self.add_surfaces(tail, position)
 
         # Return self
-        return self.aerodynamicSurfaces[-1]
+        return tail
 
-    def addNose(self, length, kind, distanceToCM):
+    def add_nose(self, length, kind, position, name="Nosecone"):
         """Creates a nose cone, storing its parameters as part of the
-        aerodynamicSurfaces list. Its parameters are the axial position
+        aerodynamic_surfaces list. Its parameters are the axial position
         along the rocket and its derivative of the coefficient of lift
         in respect to angle of attack.
 
 
         Parameters
         ----------
         length : int, float
             Nose cone length or height in meters. Must be a positive
             value.
         kind : string
             Nose cone type. Von Karman, conical, ogive, and lvhaack are
             supported.
-        distanceToCM : int, float
-            Nose cone position relative to rocket unloaded center of
-            mass, considering positive direction from center of mass to
-            nose cone. Consider the center point belonging to the nose
-            cone base to calculate distance.
+        position : int, float
+            Nose cone tip coordinate relative to the rocket's coordinate system.
+            See `Rocket.coordinate_system_orientation` for more information.
+        name : string
+            Nose cone name. Default is "Nose Cone".
 
         Returns
         -------
-        cldata : Function
-            Object of the Function class. Contains nose's lift data.
-        self : Rocket
-            Object of the Rocket class.
+        nose : Nose
+            Nose cone object created.
         """
-        # Analyze type
-        if kind == "conical":
-            k = 1 - 1 / 3
-        elif kind == "ogive":
-            k = 1 - 0.534
-        elif kind == "lvhaack":
-            k = 1 - 0.437
-        else:
-            k = 0.5
-
-        # Calculate cp position relative to cm
-        if distanceToCM > 0:
-            cpz = distanceToCM + k * length
-        else:
-            cpz = distanceToCM - k * length
-
-        # Calculate clalpha
-        clalpha = 2
-        cldata = Function(
-            lambda x: clalpha * x,
-            "Alpha (rad)",
-            "Cl",
-            interpolation="linear",
-            extrapolation="natural",
-        )
-
-        # Store values
-        nose = [(0, 0, cpz), cldata, "Nose Cone"]
-        self.aerodynamicSurfaces.append(nose)
+        # Create a nose as an object of NoseCone class
+        nose = NoseCone(length, kind, self.radius, self.radius, name)
 
-        # Refresh static margin calculation
-        self.evaluateStaticMargin()
+        # Add nose to the list of aerodynamic surfaces
+        self.add_surfaces(nose, position)
 
         # Return self
-        return self.aerodynamicSurfaces[-1]
+        return nose
+
+    def add_fins(self, *args, **kwargs):
+        """See Rocket.add_trapezoidal_fins for documentation.
+        This method is set to be deprecated in version 1.0.0 and fully removed
+        by version 2.0.0. Use Rocket.add_trapezoidal_fins instead. It keeps the
+        same arguments and signature."""
+        warnings.warn(
+            "This method is set to be deprecated in version 1.0.0 and fully "
+            "removed by version 2.0.0. Use Rocket.add_trapezoidal_fins instead",
+            PendingDeprecationWarning,
+        )
+        return self.add_trapezoidal_fins(*args, **kwargs)
 
-    def addFins(
+    def add_trapezoidal_fins(
         self,
         n,
+        root_chord,
+        tip_chord,
         span,
-        rootChord,
-        tipChord,
-        distanceToCM,
-        radius=0,
-        cantAngle=0,
+        position,
+        cant_angle=0,
+        sweep_length=None,
+        sweep_angle=None,
+        radius=None,
         airfoil=None,
+        name="Fins",
     ):
-        """Create a fin set, storing its parameters as part of the
-        aerodynamicSurfaces list. Its parameters are the axial position
-        along the rocket and its derivative of the coefficient of lift
-        in respect to angle of attack.
+        """Create a trapezoidal fin set, storing its parameters as part of the
+        aerodynamic_surfaces list. Its parameters are the axial position along
+        the rocket and its derivative of the coefficient of lift in respect to
+        angle of attack.
 
         Parameters
         ----------
         n : int
             Number of fins, from 2 to infinity.
         span : int, float
             Fin span in meters.
-        rootChord : int, float
+        root_chord : int, float
             Fin root chord in meters.
-        tipChord : int, float
+        tip_chord : int, float
             Fin tip chord in meters.
-        distanceToCM : int, float
-            Fin set position relative to rocket unloaded center of
-            mass, considering positive direction from center of mass to
-            nose cone. Consider the center point belonging to the top
-            of the fins to calculate distance.
-        radius : int, float, optional
-            Reference radius to calculate lift coefficient. If 0, which
-            is default, use rocket radius. Otherwise, enter the radius
-            of the rocket in the section of the fins, as this impacts
-            its lift coefficient.
-        cantAngle : int, float, optional
+        position : int, float
+            Fin set position relative to the rocket's coordinate system.
+            By fin set position, understand the point belonging to the root
+            chord which is highest in the rocket coordinate system (i.e.
+            generally the point closest to the nose cone tip).
+            See `Rocket.coordinate_system_orientation` for more information.
+        cant_angle : int, float, optional
             Fins cant angle with respect to the rocket centerline. Must
             be given in degrees.
-        airfoil : string
-            Fin's lift curve. It must be a .csv file. The .csv file shall
-            contain no headers and the first column must specify time in
-            seconds, while the second column specifies lift coefficient. Lift
-            coefficient is dimensionaless.
+        sweep_length : int, float, optional
+            Fins sweep length in meters. By sweep length, understand the axial
+            distance between the fin root leading edge and the fin tip leading
+            edge measured parallel to the rocket centerline. If not given, the
+            sweep length is assumed to be equal the root chord minus the tip
+            chord, in which case the fin is a right trapezoid with its base
+            perpendicular to the rocket's axis. Cannot be used in conjunction
+            with sweep_angle.
+        sweep_angle : int, float, optional
+            Fins sweep angle with respect to the rocket centerline. Must be
+            given in degrees. If not given, the sweep angle is automatically
+            calculated, in which case the fin is assumed to be a right trapezoid
+            with its base perpendicular to the rocket's axis. Cannot be used in
+            conjunction with sweep_length.
+        radius : int, float, optional
+            Reference radius to calculate lift coefficient. If None, which is
+            default, use rocket radius.
+        airfoil : tuple, optional
+            Default is null, in which case fins will be treated as flat plates.
+            Otherwise, if tuple, fins will be considered as airfoils. The
+            tuple's first item specifies the airfoil's lift coefficient
+            by angle of attack and must be either a .csv, .txt, ndarray
+            or callable. The .csv and .txt files must contain no headers
+            and the first column must specify the angle of attack, while
+            the second column must specify the lift coefficient. The
+            ndarray should be as [(x0, y0), (x1, y1), (x2, y2), ...]
+            where x0 is the angle of attack and y0 is the lift coefficient.
+            If callable, it should take an angle of attack as input and
+            return the lift coefficient at that angle of attack.
+            The tuple's second item is the unit of the angle of attack,
+            accepting either "radians" or "degrees".
 
         Returns
         -------
-        cldata : Function
-            Object of the Function class. Contains fin's lift data.
-        self : Rocket
-            Object of the Rocket class.
+        fin_set : TrapezoidalFins
+            Fin set object created.
         """
 
-        # Retrieve parameters for calculations
-        Cr = rootChord
-        Ct = tipChord
-        Yr = rootChord + tipChord
-        s = span
-        Af = Yr * s / 2  # fin area
-        Ymac = (
-            (s / 3) * (Cr + 2 * Ct) / Yr
-        )  # span wise position of fin's mean aerodynamic chord
-        Lf = np.sqrt((rootChord / 2 - tipChord / 2) ** 2 + span ** 2)
-        radius = self.radius if radius == 0 else radius
-        d = 2 * radius
-        cantAngleRad = np.radians(cantAngle)
-        trapezoidalConstant = ((Yr) / 2) * (radius ** 2) * s
-        trapezoidalConstant += ((Cr + 2 * Ct) / 3) * radius * (s ** 2)
-        trapezoidalConstant += ((Cr + 3 * Ct) / 12) * (s ** 3)
-
-        # Save geometric parameters for later Fin Flutter Analysis and Roll Moment Calculation
-        self.rootChord = Cr
-        self.tipChord = Ct
-        self.span = s
-        self.distanceRocketFins = distanceToCM
-
-        # Calculate cp position relative to cm
-        if distanceToCM < 0:
-            cpz = distanceToCM - (
-                ((Cr - Ct) / 3) * ((Cr + 2 * Ct) / (Cr + Ct))
-                + (1 / 6) * (Cr + Ct - Cr * Ct / (Cr + Ct))
-            )
-        else:
-            cpz = distanceToCM + (
-                ((Cr - Ct) / 3) * ((Cr + 2 * Ct) / (Cr + Ct))
-                + (1 / 6) * (Cr + Ct - Cr * Ct / (Cr + Ct))
-            )
+        # Modify radius if not given, use rocket radius, otherwise use given.
+        radius = radius if radius is not None else self.radius
 
-        # Calculate lift parameters for planar fins
-        if not airfoil:
-            # Calculate clalpha
-            clalpha = (4 * n * (s / d) ** 2) / (1 + np.sqrt(1 + (2 * Lf / Yr) ** 2))
-            clalpha *= 1 + radius / (s + radius)
-
-            # # Create a function of lift values by attack angle
-            cldata = Function(
-                lambda x: clalpha * x, "Alpha (rad)", "Cl", interpolation="linear"
-            )
-            # Parameters for Roll Moment. Documented at: https://github.com/Projeto-Jupiter/RocketPy/blob/develop/docs/technical/aerodynamics/Roll_Equations.pdf
-            clfDelta = n * (Ymac + radius) * clalpha / d
-            cldOmega = (
-                n * clalpha * np.cos(cantAngleRad) * trapezoidalConstant / (Af * d)
-            )
-            rollParameters = (
-                [clfDelta, cldOmega, cantAngleRad] if cantAngleRad != 0 else [0, 0, 0]
-            )
-
-            # Store values
-            fin = [(0, 0, cpz), cldata, rollParameters, "Fins"]
-            self.aerodynamicSurfaces.append(fin)
-
-            # Refresh static margin calculation
-            self.evaluateStaticMargin()
-
-            # Return self
-            return self.aerodynamicSurfaces[-1]
+        # Create a fin set as an object of TrapezoidalFins class
+        fin_set = TrapezoidalFins(
+            n,
+            root_chord,
+            tip_chord,
+            span,
+            radius,
+            cant_angle,
+            sweep_length,
+            sweep_angle,
+            airfoil,
+            name,
+        )
 
-        else:
+        # Add fin set to the list of aerodynamic surfaces
+        self.add_surfaces(fin_set, position)
 
-            def cnalfa1(cn):
-                """Calculates the normal force coefficient derivative of a 3D
-                airfoil for a given Cnalfa0
-
-                Parameters
-                ----------
-                cn : int
-                    Normal force coefficient derivative of a 2D airfoil.
-
-                Returns
-                -------
-                Cnalfa1 : int
-                    Normal force coefficient derivative of a 3D airfoil.
-                """
-
-                # Retrieve parameters for calculations
-                Af = (Cr + Ct) * span / 2
-                # fin area
-                AR = 2 * (span ** 2) / Af  # Aspect ratio
-                gamac = np.arctan((Cr - Ct) / (2 * span))
-                # mid chord angle
-                FD = 2 * np.pi * AR / (cn * np.cos(gamac))
-                Cnalfa1 = (
-                    cn
-                    * FD
-                    * (Af / self.area)
-                    * np.cos(gamac)
-                    / (2 + FD * (1 + (4 / FD ** 2)) ** 0.5)
-                )
-                return Cnalfa1
+        # Return the created aerodynamic surface
+        return fin_set
 
-            # Import the lift curve as a function of lift values by attack angle
-            read = genfromtxt(airfoil, delimiter=",")
+    def add_elliptical_fins(
+        self,
+        n,
+        root_chord,
+        span,
+        position,
+        cant_angle=0,
+        radius=None,
+        airfoil=None,
+        name="Fins",
+    ):
+        """Create an elliptical fin set, storing its parameters as part of the
+        aerodynamic_surfaces list. Its parameters are the axial position along
+        the rocket and its derivative of the coefficient of lift in respect to
+        angle of attack.
 
-            # Applies number of fins to lift coefficient data
-            data = [[cl[0], (n / 2) * cnalfa1(cl[1])] for cl in read]
-            cldata = Function(
-                data,
-                "Alpha (rad)",
-                "Cl",
-                interpolation="linear",
-                extrapolation="natural",
-            )
+        Parameters
+        ----------
+        n : int
+            Number of fins, from 2 to infinity.
+        root_chord : int, float
+            Fin root chord in meters.
+        span : int, float
+            Fin span in meters.
+        position : int, float
+            Fin set position relative to the rocket's coordinate system. By fin
+            set position, understand the point belonging to the root chord which
+            is highest in the rocket coordinate system (i.e. generally the point
+            closest to the nose cone tip).
+            See `Rocket.coordinate_system_orientation` for more information.
+        cant_angle : int, float, optional
+            Fins cant angle with respect to the rocket centerline. Must be given
+            in degrees.
+        radius : int, float, optional
+            Reference radius to calculate lift coefficient. If None, which
+            is default, use rocket radius.
+        airfoil : tuple, optional
+            Default is null, in which case fins will be treated as flat plates.
+            Otherwise, if tuple, fins will be considered as airfoils. The
+            tuple's first item specifies the airfoil's lift coefficient
+            by angle of attack and must be either a .csv, .txt, ndarray
+            or callable. The .csv and .txt files must contain no headers
+            and the first column must specify the angle of attack, while
+            the second column must specify the lift coefficient. The
+            ndarray should be as [(x0, y0), (x1, y1), (x2, y2), ...]
+            where x0 is the angle of attack and y0 is the lift coefficient.
+            If callable, it should take an angle of attack as input and
+            return the lift coefficient at that angle of attack.
+            The tuple's second item is the unit of the angle of attack,
+            accepting either "radians" or "degrees".
 
-            # Takes an approximation to an angular coefficient
-            clalpha = cldata.differentiate(x=0, dx=1e-2)
+        Returns
+        -------
+        fin_set : EllipticalFins
+            Fin set object created.
+        """
 
-            # Parameters for Roll Moment. Documented at: https://github.com/Projeto-Jupiter/RocketPy/blob/develop/docs/technical/aerodynamics/Roll_Equations.pdf
-            clfDelta = n * (Ymac + radius) * clalpha / d
-            cldOmega = (
-                n * clalpha * np.cos(cantAngleRad) * trapezoidalConstant / (Af * d)
-            )
-            rollParameters = (
-                [clfDelta, cldOmega, cantAngleRad] if cantAngleRad != 0 else [0, 0, 0]
-            )
+        # Modify radius if not given, use rocket radius, otherwise use given.
+        radius = radius if radius is not None else self.radius
 
-            # Store values
-            fin = [(0, 0, cpz), cldata, rollParameters, "Fins"]
-            self.aerodynamicSurfaces.append(fin)
+        # Create a fin set as an object of EllipticalFins class
+        fin_set = EllipticalFins(n, root_chord, span, radius, cant_angle, airfoil, name)
 
-            # Refresh static margin calculation
-            self.evaluateStaticMargin()
+        # Add fin set to the list of aerodynamic surfaces
+        self.add_surfaces(fin_set, position)
 
-            # Return self
-            return self.aerodynamicSurfaces[-1]
+        # Return self
+        return fin_set
 
-    def addParachute(
-        self, name, CdS, trigger, samplingRate=100, lag=0, noise=(0, 0, 0)
+    def add_parachute(
+        self, name, cd_s, trigger, sampling_rate=100, lag=0, noise=(0, 0, 0)
     ):
         """Creates a new parachute, storing its parameters such as
         opening delay, drag coefficients and trigger function.
 
         Parameters
         ----------
         name : string
             Parachute name, such as drogue and main. Has no impact in
             simulation, as it is only used to display data in a more
             organized matter.
-        CdS : float
+        cd_s : float
             Drag coefficient times reference area for parachute. It is
             used to compute the drag force exerted on the parachute by
-            the equation F = ((1/2)*rho*V^2)*CdS, that is, the drag
+            the equation F = ((1/2)*rho*V^2)*cd_s, that is, the drag
             force is the dynamic pressure computed on the parachute
-            times its CdS coefficient. Has units of area and must be
+            times its cd_s coefficient. Has units of area and must be
             given in squared meters.
-        trigger : function
-            Function which defines if the parachute ejection system is
-            to be triggered. It must take as input the freestream
-            pressure in pascal and the state vector of the simulation,
-            which is defined by [x, y, z, vx, vy, vz, e0, e1, e2, e3, wx, wy, wz].
-            It will be called according to the sampling rate given next.
-            It should return True if the parachute ejection system is
-            to be triggered and False otherwise.
-        samplingRate : float, optional
+        trigger : function, float, string
+            Trigger for the parachute deployment. Can be a float with the height
+            in which the parachute is ejected (ejection happens after apogee); or
+            the string "apogee", for ejection at apogee.
+            Can also be a function which defines if the parachute ejection
+            system is to be triggered. It must take as input the freestream
+            pressure in pascal, the height in meters (above ground level), and
+            the state vector of the simulation, which is defined by
+            [x, y, z, vx, vy, vz, e0, e1, e2, e3, wx, wy, wz].
+            The trigger will be called according to the sampling rate given next.
+            It should return True if the parachute ejection system is to be
+            triggered and False otherwise.
+        sampling_rate : float, optional
             Sampling rate in which the trigger function works. It is used to
             simulate the refresh rate of onboard sensors such as barometers.
             Default value is 100. Value must be given in hertz.
         lag : float, optional
             Time between the parachute ejection system is triggered and the
             parachute is fully opened. During this time, the simulation will
             consider the rocket as flying without a parachute. Default value
@@ -742,89 +1037,73 @@
             List in the format (mean, standard deviation, time-correlation).
             The values are used to add noise to the pressure signal which is
             passed to the trigger function. Default value is (0, 0, 0). Units
             are in pascal.
 
         Returns
         -------
-        parachute : Parachute Object
-            Parachute object containing trigger, samplingRate, lag, CdS, noise
-            and name as attributes. Furthermore, it stores cleanPressureSignal,
-            noiseSignal and noisyPressureSignal which are filled in during
+        parachute : Parachute
+            Parachute  containing trigger, sampling_rate, lag, cd_s, noise
+            and name. Furthermore, it stores clean_pressure_signal,
+            noise_signal and noisyPressureSignal which are filled in during
             Flight simulation.
         """
-        # Create an object to serve as the parachute
-        parachute = type("", (), {})()
-
-        # Store Cds coefficient, lag, name and trigger function
-        parachute.trigger = trigger
-        parachute.samplingRate = samplingRate
-        parachute.lag = lag
-        parachute.CdS = CdS
-        parachute.name = name
-        parachute.noiseBias = noise[0]
-        parachute.noiseDeviation = noise[1]
-        parachute.noiseCorr = (noise[2], (1 - noise[2] ** 2) ** 0.5)
-        alpha, beta = parachute.noiseCorr
-        parachute.noiseSignal = [[-1e-6, np.random.normal(noise[0], noise[1])]]
-        parachute.noiseFunction = lambda: alpha * parachute.noiseSignal[-1][
-            1
-        ] + beta * np.random.normal(noise[0], noise[1])
-        parachute.cleanPressureSignal = []
-        parachute.noisyPressureSignal = []
+        # Create a parachute
+        parachute = Parachute(name, cd_s, trigger, sampling_rate, lag, noise)
 
         # Add parachute to list of parachutes
         self.parachutes.append(parachute)
 
         # Return self
         return self.parachutes[-1]
 
-    def setRailButtons(self, distanceToCM, angularPosition=45):
-        """Adds rail buttons to the rocket, allowing for the
-        calculation of forces exerted by them when the rocket is
-        sliding in the launch rail. Furthermore, rail buttons are
-        also needed for the simulation of the planar flight phase,
-        when the rocket experiences 3 degrees of freedom motion while
-        only one rail button is still in the launch rail.
+    def set_rail_buttons(
+        self, upper_button_position, lower_button_position, angular_position=45
+    ):
+        """Adds rail buttons to the rocket, allowing for the calculation of
+        forces exerted by them when the rocket is sliding in the launch rail.
+        For the simulation, only two buttons are needed, which are the two
+        closest to the nozzle.
 
         Parameters
         ----------
-        distanceToCM : tuple, list, array
-            Two values organized in a tuple, list or array which
-            represent the distance of each of the two rail buttons
-            to the center of mass of the rocket without propellant.
-            If the rail button is positioned above the center of mass,
-            its distance should be a positive value. If it is below,
-            its distance should be a negative value. The order does
-            not matter. All values should be in meters.
-        angularPosition : float
-            Angular postion of the rail buttons in degrees measured
+        upper_button_position : int, float
+            Position of the rail button furthest from the nozzle relative to
+            the rocket's coordinate system, in meters.
+            See `Rocket.coordinate_system_orientation` for more information.
+        lower_button_position : int, float
+            Position of the rail button closest to the nozzle relative to
+            the rocket's coordinate system, in meters.
+            See `Rocket.coordinate_system_orientation` for more information.
+        angular_position : float, optional
+            Angular position of the rail buttons in degrees measured
             as the rotation around the symmetry axis of the rocket
             relative to one of the other principal axis.
             Default value is 45 degrees, generally used in rockets with
             4 fins.
 
         Returns
         -------
-        None
+        rail_buttons : RailButtons
+            RailButtons object created
         """
-        # Order distance to CM
-        if distanceToCM[0] < distanceToCM[1]:
-            distanceToCM.reverse()
-        # Save
-        self.railButtons = self.railButtonPair(distanceToCM, angularPosition)
-
-        return None
+        # Create a rail buttons object
+        buttons_distance = abs(upper_button_position - lower_button_position)
+        rail_buttons = RailButtons(
+            buttons_distance=buttons_distance, angular_position=angular_position
+        )
+        self.rail_buttons.add(rail_buttons, lower_button_position)
+        return rail_buttons
 
-    def addCMEccentricity(self, x, y):
+    def add_cm_eccentricity(self, x, y):
         """Moves line of action of aerodynamic and thrust forces by
         equal translation amount to simulate an eccentricity in the
         position of the center of mass of the rocket relative to its
         geometrical center line. Should not be used together with
-        addCPEccentricity and addThrustEccentricity.
+        add_cp_eccentricity and add_thrust_eccentricity.
 
         Parameters
         ----------
         x : float
             Distance in meters by which the CM is to be translated in
             the x direction relative to geometrical center line.
         y : float
@@ -833,25 +1112,25 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move center of pressure to -x and -y
-        self.cpEccentricityX = -x
-        self.cpEccentricityY = -y
+        self.cp_eccentricity_x = -x
+        self.cp_eccentricity_y = -y
 
         # Move thrust center by -x and -y
-        self.thrustEccentricityY = -x
-        self.thrustEccentricityX = -y
+        self.thrust_eccentricity_y = -x
+        self.thrust_eccentricity_x = -y
 
         # Return self
         return self
 
-    def addCPEccentricity(self, x, y):
+    def add_cp_eccentricity(self, x, y):
         """Moves line of action of aerodynamic forces to simulate an
         eccentricity in the position of the center of pressure relative
         to the center of mass of the rocket.
 
         Parameters
         ----------
         x : float
@@ -863,23 +1142,23 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move center of pressure by x and y
-        self.cpEccentricityX = x
-        self.cpEccentricityY = y
+        self.cp_eccentricity_x = x
+        self.cp_eccentricity_y = y
 
         # Return self
         return self
 
-    def addThrustEccentricity(self, x, y):
+    def add_thrust_eccentricity(self, x, y):
         """Moves line of action of thrust forces to simulate a
-        disalignment of the thrust vector and the center of mass.
+        misalignment of the thrust vector and the center of mass.
 
         Parameters
         ----------
         x : float
             Distance in meters by which the line of action of the
             thrust force is to be translated in the x direction
             relative to the center of mass axial line.
@@ -890,16 +1169,16 @@
 
         Returns
         -------
         self : Rocket
             Object of the Rocket class.
         """
         # Move thrust line by x and y
-        self.thrustEccentricityY = x
-        self.thrustEccentricityX = y
+        self.thrust_eccentricity_y = x
+        self.thrust_eccentricity_x = y
 
         # Return self
         return self
 
     def info(self):
         """Prints out a summary of the data and graphs available about
         the Rocket.
@@ -908,182 +1187,69 @@
         ----------
         None
 
         Return
         ------
         None
         """
-        # Print inertia details
-        print("Inertia Details")
-        print("Rocket Dry Mass: " + str(self.mass) + " kg (No Propellant)")
-        print("Rocket Total Mass: " + str(self.totalMass(0)) + " kg (With Propellant)")
-
-        # Print rocket geometrical parameters
-        print("\nGeometrical Parameters")
-        print("Rocket Radius: " + str(self.radius) + " m")
-
-        # Print rocket aerodynamics quantities
-        print("\nAerodynamics Stability")
-        print("Initial Static Margin: " + "{:.3f}".format(self.staticMargin(0)) + " c")
-        print(
-            "Final Static Margin: "
-            + "{:.3f}".format(self.staticMargin(self.motor.burnOutTime))
-            + " c"
-        )
-
-        # Print parachute data
-        for chute in self.parachutes:
-            print("\n" + chute.name.title() + " Parachute")
-            print("CdS Coefficient: " + str(chute.CdS) + " m2")
-
-        # Show plots
-        print("\nAerodynamics Plots")
-        self.powerOnDrag()
+        # All prints
+        self.prints.all()
 
-        # Return None
         return None
 
-    def allInfo(self):
+    def all_info(self):
         """Prints out all data and graphs available about the Rocket.
 
         Parameters
         ----------
         None
 
         Return
         ------
         None
         """
-        # Print inertia details
-        print("Inertia Details")
-        print("Rocket Mass: {:.3f} kg (No Propellant)".format(self.mass))
-        print("Rocket Mass: {:.3f} kg (With Propellant)".format(self.totalMass(0)))
-        print("Rocket Inertia I: {:.3f} kg*m2".format(self.inertiaI))
-        print("Rocket Inertia Z: {:.3f} kg*m2".format(self.inertiaZ))
-
-        # Print rocket geometrical parameters
-        print("\nGeometrical Parameters")
-        print("Rocket Maximum Radius: " + str(self.radius) + " m")
-        print("Rocket Frontal Area: " + "{:.6f}".format(self.area) + " m2")
-        print("\nRocket Distances")
-        print(
-            "Rocket Center of Mass - Nozzle Exit Distance: "
-            + str(self.distanceRocketNozzle)
-            + " m"
-        )
-        print(
-            "Rocket Center of Mass - Propellant Center of Mass Distance: "
-            + str(self.distanceRocketPropellant)
-            + " m"
-        )
-        print(
-            "Rocket Center of Mass - Rocket Loaded Center of Mass: "
-            + "{:.3f}".format(self.centerOfMass(0))
-            + " m"
-        )
-        print("\nAerodynamic Components Parameters")
-        print("Currently not implemented.")
-
-        # Print rocket aerodynamics quantities
-        print("\nAerodynamics Lift Coefficient Derivatives")
-        for aerodynamicSurface in self.aerodynamicSurfaces:
-            name = aerodynamicSurface[-1]
-            clalpha = aerodynamicSurface[1].differentiate(x=1e-2, dx=1e-3)
-            print(
-                name + " Lift Coefficient Derivative: {:.3f}".format(clalpha) + "/rad"
-            )
-
-        print("\nAerodynamics Center of Pressure")
-        for aerodynamicSurface in self.aerodynamicSurfaces:
-            name = aerodynamicSurface[-1]
-            cpz = aerodynamicSurface[0][2]
-            print(name + " Center of Pressure to CM: {:.3f}".format(cpz) + " m")
-        print(
-            "Distance - Center of Pressure to CM: "
-            + "{:.3f}".format(self.cpPosition)
-            + " m"
-        )
-        print("Initial Static Margin: " + "{:.3f}".format(self.staticMargin(0)) + " c")
-        print(
-            "Final Static Margin: "
-            + "{:.3f}".format(self.staticMargin(self.motor.burnOutTime))
-            + " c"
-        )
 
-        # Print parachute data
-        for chute in self.parachutes:
-            print("\n" + chute.name.title() + " Parachute")
-            print("CdS Coefficient: " + str(chute.CdS) + " m2")
-            if chute.trigger.__name__ == "<lambda>":
-                line = getsourcelines(chute.trigger)[0][0]
-                print(
-                    "Ejection signal trigger: "
-                    + line.split("lambda ")[1].split(",")[0].split("\n")[0]
-                )
-            else:
-                print("Ejection signal trigger: " + chute.trigger.__name__)
-            print("Ejection system refresh rate: " + str(chute.samplingRate) + " Hz.")
-            print(
-                "Time between ejection signal is triggered and the "
-                "parachute is fully opened: " + str(chute.lag) + " s"
-            )
+        # All prints and plots
+        self.info()
+        self.plots.all()
 
-        # Show plots
-        print("\nMass Plots")
-        self.totalMass()
-        self.reducedMass()
-        print("\nAerodynamics Plots")
-        self.staticMargin()
-        self.powerOnDrag()
-        self.powerOffDrag()
-        self.thrustToWeight.plot(lower=0, upper=self.motor.burnOutTime)
-
-        # ax = plt.subplot(415)
-        # ax.plot(  , self.rocket.motor.thrust()/(self.env.g() * self.rocket.totalMass()))
-        # ax.set_xlim(0, self.rocket.motor.burnOutTime)
-        # ax.set_xlabel("Time (s)")
-        # ax.set_ylabel("Thrust/Weight")
-        # ax.set_title("Thrust-Weight Ratio")
-
-        # Return None
         return None
 
-    def addFin(
+    def add_fin(
         self,
-        numberOfFins=4,
+        number_of_fins=4,
         cl=2 * np.pi,
         cpr=1,
         cpz=1,
         gammas=[0, 0, 0, 0],
-        angularPositions=None,
+        angular_positions=None,
     ):
         "Hey! I will document this function later"
-        self.aerodynamicSurfaces = []
+        self.aerodynamic_surfaces = Components()
         pi = np.pi
-        # Calculate angular postions if not given
-        if angularPositions is None:
-            angularPositions = np.array(range(numberOfFins)) * 2 * pi / numberOfFins
+        # Calculate angular positions if not given
+        if angular_positions is None:
+            angular_positions = (
+                np.array(range(number_of_fins)) * 2 * pi / number_of_fins
+            )
         else:
-            angularPositions = np.array(angularPositions) * pi / 180
+            angular_positions = np.array(angular_positions) * pi / 180
         # Convert gammas to degree
         if isinstance(gammas, (int, float)):
-            gammas = [(pi / 180) * gammas for i in range(numberOfFins)]
+            gammas = [(pi / 180) * gammas for i in range(number_of_fins)]
         else:
             gammas = [(pi / 180) * gamma for gamma in gammas]
-        for i in range(numberOfFins):
+        for i in range(number_of_fins):
             # Get angular position and inclination for current fin
-            angularPosition = angularPositions[i]
+            angularPosition = angular_positions[i]
             gamma = gammas[i]
             # Calculate position vector
             cpx = cpr * np.cos(angularPosition)
             cpy = cpr * np.sin(angularPosition)
             positionVector = np.array([cpx, cpy, cpz])
             # Calculate chord vector
             auxVector = np.array([cpy, -cpx, 0]) / (cpr)
             chordVector = (
                 np.cos(gamma) * np.array([0, 0, 1]) - np.sin(gamma) * auxVector
             )
-            self.aerodynamicSurfaces.append([positionVector, chordVector])
+            self.aerodynamic_surfaces.append([positionVector, chordVector])
         return None
-
-    # Variables
-    railButtonPair = namedtuple("railButtonPair", "distanceToCM angularPosition")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rocketpy-0.9.9/rocketpy/SolidMotor.py` & `rocketpy-1.0.0a1/rocketpy/motors/SolidMotor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,833 +1,697 @@
 # -*- coding: utf-8 -*-
 
-__author__ = "Giovani Hidalgo Ceotto, Oscar Mauricio Prada Ramirez"
-__copyright__ = "Copyright 20XX, Projeto Jupiter"
+__author__ = "Giovani Hidalgo Ceotto, Pedro Henrique Marinho Bressan, Mateus Stano Junqueira, Oscar Mauricio Prada Ramirez, João Lemes Gribel Soares, Lucas Kierulff Balabram, Lucas Azevedo Pezente"
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __license__ = "MIT"
 
-import re
-import math
-import bisect
-import warnings
-import time
-from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
-
 import numpy as np
 from scipy import integrate
-from scipy import linalg
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
 
-from .Function import Function
+from rocketpy.plots.solid_motor_plots import _SolidMotorPlots
+from rocketpy.prints.solid_motor_prints import _SolidMotorPrints
+
+try:
+    from functools import cached_property
+except ImportError:
+    from rocketpy.tools import cached_property
+
+from rocketpy.Function import Function, funcify_method, reset_funcified_methods
+
+from .Motor import Motor
 
 
-class SolidMotor:
-    """Class to specify characteristics and useful operations for solid
-    motors.
+class SolidMotor(Motor):
+    """Class to specify characteristics and useful operations for solid motors.
 
     Attributes
     ----------
 
         Geometrical attributes:
-        Motor.nozzleRadius : float
+        Motor.coordinate_system_orientation : str
+            Orientation of the motor's coordinate system. The coordinate system
+            is defined by the motor's axis of symmetry. The origin of the
+            coordinate system  may be placed anywhere along such axis, such as
+            at the nozzle area, and must be kept the same for all other
+            positions specified. Options are "nozzle_to_combustion_chamber" and
+            "combustion_chamber_to_nozzle".
+        Motor.nozzle_radius : float
             Radius of motor nozzle outlet in meters.
-        Motor.throatRadius : float
+        Motor.nozzle_position : float
+            Motor's nozzle outlet position in meters, specified in the motor's
+            coordinate system. See `Motor.coordinate_system_orientation` for
+            more information.
+        Motor.throat_radius : float
             Radius of motor nozzle throat in meters.
-        Motor.grainNumber : int
+        Motor.grain_number : int
             Number of solid grains.
-        Motor.grainSeparation : float
+        Motor.grains_center_of_mass_position : float
+            Position of the center of mass of the grains in meters, specified in
+            the motor's coordinate system.
+            See `Motor.coordinate_system_orientation` for more information.
+        Motor.grain_separation : float
             Distance between two grains in meters.
-        Motor.grainDensity : float
+        Motor.grain_density : float
             Density of each grain in kg/meters cubed.
-        Motor.grainOuterRadius : float
+        Motor.grain_outer_radius : float
             Outer radius of each grain in meters.
-        Motor.grainInitialInnerRadius : float
+        Motor.grain_initial_inner_radius : float
             Initial inner radius of each grain in meters.
-        Motor.grainInitialHeight : float
+        Motor.grain_initial_height : float
             Initial height of each grain in meters.
         Motor.grainInitialVolume : float
             Initial volume of each grain in meters cubed.
-        Motor.grainInnerRadius : Function
+        Motor.grain_inner_radius : Function
             Inner radius of each grain in meters as a function of time.
-        Motor.grainHeight : Function
+        Motor.grain_height : Function
             Height of each grain in meters as a function of time.
 
         Mass and moment of inertia attributes:
         Motor.grainInitialMass : float
             Initial mass of each grain in kg.
-        Motor.propellantInitialMass : float
+        Motor.dry_mass : float
+            The total mass of the motor structure, including chambers
+            and tanks, when it is empty and does not contain any propellant.
+        Motor.propellant_initial_mass : float
             Total propellant initial mass in kg.
-        Motor.mass : Function
-            Propellant total mass in kg as a function of time.
-        Motor.massDot : Function
+        Motor.total_mass : Function
+            Total motor mass in kg as a function of time, defined as the sum
+            of propellant and dry mass.
+        Motor.propellant_mass : Function
+            Total propellant mass in kg as a function of time.
+        Motor.total_mass_flow_rate : Function
             Time derivative of propellant total mass in kg/s as a function
-            of time.
-        Motor.inertiaI : Function
-            Propellant moment of inertia in kg*meter^2 with respect to axis
-            perpendicular to axis of cylindrical symmetry of each grain,
-            given as a function of time.
-        Motor.inertiaIDot : Function
-            Time derivative of inertiaI given in kg*meter^2/s as a function
-            of time.
-        Motor.inertiaZ : Function
-            Propellant moment of inertia in kg*meter^2 with respect to axis of
-            cylindrical symmetry of each grain, given as a function of time.
-        Motor.inertiaDot : Function
-            Time derivative of inertiaZ given in kg*meter^2/s as a function
-            of time.
+            of time as obtained by the thrust source.
+        Motor.center_of_mass : Function
+            Position of the motor center of mass in
+            meters as a function of time.
+            See `Motor.coordinate_system_orientation` for more information
+            regarding the motor's coordinate system.
+        Motor.center_of_propellant_mass : Function
+            Position of the motor propellant center of mass in meters as a
+            function of time.
+            See `Motor.coordinate_system_orientation` for more information
+            regarding the motor's coordinate system.
+        Motor.I_11 : Function
+            Component of the motor's inertia tensor relative to the e_1 axis
+            in kg*m^2, as a function of time. The e_1 axis is the direction
+            perpendicular to the motor body axis of symmetry, centered at
+            the instantaneous motor center of mass.
+        Motor.I_22 : Function
+            Component of the motor's inertia tensor relative to the e_2 axis
+            in kg*m^2, as a function of time. The e_2 axis is the direction
+            perpendicular to the motor body axis of symmetry, centered at
+            the instantaneous motor center of mass.
+            Numerically equivalent to I_11 due to symmetry.
+        Motor.I_33 : Function
+            Component of the motor's inertia tensor relative to the e_3 axis
+            in kg*m^2, as a function of time. The e_3 axis is the direction of
+            the motor body axis of symmetry, centered at the instantaneous
+            motor center of mass.
+        Motor.I_12 : Function
+            Component of the motor's inertia tensor relative to the e_1 and
+            e_2 axes in kg*m^2, as a function of time. See Motor.I_11 and
+            Motor.I_22 for more information.
+        Motor.I_13 : Function
+            Component of the motor's inertia tensor relative to the e_1 and
+            e_3 axes in kg*m^2, as a function of time. See Motor.I_11 and
+            Motor.I_33 for more information.
+        Motor.I_23 : Function
+            Component of the motor's inertia tensor relative to the e_2 and
+            e_3 axes in kg*m^2, as a function of time. See Motor.I_22 and
+            Motor.I_33 for more information.
+        Motor.propellant_I_11 : Function
+            Component of the propellant inertia tensor relative to the e_1
+            axis in kg*m^2, as a function of time. The e_1 axis is the
+            direction perpendicular to the motor body axis of symmetry,
+            centered at the instantaneous propellant center of mass.
+        Motor.propellant_I_22 : Function
+            Component of the propellant inertia tensor relative to the e_2
+            axis in kg*m^2, as a function of time. The e_2 axis is the
+            direction perpendicular to the motor body axis of symmetry,
+            centered at the instantaneous propellant center of mass.
+            Numerically equivalent to propellant_I_11 due to symmetry.
+        Motor.propellant_I_33 : Function
+            Component of the propellant inertia tensor relative to the e_3
+            axis in kg*m^2, as a function of time. The e_3 axis is the
+            direction of the motor body axis of symmetry, centered at the
+            instantaneous propellant center of mass.
+        Motor.propellant_I_12 : Function
+            Component of the propellant inertia tensor relative to the e_1 and
+            e_2 axes in kg*m^2, as a function of time. See Motor.propellant_I_11
+            and Motor.propellant_I_22 for more information.
+        Motor.propellant_I_13 : Function
+            Component of the propellant inertia tensor relative to the e_1 and
+            e_3 axes in kg*m^2, as a function of time. See Motor.propellant_I_11
+            and Motor.propellant_I_33 for more information.
+        Motor.propellant_I_23 : Function
+            Component of the propellant inertia tensor relative to the e_2 and
+            e_3 axes in kg*m^2, as a function of time. See Motor.propellant_I_22
+            and Motor.propellant_I_33 for more information.
 
         Thrust and burn attributes:
         Motor.thrust : Function
             Motor thrust force, in Newtons, as a function of time.
-        Motor.totalImpulse : float
+        Motor.total_impulse : float
             Total impulse of the thrust curve in N*s.
-        Motor.maxThrust : float
+        Motor.max_thrust : float
             Maximum thrust value of the given thrust curve, in N.
-        Motor.maxThrustTime : float
+        Motor.max_thrust_time : float
             Time, in seconds, in which the maximum thrust value is achieved.
-        Motor.averageThrust : float
+        Motor.average_thrust : float
             Average thrust of the motor, given in N.
-        Motor.burnOutTime : float
-            Total motor burn out time, in seconds. Must include delay time
-            when the motor takes time to ignite. Also seen as time to end thrust
-            curve.
-        Motor.exhaustVelocity : float
+        Motor.burn_time : tuple of float
+            Tuple containing the initial and final time of the motor's burn time
+            in seconds.
+        Motor.burn_start_time : float
+            Motor burn start time, in seconds.
+        Motor.burn_out_time : float
+            Motor burn out time, in seconds.
+        Motor.burn_duration : float
+            Total motor burn duration, in seconds. It is the difference between the burn_out_time and the burn_start_time.
+        Motor.exhaust_velocity : float
             Propulsion gases exhaust velocity, assumed constant, in m/s.
-        Motor.burnArea : Function
+        Motor.burn_area : Function
             Total burn area considering all grains, made out of inner
             cylindrical burn area and grain top and bottom faces. Expressed
             in meters squared as a function of time.
         Motor.Kn : Function
-            Motor Kn as a function of time. Defined as burnArea divided by
+            Motor Kn as a function of time. Defined as burn_area divided by
             nozzle throat cross sectional area. Has no units.
-        Motor.burnRate : Function
+        Motor.burn_rate : Function
             Propellant burn rate in meter/second as a function of time.
         Motor.interpolate : string
             Method of interpolation used in case thrust curve is given
             by data set in .csv or .eng, or as an array. Options are 'spline'
             'akima' and 'linear'. Default is "linear".
     """
 
     def __init__(
         self,
-        thrustSource,
-        burnOut,
-        grainNumber,
-        grainDensity,
-        grainOuterRadius,
-        grainInitialInnerRadius,
-        grainInitialHeight,
-        grainSeparation=0,
-        nozzleRadius=0.0335,
-        throatRadius=0.0114,
-        reshapeThrustCurve=False,
-        interpolationMethod="linear",
+        thrust_source,
+        dry_mass,
+        center_of_dry_mass,
+        dry_inertia,
+        grains_center_of_mass_position,
+        grain_number,
+        grain_density,
+        grain_outer_radius,
+        grain_initial_inner_radius,
+        grain_initial_height,
+        grain_separation,
+        nozzle_radius,
+        burn_time=None,
+        nozzle_position=0,
+        throat_radius=0.01,
+        reshape_thrust_curve=False,
+        interpolation_method="linear",
+        coordinate_system_orientation="nozzle_to_combustion_chamber",
     ):
         """Initialize Motor class, process thrust curve and geometrical
         parameters and store results.
 
         Parameters
         ----------
-        thrustSource : int, float, callable, string, array
+        thrust_source : int, float, callable, string, array
             Motor's thrust curve. Can be given as an int or float, in which
             case the thrust will be considered constant in time. It can
             also be given as a callable function, whose argument is time in
             seconds and returns the thrust supplied by the motor in the
             instant. If a string is given, it must point to a .csv or .eng file.
             The .csv file shall contain no headers and the first column must
             specify time in seconds, while the second column specifies thrust.
             Arrays may also be specified, following rules set by the class
             Function. See help(Function). Thrust units are Newtons.
-        burnOut : int, float
-            Motor burn out time in seconds.
-        grainNumber : int
+        burn_time: float, tuple of float, optional
+            Motor's burn time.
+            If a float is given, the burn time is assumed to be between 0 and the
+            given float, in seconds.
+            If a tuple of float is given, the burn time is assumed to be between
+            the first and second elements of the tuple, in seconds.
+            If not specified, automatically sourced as the range between the first- and
+            last-time step of the motor's thrust curve. This can only be used if the
+            motor's thrust is defined by a list of points, such as a .csv file, a .eng
+            file or a Function instance whose source is a list.
+        dry_mass : int, float
+            The total mass of the motor structure, including chambers
+            and tanks, when it is empty and does not contain any propellant.
+        center_of_dry_mass : int, float
+            The position, in meters, of the motor's center of mass with respect
+            to the motor's coordinate system when it is devoid of propellant.
+            See `Motor.coordinate_system_orientation`.
+        dry_inertia : tuple, list
+            Tuple or list containing the motor's dry mass inertia tensor
+            components, in kg*m^2. This inertia is defined with respect to the
+            the `center_of_dry_mass` position.
+            Assuming e_3 is the rocket's axis of symmetry, e_1 and e_2 are
+            orthogonal and form a plane perpendicular to e_3, the dry mass
+            inertia tensor components must be given in the following order:
+            (I_11, I_22, I_33, I_12, I_13, I_23), where I_ij is the
+            component of the inertia tensor in the direction of e_i x e_j.
+            Alternatively, the inertia tensor can be given as (I_11, I_22, I_33),
+            where I_12 = I_13 = I_23 = 0.
+        grains_center_of_mass_position : float
+            Position of the center of mass of the grains in meters. More specifically,
+            the coordinate of the center of mass specified in the motor's coordinate
+            system. See `Motor.coordinate_system_orientation` for more information.
+        grain_number : int
             Number of solid grains
-        grainDensity : int, float
+        grain_density : int, float
             Solid grain density in kg/m3.
-        grainOuterRadius : int, float
+        grain_outer_radius : int, float
             Solid grain outer radius in meters.
-        grainInitialInnerRadius : int, float
+        grain_initial_inner_radius : int, float
             Solid grain initial inner radius in meters.
-        grainInitialHeight : int, float
+        grain_initial_height : int, float
             Solid grain initial height in meters.
-        grainSeparation : int, float, optional
-            Distance between grains, in meters. Default is 0.
-        nozzleRadius : int, float, optional
-            Motor's nozzle outlet radius in meters. Used to calculate Kn curve.
-            Optional if the Kn curve is not interesting. Its value does not impact
-            trajectory simulation.
-        throatRadius : int, float, optional
-            Motor's nozzle throat radius in meters. Its value has very low
-            impact in trajectory simulation, only useful to analyze
-            dynamic instabilities, therefore it is optional.
-        reshapeThrustCurve : boolean, tuple, optional
+        grain_separation : int, float
+            Distance between grains, in meters.
+        nozzle_radius : int, float
+            Motor's nozzle outlet radius in meters.
+        nozzle_position : int, float, optional
+            Motor's nozzle outlet position in meters, in the motor's coordinate
+            system. See `Motor.coordinate_system_orientation` for details.
+            Default is 0, in which case the origin of the coordinate system
+            is placed at the motor's nozzle outlet.
+        throat_radius : int, float, optional
+            Motor's nozzle throat radius in meters. Used to calculate Kn curve.
+            Optional if the Kn curve is not interesting. Its value does not
+            impact trajectory simulation.
+        reshape_thrust_curve : boolean, tuple, optional
             If False, the original thrust curve supplied is not altered. If a
             tuple is given, whose first parameter is a new burn out time and
             whose second parameter is a new total impulse in Ns, the thrust
             curve is reshaped to match the new specifications. May be useful
             for motors whose thrust curve shape is expected to remain similar
             in case the impulse and burn time varies slightly. Default is
             False.
-        interpolationMethod : string, optional
+        interpolation_method : string, optional
             Method of interpolation to be used in case thrust curve is given
             by data set in .csv or .eng, or as an array. Options are 'spline'
             'akima' and 'linear'. Default is "linear".
+        coordinate_system_orientation : string, optional
+            Orientation of the motor's coordinate system. The coordinate system
+            is defined by the motor's axis of symmetry. The origin of the
+            coordinate system  may be placed anywhere along such axis, such as
+            at the nozzle area, and must be kept the same for all other
+            positions specified. Options are "nozzle_to_combustion_chamber" and
+            "combustion_chamber_to_nozzle". Default is "nozzle_to_combustion_chamber".
 
         Returns
         -------
         None
         """
-        # Thrust parameters
-        self.interpolate = interpolationMethod
-        self.burnOutTime = burnOut
-
-        # Check if thrustSource is csv, eng, function or other
-        if isinstance(thrustSource, str):
-            # Determine if csv or eng
-            if thrustSource[-3:] == "eng":
-                # Import content
-                comments, desc, points = self.importEng(thrustSource)
-                # Process description and points
-                # diameter = float(desc[1])/1000
-                # height = float(desc[2])/1000
-                # mass = float(desc[4])
-                # nozzleRadius = diameter/4
-                # throatRadius = diameter/8
-                # grainNumber = grainnumber
-                # grainVolume = height*np.pi*((diameter/2)**2 -(diameter/4)**2)
-                # grainDensity = mass/grainVolume
-                # grainOuterRadius = diameter/2
-                # grainInitialInnerRadius = diameter/4
-                # grainInitialHeight = height
-                thrustSource = points
-                self.burnOutTime = points[-1][0]
-
-        # Create thrust function
-        self.thrust = Function(
-            thrustSource, "Time (s)", "Thrust (N)", self.interpolate, "zero"
-        )
-        if callable(thrustSource) or isinstance(thrustSource, (int, float)):
-            self.thrust.setDiscrete(0, burnOut, 50, self.interpolate, "zero")
+        super().__init__(
+            thrust_source,
+            dry_mass,
+            center_of_dry_mass,
+            dry_inertia,
+            nozzle_radius,
+            burn_time,
+            nozzle_position,
+            reshape_thrust_curve,
+            interpolation_method,
+            coordinate_system_orientation,
+        )
+        # Nozzle parameters
+        self.throat_radius = throat_radius
+        self.throatArea = np.pi * throat_radius**2
+
+        # Grain parameters
+        self.grains_center_of_mass_position = grains_center_of_mass_position
+        self.grain_number = grain_number
+        self.grain_separation = grain_separation
+        self.grain_density = grain_density
+        self.grain_outer_radius = grain_outer_radius
+        self.grain_initial_inner_radius = grain_initial_inner_radius
+        self.grain_initial_height = grain_initial_height
 
-        # Reshape curve and calculate impulse
-        if reshapeThrustCurve:
-            self.reshapeThrustCurve(*reshapeThrustCurve)
-        else:
-            self.evaluateTotalImpulse()
-
-        # Define motor attributes
-        # Grain and nozzle parameters
-        self.nozzleRadius = nozzleRadius
-        self.throatRadius = throatRadius
-        self.grainNumber = grainNumber
-        self.grainSeparation = grainSeparation
-        self.grainDensity = grainDensity
-        self.grainOuterRadius = grainOuterRadius
-        self.grainInitialInnerRadius = grainInitialInnerRadius
-        self.grainInitialHeight = grainInitialHeight
-        # Other quantities that will be computed
-        self.massDot = None
-        self.mass = None
-        self.grainInnerRadius = None
-        self.grainHeight = None
-        self.burnArea = None
-        self.Kn = None
-        self.burnRate = None
-        self.inertiaI = None
-        self.inertiaIDot = None
-        self.inertiaZ = None
-        self.inertiaZDot = None
-        self.maxThrust = None
-        self.maxThrustTime = None
-        self.averageThrust = None
-
-        # Compute quantities
-        # Thrust information - maximum and average
-        self.maxThrust = np.amax(self.thrust.source[:, 1])
-        maxThrustIndex = np.argmax(self.thrust.source[:, 1])
-        self.maxThrustTime = self.thrust.source[maxThrustIndex, 0]
-        self.averageThrust = self.totalImpulse / self.burnOutTime
         # Grains initial geometrical parameters
         self.grainInitialVolume = (
-            self.grainInitialHeight
+            self.grain_initial_height
             * np.pi
-            * (self.grainOuterRadius ** 2 - self.grainInitialInnerRadius ** 2)
+            * (self.grain_outer_radius**2 - self.grain_initial_inner_radius**2)
         )
-        self.grainInitialMass = self.grainDensity * self.grainInitialVolume
-        self.propellantInitialMass = self.grainNumber * self.grainInitialMass
-        # Dynamic quantities
-        self.evaluateMassDot()
-        self.evaluateMass()
-        self.evaluateGeometry()
-        self.evaluateInertia()
+        self.grainInitialMass = self.grain_density * self.grainInitialVolume
 
-    def reshapeThrustCurve(
-        self, burnTime, totalImpulse, oldTotalImpulse=None, startAtZero=True
-    ):
-        """Transforms the thrust curve supplied by changing its total
-        burn time and/or its total impulse, without altering the
-        general shape of the curve. May translate the curve so that
-        thrust starts at time equals 0, without any delays.
+        self.evaluate_geometry()
 
-        Parameters
-        ----------
-        burnTime : float
-            New desired burn out time in seconds.
-        totalImpulse : float
-            New desired total impulse.
-        oldTotalImpulse : float, optional
-            Specify the total impulse of the given thrust curve,
-            overriding the value calculated by numerical integration.
-            If left as None, the value calculated by numerical
-            integration will be used in order to reshape the curve.
-        startAtZero: bool, optional
-            If True, trims the initial thrust curve points which
-            are 0 Newtons, translating the thrust curve so that
-            thrust starts at time equals 0. If False, no translation
-            is applied.
+        # Initialize plots and prints object
+        self.prints = _SolidMotorPrints(self)
+        self.plots = _SolidMotorPlots(self)
+        return None
+
+    @funcify_method("Time (s)", "Mass (kg)")
+    def propellant_mass(self):
+        """Evaluates the total propellant mass as a function of time.
 
         Returns
         -------
-        None
+        Function
+            Mass of the motor, in kg.
         """
-        # Retrieve current thrust curve data points
-        timeArray = self.thrust.source[:, 0]
-        thrustArray = self.thrust.source[:, 1]
-        # Move start to time = 0
-        if startAtZero and timeArray[0] != 0:
-            timeArray = timeArray - timeArray[0]
-
-        # Reshape time - set burn time to burnTime
-        self.thrust.source[:, 0] = (burnTime / timeArray[-1]) * timeArray
-        self.burnOutTime = burnTime
-        self.thrust.setInterpolation(self.interpolate)
-
-        # Reshape thrust - set total impulse
-        if oldTotalImpulse is None:
-            oldTotalImpulse = self.evaluateTotalImpulse()
-        self.thrust.source[:, 1] = (totalImpulse / oldTotalImpulse) * thrustArray
-        self.thrust.setInterpolation(self.interpolate)
-
-        # Store total impulse
-        self.totalImpulse = totalImpulse
-
-        # Return reshaped curve
-        return self.thrust
-
-    def evaluateTotalImpulse(self):
-        """Calculates and returns total impulse by numerical
-        integration of the thrust curve in SI units. The value is
-        also stored in self.totalImpulse.
+        return self.grain_volume * self.grain_density * self.grain_number
 
-        Parameters
-        ----------
-        None
+    @funcify_method("Time (s)", "Grain volume (m³)")
+    def grain_volume(self):
+        """Evaluates the total propellant volume as a function of time. The
+        propellant is assumed to be a cylindrical Bates grain under uniform
+        burn.
 
         Returns
         -------
-        self.totalImpulse : float
-            Motor total impulse in Ns.
+        Function
+            Propellant volume as a function of time.
         """
-        # Calculate total impulse
-        self.totalImpulse = self.thrust.integral(0, self.burnOutTime)
+        cross_section_area = np.pi * (
+            self.grain_outer_radius**2 - self.grain_inner_radius**2
+        )
+        return cross_section_area * self.grain_height
 
-        # Return total impulse
-        return self.totalImpulse
+    @funcify_method("Time (s)", "Exhaust velocity (m/s)")
+    def exhaust_velocity(self):
+        """Exhaust velocity by assuming it as a constant. The formula used is
+        total impulse/propellant initial mass.
 
-    @property
-    def exhaustVelocity(self):
-        """Calculates and returns exhaust velocity by assuming it
-        as a constant. The formula used is total impulse/propellant
-        initial mass. The value is also stored in
-        self.exhaustVelocity.
+        Returns
+        -------
+        self.exhaust_velocity : rocketpy.Function
+            Gas exhaust velocity of the motor.
+        """
+        return self.total_impulse / self.propellant_initial_mass
 
-        Parameters
-        ----------
-        None
+    @property
+    def propellant_initial_mass(self):
+        """Returns the initial propellant mass.
 
         Returns
         -------
-        self.exhaustVelocity : float
-            Constant gas exhaust velocity of the motor.
+        float
+            Initial propellant mass in kg.
         """
-        return self.totalImpulse / self.propellantInitialMass
-
-    def evaluateMassDot(self):
-        """Calculates and returns the time derivative of propellant
-        mass by assuming constant exhaust velocity. The formula used
-        is the opposite of thrust divided by exhaust velocity. The
-        result is a function of time, object of the Function class,
-        which is stored in self.massDot.
+        return self.grain_number * self.grainInitialMass
 
-        Parameters
-        ----------
-        None
+    @property
+    def mass_flow_rate(self):
+        """Time derivative of propellant mass. Assumes constant exhaust
+        velocity. The formula used is the opposite of thrust divided by
+        exhaust velocity.
 
         Returns
         -------
-        self.massDot : Function
-            Time derivative of total propellant mas as a function
-            of time.
-        """
-        # Create mass dot Function
-        self.massDot = self.thrust / (-self.exhaustVelocity)
-        self.massDot.setOutputs("Mass Dot (kg/s)")
-        self.massDot.setExtrapolation("zero")
-
-        # Return Function
-        return self.massDot
-
-    def evaluateMass(self):
-        """Calculates and returns the total propellant mass curve by
-        numerically integrating the MassDot curve, calculated in
-        evaluateMassDot. Numerical integration is done with the
-        Trapezoidal Rule, given the same result as scipy.integrate.
-        odeint but 100x faster. The result is a function of time,
-        object of the class Function, which is stored in self.mass.
+        self.mass_flow_rate : Function
+            Time derivative of total propellant mass as a function of time.
+
+        See Also
+        --------
+        `Motor.total_mass_flow_rate` :
+            Calculates the total mass flow rate of the motor assuming
+            constant exhaust velocity.
+        """
+        try:
+            return self._massFlowRate
+        except AttributeError:
+            self._massFlowRate = self.total_mass_flow_rate
+            return self._massFlowRate
+
+    @mass_flow_rate.setter
+    def mass_flow_rate(self, value):
+        """Sets the mass flow rate of the motor.
 
         Parameters
         ----------
-        None
+        value : Function
+            Mass flow rate in kg/s.
 
         Returns
         -------
-        self.mass : Function
-            Total propellant mass as a function of time.
+        None
         """
-        # Retrieve mass dot curve data
-        t = self.massDot.source[:, 0]
-        ydot = self.massDot.source[:, 1]
-
-        # Set initial conditions
-        T = [0]
-        y = [self.propellantInitialMass]
-
-        # Solve for each time point
-        for i in range(1, len(t)):
-            T += [t[i]]
-            y += [y[i - 1] + 0.5 * (t[i] - t[i - 1]) * (ydot[i] + ydot[i - 1])]
-
-        # Create Function
-        self.mass = Function(
-            np.concatenate(([T], [y])).transpose(),
-            "Time (s)",
-            "Propellant Total Mass (kg)",
-            self.interpolate,
-            "constant",
-        )
+        self._massFlowRate = value.reset("Time (s)", "grain mass flow rate (kg/s)")
+        self.evaluate_geometry()
 
-        # Return Mass Function
-        return self.mass
+    @funcify_method("Time (s)", "center of mass (m)", "linear")
+    def center_of_propellant_mass(self):
+        """Position of the propellant center of mass as a function of time.
+        The position is specified as a scalar, relative to the motor's
+        coordinate system.
 
-    @property
-    def throatArea(self):
-        return np.pi * self.throatRadius ** 2
+        Returns
+        -------
+        rocketpy.Function
+            Position of the propellant center of mass as a function of time.
+        """
+        timeSource = self.grain_inner_radius.x_array
+        center_of_mass = np.full_like(timeSource, self.grains_center_of_mass_position)
+        return np.column_stack((timeSource, center_of_mass))
 
-    def evaluateGeometry(self):
-        """Calculates grain inner radius and grain height as a
-        function of time by assuming that every propellant mass
-        burnt is exhausted. In order to do that, a system of
-        differential equations is solved using scipy.integrate.
-        odeint. Furthermore, the function calculates burn area,
-        burn rate and Kn as a function of time using the previous
-        results. All functions are stored as objects of the class
-        Function in self.grainInnerRadius, self.grainHeight, self.
-        burnArea, self.burnRate and self.Kn.
+    def evaluate_geometry(self):
+        """Calculates grain inner radius and grain height as a function of time
+        by assuming that every propellant mass burnt is exhausted. In order to
+        do that, a system of differential equations is solved using
+        scipy.integrate.odeint. Furthermore, the function calculates burn area,
+        burn rate and Kn as a function of time using the previous results. All
+        functions are stored as objects of the class Function in
+        self.grain_inner_radius, self.grain_height, self.burn_area, self.burn_rate
+        and self.Kn.
 
-        Parameters
-        ----------
-        None
 
         Returns
         -------
-        geometry : list of Functions
-            First element is the Function representing the inner
-            radius of a grain as a function of time. Second
-            argument is the Function representing the height of a
-            grain as a function of time.
+        geometry : list of rocketpy.Functions
+            First element is the Function representing the inner radius of a
+            grain as a function of time. Second argument is the Function
+            representing the height of a grain as a function of time.
         """
         # Define initial conditions for integration
-        y0 = [self.grainInitialInnerRadius, self.grainInitialHeight]
+        y0 = [self.grain_initial_inner_radius, self.grain_initial_height]
 
         # Define time mesh
-        t = self.massDot.source[:, 0]
+        t = self.thrust.source[:, 0]
+        t_span = t[0], t[-1]
 
-        density = self.grainDensity
-        rO = self.grainOuterRadius
+        density = self.grain_density
+        rO = self.grain_outer_radius
 
         # Define system of differential equations
-        def geometryDot(y, t):
-            grainMassDot = self.massDot(t) / self.grainNumber
+        def geometryDot(t, y):
+            grainMassDot = self.mass_flow_rate(t) / self.grain_number
             rI, h = y
             rIDot = (
-                -0.5 * grainMassDot / (density * np.pi * (rO ** 2 - rI ** 2 + rI * h))
+                -0.5 * grainMassDot / (density * np.pi * (rO**2 - rI**2 + rI * h))
             )
-            hDot = 1.0 * grainMassDot / (density * np.pi * (rO ** 2 - rI ** 2 + rI * h))
+            hDot = 1.0 * grainMassDot / (density * np.pi * (rO**2 - rI**2 + rI * h))
             return [rIDot, hDot]
 
+        def terminateBurn(t, y):
+            end_function = (self.grain_outer_radius - y[0]) * y[1]
+            return end_function
+
+        terminateBurn.terminal = True
+        terminateBurn.direction = -1
+
         # Solve the system of differential equations
-        sol = integrate.odeint(geometryDot, y0, t)
+        sol = integrate.solve_ivp(
+            geometryDot,
+            t_span,
+            y0,
+            events=terminateBurn,
+            atol=1e-12,
+            rtol=1e-11,
+            method="LSODA",
+        )
+
+        self.grainBurnOut = sol.t[-1]
 
         # Write down functions for innerRadius and height
-        self.grainInnerRadius = Function(
-            np.concatenate(([t], [sol[:, 0]])).transpose().tolist(),
+        self.grain_inner_radius = Function(
+            np.concatenate(([sol.t], [sol.y[0]])).transpose().tolist(),
             "Time (s)",
             "Grain Inner Radius (m)",
             self.interpolate,
             "constant",
         )
-        self.grainHeight = Function(
-            np.concatenate(([t], [sol[:, 1]])).transpose().tolist(),
+        self.grain_height = Function(
+            np.concatenate(([sol.t], [sol.y[1]])).transpose().tolist(),
             "Time (s)",
             "Grain Height (m)",
             self.interpolate,
             "constant",
         )
 
-        # Create functions describing burn rate, Kn and burn area
-        self.evaluateBurnArea()
-        self.evaluateKn()
-        self.evaluateBurnRate()
-
-        return [self.grainInnerRadius, self.grainHeight]
-
-    def evaluateBurnArea(self):
-        """Calculates the BurnArea of the grain for
-        each time. Assuming that the grains are cylindrical
-        BATES grains.
+        reset_funcified_methods(self)
 
-        Parameters
-        ----------
-        None
+        return [self.grain_inner_radius, self.grain_height]
+
+    @funcify_method("Time (s)", "burn area (m²)")
+    def burn_area(self):
+        """Calculates the BurnArea of the grain for each time. Assuming that
+        the grains are cylindrical BATES grains.
 
         Returns
         -------
-        burnArea : Function
-        Function representing the burn area progression with the time.
+        burn_area : rocketpy.Function
+            Function representing the burn area progression with the time.
         """
-        self.burnArea = (
+        burn_area = (
             2
             * np.pi
             * (
-                self.grainOuterRadius ** 2
-                - self.grainInnerRadius ** 2
-                + self.grainInnerRadius * self.grainHeight
+                self.grain_outer_radius**2
+                - self.grain_inner_radius**2
+                + self.grain_inner_radius * self.grain_height
             )
-            * self.grainNumber
+            * self.grain_number
         )
-        self.burnArea.setOutputs("Burn Area (m2)")
-        return self.burnArea
+        return burn_area
 
-    def evaluateBurnRate(self):
-        """Calculates the BurnRate with respect to time.
-        This evaluation assumes that it was already
-        calculated the massDot, burnArea timeseries.
-
-        Parameters
-        ----------
-        None
+    @funcify_method("Time (s)", "burn rate (m/s)")
+    def burn_rate(self):
+        """Calculates the BurnRate with respect to time. This evaluation
+        assumes that it was already calculated the massDot, burn_area time
+        series.
 
         Returns
         -------
-        burnRate : Function
-        Rate of progression of the inner radius during the combustion.
+        burn_rate : rocketpy.Function
+            Rate of progression of the inner radius during the combustion.
         """
-        self.burnRate = (-1) * self.massDot / (self.burnArea * self.grainDensity)
-        self.burnRate.setOutputs("Burn Rate (m/s)")
-        return self.burnRate
+        return -1 * self.mass_flow_rate / (self.burn_area * self.grain_density)
+
+    @cached_property
+    def Kn(self):
+        """Calculates the motor Kn as a function of time. Defined as burn_area
+        divided by the nozzle throat cross sectional area.
 
-    def evaluateKn(self):
+        Returns
+        -------
+        Kn : rocketpy.Function
+            Kn as a function of time.
+        """
         KnSource = (
             np.concatenate(
                 (
-                    [self.grainInnerRadius.source[:, 1]],
-                    [self.burnArea.source[:, 1] / self.throatArea],
+                    [self.grain_inner_radius.source[:, 1]],
+                    [self.burn_area.source[:, 1] / self.throatArea],
                 )
             ).transpose()
         ).tolist()
-        self.Kn = Function(
+        Kn = Function(
             KnSource,
             "Grain Inner Radius (m)",
             "Kn (m2/m2)",
             self.interpolate,
             "constant",
         )
-        return self.Kn
-
-    def evaluateInertia(self):
-        """Calculates propellant inertia I, relative to directions
-        perpendicular to the rocket body axis and its time derivative
-        as a function of time. Also calculates propellant inertia Z,
-        relative to the axial direction, and its time derivative as a
-        function of time. Products of inertia are assumed null due to
-        symmetry. The four functions are stored as an object of the
-        Function class.
+        return Kn
 
-        Parameters
-        ----------
-        None
+    @funcify_method("Time (s)", "Inertia I_11 (kg m²)")
+    def propellant_I_11(self):
+        """Inertia tensor 11 component of the propellant, the inertia is
+        relative to the e_1 axis, centered at the instantaneous propellant
+        center of mass.
 
         Returns
         -------
-        list of Functions
-            The first argument is the Function representing inertia I,
-            while the second argument is the Function representing
-            inertia Z.
-        """
+        Function
+            Propellant inertia tensor 11 component at time t.
+
+        Notes
+        -----
+        The e_1 direction is assumed to be the direction perpendicular to the
+        motor body axis.
 
-        # Inertia I
-        # Calculate inertia I for each grain
-        grainMass = self.mass / self.grainNumber
-        grainMassDot = self.massDot / self.grainNumber
-        grainNumber = self.grainNumber
-        grainInertiaI = grainMass * (
-            (1 / 4) * (self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2)
-            + (1 / 12) * self.grainHeight ** 2
+        References
+        ----------
+        .. [1] https://en.wikipedia.org/wiki/Moment_of_inertia#Inertia_tensor
+        """
+        grainMass = self.propellant_mass / self.grain_number
+        grain_number = self.grain_number
+        grainInertia11 = grainMass * (
+            (1 / 4) * (self.grain_outer_radius**2 + self.grain_inner_radius**2)
+            + (1 / 12) * self.grain_height**2
         )
 
         # Calculate each grain's distance d to propellant center of mass
-        initialValue = (grainNumber - 1) / 2
-        d = np.linspace(-initialValue, initialValue, grainNumber)
-        d = d * (self.grainInitialHeight + self.grainSeparation)
+        # Assuming each grain's COM are evenly spaced
+        initialValue = (grain_number - 1) / 2
+        d = np.linspace(-initialValue, initialValue, grain_number)
+        d = d * (self.grain_initial_height + self.grain_separation)
 
         # Calculate inertia for all grains
-        self.inertiaI = grainNumber * grainInertiaI + grainMass * np.sum(d ** 2)
-        self.inertiaI.setOutputs("Propellant Inertia I (kg*m2)")
-
-        # Inertia I Dot
-        # Calculate each grain's inertia I dot
-        grainInertiaIDot = (
-            grainMassDot
-            * (
-                (1 / 4) * (self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2)
-                + (1 / 12) * self.grainHeight ** 2
-            )
-            + grainMass
-            * ((1 / 2) * self.grainInnerRadius - (1 / 3) * self.grainHeight)
-            * self.burnRate
-        )
+        I_11 = grain_number * grainInertia11 + grainMass * np.sum(d**2)
 
-        # Calculate inertia I dot for all grains
-        self.inertiaIDot = grainNumber * grainInertiaIDot + grainMassDot * np.sum(
-            d ** 2
-        )
-        self.inertiaIDot.setOutputs("Propellant Inertia I Dot (kg*m2/s)")
+        return I_11
 
-        # Inertia Z
-        self.inertiaZ = (
-            (1 / 2.0)
-            * self.mass
-            * (self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2)
-        )
-        self.inertiaZ.setOutputs("Propellant Inertia Z (kg*m2)")
-
-        # Inertia Z Dot
-        self.inertiaZDot = (1 / 2.0) * self.massDot * (
-            self.grainOuterRadius ** 2 + self.grainInnerRadius ** 2
-        ) + self.mass * self.grainInnerRadius * self.burnRate
-        self.inertiaZDot.setOutputs("Propellant Inertia Z Dot (kg*m2/s)")
-
-        return [self.inertiaI, self.inertiaZ]
-
-    def importEng(self, fileName):
-        """Read content from .eng file and process it, in order to
-        return the comments, description and data points.
-
-        Parameters
-        ----------
-        fileName : string
-            Name of the .eng file. E.g. 'test.eng'.
-            Note that the .eng file must not contain the 0 0 point.
+    @funcify_method("Time (s)", "Inertia I_22 (kg m²)")
+    def propellant_I_22(self):
+        """Inertia tensor 22 component of the propellant, the inertia is
+        relative to the e_2 axis, centered at the instantaneous propellant
+        center of mass.
 
         Returns
         -------
-        comments : list
-            All comments in the .eng file, separated by line in a list. Each
-            line is an entry of the list.
-        description: list
-            Description of the motor. All attributes are returned separated in
-            a list. E.g. "F32 24 124 5-10-15 .0377 .0695 RV\n" is return as
-            ['F32', '24', '124', '5-10-15', '.0377', '.0695', 'RV\n']
-        dataPoints: list
-            List of all data points in file. Each data point is an entry in
-            the returned list and written as a list of two entries.
-        """
-        # Initialize arrays
-        comments = []
-        description = []
-        dataPoints = [[0, 0]]
-
-        # Open and read .eng file
-        with open(fileName) as file:
-            for line in file:
-                if re.search(r";.*", line):
-                    # Extract comment
-                    comments.append(re.findall(r";.*", line)[0])
-                    line = re.sub(r";.*", "", line)
-                if line.strip():
-                    if description == []:
-                        # Extract description
-                        description = line.strip().split(" ")
-                    else:
-                        # Extract thrust curve data points
-                        time, thrust = re.findall(r"[-+]?\d*\.\d+|[-+]?\d+", line)
-                        dataPoints.append([float(time), float(thrust)])
-
-        # Return all extract content
-        return comments, description, dataPoints
-
-    def exportEng(self, fileName, motorName):
-        """Exports thrust curve data points and motor description to
-        .eng file format. A description of the format can be found
-        here: http://www.thrustcurve.org/raspformat.shtml
+        Function
+            Propellant inertia tensor 22 component at time t.
 
-        Parameters
-        ----------
-        fileName : string
-            Name of the .eng file to be exported. E.g. 'test.eng'
-        motorName : string
-            Name given to motor. Will appear in the description of the
-            .eng file. E.g. 'Mandioca'
+        Notes
+        -----
+        The e_2 direction is assumed to be the direction perpendicular to the
+        motor body axis, and perpendicular to e_1.
 
-        Returns
-        -------
-        None
+        References
+        ----------
+        .. [1] https://en.wikipedia.org/wiki/Moment_of_inertia#Inertia_tensor
         """
-        # Open file
-        file = open(fileName, "w")
+        return self.I_11
 
-        # Write first line
-        file.write(
-            motorName
-            + " {:3.1f} {:3.1f} 0 {:2.3} {:2.3} RocketPy\n".format(
-                2000 * self.grainOuterRadius,
-                1000
-                * self.grainNumber
-                * (self.grainInitialHeight + self.grainSeparation),
-                self.propellantInitialMass,
-                self.propellantInitialMass,
-            )
-        )
-
-        # Write thrust curve data points
-        for time, thrust in self.thrust.source[1:-1, :]:
-            # time, thrust = item
-            file.write("{:.4f} {:.3f}\n".format(time, thrust))
-
-        # Write last line
-        file.write("{:.4f} {:.3f}\n".format(self.thrust.source[-1, 0], 0))
+    @funcify_method("Time (s)", "Inertia I_33 (kg m²)")
+    def propellant_I_33(self):
+        """Inertia tensor 33 component of the propellant, the inertia is
+        relative to the e_3 axis, centered at the instantaneous propellant
+        center of mass.
 
-        # Close file
-        file.close()
-
-        return None
+        Returns
+        -------
+        Function
+            Propellant inertia tensor 33 component at time t.
 
-    def info(self):
-        """Prints out a summary of the data and graphs available about
-        the Motor.
+        Notes
+        -----
+        The e_3 direction is assumed to be the axial direction of the rocket
+        motor.
 
-        Parameters
+        References
         ----------
-        None
-
-        Return
-        ------
-        None
+        .. [1] https://en.wikipedia.org/wiki/Moment_of_inertia#Inertia_tensor
         """
-        # Print motor details
-        print("\nMotor Details")
-        print("Total Burning Time: " + str(self.burnOutTime) + " s")
-        print(
-            "Total Propellant Mass: "
-            + "{:.3f}".format(self.propellantInitialMass)
-            + " kg"
-        )
-        print(
-            "Propellant Exhaust Velocity: "
-            + "{:.3f}".format(self.exhaustVelocity)
-            + " m/s"
-        )
-        print("Average Thrust: " + "{:.3f}".format(self.averageThrust) + " N")
-        print(
-            "Maximum Thrust: "
-            + str(self.maxThrust)
-            + " N at "
-            + str(self.maxThrustTime)
-            + " s after ignition."
+        I_33 = (
+            (1 / 2.0)
+            * self.propellant_mass
+            * (self.grain_outer_radius**2 + self.grain_inner_radius**2)
         )
-        print("Total Impulse: " + "{:.3f}".format(self.totalImpulse) + " Ns")
+        return I_33
 
-        # Show plots
-        print("\nPlots")
-        self.thrust()
+    @funcify_method("Time (s)", "Inertia I_12 (kg m²)")
+    def propellant_I_12(self):
+        return 0
+
+    @funcify_method("Time (s)", "Inertia I_13 (kg m²)")
+    def propellant_I_13(self):
+        return 0
+
+    @funcify_method("Time (s)", "Inertia I_23 (kg m²)")
+    def propellant_I_23(self):
+        return 0
 
+    def info(self):
+        """Prints out basic data about the Motor."""
+        self.prints.all()
+        self.plots.thrust()
         return None
 
-    def allInfo(self):
-        """Prints out all data and graphs available about the Motor.
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-        None
-        """
-        # Print nozzle details
-        print("Nozzle Details")
-        print("Nozzle Radius: " + str(self.nozzleRadius) + " m")
-        print("Nozzle Throat Radius: " + str(self.throatRadius) + " m")
-
-        # Print grain details
-        print("\nGrain Details")
-        print("Number of Grains: " + str(self.grainNumber))
-        print("Grain Spacing: " + str(self.grainSeparation) + " m")
-        print("Grain Density: " + str(self.grainDensity) + " kg/m3")
-        print("Grain Outer Radius: " + str(self.grainOuterRadius) + " m")
-        print("Grain Inner Radius: " + str(self.grainInitialInnerRadius) + " m")
-        print("Grain Height: " + str(self.grainInitialHeight) + " m")
-        print("Grain Volume: " + "{:.3f}".format(self.grainInitialVolume) + " m3")
-        print("Grain Mass: " + "{:.3f}".format(self.grainInitialMass) + " kg")
-
-        # Print motor details
-        print("\nMotor Details")
-        print("Total Burning Time: " + str(self.burnOutTime) + " s")
-        print(
-            "Total Propellant Mass: "
-            + "{:.3f}".format(self.propellantInitialMass)
-            + " kg"
-        )
-        print(
-            "Propellant Exhaust Velocity: "
-            + "{:.3f}".format(self.exhaustVelocity)
-            + " m/s"
-        )
-        print("Average Thrust: " + "{:.3f}".format(self.averageThrust) + " N")
-        print(
-            "Maximum Thrust: "
-            + str(self.maxThrust)
-            + " N at "
-            + str(self.maxThrustTime)
-            + " s after ignition."
-        )
-        print("Total Impulse: " + "{:.3f}".format(self.totalImpulse) + " Ns")
-
-        # Show plots
-        print("\nPlots")
-        self.thrust()
-        self.mass()
-        self.massDot()
-        self.grainInnerRadius()
-        self.grainHeight()
-        self.burnRate()
-        self.burnArea()
-        self.Kn()
-        self.inertiaI()
-        self.inertiaIDot()
-        self.inertiaZ()
-        self.inertiaZDot()
+    def all_info(self):
+        """Prints out all data and graphs available about the Motor."""
+        self.prints.all()
+        self.plots.all()
 
         return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rocketpy-0.9.9/rocketpy/__init__.py` & `rocketpy-1.0.0a1/rocketpy/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,37 +8,50 @@
 parachutes. Weather conditions, such as wind profile, can be imported from
 sophisticated datasets, allowing for realistic scenarios. Furthermore, the
 implementation facilitates complex simulations, such as multi-stage rockets,
 design and trajectory optimization and dispersion analysis.
 """
 
 __author__ = "Giovani Hidalgo Ceotto"
+__copyright__ = "Copyright 20XX, RocketPy Team"
 __copyright__ = "Copyright 20XX, Projeto Jupiter"
 __credits__ = ["Matheus Marques Araujo", "Rodrigo Schmitt", "Guilherme Tavares"]
 __license__ = "MIT"
-__version__ = "0.9.9"
+__version__ = "1.0.0a1"
 __maintainer__ = "Giovani Hidalgo Ceotto"
 __email__ = "ghceotto@gmail.com"
 __status__ = "Production"
 
-import re
-import math
-import bisect
-import warnings
-import time
-from datetime import datetime, timedelta
-from inspect import signature, getsourcelines
-from collections import namedtuple
-
-import numpy as np
-from scipy import integrate
-from scipy import linalg
-import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from matplotlib import cm
-
-from .Function import Function
+from .AeroSurface import (
+    AeroSurface,
+    EllipticalFins,
+    Fins,
+    NoseCone,
+    RailButtons,
+    Tail,
+    TrapezoidalFins,
+)
+from .Components import Components
 from .Environment import Environment
-from .SolidMotor import SolidMotor
-from .Rocket import Rocket
+from .EnvironmentAnalysis import EnvironmentAnalysis
 from .Flight import Flight
+from .Function import Function
+from .motors import (
+    CylindricalTank,
+    EmptyMotor,
+    Fluid,
+    GenericMotor,
+    HybridMotor,
+    LevelBasedTank,
+    LiquidMotor,
+    MassBasedTank,
+    MassFlowRateBasedTank,
+    SolidMotor,
+    SphericalTank,
+    Tank,
+    TankGeometry,
+    UllageBasedTank,
+)
+from .plots import *
+from .prints import *
+from .Rocket import Rocket
 from .utilities import *
```

### Comparing `rocketpy-0.9.9/rocketpy.egg-info/PKG-INFO` & `rocketpy-1.0.0a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: rocketpy
-Version: 0.9.9
+Version: 1.0.0a1
 Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/giovaniceotto/RocketPy
+Home-page: https://github.com/RocketPy-Team/RocketPy
 Author: Giovani Hidalgo Ceotto
 Author-email: ghceotto@gmail.com
 Maintainer: RocketPy Developers
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: env_analysis
+Provides-Extra: all
 License-File: LICENSE
 
-![RocketPy Logo](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
+![RocketPy Logo](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_Black.svg)
 
 <br>
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RocketPy-Team/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb)
 [![PyPI](https://img.shields.io/pypi/v/rocketpy?color=g)](https://pypi.org/project/rocketpy/)
 [![Documentation Status](https://readthedocs.org/projects/rocketpyalpha/badge/?version=latest)](https://docs.rocketpy.org/en/latest/?badge=latest)
-[![Build Status](https://app.travis-ci.com/Projeto-Jupiter/RocketPy.svg?branch=master)](https://app.travis-ci.com/Projeto-Jupiter/RocketPy)
-[![Contributors](https://img.shields.io/github/contributors/Projeto-Jupiter/rocketpy)](https://github.com/Projeto-Jupiter/RocketPy/graphs/contributors)
+[![Build Status](https://app.travis-ci.com/RocketPy-Team/RocketPy.svg?branch=master)](https://app.travis-ci.com/RocketPy-Team/RocketPy)
+[![Contributors](https://img.shields.io/github/contributors/RocketPy-Team/rocketpy)](https://github.com/RocketPy-Team/RocketPy/graphs/contributors)
 [![Chat on Discord](https://img.shields.io/discord/765037887016140840?logo=discord)](https://discord.gg/b6xYnNh)
+[![Sponsor RocketPy](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/RocketPy-Team)
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/rocketpy)
 [![DOI](https://img.shields.io/badge/DOI-10.1061%2F%28ASCE%29AS.1943--5525.0001331-blue.svg)](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331)
 
 <img src="https://static.scarf.sh/a.png?x-pxid=6f4094ab-00fa-4a8d-9247-b7ed27e7164d" />
 
 # RocketPy
-RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profile, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
+
+RocketPy is the next-generation trajectory simulation solution for High-Power Rocketry. The code is written as a [Python](http://www.python.org) library and allows for a complete 6 degrees of freedom simulation of a rocket's flight trajectory, including high-fidelity variable mass effects as well as descent under parachutes. Weather conditions, such as wind profiles, can be imported from sophisticated datasets, allowing for realistic scenarios. Furthermore, the implementation facilitates complex simulations, such as multi-stage rockets, design and trajectory optimization and dispersion analysis.
 
 <br>
 
 ## Main features
+
 <details>
 <summary>Nonlinear 6 degrees of freedom simulations</summary>
 <ul>
   <li>Rigorous treatment of mass variation effects</li>
   <li>Solved using LSODA with adjustable error tolerances</li>
   <li>Highly optimized to run fast</li>
 </ul>
@@ -69,17 +72,18 @@
 <ul>
   <li>Test the exact code that will fly</li>
   <li>Sensor data can be augmented with noise</li>
 </ul>
 </details>
 
 <details>
-<summary>Solid motors models</summary>
+<summary>Solid, Hybrid and Liquid motors models</summary>
 <ul>
   <li>Burn rate and mass variation properties from thrust curve</li>
+  <li>Define custom rocket tanks based on their flux data</li>
   <li>CSV and ENG file support</li>
 </ul>
 </details>
 
 <details>
 <summary>Monte Carlo simulations</summary>
 <ul>
@@ -88,61 +92,70 @@
 </ul>
 </details>
 
 <details>
 <summary>Flexible and modular</summary>
 <ul>
   <li>Straightforward engineering analysis (e.g. apogee and lifting off speed as a function of mass)</li>
-  <li>Non-standard flights (e.g. parachute drop test from helicopter)</li>
+  <li>Non-standard flights (e.g. parachute drop test from a helicopter)</li>
   <li>Multi-stage rockets</li>
   <li>Custom continuous and discrete control laws</li>
   <li>Create new classes (e.g. other types of motors)</li>
 </ul>
 </details>
 
+<details>
+<summary>Integration with MATLAB®</summary>
+<ul>
+  <li>Straightforward way to run RocketPy from MATLAB®</li>
+  <li>Convert RocketPy results to MATLAB® variables so that they can be processed by MATLAB®</li>
+</ul>
+</details>
+
 <br>
 
 ## Validation
 
 RocketPy's features have been validated in our latest [research article published in the Journal of Aerospace Engineering](http://dx.doi.org/10.1061/%28ASCE%29AS.1943-5525.0001331).
 
 The table below shows a comparison between experimental data and the output from RocketPy.
 Flight data and rocket parameters used in this comparison were kindly provided by [EPFL Rocket Team](https://github.com/EPFLRocketTeam) and [Notre Dame Rocket Team](https://ndrocketry.weebly.com/).
 
-|         Mission         |    Result Paramater    | RocketPy  | Measured  | Relative Error |
-|:-----------------------:|:-----------------------|:---------:|:---------:|:--------------:|
-|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**   |
-|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**   |
-|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **4.24 %**   |
-|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**  |
-|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**  |
-|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**   |
+|         Mission         |    Result Parameter    | RocketPy  | Measured  | Relative Error  |
+|:-----------------------:|:-----------------------|:---------:|:---------:|:---------------:|
+|   Bella Lui Kaltbrumn   | Apogee altitude (m)    |   461.03  |   458.97  |   **0.45 %**    |
+|   Bella Lui Kaltbrumn   | Apogee time (s)        |    10.61  |    10.56  |   **0.47 %**    |
+|   Bella Lui Kaltbrumn   | Maximum velocity (m/s) |    86.18  |    90.00  |   **-4.24 %**   |
+|   NDRT launch vehicle   | Apogee altitude (m)    | 1,310.44  | 1,320.37  |   **-0.75 %**   |
+|   NDRT launch vehicle   | Apogee time (s)        |    16.77  |    17.10  |   **-1.90 %**   |
+|   NDRT launch vehicle   | Maximum velocity (m/s) |   172.86  |   168.95  |   **2.31 %**    |
 
 <br>
 
 ## Documentation
 
 Check out documentation details using the links below:
 
-  - [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
-  - [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
-  - [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
+- [User Guide](https://docs.rocketpy.org/en/latest/user/index.html)
+- [Code Documentation](https://docs.rocketpy.org/en/latest/reference/index.html)
+- [Development Guide](https://docs.rocketpy.org/en/latest/development/index.html)
 
 <br>
 
 # Join Our Community!
-RocketPy is growing fast! Many university groups and rocket hobbyist have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
+
+RocketPy is growing fast! Many university groups and rocket hobbyists have already started using it. The number of stars and forks for this repository is skyrocketing. And this is all thanks to a great community of users, engineers, developers, marketing specialists, and everyone interested in helping.
 
 If you want to be a part of this and make RocketPy your own, join our [Discord](https://discord.gg/b6xYnNh) server today!
 
 <br>
 
 # Previewing
 
-You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/giovaniceotto/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb).  No installation required!
+You can preview RocketPy's main functionalities by browsing through a sample notebook in [Google Colab](https://colab.research.google.com/github/RocketPy-Team/rocketpy/blob/master/docs/notebooks/getting_started_colab.ipynb). No installation is required!
 
 When you are ready to run RocketPy locally, you can read the *Getting Started* section!
 
 <br>
 
 # Getting Started
 
@@ -157,188 +170,226 @@
 For other installation options, visit our [Installation Docs](https://docs.rocketpy.org/en/latest/user/installation.html).
 To learn more about RocketPy's requirements, visit our [Requirements Docs](https://docs.rocketpy.org/en/latest/user/requirements.html).
 
 <br>
 
 ## Running Your First Simulation
 
-In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _nbks_ folder. Open _Getting Started - Examples.ipynb_ and you are ready to go.
+In order to run your first rocket trajectory simulation using RocketPy, you can start a Jupyter Notebook and navigate to the _docs/notebooks_ folder. Open _getting_started.ipynb_ and you are ready to go.
 
 Otherwise, you may want to create your own script or your own notebook using RocketPy. To do this, let's see how to use RocketPy's four main classes:
 
 - Environment - Keeps data related to weather.
-- SolidMotor - Keeps data related to solid motors. Hybrid motor support is coming in the next weeks.
+- Motor - Subdivided into SolidMotor, HybridMotor and LiquidMotor. Keeps data related to rocket motors.
 - Rocket - Keeps data related to a rocket.
 - Flight - Runs the simulation and keeps the results.
 
 The following image shows how the four main classes interact with each other:
 
-![Diagram](https://raw.githubusercontent.com/Projeto-Jupiter/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
+![Diagram](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/Fluxogram-Page-2.svg)
 
 A typical workflow starts with importing these classes from RocketPy:
 
 ```python
 from rocketpy import Environment, Rocket, SolidMotor, Flight
 ```
 
+An optional step is to import datetime, which is used to define the date of the simulation:
+
+```python
+import datetime
+```
+
 Then create an Environment object. To learn more about it, you can use:
 
 ```python
 help(Environment)
 ```
 
 A sample code is:
 
 ```python
-Env = Environment(
-    railLength=5.2,
+env = Environment(
     latitude=32.990254,
     longitude=-106.974998,
     elevation=1400,
-    date=(2020, 3, 4, 12) # Tomorrow's date in year, month, day, hour UTC format
 ) 
 
-Env.setAtmosphericModel(type='Forecast', file='GFS')
+tomorrow = datetime.date.today() + datetime.timedelta(days=1)
+
+env.set_date(
+  (tomorrow.year, tomorrow.month, tomorrow.day, 12), timezone="America/Denver"
+) # Tomorrow's date in year, month, day, hour UTC format
+
+env.set_atmospheric_model(type='Forecast', file='GFS')
 ```
 
 This can be followed up by starting a Solid Motor object. To get help on it, just use:
 
 ```python
 help(SolidMotor)
 ```
 
 A sample Motor object can be created by the following code:
 
 ```python
 Pro75M1670 = SolidMotor(
-    thrustSource="../data/motors/Cesaroni_M1670.eng",
-    burnOut=3.9,
-    grainNumber=5,
-    grainSeparation=5/1000,
-    grainDensity=1815,
-    grainOuterRadius=33/1000,
-    grainInitialInnerRadius=15/1000,
-    grainInitialHeight=120/1000,
-    nozzleRadius=33/1000,
-    throatRadius=11/1000,
-    interpolationMethod='linear'
+    thrust_source="data/motors/Cesaroni_M1670.eng",
+    dry_mass=1.815,
+    dry_inertia=(0.125, 0.125, 0.002),
+    center_of_dry_mass=0.317,
+    grains_center_of_mass_position=0.397,
+    burn_time=3.9,
+    grain_number=5,
+    grain_separation=0.005,
+    grain_density=1815,
+    grain_outer_radius=0.033,
+    grain_initial_inner_radius=0.015,
+    grain_initial_height=0.12,
+    nozzle_radius=0.033,
+    throat_radius=0.011,
+    interpolation_method="linear",
+    nozzle_position=0,
+    coordinate_system_orientation="nozzle_to_combustion_chamber",
 )
 ```
 
 With a Solid Motor defined, you are ready to create your Rocket object. As you may have guessed, to get help on it, use:
 
 ```python
 help(Rocket)
 ```
 
 A sample code to create a Rocket is:
 
 ```python
-Calisto = Rocket(
-    motor=Pro75M1670,
-    radius=127/2000,
-    mass=19.197-2.956,
-    inertiaI=6.60,
-    inertiaZ=0.0351,
-    distanceRocketNozzle=-1.255,
-    distanceRocketPropellant=-0.85704,
-    powerOffDrag='../data/calisto/powerOffDragCurve.csv',
-    powerOnDrag='../data/calisto/powerOnDragCurve.csv'
+calisto = Rocket(
+    radius=0.0635,
+    mass=14.426,  # without motor
+    inertia=(6.321, 6.321, 0.034),
+    power_off_drag="data/calisto/powerOffDragCurve.csv",
+    power_on_drag="data/calisto/powerOnDragCurve.csv",
+    center_of_mass_without_motor=0,
+    coordinate_system_orientation="tail_to_nose",
 )
 
-Calisto.setRailButtons([0.2, -0.5])
+buttons = calisto.set_rail_buttons(
+    upper_button_position=0.0818,
+    lower_button_position=-0.6182,
+    angular_position=45,
+)
 
-NoseCone = Calisto.addNose(length=0.55829, kind="vonKarman", distanceToCM=0.71971)
+calisto.add_motor(Pro75M1670, position=-1.255)
 
-FinSet = Calisto.addFins(4, span=0.100, rootChord=0.120, tipChord=0.040, distanceToCM=-1.04956)
+nose = calisto.add_nose(
+    length=0.55829, kind="vonKarman", position=1.278
+)
+
+fins = calisto.add_trapezoidal_fins(
+    n=4,
+    root_chord=0.120,
+    tip_chord=0.040,
+    span=0.100,
+    sweep_length=None,
+    cant_angle=0,
+    position=-1.04956,
+)
 
-Tail = Calisto.addTail(topRadius=0.0635, bottomRadius=0.0435, length=0.060, distanceToCM=-1.194656)
+tail = calisto.add_tail(
+    top_radius=0.0635, bottom_radius=0.0435, length=0.060, position=-1.194656
+)
 ```
 
 You may want to add parachutes to your rocket as well:
 
 ```python
-def drogueTrigger(p, y):
-    return True if y[5] < 0 else False
-
-def mainTrigger(p, y):
-    return True if y[5] < 0 and y[2] < 800 else False
+main = calisto.add_parachute(
+    name="main",
+    cd_s=10.0,
+    trigger=800,  # ejection altitude in meters
+    sampling_rate=105,
+    lag=1.5,
+    noise=(0, 8.3, 0.5),
+)
 
-Main = Calisto.addParachute('Main',
-                            CdS=10.0,
-                            trigger=mainTrigger, 
-                            samplingRate=105,
-                            lag=1.5,
-                            noise=(0, 8.3, 0.5))
-
-Drogue = Calisto.addParachute('Drogue',
-                              CdS=1.0,
-                              trigger=drogueTrigger, 
-                              samplingRate=105,
-                              lag=1.5,
-                              noise=(0, 8.3, 0.5))
+drogue = calisto.add_parachute(
+    name="drogue",
+    cd_s=1.0,
+    trigger="apogee",  # ejection at apogee
+    sampling_rate=105,
+    lag=1.5,
+    noise=(0, 8.3, 0.5),
+)
 ```
 
 Finally, you can create a Flight object to simulate your trajectory. To get help on the Flight class, use:
 
 ```python
 help(Flight)
 ```
 
 To actually create a Flight object, use:
 
 ```python
-TestFlight = Flight(rocket=Calisto, environment=Env, inclination=85, heading=0)
+test_flight = Flight(
+  rocket=calisto, environment=env, rail_length=5.2, inclination=85, heading=0
+)
 ```
 
-Once the TestFlight object is created, your simulation is done! Use the following code to get a summary of the results:
+Once the Flight object is created, your simulation is done! Use the following code to get a summary of the results:
 
 ```python
-TestFlight.info()
+test_flight.info()
 ```
 
-To seel all available results, use:
+To see all available results, use:
 
 ```python
-TestFlight.allInfo()
+test_flight.all_info()
 ```
 
-Here is just a quick taste of what RocketPy is able to calculate. There are hundred of plots and data points computed by RocketPy to enhance your analyses.
+Here is just a quick taste of what RocketPy is able to calculate. There are hundreds of plots and data points computed by RocketPy to enhance your analyses.
+
+![6-DOF Trajectory Plot](https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/rocketpy_example_trajectory.svg)
 
-![6-DOF Trajectory Plot](docs/static/rocketpy_example_trajectory.svg)
+If you want to see the trajectory on Google Earth, RocketPy acn easily export a KML file for you:
+
+```python
+test_flight.export_kml(file_name="test_flight.kml")
+```
 
 <br>
 
 # Authors and Contributors
 
 This package was originally created by [Giovani Ceotto](https://github.com/giovaniceotto/) as part of his work at [Projeto Jupiter](https://github.com/Projeto-Jupiter/). [Rodrigo Schmitt](https://github.com/rodrigo-schmitt/) was one of the first contributors.
 
 Later, [Guilherme Fernandes](https://github.com/Gui-FernandesBR/) and [Lucas Azevedo](https://github.com/lucasfourier/) joined the team to work on the expansion and sustainability of this project.
 
-Since then, the [RocketPy Team](https://github.com/orgs/Projeto-Jupiter/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
+Since then, the [RocketPy Team](https://github.com/orgs/RocketPy-Team/teams/rocketpy-team) has been growing fast and our contributors are what makes us special!
 
-[![GitHub Contributors Image](https://contrib.rocks/image?repo=Projeto-Jupiter/RocketPy)](https://github.com/Projeto-Jupiter/RocketPy/contributors)
+[![GitHub Contributors Image](https://contrib.rocks/image?repo=RocketPy-Team/RocketPy)](https://github.com/RocketPy-Team/RocketPy/contributors)
 
-See a [detailed list of contributors](https://github.com/Projeto-Jupiter/RocketPy/contributors) who are actively working on RocketPy.
+See a [detailed list of contributors](https://github.com/RocketPy-Team/RocketPy/contributors) who are actively working on RocketPy.
 
 ## Supporting RocketPy and Contributing
 
-The easiest way to help RocketPy is to demonstrate your support by starring our repository! ![GitHub Repo stars](https://img.shields.io/github/stars/Projeto-Jupiter/RocketPy?style=social)
+The easiest way to help RocketPy is to demonstrate your support by starring our repository!
+[![starcharts stargazers over time](https://starchart.cc/rocketpy-team/rocketpy.svg)](https://starchart.cc/rocketpy-team/rocketpy)
 
-<br>
+You can also become a [sponsor](https://github.com/sponsors/RocketPy-Team) and help us financially to keep the project going.
 
 If you are actively using RocketPy in one of your projects, reaching out to our core team via [Discord](https://discord.gg/b6xYnNh) and providing feedback can help improve RocketPy a lot!
 
-And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more on how you can contribute with the development of this next-gen trajectory simulation solution for rocketry.
+And if you are interested in going one step further, please read [CONTRIBUTING.md](https://github.com/RocketPy-Team/RocketPy/blob/master/CONTRIBUTING.md) for details on our code of conduct and learn more about how you can contribute to the development of this next-gen trajectory simulation solution for rocketry.
 
 <br>
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Projeto-Jupiter/RocketPy/blob/master/LICENSE) file for details
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/RocketPy-Team/RocketPy/blob/master/LICENSE) file for details
 
 <br>
 
 ## Release Notes
-Want to know which bugs have been fixed and new features of each version? Check out the [release notes](https://github.com/Projeto-Jupiter/RocketPy/releases).
-
 
+Want to know which bugs have been fixed and the new features of each version? Check out the [release notes](https://github.com/RocketPy-Team/RocketPy/releases).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

