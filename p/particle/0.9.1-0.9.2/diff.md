# Comparing `tmp/Particle-0.9.1.tar.gz` & `tmp/Particle-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Particle-0.9.1.tar", last modified: Tue Jan 14 11:18:03 2020, max compression
+gzip compressed data, was "dist/Particle-0.9.2.tar", last modified: Fri Feb 14 14:13:51 2020, max compression
```

## Comparing `Particle-0.9.1.tar` & `Particle-0.9.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/
--rw-r--r--   0 vsts      (1001) docker     (117)    15025 2020-01-14 11:18:03.000000 Particle-0.9.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/Particle.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)    15025 2020-01-14 11:18:02.000000 Particle-0.9.1/Particle.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     1956 2020-01-14 11:18:03.000000 Particle-0.9.1/Particle.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2020-01-14 11:18:02.000000 Particle-0.9.1/Particle.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      161 2020-01-14 11:18:02.000000 Particle-0.9.1/Particle.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       15 2020-01-14 11:18:02.000000 Particle-0.9.1/Particle.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (117)    11161 2020-01-14 11:17:52.000000 Particle-0.9.1/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/
--rw-r--r--   0 vsts      (1001) docker     (117)      929 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1884 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      285 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/converters/
--rw-r--r--   0 vsts      (1001) docker     (117)      416 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/converters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     7339 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/converters/bimap.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1121 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/converters/evtgen.py
--rw-r--r--   0 vsts      (1001) docker     (117)      597 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/converters/geant.py
--rw-r--r--   0 vsts      (1001) docker     (117)      620 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/converters/pythia.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/data/
--rw-r--r--   0 vsts      (1001) docker     (117)     3011 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/README.rst
--rw-r--r--   0 vsts      (1001) docker     (117)      319 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)   111526 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/conversions.csv
--rw-r--r--   0 vsts      (1001) docker     (117)    81873 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/mass_width_2008.fwf
--rw-r--r--   0 vsts      (1001) docker     (117)    11594 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/mass_width_2008_ext.fwf
--rw-r--r--   0 vsts      (1001) docker     (117)    29668 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/mass_width_2018.mcd
--rw-r--r--   0 vsts      (1001) docker     (117)    30055 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/mass_width_2019.mcd
--rw-r--r--   0 vsts      (1001) docker     (117)    46197 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/particle2008.csv
--rw-r--r--   0 vsts      (1001) docker     (117)    49453 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/particle2018.csv
--rw-r--r--   0 vsts      (1001) docker     (117)    42973 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/particle2019.csv
--rw-r--r--   0 vsts      (1001) docker     (117)    13037 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/pdgid_to_evtgenname.csv
--rw-r--r--   0 vsts      (1001) docker     (117)     9887 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/pdgid_to_geant3id.csv
--rw-r--r--   0 vsts      (1001) docker     (117)    12786 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/pdgid_to_latexname.csv
--rw-r--r--   0 vsts      (1001) docker     (117)     6200 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/data/pdgid_to_pythiaid.csv
--rw-r--r--   0 vsts      (1001) docker     (117)      250 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/geant/
--rw-r--r--   0 vsts      (1001) docker     (117)      273 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/geant/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1766 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/geant/geant3id.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/particle/
--rw-r--r--   0 vsts      (1001) docker     (117)      489 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    14685 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/convert.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3223 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/enums.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3039 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/kinematics.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1381 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/literals.py
--rw-r--r--   0 vsts      (1001) docker     (117)    34149 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/particle.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1798 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/regex.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4035 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/particle/utilities.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/pdgid/
--rw-r--r--   0 vsts      (1001) docker     (117)     5175 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pdgid/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    19692 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pdgid/functions.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1151 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pdgid/literals.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1620 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pdgid/pdgid.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/particle/pythia/
--rw-r--r--   0 vsts      (1001) docker     (117)      273 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pythia/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1528 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/pythia/pythiaid.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3360 2020-01-14 11:17:52.000000 Particle-0.9.1/particle/shared_literals.py
--rw-r--r--   0 vsts      (1001) docker     (117)       92 2020-01-14 11:18:03.000000 Particle-0.9.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)     2604 2020-01-14 11:17:52.000000 Particle-0.9.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2669 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/converters/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/converters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1277 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/converters/test_maps.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/geant/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/geant/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1071 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/geant/test_geant3id.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/particle/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    12733 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_decfilenames.py
--rw-r--r--   0 vsts      (1001) docker     (117)      617 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_enums.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1767 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_generation.py
--rw-r--r--   0 vsts      (1001) docker     (117)      923 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_kinematics.py
--rw-r--r--   0 vsts      (1001) docker     (117)      351 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_literals.py
--rw-r--r--   0 vsts      (1001) docker     (117)    16658 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_particle.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1985 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/particle/test_utilities.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/pdgid/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pdgid/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    17886 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pdgid/test_functions.py
--rw-r--r--   0 vsts      (1001) docker     (117)      350 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pdgid/test_literals.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2322 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pdgid/test_pdgid.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-14 11:18:03.000000 Particle-0.9.1/tests/pythia/
--rw-r--r--   0 vsts      (1001) docker     (117)      201 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pythia/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1103 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/pythia/test_pythiaid.py
--rw-r--r--   0 vsts      (1001) docker     (117)      279 2020-01-14 11:17:52.000000 Particle-0.9.1/tests/test_package.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/
+-rw-r--r--   0 vsts      (1001) docker     (115)    15214 2020-02-14 14:13:51.000000 Particle-0.9.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (115)    15214 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (115)     1956 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)        1 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)      161 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)       15 2020-02-14 14:13:51.000000 Particle-0.9.2/Particle.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (115)    11318 2020-02-14 14:13:42.000000 Particle-0.9.2/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/
+-rw-r--r--   0 vsts      (1001) docker     (115)      929 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1884 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      285 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/converters/
+-rw-r--r--   0 vsts      (1001) docker     (115)      416 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/converters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     7339 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/converters/bimap.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1121 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/converters/evtgen.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      597 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/converters/geant.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      620 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/converters/pythia.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/data/
+-rw-r--r--   0 vsts      (1001) docker     (115)     3011 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (115)      319 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)   111526 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/conversions.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)    81873 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/mass_width_2008.fwf
+-rw-r--r--   0 vsts      (1001) docker     (115)    11594 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/mass_width_2008_ext.fwf
+-rw-r--r--   0 vsts      (1001) docker     (115)    29668 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/mass_width_2018.mcd
+-rw-r--r--   0 vsts      (1001) docker     (115)    30055 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/mass_width_2019.mcd
+-rw-r--r--   0 vsts      (1001) docker     (115)    46197 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/particle2008.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)    49453 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/particle2018.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)    42973 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/particle2019.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)    13037 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/pdgid_to_evtgenname.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)     9887 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/pdgid_to_geant3id.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)    12786 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/pdgid_to_latexname.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)     6200 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/data/pdgid_to_pythiaid.csv
+-rw-r--r--   0 vsts      (1001) docker     (115)      250 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/geant/
+-rw-r--r--   0 vsts      (1001) docker     (115)      273 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/geant/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1766 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/geant/geant3id.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/particle/
+-rw-r--r--   0 vsts      (1001) docker     (115)      489 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    14685 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/convert.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3223 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3039 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/kinematics.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1381 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/literals.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    34543 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/particle.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1798 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/regex.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     4035 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/particle/utilities.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/pdgid/
+-rw-r--r--   0 vsts      (1001) docker     (115)     5175 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pdgid/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    19692 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pdgid/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1151 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pdgid/literals.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1620 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pdgid/pdgid.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/particle/pythia/
+-rw-r--r--   0 vsts      (1001) docker     (115)      273 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pythia/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1528 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/pythia/pythiaid.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     3360 2020-02-14 14:13:42.000000 Particle-0.9.2/particle/shared_literals.py
+-rw-r--r--   0 vsts      (1001) docker     (115)       92 2020-02-14 14:13:51.000000 Particle-0.9.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (115)     2604 2020-02-14 14:13:42.000000 Particle-0.9.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2669 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/converters/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/converters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1277 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/converters/test_maps.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/geant/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/geant/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1071 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/geant/test_geant3id.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/particle/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    12733 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_decfilenames.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      617 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1767 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_generation.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      923 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_kinematics.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      351 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_literals.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    16705 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_particle.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1985 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/particle/test_utilities.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/pdgid/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pdgid/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)    17886 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pdgid/test_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      350 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pdgid/test_literals.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     2322 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pdgid/test_pdgid.py
+drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2020-02-14 14:13:51.000000 Particle-0.9.2/tests/pythia/
+-rw-r--r--   0 vsts      (1001) docker     (115)      201 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pythia/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (115)     1103 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/pythia/test_pythiaid.py
+-rw-r--r--   0 vsts      (1001) docker     (115)      279 2020-02-14 14:13:42.000000 Particle-0.9.2/tests/test_package.py
```

### Comparing `Particle-0.9.1/PKG-INFO` & `Particle-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: Particle
-Version: 0.9.1
+Version: 0.9.2
 Summary: PDG particle data and identification codes
 Home-page: https://github.com/scikit-hep/particle
 Author: Eduardo Rodrigues
 Author-email: eduardo.rodrigues@cern.ch
 Maintainer: The Scikit-HEP admins
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: BSD 3-Clause License
 Description: .. image:: https://github.com/scikit-hep/particle/raw/master/docs/ParticleLogo300.png
             :alt: particle
             :target: https://github.com/scikit-hep/particle
         
         
