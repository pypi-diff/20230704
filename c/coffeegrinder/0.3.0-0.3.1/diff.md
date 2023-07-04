# Comparing `tmp/coffeegrinder-0.3.0.tar.gz` & `tmp/coffeegrinder-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeegrinder-0.3.0.tar", last modified: Mon Jul  3 10:23:31 2023, max compression
+gzip compressed data, was "coffeegrinder-0.3.1.tar", last modified: Tue Jul  4 06:34:06 2023, max compression
```

## Comparing `coffeegrinder-0.3.0.tar` & `coffeegrinder-0.3.1.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.732088 coffeegrinder-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/scripts/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.732088 coffeegrinder-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/src/coffee/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/DEPENDENCIES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/src/coffee/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/actions/gp_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/actions/hdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/actions/mpl_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/src/coffee/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.736088 coffeegrinder-0.3.0/src/coffee/diffop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/fd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/diffop/sbp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/sbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/sbp/dissipation.py
--rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/sbp/dissipation_testing.nb
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/diffop/sbp/sbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/free_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/ibvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/io/simulation_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/mpi/mpiinterfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/solvers/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffee/tslices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/tslices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/src/coffee/tslices/tslices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 10:23:31.000000 coffeegrinder-0.3.0/src/coffeegrinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.732088 coffeegrinder-0.3.0/systems/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.740088 coffeegrinder-0.3.0/systems/OneDAdvection_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/systems/OneDAdvection_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/OneDAdvection_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:23:31.744088 coffeegrinder-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-03 10:23:21.000000 coffeegrinder-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.239023 coffeegrinder-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.247022 coffeegrinder-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/scripts/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.243023 coffeegrinder-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/src/coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/hdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/mpl_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/diffop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/diffop/sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation_testing.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/sbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/free_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/ibvp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/io/simulation_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/mpi/mpiinterfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/tslices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/tslices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/tslices/tslices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:34:05.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.243023 coffeegrinder-0.3.1/systems/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvection_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tox.ini
```

### Comparing `coffeegrinder-0.3.0/.coveragerc` & `coffeegrinder-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/.github/workflows/python-publish.yml` & `coffeegrinder-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/.gitignore` & `coffeegrinder-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/.readthedocs.yml` & `coffeegrinder-0.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/CONTRIBUTING.rst` & `coffeegrinder-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/LICENSE.txt` & `coffeegrinder-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/PKG-INFO` & `coffeegrinder-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.3.0
+Version: 0.3.1
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -59,17 +59,20 @@
 
 
 Installation
 ------------
 
 There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-    pip install coffeegrinder  
-    pip install coffeegrinder[MPI]  
-    pip install coffeegrinder[JAX]  
+    pip install coffeegrinder
+
+    pip install coffeegrinder[MPI]
+
+    pip install coffeegrinder[JAX]
+
     pip install coffeegrinder[MPI-JAX]
 
 Getting started
 ---------------
 
 There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
```

### Comparing `coffeegrinder-0.3.0/README.rst` & `coffeegrinder-0.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,20 @@
 
 
 Installation
 ------------
 
 There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-    pip install coffeegrinder  
-    pip install coffeegrinder[MPI]  
-    pip install coffeegrinder[JAX]  
+    pip install coffeegrinder
+
+    pip install coffeegrinder[MPI]
+
+    pip install coffeegrinder[JAX]
+
     pip install coffeegrinder[MPI-JAX]
 
 Getting started
 ---------------
 
 There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
```

### Comparing `coffeegrinder-0.3.0/docs/Makefile` & `coffeegrinder-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/docs/conf.py` & `coffeegrinder-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/docs/index.rst` & `coffeegrinder-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/scripts/compare.py` & `coffeegrinder-0.3.1/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/setup.cfg` & `coffeegrinder-0.3.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy
 	h5py
 	scipy
-	PyGnuplot
 	matplotlib
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `coffeegrinder-0.3.0/setup.py` & `coffeegrinder-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/__init__.py` & `coffeegrinder-0.3.1/src/coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/actions/actions.py` & `coffeegrinder-0.3.1/src/coffee/actions/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from builtins import object
-from coffee.backend import backend as be
+from coffee.settings import be
 
 
 class Prototype(object):
     """The prototype of all actions.
 
     This class provides basic functionality that all actions require.
```

