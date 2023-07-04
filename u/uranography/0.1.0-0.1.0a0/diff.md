# Comparing `tmp/uranography-0.1.0.tar.gz` & `tmp/uranography-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uranography-0.1.0.tar", last modified: Tue Jul  4 18:13:25 2023, max compression
+gzip compressed data, was "uranography-0.1.0a0.tar", last modified: Mon Jun 26 22:45:05 2023, max compression
```

## Comparing `uranography-0.1.0.tar` & `uranography-0.1.0a0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.379583 uranography-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.351583 uranography-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.355583 uranography-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-04 18:13:12.000000 uranography-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-04 18:13:12.000000 uranography-0.1.0/.github/workflows/build_docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-04 18:13:12.000000 uranography-0.1.0/.github/workflows/python_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-04 18:13:12.000000 uranography-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 18:13:12.000000 uranography-0.1.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 18:13:12.000000 uranography-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-04 18:13:25.379583 uranography-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-04 18:13:12.000000 uranography-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.359583 uranography-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)   590780 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/asphere.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)   708604 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/mollweide.html
--rw-r--r--   0 runner    (1001) docker     (123)   648200 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/planisphere.html
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.367583 uranography-0.1.0/docs/usage_figures/
--rw-r--r--   0 runner    (1001) docker     (123)  1684623 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage_figures/adjusted_healpix.html
--rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage_figures/adjusted_planisphere.png
--rw-r--r--   0 runner    (1001) docker     (123)  1684734 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage_figures/basic_healpix.html
--rw-r--r--   0 runner    (1001) docker     (123)   266465 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage_figures/basic_planisphere.html
--rw-r--r--   0 runner    (1001) docker     (123)   532920 2023-07-04 18:13:12.000000 uranography-0.1.0/docs/usage_figures/simple_horizon.html
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-04 18:13:12.000000 uranography-0.1.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.367583 uranography-0.1.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   145833 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/exposures.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/intro_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   400320 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/r_depth.fits
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/rubin_idealized.txt
--rw-r--r--   0 runner    (1001) docker     (123)   400320 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/sample_survey_footprint.fits
--rw-r--r--   0 runner    (1001) docker     (123)    44647 2023-07-04 18:13:12.000000 uranography-0.1.0/notebooks/uranography.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-04 18:13:12.000000 uranography-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 18:13:12.000000 uranography-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 18:13:25.379583 uranography-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:13:12.000000 uranography-0.1.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.371583 uranography-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_armillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_horizon.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_mollweide.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_planisphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_readjs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_spheremap.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 18:13:12.000000 uranography-0.1.0/tests/test_stars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.375583 uranography-0.1.0/uranography/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/armillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/horizon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.379583 uranography-0.1.0/uranography/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/coord_utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/horizon.js
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/hp.js
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/laea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/mollweide.js
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/orthographic.js
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/update.js
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/js/update_map.js
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/mollweide.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/planisphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/readjs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    56686 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/spheremap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-04 18:13:12.000000 uranography-0.1.0/uranography/stars.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:13:25.375583 uranography-0.1.0/uranography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:13:25.000000 uranography-0.1.0/uranography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.616664 uranography-0.1.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.576664 uranography-0.1.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.584664 uranography-0.1.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-26 22:44:50.000000 uranography-0.1.0a0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-26 22:44:50.000000 uranography-0.1.0a0/.github/workflows/build_docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 22:44:50.000000 uranography-0.1.0a0/.github/workflows/python_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-26 22:44:50.000000 uranography-0.1.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 22:44:50.000000 uranography-0.1.0a0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 22:44:50.000000 uranography-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-26 22:45:05.616664 uranography-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-26 22:44:50.000000 uranography-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.592664 uranography-0.1.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   590780 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/asphere.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   708604 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/mollweide.html
+-rw-r--r--   0 runner    (1001) docker     (123)   648200 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/planisphere.html
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.600664 uranography-0.1.0a0/docs/usage_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)  1684623 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage_figures/adjusted_healpix.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage_figures/adjusted_planisphere.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1684734 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage_figures/basic_healpix.html
+-rw-r--r--   0 runner    (1001) docker     (123)   266465 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage_figures/basic_planisphere.html
+-rw-r--r--   0 runner    (1001) docker     (123)   532920 2023-06-26 22:44:50.000000 uranography-0.1.0a0/docs/usage_figures/simple_horizon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-26 22:44:50.000000 uranography-0.1.0a0/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.604664 uranography-0.1.0a0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   145833 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/exposures.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/intro_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   400320 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/r_depth.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/rubin_idealized.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   400320 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/sample_survey_footprint.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    44647 2023-06-26 22:44:50.000000 uranography-0.1.0a0/notebooks/uranography.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-26 22:44:50.000000 uranography-0.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 22:44:50.000000 uranography-0.1.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 22:45:05.616664 uranography-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 22:44:50.000000 uranography-0.1.0a0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.608664 uranography-0.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_armillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_horizon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_mollweide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_planisphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_readjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_spheremap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-26 22:44:50.000000 uranography-0.1.0a0/tests/test_stars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.612664 uranography-0.1.0a0/uranography/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/armillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/horizon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.616664 uranography-0.1.0a0/uranography/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/coord_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/horizon.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/hp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/laea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/mollweide.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/orthographic.js
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/js/update_map.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/mollweide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/planisphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/readjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56686 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/spheremap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-26 22:44:50.000000 uranography-0.1.0a0/uranography/stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 22:45:05.612664 uranography-0.1.0a0/uranography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 22:45:05.000000 uranography-0.1.0a0/uranography.egg-info/top_level.txt
```

### Comparing `uranography-0.1.0/.github/workflows/build.yaml` & `uranography-0.1.0a0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/.github/workflows/build_docs.yaml` & `uranography-0.1.0a0/.github/workflows/build_docs.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 name: Build and Upload Docs
 