-        Particle: PDG particle data and identification codes
-        ====================================================
+        ``Particle``: PDG particle data and identification codes
+        ========================================================
+        
+        .. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
+           :alt: Scikit-HEP project package
+           :target: https://scikit-hep.org
         
         .. image:: https://img.shields.io/pypi/v/particle.svg
           :alt: PyPI
           :target: https://pypi.python.org/pypi/particle
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2552429.svg
           :target: https://doi.org/10.5281/zenodo.2552429
```

### Comparing `Particle-0.9.1/Particle.egg-info/PKG-INFO` & `Particle-0.9.2/Particle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: Particle
-Version: 0.9.1
+Version: 0.9.2
 Summary: PDG particle data and identification codes
 Home-page: https://github.com/scikit-hep/particle
 Author: Eduardo Rodrigues
 Author-email: eduardo.rodrigues@cern.ch
 Maintainer: The Scikit-HEP admins
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: BSD 3-Clause License
 Description: .. image:: https://github.com/scikit-hep/particle/raw/master/docs/ParticleLogo300.png
             :alt: particle
             :target: https://github.com/scikit-hep/particle
         
         
-        Particle: PDG particle data and identification codes
-        ====================================================
+        ``Particle``: PDG particle data and identification codes
+        ========================================================
+        
+        .. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
+           :alt: Scikit-HEP project package
+           :target: https://scikit-hep.org
         
         .. image:: https://img.shields.io/pypi/v/particle.svg
           :alt: PyPI
           :target: https://pypi.python.org/pypi/particle
         
         .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2552429.svg
           :target: https://doi.org/10.5281/zenodo.2552429