### Comparing `coffeegrinder-0.3.0/src/coffee/actions/hdf_output.py` & `coffeegrinder-0.3.1/src/coffee/actions/hdf_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 I think of this method as a plugin for the system. The user writes a new output
 method for some kind of new data type in a sub class of SimOutputType and
 'plugs' this method into the 'action' list of SimOutput.
 """
 from builtins import str
 from builtins import object
-from coffee.backend import backend as be
+from coffee.settings import be
 
 from .actions import Prototype
 from ..io.simulation_data import dgTypes, systemD, DataGroup, sysDTypes
 from functools import reduce
 
 
 # A utility class to write to SimulationHDF via the
```

### Comparing `coffeegrinder-0.3.0/src/coffee/actions/mpl_plotter.py` & `coffeegrinder-0.3.1/src/coffee/actions/mpl_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from builtins import range
 import time
 
 # from pylab import *
 import pylab
-from coffee.backend import backend as be
+from coffee.settings import be
 
 from coffee.actions import Prototype
 
 
 class Plotter(Prototype):
     """An action that plots data using matplotlib."""
```

### Comparing `coffeegrinder-0.3.0/src/coffee/backend/backend.py` & `coffeegrinder-0.3.1/src/coffee/backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 """
-Methods that wrap common computations
+Methods that wrap common computations.
 """
 
-
 class Backend:
     def __init__(self):
         self.backend_name = None
-        self._backend = None
+        self.backend = None
 
     def set_backend(self, backend_name="numpy"):
         self.backend_name = backend_name
-        self._backend = self._get_backend(backend_name)
+        self.backend = self.get_backend(backend_name)
+
+        # Set constants
+        self.pi = self.backend.pi
 
-    def _get_backend(self, backend_name):
+        # Return backend instance
+        return self.backend
+
+    def get_backend(self, backend_name):
         """
         Returns an instance of the specified backend class.
 
         This function creates and returns an instance of the backend class specified by the
         `backend_name` argument. Currently supported backends are "numpy" and others can be
         added as needed.
 
@@ -40,135 +45,141 @@
 
         if backend_name not in backends:
             raise ValueError(f"Unsupported backend: {backend_name}")
 
         return backends[backend_name]()
 
     def abs(self, *args, **kwargs):
-        return self._backend.abs(*args, **kwargs)
+        return self.backend.abs(*args, **kwargs)
 
     def absolute(self, *args, **kwargs):
-        return self._backend.absolute(*args, **kwargs)
+        return self.backend.absolute(*args, **kwargs)
 
     def any(self, *args, **kwargs):
-        return self._backend.any(*args, **kwargs)
+        return self.backend.any(*args, **kwargs)
 
     def apply_along_axis(self, *args, **kwargs):
-        return self._backend.apply_along_axis(*args, **kwargs)
+        return self.backend.apply_along_axis(*args, **kwargs)
 
     def apply_over_axes(self, *args, **kwargs):
-        return self._backend.apply_over_axes(*args, **kwargs)
+        return self.backend.apply_over_axes(*args, **kwargs)
 
     def arange(self, *args, **kwargs):
-        return self._backend.arange(*args, **kwargs)
+        return self.backend.arange(*args, **kwargs)
 
     def array(self, *args, **kwargs):
-        return self._backend.array(*args, **kwargs)
+        return self.backend.array(*args, **kwargs)
 
     def array_equal(self, *args, **kwargs):
-        return self._backend.array_equal(*args, **kwargs)
+        return self.backend.array_equal(*args, **kwargs)
 
     def asarray(self, *args, **kwargs):
-        return self._backend.asarray(*args, **kwargs)
+        return self.backend.asarray(*args, **kwargs)
 
     def atleast_1d(self, *args, **kwargs):
-        return self._backend.atleast_1d(*args, **kwargs)
+        return self.backend.atleast_1d(*args, **kwargs)
 
     def atleast_2d(self, *args, **kwargs):
-        return self._backend.atleast_2d(*args, **kwargs)
+        return self.backend.atleast_2d(*args, **kwargs)
 
     def convolve(self, *args, **kwargs):
-        return self._backend.convolve(*args, **kwargs)
+        return self.backend.convolve(*args, **kwargs)
+    
+    def cos(self, *args, **kwargs):
+        return self.backend.cos(*args, **kwargs)
 
     def diag(self, *args, **kwargs):
-        return self._backend.diag(*args, **kwargs)
+        return self.backend.diag(*args, **kwargs)
 
     def dot(self, *args, **kwargs):
-        return self._backend.dot(*args, **kwargs)
+        return self.backend.dot(*args, **kwargs)
 
     def dtype(self, *args, **kwargs):
-        return self._backend.dtype(*args, **kwargs)
+        return self.backend.dtype(*args, **kwargs)
 
     def empty(self, *args, **kwargs):
-        return self._backend.empty(*args, **kwargs)
+        return self.backend.empty(*args, **kwargs)
 
     def empty_like(self, *args, **kwargs):
-        return self._backend.empty_like(*args, **kwargs)
+        return self.backend.empty_like(*args, **kwargs)
 
     def exp(self, *args, **kwargs):
-        return self._backend.exp(*args, **kwargs)
+        return self.backend.exp(*args, **kwargs)
 
     def fromiter(self, *args, **kwargs):
-        return self._backend.fromiter(*args, **kwargs)
+        return self.backend.fromiter(*args, **kwargs)
 
     def lib_stride_tricks_as_strided(self, *args, **kwargs):