-"on":
+on:
   push:
-    tags:
-      - "*"
     branches:
-      - "main"
-  pull_request: {}
+      - main
+  pull_request:
+    branches:
+      - main
   workflow_dispatch:
 
 jobs:
   build_sphinx_docs:
     name: Build and upload documentation
     runs-on: ubuntu-latest
     steps:
```

### Comparing `uranography-0.1.0/.github/workflows/python_tests.yaml` & `uranography-0.1.0a0/.github/workflows/python_tests.yaml`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/.gitignore` & `uranography-0.1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/LICENSE` & `uranography-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/README.md` & `uranography-0.1.0a0/docs/README.md`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/Makefile` & `uranography-0.1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/api.rst` & `uranography-0.1.0a0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/asphere.html` & `uranography-0.1.0a0/docs/asphere.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/installation.rst` & `uranography-0.1.0a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/introduction.rst` & `uranography-0.1.0a0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/mollweide.html` & `uranography-0.1.0a0/docs/mollweide.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/planisphere.html` & `uranography-0.1.0a0/docs/planisphere.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage.rst` & `uranography-0.1.0a0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage_figures/adjusted_healpix.html` & `uranography-0.1.0a0/docs/usage_figures/adjusted_healpix.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage_figures/adjusted_planisphere.png` & `uranography-0.1.0a0/docs/usage_figures/adjusted_planisphere.png`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage_figures/basic_healpix.html` & `uranography-0.1.0a0/docs/usage_figures/basic_healpix.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage_figures/basic_planisphere.html` & `uranography-0.1.0a0/docs/usage_figures/basic_planisphere.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/docs/usage_figures/simple_horizon.html` & `uranography-0.1.0a0/docs/usage_figures/simple_horizon.html`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/environment.yaml` & `uranography-0.1.0a0/environment.yaml`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/exposures.txt` & `uranography-0.1.0a0/notebooks/exposures.txt`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/intro_example.ipynb` & `uranography-0.1.0a0/notebooks/intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/r_depth.fits` & `uranography-0.1.0a0/notebooks/r_depth.fits`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/rubin_idealized.txt` & `uranography-0.1.0a0/notebooks/rubin_idealized.txt`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/sample_survey_footprint.fits` & `uranography-0.1.0a0/notebooks/sample_survey_footprint.fits`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/notebooks/uranography.ipynb` & `uranography-0.1.0a0/notebooks/uranography.ipynb`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/pyproject.toml` & `uranography-0.1.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 [project.urls]
 "Homepage" = "https://github.com/lsst/uranography"
 
 [project.optional-dependencies]
 test = [
     "pytest",
-    "black",
-    "pytest-black",
-    "flake8 < 5",
-    "pytest-flake8",
+    "black == 22.10.0",
+    "pytest-black == 0.3.12",
+    "flake8 == 4.0.1",
+    "pytest-flake8 == 1.1.1",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "setuptools_scm.get_version" }
 
 [tool.setuptools.packages.find]
 where = [ "" ]