```

### Comparing `Particle-0.9.1/Particle.egg-info/SOURCES.txt` & `Particle-0.9.2/Particle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/README.rst` & `Particle-0.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .. image:: https://github.com/scikit-hep/particle/raw/master/docs/ParticleLogo300.png
     :alt: particle
     :target: https://github.com/scikit-hep/particle
 
 
-Particle: PDG particle data and identification codes
-====================================================
+``Particle``: PDG particle data and identification codes
+========================================================
+
+.. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
+   :alt: Scikit-HEP project package
+   :target: https://scikit-hep.org
 
 .. image:: https://img.shields.io/pypi/v/particle.svg
   :alt: PyPI
   :target: https://pypi.python.org/pypi/particle
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2552429.svg
   :target: https://doi.org/10.5281/zenodo.2552429
```

### Comparing `Particle-0.9.1/particle/__init__.py` & `Particle-0.9.2/particle/__init__.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/__main__.py` & `Particle-0.9.2/particle/__main__.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/converters/bimap.py` & `Particle-0.9.2/particle/converters/bimap.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/converters/evtgen.py` & `Particle-0.9.2/particle/converters/evtgen.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/converters/geant.py` & `Particle-0.9.2/particle/converters/geant.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/converters/pythia.py` & `Particle-0.9.2/particle/converters/pythia.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/README.rst` & `Particle-0.9.2/particle/data/README.rst`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/conversions.csv` & `Particle-0.9.2/particle/data/conversions.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/mass_width_2008.fwf` & `Particle-0.9.2/particle/data/mass_width_2008.fwf`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/mass_width_2008_ext.fwf` & `Particle-0.9.2/particle/data/mass_width_2008_ext.fwf`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/mass_width_2018.mcd` & `Particle-0.9.2/particle/data/mass_width_2018.mcd`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/mass_width_2019.mcd` & `Particle-0.9.2/particle/data/mass_width_2019.mcd`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/particle2008.csv` & `Particle-0.9.2/particle/data/particle2008.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/particle2018.csv` & `Particle-0.9.2/particle/data/particle2018.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/particle2019.csv` & `Particle-0.9.2/particle/data/particle2019.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/pdgid_to_evtgenname.csv` & `Particle-0.9.2/particle/data/pdgid_to_evtgenname.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/pdgid_to_geant3id.csv` & `Particle-0.9.2/particle/data/pdgid_to_geant3id.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/pdgid_to_latexname.csv` & `Particle-0.9.2/particle/data/pdgid_to_latexname.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/data/pdgid_to_pythiaid.csv` & `Particle-0.9.2/particle/data/pdgid_to_pythiaid.csv`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/geant/geant3id.py` & `Particle-0.9.2/particle/geant/geant3id.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/convert.py` & `Particle-0.9.2/particle/particle/convert.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/enums.py` & `Particle-0.9.2/particle/particle/enums.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/kinematics.py` & `Particle-0.9.2/particle/particle/kinematics.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/literals.py` & `Particle-0.9.2/particle/particle/literals.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/particle.py` & `Particle-0.9.2/particle/particle/particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     width_upper
         The upper uncertainty on the particle decay width, in MeV.
     """
 
     pdgid = attr.ib(converter=PDGID)
     pdg_name = attr.ib()
-    mass = attr.ib()
+    mass = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     mass_upper = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     mass_lower = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     width = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     width_upper = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     width_lower = attr.ib(-1, converter=lambda v: None if v < 0 else v)
     _three_charge = attr.ib(Charge.u, converter=Charge)  # charge * 3
     I = attr.ib(None, converter=_isospin_converter)
@@ -184,18 +184,16 @@
     anti_flag = attr.ib(0, converter=Inv)  # Info about particle name for anti-particles
     rank = attr.ib(0)
     status = attr.ib(Status.Nonexistent, converter=Status)
     quarks = attr.ib("", converter=str)
     latex_name = attr.ib("Unknown")
 
     def __repr__(self):
-        return '<{self.__class__.__name__}: name="{self!s}", pdgid={pdgid}, mass={mass} MeV>'.format(
-            self=self,
-            pdgid=int(self.pdgid),
-            mass=str_with_unc(self.mass, self.mass_upper, self.mass_lower),
+        return '<{self.__class__.__name__}: name="{self!s}", pdgid={pdgid}, mass={mass}>'.format(
+            self=self, pdgid=int(self.pdgid), mass=self._str_mass()
         )
 
     _table = None  # Loaded table of entries
     _table_names = None  # Names of loaded tables
 
     @classmethod
     def table_names(cls):
@@ -289,24 +287,28 @@
         floatfmt: str, optional, default is '.12g'
             Number formatting, see the tabulate's package
             tabulate function for a description of available options.
         numalign: str or None, oprional, default is 'decimal'
             Column alignment for numbers, see the tabulate's package
             tabulate function for a description of available options.
 
+        Returns
+        -------
+        str or None if filename is None or not, respectively.
+
         Note
         ----
         Uses the `tabulate` package.
 
         Examples
         --------
-        Particle.dump_table()
-        Particle.dump_table(n_rows=5)
-        Particle.dump_table(exclusive_fields=['pdgid', 'pdg_name'])
-        Particle.dump_table(filter_fn=lambda p: p.pdgid.has_bottom)
+        print(Particle.dump_table())
+        print(Particle.dump_table(n_rows=5))
+        print(Particle.dump_table(exclusive_fields=['pdgid', 'pdg_name']))
+        print(Particle.dump_table(filter_fn=lambda p: p.pdgid.has_bottom))
         Particle.dump_table(filename='output.txt', tablefmt='rst')
         """
         from tabulate import tabulate
 
         if not cls.table_loaded():
             cls.load_table()
 