-        return self._backend.lib_stride_tricks_as_strided(*args, **kwargs)
+        return self.backend.lib_stride_tricks_as_strided(*args, **kwargs)
 
     def linspace(self, *args, **kwargs):
-        return self._backend.linspace(*args, **kwargs)
+        return self.backend.linspace(*args, **kwargs)
 
     def log(self, *args, **kwargs):
-        return self._backend.log(*args, **kwargs)
+        return self.backend.log(*args, **kwargs)
 
     def log2(self, *args, **kwargs):
-        return self._backend.log2(*args, **kwargs)
+        return self.backend.log2(*args, **kwargs)
 
     def mat(self, *args, **kwargs):
-        return self._backend.mat(*args, **kwargs)
+        return self.backend.mat(*args, **kwargs)
 
     def max(self, *args, **kwargs):
-        return self._backend.max(*args, **kwargs)
+        return self.backend.max(*args, **kwargs)
 
     def min(self, *args, **kwargs):
-        return self._backend.min(*args, **kwargs)
+        return self.backend.min(*args, **kwargs)
 
     def ndarray(self, *args, **kwargs):
-        return self._backend.ndarray(*args, **kwargs)
+        return self.backend.ndarray(*args, **kwargs)
 
     def nonzero(self, *args, **kwargs):
-        return self._backend.nonzero(*args, **kwargs)
+        return self.backend.nonzero(*args, **kwargs)
 
     def ones(self, *args, **kwargs):
-        return self._backend.ones(*args, **kwargs)
+        return self.backend.ones(*args, **kwargs)
 
     def ones_like(self, *args, **kwargs):
-        return self._backend.ones_like(*args, **kwargs)
+        return self.backend.ones_like(*args, **kwargs)
 
     def power(self, *args, **kwargs):
-        return self._backend.power(*args, **kwargs)
+        return self.backend.power(*args, **kwargs)
 
     def savetxt(self, *args, **kwargs):
-        return self._backend.savetxt(*args, **kwargs)
+        return self.backend.savetxt(*args, **kwargs)
 
     def set_printoptions(self, *args, **kwargs):
-        return self._backend.set_printoptions(*args, **kwargs)
+        return self.backend.set_printoptions(*args, **kwargs)
+    
+    def sin(self, *args, **kwargs):
+        return self.backend.sin(*args, **kwargs)
 
     def squeeze(self, *args, **kwargs):
-        return self._backend.squeeze(*args, **kwargs)
+        return self.backend.squeeze(*args, **kwargs)
 
     def sum(self, *args, **kwargs):
-        return self._backend.sum(*args, **kwargs)
+        return self.backend.sum(*args, **kwargs)
 
     def tan(self, *args, **kwargs):
-        return self._backend.tan(*args, **kwargs)
+        return self.backend.tan(*args, **kwargs)
 
     def union1d(self, *args, **kwargs):
-        return self._backend.union1d(*args, **kwargs)
+        return self.backend.union1d(*args, **kwargs)
 
     def vectorize(self, *args, **kwargs):
-        return self._backend.vectorize(*args, **kwargs)
+        return self.backend.vectorize(*args, **kwargs)
 
     def where(self, *args, **kwargs):
-        return self._backend.where(*args, **kwargs)
+        return self.backend.where(*args, **kwargs)
 
     def zeros(self, *args, **kwargs):
-        return self._backend.zeros(*args, **kwargs)
+        return self.backend.zeros(*args, **kwargs)
 
     def zeros_like(self, *args, **kwargs):
-        return self._backend.zeros_like(*args, **kwargs)
+        return self.backend.zeros_like(*args, **kwargs)
 
 
 class BackendBase:
     def __init__(self):
         pass
 
 
@@ -185,14 +196,17 @@
         except ImportError:
             raise ImportError(
                 "NumPy library is not installed. Please install NumPy to use this function."
             )
 
         self.np = np
 
+        # Constants
+        self.pi = np.pi
+
     def abs(self, *args, **kwargs):
         return self.np.abs(*args, **kwargs)
 
     def absolute(self, *args, **kwargs):
         return self.np.absolute(*args, **kwargs)
 
     def any(self, *args, **kwargs):
@@ -220,14 +234,17 @@
         return self.np.atleast_1d(*args, **kwargs)
 
     def atleast_2d(self, *args, **kwargs):
         return self.np.atleast_2d(*args, **kwargs)
 
     def convolve(self, *args, **kwargs):
         return self.np.convolve(*args, **kwargs)
+    
+    def cos(self, *args, **kwargs):
+        return self.np.cos(*args, **kwargs)
 
     def diag(self, *args, **kwargs):
         return self.np.diag(*args, **kwargs)
 
     def dot(self, *args, **kwargs):
         return self.np.dot(*args, **kwargs)
 
@@ -283,14 +300,17 @@
         return self.np.power(*args, **kwargs)
 
     def savetxt(self, *args, **kwargs):
         return self.np.savetxt(*args, **kwargs)
 
     def set_printoptions(self, *args, **kwargs):
         return self.np.set_printoptions(*args, **kwargs)