```

### Comparing `uranography-0.1.0/tests/helpers.py` & `uranography-0.1.0a0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_armillary.py` & `uranography-0.1.0a0/tests/test_armillary.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_horizon.py` & `uranography-0.1.0a0/tests/test_horizon.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_mollweide.py` & `uranography-0.1.0a0/tests/test_mollweide.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_planisphere.py` & `uranography-0.1.0a0/tests/test_planisphere.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_sphere.py` & `uranography-0.1.0a0/tests/test_sphere.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_spheremap.py` & `uranography-0.1.0a0/tests/test_spheremap.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/tests/test_stars.py` & `uranography-0.1.0a0/tests/test_stars.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/armillary.py` & `uranography-0.1.0a0/uranography/armillary.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/camera.py` & `uranography-0.1.0a0/uranography/camera.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/horizon.py` & `uranography-0.1.0a0/uranography/horizon.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/coord_utils.js` & `uranography-0.1.0a0/uranography/js/coord_utils.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,15 @@
     return coords
 }
 
 let data = {}
 try {
     data = data_source.data
 } catch (e) {
+    console.log("****************HERE!*****************")
     // If we were not passed a data_source with data, assume we were 
     // passed a column of coordinate pairs to transform, and build our
     // data from that.
     data['ra'] = new Array(xs.length)
     data['decl'] = new Array(xs.length)
     for (let i = 0; i < xs.length; i++) {
         data['ra'][i] = xs[i][0]
```

### Comparing `uranography-0.1.0/uranography/js/horizon.js` & `uranography-0.1.0a0/uranography/js/horizon.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/hp.js` & `uranography-0.1.0a0/uranography/js/hp.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/laea.js` & `uranography-0.1.0a0/uranography/js/laea.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/mollweide.js` & `uranography-0.1.0a0/uranography/js/mollweide.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/orthographic.js` & `uranography-0.1.0a0/uranography/js/orthographic.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -62,14 +62,32 @@
 function cartToEq(x, y, z) {
     const theta = Math.acos(z)
     const ra = Math.atan2(y, x)
     const decl = Math.PI / 2 - theta
     return [ra, decl]
 }
 
+function get_gpu() {
+    if (!window.hasOwnProperty('gpu')) {
+        window.gpu = new GPU()
+    }
+    return window.gpu;
+}
+
+const multiplyMultiMatrix = get_gpu().createKernel(function(coeff, data) {
+    let sum = 0;
+    let hpix = this.thread.y
+    let corner = this.thread.x
+    let out_coord = this.thread.z
+    for (let in_coord = 0; in_coord < 3; in_coord++) {
+        sum += coeff[out_coord][in_coord] * data[in_coord][hpix][corner];
+    }
+    return sum;
+})
+
 function multiplyRotationMatrix(a, b) {
     let result = [
         [0.0, 0.0, 0.0],
         [0.0, 0.0, 0.0],
         [0.0, 0.0, 0.0]
     ]
     for (let x = 0; x < 3; x++) {
@@ -99,61 +117,14 @@
         [rxx, rxy, rxz],
         [ryx, ryy, ryz],
         [rzx, rzy, rzz]
     ]
     return matrix
 }
 
-let multiplyMultiMatrix = function(coeff, data) {
-    let result = []
-    for (let out_coord = 0; out_coord < 3; out_coord++) {
-        result[out_coord] = []
-        for (let hpix = 0; hpix < data[0].length; hpix++) {
-            result[out_coord][hpix] = []
-        }
-    }
-
-    for (let hpix = 0; hpix < data[0].length; hpix++) {
-        for (let corner = 0; corner < data[0][hpix].length; corner++) {
-            for (let out_coord = 0; out_coord < 3; out_coord++) {
-                result[out_coord][hpix][corner] = 0;
-                for (let in_coord = 0; in_coord < 3; in_coord++) {
-                    result[out_coord][hpix][corner] += coeff[out_coord][in_coord] * data[in_coord][hpix][corner];
-                }
-            }
-        }
-    }
-    return result
-}
-let useGPU = false
-
-try {
-    function get_gpu() {
-        if (!window.hasOwnProperty('gpu')) {
-            window.gpu = new GPU()
-        }
-        return window.gpu;
-    }
-
-    multiplyMultiMatrix = get_gpu().createKernel(function(coeff, data) {
-        let sum = 0;
-        let hpix = this.thread.y
-        let corner = this.thread.x
-        let out_coord = this.thread.z
-        for (let in_coord = 0; in_coord < 3; in_coord++) {
-            sum += coeff[out_coord][in_coord] * data[in_coord][hpix][corner];
-        }
-        return sum;
-    })
-
-    useGPU = true
-} catch (e) {
-    console.log("gpu.js not available, falling back to CPU")
-}
-
 function applyHealpixRotations(hpx, hpy, hpz, codecl, ra, orient, npoleCoords1) {
     // We are looking out of the sphere from the inside, so the center is 180 degrees 
     // from the front of the sphere, hence the pi.
     const decl_rot = Math.PI + codecl
     const ra_rot = ra - Math.PI / 2
 
     const matrix1 = computeRotationMatrix(1, 0, 0, decl_rot)
@@ -244,17 +215,15 @@
     // If they are lists, iteratate over each element. Otherwise, just apply the rotation to the point.
     if (typeof(x_hp[0]) === 'number') {
         for (let i = 0; i < x_hp.length; i++) {
             const coords = applyRotations(x_hp[i], y_hp[i], z_hp[i], centerCodecl, centerRA, orient, npoleCoords1)
             result[i] = coords[coord_idx]
         }
     } else {
-        if (useGPU) {
-            multiplyMultiMatrix.setOutput([x_hp[0].length, x_hp.length, 3]);
-        }
+        multiplyMultiMatrix.setOutput([x_hp[0].length, x_hp.length, 3]);
         const coords = applyHealpixRotations(x_hp, y_hp, z_hp, centerCodecl, centerRA, orient, npoleCoords1)
         for (let i = 0; i < x_hp.length; i++) {
             result[i] = new Array(x_hp[i].length)
             for (let j = 0; j < x_hp[i].length; j++) {
                 result[i][j] = coords[coord_idx][i][j]
             }
         }
@@ -330,17 +299,15 @@
                 data['y_orth'][i] = coords[1]
             }
             if ('z_orth' in data) {
                 data['z_orth'][i] = coords[2]
             }
         }
     } else {
-        if (useGPU) {
-            multiplyMultiMatrix.setOutput([x_hp[0].length, x_hp.length, 3]);
-        }
+        multiplyMultiMatrix.setOutput([x_hp[0].length, x_hp.length, 3]);
         const coords = applyHealpixRotations(x_hp, y_hp, z_hp, centerCodecl, centerRA, orient, npoleCoords1)
         for (let i = 0; i < x_hp.length; i++) {
             for (let j = 0; j < x_hp[i].length; j++) {
                 if ('x_orth' in data) {
                     data['x_orth'][i][j] = coords[0][i][j]
                 }
                 if ('y_orth' in data) {
```

### Comparing `uranography-0.1.0/uranography/js/update.js` & `uranography-0.1.0a0/uranography/js/update.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/js/update_map.js` & `uranography-0.1.0a0/uranography/js/update_map.js`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/mollweide.py` & `uranography-0.1.0a0/uranography/mollweide.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/planisphere.py` & `uranography-0.1.0a0/uranography/planisphere.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/readjs.py` & `uranography-0.1.0a0/uranography/readjs.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/sphere.py` & `uranography-0.1.0a0/uranography/sphere.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/spheremap.py` & `uranography-0.1.0a0/uranography/spheremap.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography/stars.py` & `uranography-0.1.0a0/uranography/stars.py`

 * *Files identical despite different names*

### Comparing `uranography-0.1.0/uranography.egg-info/SOURCES.txt` & `uranography-0.1.0a0/uranography.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 setup.cfg
 test-requirements.txt
 .github/workflows/build.yaml
 .github/workflows/build_docs.yaml
 .github/workflows/python_tests.yaml
 docs/Makefile
+docs/README.md
 docs/api.rst
 docs/architecture.rst
 docs/asphere.html
 docs/conf.py
 docs/documenteer.toml
 docs/index.rst
 docs/installation.rst
```