@@ -350,22 +352,20 @@
                         tablefmt=tablefmt,
                         floatfmt=floatfmt,
                         numalign=numalign,
                     ),
                     file=outfile,
                 )
         else:
-            print(
-                tabulate(
-                    tbl,
-                    headers=tbl_names,
-                    tablefmt=tablefmt,
-                    floatfmt=floatfmt,
-                    numalign=numalign,
-                )
+            return tabulate(
+                tbl,
+                headers=tbl_names,
+                tablefmt=tablefmt,
+                floatfmt=floatfmt,
+                numalign=numalign,
             )
 
     @classmethod
     def load_table(cls, filename=None, append=False):
         """
         Load a particle data CSV table. Optionally append to the existing data already loaded if append=True.
         As a special case, if this is called with append=True and the table is not loaded, the default will
@@ -643,15 +643,16 @@
     )
 
     def _repr_latex_(self):
         name = self.latex_name
         return ("$" + name + "$") if self.latex_name else "?"
 
     def _width_or_lifetime(self):
-        """Display either the particle width or the lifetime.
+        """
+        Display either the particle width or the lifetime.
         Internally used by the describe() method.
 
         Note
         ----
         Width errors equal to None flag an experimental upper limit on the width.
         """
         if self.width is None:
@@ -680,31 +681,44 @@
                 )
             return s
         else:
             return "Width = {width} MeV".format(
                 width=str_with_unc(self.width, self.width_upper, self.width_lower)
             )
 
