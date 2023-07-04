# Comparing `tmp/currentscape-1.0.8.tar.gz` & `tmp/currentscape-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.8.tar", last modified: Thu Jun 22 11:05:40 2023, max compression
+gzip compressed data, was "currentscape-1.0.9.tar", last modified: Mon Jul  3 11:35:21 2023, max compression
```

## Comparing `currentscape-1.0.8.tar` & `currentscape-1.0.9.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-22 11:05:23.000000 currentscape-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-22 11:05:23.000000 currentscape-1.0.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-22 11:05:23.000000 currentscape-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-22 11:05:23.000000 currentscape-1.0.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-22 11:05:23.000000 currentscape-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-22 11:05:23.000000 currentscape-1.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-22 11:05:23.000000 currentscape-1.0.8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 11:05:23.000000 currentscape-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-22 11:05:23.000000 currentscape-1.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-22 11:05:23.000000 currentscape-1.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-22 11:05:23.000000 currentscape-1.0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 11:05:23.000000 currentscape-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 11:05:23.000000 currentscape-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 11:05:23.000000 currentscape-1.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-22 11:05:40.537855 currentscape-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-22 11:05:23.000000 currentscape-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-22 11:05:23.000000 currentscape-1.0.8/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 11:05:23.000000 currentscape-1.0.8/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-22 11:05:40.000000 currentscape-1.0.8/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-22 11:05:40.000000 currentscape-1.0.8/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:05:40.000000 currentscape-1.0.8/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 11:05:40.000000 currentscape-1.0.8/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 11:05:40.000000 currentscape-1.0.8/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   183971 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 11:05:23.000000 currentscape-1.0.8/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.533855 currentscape-1.0.8/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-22 11:05:23.000000 currentscape-1.0.8/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 11:05:23.000000 currentscape-1.0.8/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.529855 currentscape-1.0.8/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-22 11:05:23.000000 currentscape-1.0.8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 11:05:23.000000 currentscape-1.0.8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:05:40.537855 currentscape-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-22 11:05:23.000000 currentscape-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:40.537855 currentscape-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 11:05:23.000000 currentscape-1.0.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-22 11:05:23.000000 currentscape-1.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.193274 currentscape-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-03 11:35:13.000000 currentscape-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 11:35:13.000000 currentscape-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-03 11:35:13.000000 currentscape-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-03 11:35:13.000000 currentscape-1.0.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-03 11:35:13.000000 currentscape-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 11:35:13.000000 currentscape-1.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-03 11:35:13.000000 currentscape-1.0.9/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 11:35:13.000000 currentscape-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-03 11:35:13.000000 currentscape-1.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-03 11:35:13.000000 currentscape-1.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-03 11:35:13.000000 currentscape-1.0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 11:35:13.000000 currentscape-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 11:35:13.000000 currentscape-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 11:35:13.000000 currentscape-1.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-03 11:35:21.205274 currentscape-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-03 11:35:13.000000 currentscape-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-07-03 11:35:13.000000 currentscape-1.0.9/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-03 11:35:13.000000 currentscape-1.0.9/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-03 11:35:21.000000 currentscape-1.0.9/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-03 11:35:21.000000 currentscape-1.0.9/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:35:21.000000 currentscape-1.0.9/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-03 11:35:21.000000 currentscape-1.0.9/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 11:35:21.000000 currentscape-1.0.9/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   183971 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 11:35:13.000000 currentscape-1.0.9/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.193274 currentscape-1.0.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.193274 currentscape-1.0.9/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.201274 currentscape-1.0.9/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-03 11:35:13.000000 currentscape-1.0.9/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 11:35:13.000000 currentscape-1.0.9/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.197274 currentscape-1.0.9/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 11:35:13.000000 currentscape-1.0.9/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 11:35:13.000000 currentscape-1.0.9/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:35:21.205274 currentscape-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 11:35:13.000000 currentscape-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:21.205274 currentscape-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-03 11:35:13.000000 currentscape-1.0.9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-03 11:35:13.000000 currentscape-1.0.9/tox.ini
```

### Comparing `currentscape-1.0.8/.github/workflows/build.yml` & `currentscape-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/.github/workflows/test.yml` & `currentscape-1.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/.pylintrc` & `currentscape-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/.zenodo.json` & `currentscape-1.0.9/.zenodo.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/CHANGELOG.rst` & `currentscape-1.0.9/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/CONTRIBUTING.md` & `currentscape-1.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/COPYING` & `currentscape-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/LICENSE.txt` & `currentscape-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/PKG-INFO` & `currentscape-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.8
+Version: 1.0.9
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -60,15 +60,15 @@
 Citation
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
-    @article {10.7554/eLife.42722,
+    @article {alonsomarder2019,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
         editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
         volume = 8,
         year = 2019,
         month = {jan},
```

### Comparing `currentscape-1.0.8/README.rst` & `currentscape-1.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Citation
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
-    @article {10.7554/eLife.42722,
+    @article {alonsomarder2019,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
         editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
         volume = 8,
         year = 2019,
         month = {jan},
```

### Comparing `currentscape-1.0.8/Tutorial.rst` & `currentscape-1.0.9/Tutorial.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/__init__.py` & `currentscape-1.0.9/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/config_parser.py` & `currentscape-1.0.9/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/currents.py` & `currentscape-1.0.9/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/currentscape.py` & `currentscape-1.0.9/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/data_processing.py` & `currentscape-1.0.9/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/datasets.py` & `currentscape-1.0.9/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/ions.py` & `currentscape-1.0.9/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/legends.py` & `currentscape-1.0.9/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/mapper.py` & `currentscape-1.0.9/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/plotting.py` & `currentscape-1.0.9/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape/voltages.py` & `currentscape-1.0.9/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.9/currentscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.8
+Version: 1.0.9
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
@@ -60,15 +60,15 @@
 Citation
 ========
 
 When you use this Currentscape software for your research, we ask you to cite the following publications (this includes poster presentations):
 
 .. code-block:: 
 
-    @article {10.7554/eLife.42722,
+    @article {alonsomarder2019,
         article_type = {journal},
         title = {Visualization of currents in neural models with similar behavior and different conductance densities},
         author = {Alonso, Leandro M and Marder, Eve},
         editor = {Westbrook, Gary L and Skinner, Frances K and Lankarany, Milad and Britton, Oliver},
         volume = 8,
         year = 2019,
         month = {jan},
```

### Comparing `currentscape-1.0.8/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.9/currentscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/doc/Makefile` & `currentscape-1.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/doc/source/conf.py` & `currentscape-1.0.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/doc/source/images/plot.png` & `currentscape-1.0.9/doc/source/images/plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/doc/source/images/quickstart_plot.png` & `currentscape-1.0.9/doc/source/images/quickstart_plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.9/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/config.json` & `currentscape-1.0.9/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.9/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.9/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.9/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.9/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/LICENSE.txt` & `currentscape-1.0.9/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.9/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/config/params/final.json` & `currentscape-1.0.9/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/config/params/pyr.json` & `currentscape-1.0.9/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.9/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.9/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.9/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/plot.py` & `currentscape-1.0.9/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/run.py` & `currentscape-1.0.9/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/examples/use_case/run_py.sh` & `currentscape-1.0.9/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.9/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/requirements_docs.txt` & `currentscape-1.0.9/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/setup.py` & `currentscape-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/extract_bNAC_config.json` & `currentscape-1.0.9/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_config_parser.py` & `currentscape-1.0.9/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_currents.py` & `currentscape-1.0.9/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.9/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_datasets.py` & `currentscape-1.0.9/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_from_paper.py` & `currentscape-1.0.9/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_ions.py` & `currentscape-1.0.9/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_mapper.py` & `currentscape-1.0.9/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_currentscape_plotting.py` & `currentscape-1.0.9/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tests/test_use_case_example.py` & `currentscape-1.0.9/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.8/tox.ini` & `currentscape-1.0.9/tox.ini`

 * *Files identical despite different names*