+    
+    def sin(self, *args, **kwargs):
+        return self.np.sin(*args, **kwargs)
 
     def squeeze(self, *args, **kwargs):
         return self.np.squeeze(*args, **kwargs)
 
     def sum(self, *args, **kwargs):
         return self.np.sum(*args, **kwargs)
```

### Comparing `coffeegrinder-0.3.0/src/coffee/diffop/fd.py` & `coffeegrinder-0.3.1/src/coffee/diffop/fd.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Stencil values are calculated using Fornberg's paper. Code for the
 calculations is available in
 `finite_difference_weights_generator.py` located in Code/Utils.
 See Fornberg's paper for the notation.
 """
 
 from builtins import object
-from coffee.backend import backend as be
+from coffee.settings import be
 
 ################################################################################
 # Finite difference default ghost point processor
 ################################################################################
 def ghost_point_processor(data, b_values):
     """A utility function that understands how data defined over ghost points
     for finite difference stencils should be handled when communicated via MPI."""
```

### Comparing `coffeegrinder-0.3.0/src/coffee/diffop/sbp/dissipation.py` & `coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/diffop/sbp/dissipation_testing.nb` & `coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation_testing.nb`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/diffop/sbp/sbp.py` & `coffeegrinder-0.3.1/src/coffee/diffop/sbp/sbp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # encoding: utf-8
 """
 A module to manage summation by parts finite difference operators.
 """
 
 import math
 import logging
-from coffee.backend import backend as be
+from coffee.settings import be
 
 ################################################################################
 # Base class for SBP operators
 ################################################################################
 BOUNDARY_TYPE_SAT = 0
 """Specifies that the simulataneous approximation term method will be used
 for boundaries."""
```

### Comparing `coffeegrinder-0.3.0/src/coffee/free_data.py` & `coffeegrinder-0.3.1/src/coffee/free_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/grid/grid.py` & `coffeegrinder-0.3.1/src/coffee/grid/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import abc
 
 try:
     from coffee.mpi import mpiinterfaces
 except ModuleNotFoundError:
     pass
 
-from coffee.backend import backend as be
+from coffee.settings import be
 
 ################################################################################
 # Base Boundary data class
 ################################################################################
 class ABCBoundary(object, metaclass=abc.ABCMeta):
     """The abstract base class for boundary classes.
```

### Comparing `coffeegrinder-0.3.0/src/coffee/ibvp.py` & `coffeegrinder-0.3.1/src/coffee/ibvp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/io/simulation_data.py` & `coffeegrinder-0.3.1/src/coffee/io/simulation_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,15 @@
 from builtins import zip
 from builtins import map
 from builtins import str
 from builtins import range
 from builtins import object
 import functools
 import h5py
-from coffee.backend import backend as be
-
-# Gnuplot currently only works with Python 2!
-try:
-    import Gnuplot
-except ImportError:
-    pass
+from coffee.settings import be
 
 NUMERICAL_TOLERANCE = 1e-14
 # Important configuration is included after these two classes
 
 
 # A wrapper class that helps ease iteration over datasets with
 # str(int) indices going from 0,1,... upwards.