+    def _str_mass(self):
+        """
+        Display a reasonable particle mass printout
+        even when no mass value is available.
+        Internally used by the describe() method.
+        """
+        if self.mass is None:
+            return "?"
+        else:
+            return "{0} MeV".format(
+                str_with_unc(self.mass, self.mass_upper, self.mass_lower)
+            )
+
     def describe(self):
         "Make a nice high-density string for a particle's properties."
         if self.pdgid == 0:
             return "Name: Unknown"
 
         val = """Name: {self!s:<14} ID: {self.pdgid:<12} Latex: {latex_name}
-Mass  = {mass} MeV
+Mass  = {mass}
 {width_or_lifetime}
 Q (charge)        = {Q:<6}  J (total angular) = {self.J!s:<7}  P (space parity) = {P}
 C (charge parity) = {C:<6}  I (isospin)       = {self.I!s:<7}  G (G-parity)     = {G}
 """.format(
             self=self,
             G=Parity_undo[self.G],
             C=Parity_undo[self.C],
             Q=Charge_undo[self.three_charge],
             P=Parity_undo[self.P],
-            mass=str_with_unc(self.mass, self.mass_upper, self.mass_lower),
+            mass=self._str_mass(),
             width_or_lifetime=self._width_or_lifetime(),
             latex_name=self._repr_latex_(),
         )
 
         if self.spin_type != SpinType.Unknown:
             val += "    SpinType: {self.spin_type!s}\n".format(self=self)
         if self.quarks:
@@ -728,15 +742,15 @@
     def html_name(self):
         "This is the name using HTML instead of LaTeX."
         return latex_to_html_name(self.latex_name)
 
     @classmethod
     def empty(cls):
         "Make a new empty particle."
-        return cls(0, "Unknown", 0.0, 0.0, 0, Inv.Same)
+        return cls(0, "Unknown", anti_flag=Inv.Same)
 
     @classmethod
     def from_pdgid(cls, value):
         """
         Get a particle from a PDGID. Uses by default the package
         extended PDG data table.
```

### Comparing `Particle-0.9.1/particle/particle/regex.py` & `Particle-0.9.2/particle/particle/regex.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/particle/utilities.py` & `Particle-0.9.2/particle/particle/utilities.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/pdgid/__init__.py` & `Particle-0.9.2/particle/pdgid/__init__.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/pdgid/functions.py` & `Particle-0.9.2/particle/pdgid/functions.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/pdgid/literals.py` & `Particle-0.9.2/particle/pdgid/literals.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/pdgid/pdgid.py` & `Particle-0.9.2/particle/pdgid/pdgid.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/pythia/pythiaid.py` & `Particle-0.9.2/particle/pythia/pythiaid.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/particle/shared_literals.py` & `Particle-0.9.2/particle/shared_literals.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/setup.py` & `Particle-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/conftest.py` & `Particle-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/converters/test_maps.py` & `Particle-0.9.2/tests/converters/test_maps.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/geant/test_geant3id.py` & `Particle-0.9.2/tests/geant/test_geant3id.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/particle/test_decfilenames.py` & `Particle-0.9.2/tests/particle/test_decfilenames.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/particle/test_enums.py` & `Particle-0.9.2/tests/particle/test_enums.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/particle/test_generation.py` & `Particle-0.9.2/tests/particle/test_generation.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/particle/test_kinematics.py` & `Particle-0.9.2/tests/particle/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/particle/test_particle.py` & `Particle-0.9.2/tests/particle/test_particle.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,16 +479,18 @@
 
     assert particle.I == isospin
 
 
 def test_default_particle():
     p = Particle.empty()
 
-    assert repr(p) == '<Particle: name="Unknown", pdgid=0, mass=0.0 MeV>'
+    assert repr(p) == '<Particle: name="Unknown", pdgid=0, mass=?>'
     assert "Name: Unknown" in p.describe()
+    assert p.mass == None
+    assert p.width == None
     assert p.spin_type == SpinType.NonDefined
     assert p.programmatic_name == "Unknown"
     assert p.status == Status.Nonexistent
 
 
 ampgen_style_names = (
     ("b", 5),
```

### Comparing `Particle-0.9.1/tests/particle/test_utilities.py` & `Particle-0.9.2/tests/particle/test_utilities.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/pdgid/test_functions.py` & `Particle-0.9.2/tests/pdgid/test_functions.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/pdgid/test_pdgid.py` & `Particle-0.9.2/tests/pdgid/test_pdgid.py`

 * *Files identical despite different names*

### Comparing `Particle-0.9.1/tests/pythia/test_pythiaid.py` & `Particle-0.9.2/tests/pythia/test_pythiaid.py`

 * *Files identical despite different names*

