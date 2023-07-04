# Comparing `tmp/coffeegrinder-0.3.1.tar.gz` & `tmp/coffeegrinder-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeegrinder-0.3.1.tar", last modified: Tue Jul  4 06:34:06 2023, max compression
+gzip compressed data, was "coffeegrinder-0.3.2.tar", last modified: Tue Jul  4 08:45:00 2023, max compression
```

## Comparing `coffeegrinder-0.3.1.tar` & `coffeegrinder-0.3.2.tar`

### file list

```diff
@@ -1,106 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.239023 coffeegrinder-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.247022 coffeegrinder-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/scripts/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.243023 coffeegrinder-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.251022 coffeegrinder-0.3.1/src/coffee/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/hdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/actions/mpl_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/diffop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/fd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/diffop/sbp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation.py
--rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation_testing.nb
--rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/diffop/sbp/sbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/free_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.255022 coffeegrinder-0.3.1/src/coffee/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/ibvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/io/simulation_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/mpi/mpiinterfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/solvers/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffee/tslices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/tslices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/src/coffee/tslices/tslices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.259023 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:34:05.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 06:34:06.000000 coffeegrinder-0.3.1/src/coffeegrinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.243023 coffeegrinder-0.3.1/systems/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.263023 coffeegrinder-0.3.1/systems/OneDAdvection_fd/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_fd/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/OneDAdvection_sbp/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:34:06.267022 coffeegrinder-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 06:33:47.000000 coffeegrinder-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.518721 coffeegrinder-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.522722 coffeegrinder-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/scripts/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.518721 coffeegrinder-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/actions/hdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/actions/mpl_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/diffop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/diffop/sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/sbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/sbp/dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/sbp/dissipation_testing.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/diffop/sbp/sbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/free_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/ibvp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.526722 coffeegrinder-0.3.2/src/coffee/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/io/simulation_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/src/coffee/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/mpi/mpiinterfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/src/coffee/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/src/coffee/tslices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/tslices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/src/coffee/tslices/tslices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 08:45:00.000000 coffeegrinder-0.3.2/src/coffeegrinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.522722 coffeegrinder-0.3.2/systems/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.530722 coffeegrinder-0.3.2/systems/OneDAdvection_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/systems/OneDAdvection_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/OneDAdvection_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:45:00.534722 coffeegrinder-0.3.2/tests/TwoDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/TwoDAdvectionMpi_sbp/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/TwoDAdvectionMpi_sbp/TwoDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tests/test_coffee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-04 08:44:48.000000 coffeegrinder-0.3.2/tox.ini
```

### Comparing `coffeegrinder-0.3.1/.coveragerc` & `coffeegrinder-0.3.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/.github/workflows/python-publish.yml` & `coffeegrinder-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/.gitignore` & `coffeegrinder-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/.readthedocs.yml` & `coffeegrinder-0.3.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/CONTRIBUTING.rst` & `coffeegrinder-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/LICENSE.txt` & `coffeegrinder-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/PKG-INFO` & `coffeegrinder-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.3.1
+Version: 0.3.2
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `coffeegrinder-0.3.1/README.rst` & `coffeegrinder-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/docs/Makefile` & `coffeegrinder-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/docs/conf.py` & `coffeegrinder-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/docs/index.rst` & `coffeegrinder-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/scripts/compare.py` & `coffeegrinder-0.3.2/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/setup.cfg` & `coffeegrinder-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/setup.py` & `coffeegrinder-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/__init__.py` & `coffeegrinder-0.3.2/src/coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/actions/actions.py` & `coffeegrinder-0.3.2/src/coffee/actions/actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/actions/hdf_output.py` & `coffeegrinder-0.3.2/src/coffee/actions/hdf_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,16 @@
         self.actions = actionTypes
         self.overwrite = overwrite
         self.cmp_ = cmp_
         for action in actionTypes:
             action.setup(self)
 
     def _doit(self, it, u):
-        pass
+        for action in self.actions:
+            action(it,u)
 
     class SimOutputType(object):
         """If you want to customise the output to the hdf file subclass this
         class.
 
         This class handles the organisation of the hdf file structure so that
         you don't have to. It slices, it dices, it picks the group to store the
```

### Comparing `coffeegrinder-0.3.1/src/coffee/actions/mpl_plotter.py` & `coffeegrinder-0.3.2/src/coffee/actions/mpl_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/backend/backend.py` & `coffeegrinder-0.3.2/src/coffee/backend/backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/diffop/fd.py` & `coffeegrinder-0.3.2/src/coffee/diffop/fd.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation.py` & `coffeegrinder-0.3.2/src/coffee/diffop/sbp/dissipation.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/diffop/sbp/dissipation_testing.nb` & `coffeegrinder-0.3.2/src/coffee/diffop/sbp/dissipation_testing.nb`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/diffop/sbp/sbp.py` & `coffeegrinder-0.3.2/src/coffee/diffop/sbp/sbp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/free_data.py` & `coffeegrinder-0.3.2/src/coffee/free_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/grid/grid.py` & `coffeegrinder-0.3.2/src/coffee/grid/grid.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/ibvp.py` & `coffeegrinder-0.3.2/src/coffee/ibvp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -172,8 +172,8 @@
         if tslice is not None:
             actions_do_actions = [
                 action.will_run(self.iteration, tslice) for action in self.theActions
             ]
             if any(actions_do_actions):
                 for i, action in enumerate(self.theActions):
                     if actions_do_actions[i]:
-                        action(self.iteration, tslice)
+                        action(self.iteration, tslice)
```

### Comparing `coffeegrinder-0.3.1/src/coffee/io/simulation_data.py` & `coffeegrinder-0.3.2/src/coffee/io/simulation_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/mpi/mpiinterfaces.py` & `coffeegrinder-0.3.2/src/coffee/mpi/mpiinterfaces.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/solvers/solvers.py` & `coffeegrinder-0.3.2/src/coffee/solvers/solvers.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/system.py` & `coffeegrinder-0.3.2/src/coffee/system.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffee/tslices/tslices.py` & `coffeegrinder-0.3.2/src/coffee/tslices/tslices.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/src/coffeegrinder.egg-info/PKG-INFO` & `coffeegrinder-0.3.2/src/coffeegrinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.3.1
+Version: 0.3.2
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `coffeegrinder-0.3.1/src/coffeegrinder.egg-info/SOURCES.txt` & `coffeegrinder-0.3.2/src/coffeegrinder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -73,8 +73,12 @@
 systems/OneDAdvection_sbp/README.txt
 systems/TwoDAdvectionMpi_sbp/README.txt
 systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py
 systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py
 systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
 tests/conftest.py
 tests/test_actions.py
-tests/test_backend.py
+tests/test_backend.py
+tests/test_coffee.py
+tests/TwoDAdvectionMpi_sbp/README.txt
+tests/TwoDAdvectionMpi_sbp/TwoDAdvection.py
+tests/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py
```

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.3.2/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_plotter.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_fd/OneDAdvection_setup.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_fd/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_plotter.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/OneDAdvection_sbp/OneDAdvection_setup.py` & `coffeegrinder-0.3.2/systems/OneDAdvection_sbp/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py` & `coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py` & `coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py` & `coffeegrinder-0.3.2/systems/TwoDAdvectionMpi_sbp/TwoDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/tests/test_actions.py` & `coffeegrinder-0.3.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/tests/test_backend.py` & `coffeegrinder-0.3.2/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.3.1/tox.ini` & `coffeegrinder-0.3.2/tox.ini`

 * *Files identical despite different names*