@@ -488,168 +482,14 @@
 
         Returns
         =======
         DataGroup :
         """
         return self.simHDF.getDgTypeAttr(dgType, attr, i, self.name)
 
-    def animate(
-        self,
-        dgType="raw",
-        gnuCommands=None,
-        gnuInitialisationCommands={"debug": 0, "persist": 1},
-        tstart=-float("Infinity"),
-        tstop=float("Infinity"),
-        animationLength=2,
-        framesPerSec=60,
-    ):
-        """A utility method that provide nice defaults for the GNUplot method.
-
-        Parameters
-        ==========
-        dgType : string
-            A key of the dbTypes dictionary. The type of data to be displayed.
-        gnuCommands : list of strings, Optional
-            A list of string commands for GnuPlot.
-        gnuInitialisationCommands : list of strings, Optional
-            A list of string commands to be parsed to GnuPlot on initialisation.
-        tstart : float, Optional
-            The time at which to start plotting data.
-        tstop : float, Optional
-            The time at which to stop plotting data.
-        animationLength : float
-            The length of time of the animation.
-        framesPerSec : int
-            The number of frames per second of display.
-        """
-        self.GNUplot(
-            self.getDgType(dgType),
-            gnuCommands=gnuCommands,
-            gnuInitialisationCommands=gnuInitialisationCommands,
-            tstart=tstart,
-            tstop=tstop,
-            animationLength=animationLength,
-            framesPerSec=framesPerSec,
-        )
-
-    def plot(
-        self,
-        time,
-        dgType="raw",
-        gnuCommands=None,
-        gnuInitialisationCommands={"debug": 0, "persist": 1},
-    ):
-        """A utility that plots the data at a particular time.
-
-        This is a wrapper to the animate method that gives the same
-        start and stop times.
-
-        Parameters
-        ==========
-        time : float
-            The time of the data that should be plotted.
-        dgType : string, Optinal
-            A key of the dgTypes dictionary.
-        gnuCommands : list of strings
-            Commands to be parsed to GnuPlot when the data is plotted.
-        gnuInitialisationCommands : list of strings
-            Commands to be parsed to GnuPlot on initialisation.
-        """
-        self.animate(
-            dgType=dgType,
-            gnuCommands=gnuCommands,
-            gnuInitialisationCommands=gnuInitialisationCommands,
-            tstart=time,
-            tstop=time,
-        )
-
-    def GNUplot(
-        self,
-        group,
-        gnuCommands=None,
-        gnuInitialisationCommands=None,
-        tstart=-float("Infinity"),
-        tstop=float("Infinity"),
-        animationLength=2,
-        framesPerSec=60,
-    ):
-        """A utility function which plots a given group.
-
-        There is no return, but gnuplot is called hence, depending on what
-        parameters are parsed, plots will be created.
-
-        Parameters
-        ==========
-        group : DataGroup
-            A DataGroup containing the data to be plotted.
-        gnuCommands : list of strings, Optional
-            A list of string commands for GnuPlot.
-        gnuInitialisationCommands : list of strings, Optional
-            A list of string commands to be parsed to GnuPlot on initialisation.
-        tstart : float, Optional
-            The time at which to start plotting data.
-        tstop : float, Optional
-            The time at which to stop plotting data.
-        animationLength : float
-            The length of time of the animation.
-        framesPerSec : int
-            The number of frames per second of display.
-        """
-        if gnuCommands is None:
-            gnuCommands = []
-        if gnuInitialisationCommands is None:
-            gnuInitialisationCommands = []
-
-        # Get x values
-        domains = self.getDgType("domain")
-
-        # Get all times
-        times = self.getDgType("time")
-        times.rV = True
-        numOfFrames = len(times)
-        frameSkip = int(numOfFrames / (animationLength * framesPerSec))
-
-        # Get data for scri
-        scrif = self.getDgType("scrif")
-        scrif.rV = True
-
-        # Initialize gnuplot
-        gnu = Gnuplot.Gnuplot(**gnuInitialisationCommands)
-        gnu.reset()
-        for command in gnuCommands:
-            gnu(command)
-
-        # Iterate across group
-        # Get starting and stoping index
-        nextFrame_index = self.indexOfTime(tstart)
-        stop_index = self.indexOfTime(tstop)
-
-        # While there is a next frame...
-        while nextFrame_index < numOfFrames:
-            # plot data
-            i = nextFrame_index
-            y = group[i]
-            gnu.title("Simulation %s at time %f" % (self.name, times[i]))
-            plotItems = []
-            for j, row in enumerate(be.atleast_2d(y[()])):
-                plotItems += [
-                    Gnuplot.Data(domains[i], row, title="Component " + str(j))
-                ]
-            plotItems += [Gnuplot.Data(domains[i], scrif[i], title="Scri+")]
-            gnu.plot(*plotItems)
-            # if there are not enough frames left set the frameSkip to 0
-            if nextFrame_index + frameSkip >= numOfFrames:
-                frameSkip = 0
-            nextFrame_index += 1 + frameSkip
-            # if the next frame is larger than the stop_index then stop
-            # plotting
-            if nextFrame_index > stop_index:
-                break
-        gnu.close()
-
     class dsReturnValue(object):
         def __init__(self, dataset):
             self.ds = dataset
 
         def __getitem__(self, key):
             return self.ds[key][()]
```

### Comparing `coffeegrinder-0.3.0/src/coffee/mpi/mpiinterfaces.py` & `coffeegrinder-0.3.1/src/coffee/mpi/mpiinterfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Classes in this module model the MPI node network and manage the relationship
 of the complete domain to each 
 """
 from builtins import range
 from builtins import object
 import abc
-from coffee.backend import backend as be
+from coffee.settings import be
 
 
 ###############################################################################
 # Abstract Base Class for MPI Interfaces
 ###############################################################################
 class MPIInterface(object, metaclass=abc.ABCMeta):
     def __init__(self, mpi_comm, *args, **kwds):
```

### Comparing `coffeegrinder-0.3.0/src/coffee/solvers/solvers.py` & `coffeegrinder-0.3.1/src/coffee/solvers/solvers.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/system.py` & `coffeegrinder-0.3.1/src/coffee/system.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/src/coffee/tslices/tslices.py` & `coffeegrinder-0.3.1/src/coffee/tslices/tslices.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 TimeSlice objects should contain all information needed to interperet the
 values of the functions being numerically evolved. In particular, aim to ensure
 that you can restart a simulation if given a timeslice, system and solver.
 """
 
 from builtins import object
 import abc
-from coffee.backend import backend as be
+from coffee.settings import be
 
 ###############################################################################
 # TimeSlice Abstract Base Class
 ##############################################################################
 class ABCTimeSlice(object, metaclass=abc.ABCMeta):
     """The abstract base class for TimeSlice objects.
```

### Comparing `coffeegrinder-0.3.0/src/coffeegrinder.egg-info/PKG-INFO` & `coffeegrinder-0.3.1/src/coffeegrinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.3.0
+Version: 0.3.1
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -59,17 +59,20 @@
 
 
 Installation
 ------------
 
 There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-    pip install coffeegrinder  
-    pip install coffeegrinder[MPI]  
-    pip install coffeegrinder[JAX]  
+    pip install coffeegrinder
+
+    pip install coffeegrinder[MPI]
+
+    pip install coffeegrinder[JAX]
+
     pip install coffeegrinder[MPI-JAX]
 
 Getting started
 ---------------
 
 There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
```

### Comparing `coffeegrinder-0.3.0/src/coffeegrinder.egg-info/SOURCES.txt` & `coffeegrinder-0.3.1/src/coffeegrinder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,21 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 scripts/compare.py
-src/coffee/DEPENDENCIES.txt
 src/coffee/__init__.py
 src/coffee/free_data.py
 src/coffee/ibvp.py
+src/coffee/settings.py
 src/coffee/system.py
 src/coffee/actions/__init__.py
 src/coffee/actions/actions.py
-src/coffee/actions/gp_plotter.py
 src/coffee/actions/hdf_output.py
 src/coffee/actions/mpl_plotter.py
 src/coffee/backend/__init__.py
 src/coffee/backend/backend.py
 src/coffee/diffop/__init__.py
 src/coffee/diffop/fd.py
 src/coffee/diffop/sbp/__init__.py
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 """
 OneDAdvection.py
 
 Created by Chris Stevens 2023
 """
 
 # Import Python libraries
-import numpy as np
-
+from coffee.settings import be
 from coffee.system import System
 from coffee.tslices import tslices
 from coffee.diffop.fd import ghost_point_processor
 from functools import partial
 
 # A simple bump function for the boundary condition
 def bump(t):
-	return np.sin(8.*t)**7.
+	return be.sin(8.*t)**7.
 
 # Class that describes a simple advection equation
 class OneDAdvection(System):
 
 	############################################################################
 	# Constructor
 	############################################################################
@@ -64,15 +63,15 @@
 
 		# Calculate spatial derivative
 		DxPsi = self.D(Psi, dx)
 
 		# Communicate spatial derivative through neighbouring MPI process(es)
 		new_derivatives, _ = U.communicate(
 			partial(ghost_point_processor),
-			data=np.array([
+			data=be.array([
 				DxPsi
 			])
 		)
 		DxPsi = new_derivatives[0]
 
 		# Evaluate right hand side
 		DtPsi = -self.char_speed*DxPsi
@@ -87,15 +86,15 @@
 	# Initial Data Routine
 	############################################################################
 
 	def initial_data(self, t0, grid):
 
 		# Set initial data
 		x   = grid.meshes[0]
-		Psi = np.zeros_like(x)
+		Psi = be.zeros_like(x)
 
 		# Return Timeslice object
 		return tslices.TimeSlice([Psi], grid, time = t0)
 
 	############################################################################
 	# Timestep Routine
 	############################################################################
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 import sys
 import os
 import numpy as np
 import h5py
 import argparse
 from mpi4py import MPI
 
-# Import standard code base
+# Import standard code base and initialize NumPy backend
+from coffee.settings import init
 from coffee.backend import backend as be
-be.set_backend("numpy")
+my_backend = be.set_backend("numpy")
+init(my_backend)
 
 from coffee import ibvp, actions, solvers, grid
 from coffee.diffop import fd
 
 # Import system to use
 import OneDAdvection
 import OneDAdvection_plotter as plotter
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 """
 OneDAdvection.py
 
 Created by Chris Stevens 2023
 """
 
 # Import Python libraries
-import numpy as np
 from functools import partial
 
+from coffee.settings import be
 from coffee.tslices import tslices
 from coffee.system import System
 from coffee.diffop.fd import ghost_point_processor
 
 # A simple bump function for the boundary condition
 def bump(t):
-	return np.sin(8.*t)**7.
+	return be.sin(8.*t)**7.
 
 # Class that describes a simple advection equation
 class OneDAdvection(System):
 
 	################################
 	# Constructor
 	################################
@@ -56,15 +56,15 @@
 
 		# Calculate spatial derivative
 		DxPsi = self.D(Psi, dx)
 
 		# Communicate spatial derivative through neighbouring MPI process(es)
 		new_derivatives, _ = U.communicate(
 			partial(ghost_point_processor),
-			data=np.array([
+			data=be.array([
 				DxPsi
 			])
 		)
 		DxPsi = new_derivatives[0]
 
 		# Evaluate right hand side
 		DtPsi = -self.char_speed*DxPsi
@@ -92,15 +92,15 @@
 	# Initial Data Routine
 	############################################################################
 
 	def initial_data(self, t0, grid):
 
 		# Set initial data
 		x   = grid.meshes[0]
-		Psi = np.zeros_like(x)
+		Psi = be.zeros_like(x)
 
 		# Return Timeslice object
 		return tslices.TimeSlice([Psi], grid, time = t0)
 
 	############################################################################
 	# Timestep Routine
 	############################################################################
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 import sys
 import os
 import numpy as np
 import h5py
 import argparse
 from mpi4py import MPI
 
-# Import standard code base
+# Import standard code base and initialize NumPy backend
+from coffee.settings import init
 from coffee.backend import backend as be
-be.set_backend("numpy")
+my_backend = be.set_backend("numpy")
+init(my_backend)
 
 from coffee import ibvp, actions, solvers, grid
 from coffee.diffop.sbp import sbp
 
 # Import system to use
 import OneDAdvection
 import OneDAdvection_plotter as plotter
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 """
 OneDAdvection.py
 
 Created by Chris Stevens 2023
 """
 
 # Import Python libraries
-import numpy as np
-
+from coffee.settings import be
 from coffee.tslices import tslices
 from coffee.system import System
 
 # A simple bump function for the boundary condition
 def bump(t):
-	return np.sin(8.*t)**7.
+	return be.sin(8.*t)**7.
 
 # Class that describes a simple advection equation
 class OneDAdvection(System):
 
 	############################################################################
 	# Constructor
 	############################################################################
@@ -73,15 +72,15 @@
 	# Initial Data Routine
 	############################################################################
 
 	def initial_data(self, t0, grid):
 
 		# Set initial data
 		x   = grid.meshes[0]
-		Psi = np.zeros_like(x)
+		Psi = be.zeros_like(x)
 
 		# Return Timeslice object
 		return tslices.TimeSlice([Psi], grid, time = t0)
 
 	############################################################################
 	# Timestep Routine
 	############################################################################
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_fd/OneDAdvection_setup.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from builtins import range
 import sys
 import os
 import numpy as np
 import h5py
 import argparse
 
-# Import standard code base
+# Import standard code base and initialize NumPy backend
+from coffee.settings import init
 from coffee.backend import backend as be
-be.set_backend("numpy")
+my_backend = be.set_backend("numpy")
+init(my_backend)
 
 from coffee import ibvp, actions, solvers, grid
 from coffee.diffop import fd
 
 # Import system to use
 import OneDAdvection
 import OneDAdvection_plotter as plotter
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 """
 OneDAdvection.py
 
 Created by Chris Stevens 2023
 """
 
 # Import Python libraries
-import numpy as np
-
+from coffee.settings import be
 from coffee.tslices import tslices
 from coffee.system import System
 
 # A simple bump function for the boundary condition
 def bump(t):
-	return np.sin(8.*t)**7.
+	return be.sin(8.*t)**7.
 
 # Class that describes a simple advection equation
 class OneDAdvection(System):
 
 	############################################################################
 	# Constructor
 	############################################################################
@@ -74,15 +73,15 @@
 	# Initial Data Routine
 	############################################################################
 	
 	def initial_data(self, t0, grid):
 
 		# Set initial data
 		x   = grid.meshes[0]
-		Psi = np.zeros_like(x)
+		Psi = be.zeros_like(x)
 
 		# Return Timeslice object
 		return tslices.TimeSlice([Psi], grid, time = t0)
 
 	############################################################################
 	# Timestep Routine
 	############################################################################
```

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/systems/OneDAdvection_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from builtins import range
 import sys
 import os
 import numpy as np
 import h5py
 import argparse
 
-# Import standard code base
+# Import standard code base and initialize NumPy backend
+from coffee.settings import init
 from coffee.backend import backend as be
-be.set_backend("numpy")
+my_backend = be.set_backend("numpy")
+init(my_backend)
 
 from coffee import ibvp, actions, solvers, grid
 from coffee.diffop.sbp import sbp
 
 # Import system to use
 import OneDAdvection
 import OneDAdvection_plotter as plotter
```

### Comparing `coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py` & `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,158 @@
 """
 TwoDAdvection.py
 
 Created by Chris Stevens 2023
 """
 
 # Import Python libraries
+from functools import partial
+
+from coffee.settings import be
+from coffee.tslices import tslices
+from coffee.system import System
+from coffee.diffop.fd import ghost_point_processor
+
+# A simple bump function for the boundary condition
+def bump(t, grid, grid_global):
+	start = grid_global[0]
+	stop  = grid_global[-1]
+	return be.sin(be.pi*start / (start - stop) - \
+	       be.pi / (start - stop)*grid)**8.* \
+		   be.sin(8.*t)**7.
+
+# Class that describes a simple advection equation
+class TwoDAdvection(System):
+
+	################################
+	# Constructor
+	################################
+
+	def __init__(self, Dx, Dy, tau, CFL, char_speed_x, char_speed_y, \
+	      		x_global, y_global):
+		super(TwoDAdvection, self).__init__()
+		self.Dx           = Dx
+		self.Dy           = Dy
+		self.tau          = tau
+		self.CFL          = CFL
+		self.char_speed_x = char_speed_x
+		self.char_speed_y = char_speed_y
+		self.x_global     = x_global
+		self.y_global     = y_global
+		self.name         = "2D Advection equation"
+		self.numvar       = 1
+
+	############################################################################
+	# Boundary functions
+	############################################################################
+		
+	# Left x boundary condition
+	def left_x(self, t, y, y_global):
+		return bump(t, y, y_global)
+	
+	# Left y boundary condition
+	def left_y(self, t, x, x_global):
+		return bump(t, x, x_global)
+
+	############################################################################
+	# Evolution Routine
+	############################################################################
+
+	def evaluate(self, t, U, intStep = None):
+
+		# Define useful variables
+		Psi = U.data[0]
+		x   = U.domain.axes[0]
+		y   = U.domain.axes[1]
+		dx  = U.domain.step_sizes[0]
+		dy  = U.domain.step_sizes[1]
+
+		# Calculate spatial derivatives by applying the 1D FD operators
+		# over the mesh
+		DxPsi = be.apply_along_axis(
+			lambda f:self.Dx(f, dx),
+			0, 
+			Psi
+			)
+		DyPsi = be.apply_along_axis(
+			lambda f:self.Dy(f, dy),
+			1, 
+			Psi
+			)
+
+		# Communicate spatial derivative through neighbouring MPI process(es)
+		new_derivatives, _ = U.communicate(
+			partial(ghost_point_processor),
+			data=be.array([
+				DxPsi, DyPsi
+			])
+		)
+		DxPsi, DyPsi = new_derivatives
+
+		# Impose boundary conditions with SAT method
+		pt_x_l = self.Dx.penalty_boundary(dx, "left")
+		pt_y_l = self.Dy.penalty_boundary(dy, "left")
+	
+		# Only two of the four boundaries require boundary conditions
+		C_x_left     = self.tau * pt_x_l * (-self.char_speed_x)
+		l_x_Psi      = self.left_x(t, y, self.y_global)
+		C_y_left     = self.tau * pt_y_l * (-self.char_speed_y)
+		l_y_Psi      = self.left_y(t, x, self.x_global)
+
+		# Evaluate right hand side
+		DtPsi = -self.char_speed_x*DxPsi - self.char_speed_y*DyPsi
+
+		# Do the external boundaries
+		b_data = U.external_slices()
+		for dim, direction, _ in b_data:
+			if dim == 0 and direction == -1: # Left x boundary)
+				DtPsi[0,:] -= C_x_left * \
+					(Psi[0,:] - l_x_Psi)
+			elif dim == 1 and direction == -1: # Left y boundary
+				DtPsi[:,0] -= C_y_left * \
+					(Psi[:,0] - l_y_Psi)
+
+		# # Output time if desired
+		# print('t =', t)
+
+		# Return RHS of evolution equation with SAT boundary condition imposed
+		return tslices.TimeSlice([DtPsi], U.domain, time = t)
+
+	############################################################################
+	# Initial Data Routine
+	############################################################################
+
+	def initial_data(self, t0, grid):
+
+		# Set initial data
+		x   = grid.meshes[0]
+		Psi = be.zeros_like(x)
+
+		# Return Timeslice object
+		return tslices.TimeSlice([Psi], grid, time = t0)
+
+	############################################################################
+	# Timestep Routine
+	############################################################################
+
+	def timestep(self, U):
+
+		return self.CFL * min(U.domain.step_sizes[0] / self.char_speed_x, \
+	  						  U.domain.step_sizes[1] / self.char_speed_y)
+#!/usr/bin/env python
+# encoding: utf-8
+
+
+"""
+TwoDAdvection.py
+
+Created by Chris Stevens 2023
+"""
+
+# Import Python libraries
 import numpy as np
 from functools import partial
 
 from coffee.tslices import tslices
 from coffee.system import System
 from coffee.diffop.fd import ghost_point_processor
```

### Comparing `coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py` & `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py` & `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 import sys
 import os
 import numpy as np
 import h5py
 import argparse
 from mpi4py import MPI
 
-# Import standard code base
+# Import standard code base and initialize NumPy backend
+from coffee.settings import init
 from coffee.backend import backend as be
-be.set_backend("numpy")
+my_backend = be.set_backend("numpy")
+init(my_backend)
 
 from coffee import ibvp, actions, solvers, grid
 from coffee.diffop.sbp import sbp
 
 # Import system to use
 import TwoDAdvection
 import TwoDAdvection_plotter as plotter
```

### Comparing `coffeegrinder-0.3.0/tests/test_actions.py` & `coffeegrinder-0.3.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/tests/test_backend.py` & `coffeegrinder-0.3.1/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.0/tox.ini` & `coffeegrinder-0.3.1/tox.ini`

 * *Files identical despite different names*

