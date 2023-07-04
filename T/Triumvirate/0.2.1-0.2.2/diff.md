# Comparing `tmp/Triumvirate-0.2.1.tar.gz` & `tmp/Triumvirate-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Triumvirate-0.2.1.tar", last modified: Mon Jun 19 15:13:48 2023, max compression
+gzip compressed data, was "Triumvirate-0.2.2.tar", last modified: Tue Jul  4 15:00:48 2023, max compression
```

## Comparing `Triumvirate-0.2.1.tar` & `Triumvirate-0.2.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    24555 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.926374 Triumvirate-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.930374 Triumvirate-0.2.1/src/Triumvirate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 15:13:48.000000 Triumvirate-0.2.1/src/Triumvirate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.934374 Triumvirate-0.2.1/src/triumvirate/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_bihankel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_fftlog.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_particles.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_particles.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_threept.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_twopt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_valid_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/_winconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28099 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/dataobjs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/dataobjs.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.938374 Triumvirate-0.2.1/src/triumvirate/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/arrayops.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/dataobjs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/fftlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/field.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/maths.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/monitor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/parameters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/particles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/threept.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/include/twopt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/parameters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/parameters.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.938374 Triumvirate-0.2.1/src/triumvirate/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/resources/params_template.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/resources/params_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.942374 Triumvirate-0.2.1/src/triumvirate/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/arrayops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/dataobjs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/fftlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74104 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/field.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/maths.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/monitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27800 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/particles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74281 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/threept.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28450 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/src/twopt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/threept.py
--rw-r--r--   0 runner    (1001) docker     (123)    47337 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/src/triumvirate/twopt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/test_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_build/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_dataobjs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.926374 Triumvirate-0.2.1/tests/test_input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.946374 Triumvirate-0.2.1/tests/test_input/ctlgs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.fits
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.h5
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/test_data_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/ctlgs/test_rand_catalogue.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.954374 Triumvirate-0.2.1/tests/test_input/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/test_params.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/test_params.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/params/tmpl_params.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:13:48.962374 Triumvirate-0.2.1/tests/test_input/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/pk2_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi0_gpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi0_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi2_gpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xi2_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xiw0.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/xiw2.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_gpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_gpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_gpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_lpp.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw000_bin0.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw000_diag.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_input/stats/zetaw202_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_threept.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-19 15:13:17.000000 Triumvirate-0.2.1/tests/test_twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.270136 Triumvirate-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-07-04 15:00:48.270136 Triumvirate-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6355 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-04 15:00:48.274136 Triumvirate-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24712 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.254135 Triumvirate-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.258135 Triumvirate-0.2.2/src/Triumvirate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49310 2023-07-04 15:00:48.000000 Triumvirate-0.2.2/src/Triumvirate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-04 15:00:48.000000 Triumvirate-0.2.2/src/Triumvirate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:00:48.000000 Triumvirate-0.2.2/src/Triumvirate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 15:00:48.000000 Triumvirate-0.2.2/src/Triumvirate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 15:00:48.000000 Triumvirate-0.2.2/src/Triumvirate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.262136 Triumvirate-0.2.2/src/triumvirate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_bihankel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_fftlog.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_particles.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_particles.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_threept.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_twopt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_valid_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/_winconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/dataobjs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/dataobjs.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.262136 Triumvirate-0.2.2/src/triumvirate/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/arrayops.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/dataobjs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/fftlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/field.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/maths.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/monitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/parameters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/particles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/threept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/include/twopt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/parameters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/parameters.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.262136 Triumvirate-0.2.2/src/triumvirate/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/resources/params_template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/resources/params_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.262136 Triumvirate-0.2.2/src/triumvirate/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/arrayops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/dataobjs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/fftlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74104 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/maths.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/monitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/particles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74281 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/threept.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28450 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/src/twopt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    63115 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47337 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/src/triumvirate/twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.266136 Triumvirate-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.266136 Triumvirate-0.2.2/tests/test_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_build/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_dataobjs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.258135 Triumvirate-0.2.2/tests/test_input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.266136 Triumvirate-0.2.2/tests/test_input/ctlgs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/test_data_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/ctlgs/test_rand_catalogue.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.270136 Triumvirate-0.2.2/tests/test_input/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/params/test_params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/params/test_params.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/params/tmpl_params.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:00:48.270136 Triumvirate-0.2.2/tests/test_input/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/bk202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/pk0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/pk0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/pk2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/pk2_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xi0_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xi0_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xi2_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xi2_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xiw0.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/xiw2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta000_bin0_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta000_bin0_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta000_diag_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta000_diag_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta202_diag_gpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zeta202_diag_lpp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zetaw000_bin0.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zetaw000_diag.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_input/stats/zetaw202_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-04 15:00:24.000000 Triumvirate-0.2.2/tests/test_twopt.py
```

### Comparing `Triumvirate-0.2.1/CHANGELOG.md` & `Triumvirate-0.2.2/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Change Log
 
+## v0.2.1 (2023-06-20)
+
+### Bug fixes
+
+Fix parity factor in three-point correlation functions in
+[``threept.cpp``](src/triumvirate/src/threept.cpp).
+
+### Maintenance
+
+- Remove reality-condition division in mode/pair counts for generality.
+- Update test data.
+- Update syntax.
+
+### Documentation
+
+Rerun tutorial notebooks.
+
+
 ## v0.2.0 (2023-06-01)
 
 ### Bug fixes
 
 Fix updating of derived parameters ``npoint`` and ``space`` in ``ParameterSet``
 in [``parameters.pyx``](src/triumvirate/parameters.pyx).
```

### Comparing `Triumvirate-0.2.1/LICENCE` & `Triumvirate-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/MANIFEST.in` & `Triumvirate-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/Makefile` & `Triumvirate-0.2.2/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # ------------------------------------------------------------------------
 # Directories
 # ------------------------------------------------------------------------
 
 # Repository root
 DIR_ROOT := $(shell pwd)
 
-# Package, build, test and dist directories
+# Package, build, test and distribution directories
 DIR_PKG := ${DIR_ROOT}/src/${PKGNAME}
 DIR_BUILD := ${DIR_ROOT}/build
 DIR_TESTS := ${DIR_ROOT}/tests
 DIR_DIST := ${DIR_ROOT}/dist
 
 # Package subdirectories
 DIR_PKG_INCLUDE := ${DIR_PKG}/include
@@ -82,26 +82,29 @@
 
 else  # OS
 
 CXX ?= g++
 
 endif  # OS
 
-# Assume default achiver. [adapt]
+# Assume default archiver. [adapt]
 AR ?= ar
 ARFLAGS ?= -rcsv
 
 # Assume default remover. [adapt]
 RM ?= rm -f
 
 
 # -- Dependencies --------------------------------------------------------
 
 DEPS := gsl fftw3
 
+# Dependencies are searched for by `pkg-config`.  Ensure the set-up of
+# `pkg-config` matches that of the dependencies (e.g. both are installed
+# by Conda in the same Conda environment).
 DEP_INCLUDES := $(shell pkg-config --cflags-only-I ${DEPS})
 DEP_CXXFLAGS := $(shell pkg-config --cflags-only-other ${DEPS})
 DEP_LDFLAGS := $(shell pkg-config --libs-only-other --libs-only-L ${DEPS})
 DEP_LDLIBS := $(shell pkg-config --libs-only-l ${DEPS})
 
 
 # -- Options -------------------------------------------------------------
@@ -155,15 +158,15 @@
 
 CXXFLAGS_OMP ?= -fopenmp
 LDFLAGS_OMP ?= -fopenmp
 # LDLIBS_OMP ?= -lgomp
 
 # # Use alternatively LLVM OpenMP implementation from Homebrew
 # # (brew formula 'libomp').
-# CXXFLAGS_OMP ?= -Xpreprocessor -fopenmp
+# CXXFLAGS_OMP ?= -I$(shell brew --prefix libomp)/include -Xpreprocessor -fopenmp
 # LDFLAGS_OMP ?= -L$(shell brew --prefix libomp)/lib
 # LDLIBS_OMP ?= -lomp
 
 else  # OS
 
 CXXFLAGS_OMP ?= -fopenmp
 LDFLAGS_OMP ?= -fopenmp
@@ -258,120 +261,162 @@
 # -- Installation --------------------------------------------------------
 
 .PHONY: install cppinstall pyinstall cpplibinstall cppappbuild \
         uninstall cppuninstall pyuninstall
 
 install: cppinstall pyinstall
 
-cppinstall: cpplibinstall cppappbuild
+cppinstall: cppinstall_ cpplibinstall cppappbuild
 
-cpplibinstall: ${PROGLIB}
+cppinstall_:
+	@echo "Installing Triumvirate C++ library/program..."
 
-cppappbuild: ${PROGEXE}
+cpplibinstall: library
+
+cppappbuild: executable
 
 pyinstall:
 	@echo "Installing Triumvirate Python package ${WOMP} OpenMP (in pip dev mode)..."
 	python -m pip install ${PIPOPTS} --editable . -vvv
 
 uninstall: cppuninstall pyuninstall
 
 cppuninstall:
 	@echo "Uninstalling Triumvirate C++ library/program..."
-	find ${DIR_BUILD} -mindepth 1 -maxdepth 1 ! -name ".gitignore" -exec rm -r {} +
+	@echo "  ... removing builds..."
+	@find ${DIR_BUILD} -mindepth 1 -maxdepth 1 ! -name ".gitignore" -exec rm -r {} +
 
 pyuninstall:
 	@echo "Uninstalling Triumvirate Python package (in pip mode)..."
 	python -m pip uninstall -y ${PKGNAME}
 
 
 # -- Components ----------------------------------------------------------
 
-${PROGEXE}: ${PROGOBJ} $(OBJS)
+.PHONY: executable library OBJS_
+
+executable: OBJS_ ${PROGEXE}
+
+${PROGEXE}: $(OBJS) ${PROGOBJ}
 	@echo "Compiling Triumvirate C++ program ${WOMP} OpenMP..."
-	if [ ! -d ${DIR_BUILDBIN} ]; then mkdir -p ${DIR_BUILDBIN}; fi
+	@if [ ! -d ${DIR_BUILDBIN} ]; then \
+	    echo "  making bin subdirectory in build directory..."; \
+	    mkdir -p ${DIR_BUILDBIN}; \
+	fi
 	$(CXX) $(CXXFLAGS) $^ -o $@ $(LDFLAGS) $(LDLIBS)
 
+library: OBJS_ ${PROGLIB}
+
 ${PROGLIB}: $(OBJS)
 	@echo "Creating Triumvirate C++ library ${WOMP} OpenMP..."
-	if [ ! -d ${DIR_BUILDLIB} ]; then mkdir -p ${DIR_BUILDLIB}; fi
+	@if [ ! -d ${DIR_BUILDLIB} ]; then \
+	    echo "  making lib subdirectory in build directory..."; \
+	    mkdir -p ${DIR_BUILDLIB}; \
+	fi
 	$(AR) $(ARFLAGS) $@ $^
 
+OBJS_:
+	@echo "Creating Triumvirate C++ object files..."
+	@if [ ! -d ${DIR_BUILDOBJ} ]; then \
+	    echo "  making obj subdirectory in build directory..."; \
+	    mkdir -p ${DIR_BUILDOBJ}; \
+	fi
+
 ${PROGOBJ}: ${PROGSRC}
-	if [ ! -d ${DIR_BUILDOBJ} ]; then mkdir -p ${DIR_BUILDOBJ}; fi
 	$(CXX) -c $(CPPFLAGS) $(CXXFLAGS) $< -o $@
 
 $(OBJS): ${DIR_BUILDOBJ}/%.o: ${DIR_PKG_SRC}/%.cpp
-	if [ ! -d ${DIR_BUILDOBJ} ]; then mkdir -p ${DIR_BUILDOBJ}; fi
 	$(CXX) -c $(CPPFLAGS) $(CXXFLAGS) $< -o $@
 
 -include $(DEPS)
 
 
 # -- Configuration -------------------------------------------------------
 
 .PHONY: checkopts
 
 checkopts:
 	@echo "Checking options parsed by Makefile..."
-	@echo "MAKEFLAGS: ${MAKEFLAGS}"
-	@echo "MAKEFLAGS_JOBS: ${MAKEFLAGS_JOBS}"
-	@echo "SCM_VER_SCHEME: ${SCM_VER_SCHEME}"
-	@echo "SCM_LOC_SCHEME: ${SCM_LOC_SCHEME}"
-	@echo "CXX: ${CXX}"
-	@echo "INCLUDES: ${INCLUDES}"
-	@echo "CPPFLAGS: ${CPPFLAGS}"
-	@echo "CXXFLAGS: ${CXXFLAGS}"
-	@echo "LDFLAGS: ${LDFLAGS}"
-	@echo "LDLIBS: ${LDLIBS}"
-	@echo "CXXFLAGS_OMP: ${CXXFLAGS_OMP}"
-	@echo "LDFLAGS_OMP: ${LDFLAGS_OMP}"
-	@echo "LDLIBS_OMP: ${LDLIBS_OMP}"
-	@echo "AR: ${AR}"
-	@echo "ARFLAGS: ${ARFLAGS}"
-	@echo "RM: ${RM}"
-	@echo "PIPOPTS: ${PIPOPTS}"
+	@echo "  MAKEFLAGS=${MAKEFLAGS}"
+	@echo "  MAKEFLAGS_JOBS=${MAKEFLAGS_JOBS}"
+	@echo "  SCM_VER_SCHEME=${SCM_VER_SCHEME}"
+	@echo "  SCM_LOC_SCHEME=${SCM_LOC_SCHEME}"
+	@echo "  CXX=${CXX}"
+	@echo "  INCLUDES=${INCLUDES}"
+	@echo "  CPPFLAGS=${CPPFLAGS}"
+	@echo "  CXXFLAGS=${CXXFLAGS}"
+	@echo "  LDFLAGS=${LDFLAGS}"
+	@echo "  LDLIBS=${LDLIBS}"
+	@echo "  CXXFLAGS_OMP=${CXXFLAGS_OMP}"
+	@echo "  LDFLAGS_OMP=${LDFLAGS_OMP}"
+	@echo "  LDLIBS_OMP=${LDLIBS_OMP}"
+	@echo "  AR=${AR}"
+	@echo "  ARFLAGS={ARFLAGS}"
+	@echo "  RM=${RM}"
+	@echo "  PIPOPTS=${PIPOPTS}"
 
 
 # ------------------------------------------------------------------------
 # Testing
 # ------------------------------------------------------------------------
 
 .PHONY: test pytest
 
 test: pytest
 
 pytest:
 	@echo "Peforming Triumvirate Python tests..."
-	if [ ! -d ${DIR_TESTOUT} ]; then mkdir -p ${DIR_TESTOUT}; fi
+	@if [ ! -d ${DIR_TESTOUT} ]; then \
+	    echo "  making output subdirectory in test directory..."; \
+	    mkdir -p ${DIR_TESTOUT}; \
+	fi
 	pytest
 
 
 # ------------------------------------------------------------------------
 # Cleaning
 # ------------------------------------------------------------------------
 
-.PHONY: clean cppclean pyclean testclean distclean
+.PHONY: clean buildclean testclean distclean runclean cppclean pyclean
+
+clean: buildclean testclean distclean runclean
 
-clean: cppclean pyclean testclean distclean
+buildclean: cppclean pyclean
 
 cppclean:
 	@echo "Cleaning up Triumvirate C++ build..."
-	$(RM) -r core
-	find ${DIR_BUILD} -mindepth 1 -maxdepth 1 ! -name ".gitignore" -exec rm -r {} +
+	@echo "  removing builds..."
+	@find ${DIR_BUILD} -mindepth 1 -maxdepth 1 ! -name ".gitignore" -exec rm -r {} +
 
 pyclean:
-	@echo "Cleaning up Triumvirate Python/Cython build..."
-	find ${DIR_PKG} -maxdepth 1 \( -name "*.cpp" -or -name "*.so" \) -exec rm {} +
-	find . -type d -name "__pycache__" -exec rm -r {} +
-	find . -type d -name ".ipynb_checkpoints" -exec rm -r {} +
+	@echo "Cleaning up Triumvirate Python build..."
+	@echo "  removing Cythonised C/C++ scripts..."
+	@find ${DIR_PKG} -maxdepth 1 -name "*.cpp" -exec rm {} +
+	@echo "  removing Cythonised extensions..."
+	@find ${DIR_PKG} -maxdepth 1 -name "*.so" -exec rm {} +
+	@echo "  removing compiled bytecode..."
+	@find . -type d -name "__pycache__" -exec rm -r {} +
+	@echo "  removing Jupyter notebook checkpoints..."
+	@find . -type d -name ".ipynb_checkpoints" -exec rm -r {} +
 
 testclean:
 	@echo "Cleaning up Triumvirate tests..."
-	$(RM) -r ${DIR_TESTBUILD}/* ${DIR_TESTOUT}/*
-	$(RM) -r core
-	find . -type d -name ".pytest_cache" -exec rm -r {} +
+	@echo "  removing test builds and outputs..."
+	@$(RM) -r ${DIR_TESTBUILD}/* ${DIR_TESTOUT}/*
+	@echo "  removing pytest cache..."
+	@find . -type d -name ".pytest_cache" -exec rm -r {} +
+	@echo "  removing core dumps..."
+	@$(RM) -r core
 
 distclean:
 	@echo "Cleaning up Triumvirate distributions..."
-	$(RM) -r ${DIR_DIST}/
-	$(RM) -r wheelhouse/
-	find . -name ".egg-info" -exec rm -r {} +
+	@echo "  removing distribution outputs..."
+	@$(RM) -r ${DIR_DIST}/
+	@echo "  removing wheels..."
+	@find . -type d -name "wheelhouse" -exec rm -r {} +
+	@echo "  removing eggs..."
+	@find . -name "*.egg-info" -exec rm -r {} +
+
+runclean:
+	@echo "Cleaning up Triumvirate runs..."
+	@echo "  removing core dumps..."
+	@$(RM) -r core
```

### Comparing `Triumvirate-0.2.1/PKG-INFO` & `Triumvirate-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.2.1
+Version: 0.2.2
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -753,19 +753,19 @@
 
 .. image:: https://img.shields.io/pypi/v/Triumvirate?logo=PyPI&color=informational
     :target: https://pypi.org/project/Triumvirate
     :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/msw/triumvirate?logo=Anaconda&color=informational
     :target: https://anaconda.org/msw/triumvirate
-    :alt: conda
+    :alt: Conda
 
 |Triumvirate| as a Python package is distributed through
 `PyPI <https://pypi.org/project/Triumvirate>`_ and
-`conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
+`Conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
 can be found on the `Installation
 <https://triumvirate.readthedocs.io/en/latest/installation.html#python-package>`__
 page in the documentation.
 
 
 C++ library & program
 ---------------------
```

### Comparing `Triumvirate-0.2.1/README.md` & `Triumvirate-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/README.rst` & `Triumvirate-0.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
 .. image:: https://img.shields.io/pypi/v/Triumvirate?logo=PyPI&color=informational
     :target: https://pypi.org/project/Triumvirate
     :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/msw/triumvirate?logo=Anaconda&color=informational
     :target: https://anaconda.org/msw/triumvirate
-    :alt: conda
+    :alt: Conda
 
 |Triumvirate| as a Python package is distributed through
 `PyPI <https://pypi.org/project/Triumvirate>`_ and
-`conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
+`Conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
 can be found on the `Installation
 <https://triumvirate.readthedocs.io/en/latest/installation.html#python-package>`__
 page in the documentation.
 
 
 C++ library & program
 ---------------------
```

### Comparing `Triumvirate-0.2.1/pyproject.toml` & `Triumvirate-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [project]
 name = 'Triumvirate'
 authors = [{name = 'Mike S Wang'}, {name = 'Naonori S Sugiyama'}]
 maintainers = [{name = 'Mike S Wang', email = "mikeshengbo.wang@ed.ac.uk"}]
 license = {file = "LICENCE"}
 requires-python = '>=3.8'
 dependencies = [
-    'numpy',
+    'numpy>=1.17',
     'scipy',
     'astropy>=4.2',
     'pyyaml>4',
 ]
 description = "Three-point clustering measurements in large-scale structure analyses."
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `Triumvirate-0.2.1/setup.cfg` & `Triumvirate-0.2.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 python_requires = >=3.8
 setup_requires = 
 	setuptools>=61.0.0
 	setuptools_scm>=6.4.0
 	Cython>=0.25
 	oldest-supported-numpy
 install_requires = 
-	numpy
+	numpy>=1.17
 	scipy
 	astropy>=4.2
 	pyyaml>4
 
 [options.extras_require]
 nbk = 
 	nbodykit
```

### Comparing `Triumvirate-0.2.1/setup.py` & `Triumvirate-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             self.parallel = _num_procs
 
     def build_extensions(self):
         """Modify compiler and compilation configuration in
         :meth:`Cython.Distutils.build_ext.build_extensions`.
 
         """
-        OPTS_TO_REMOVE = ['-Wstrict-prototypes',]  # noqa: E231
+        OPTS_TO_REMOVE = ['-Wstrict-prototypes', '-Wl,-pie',]  # noqa: E231
         for opt in OPTS_TO_REMOVE:
             try:
                 self.compiler.compiler_so.remove(opt)
             except ValueError:
                 pass
 
         try:
@@ -178,15 +178,15 @@
     """
 
     def build_libraries(self, libraries):
         """Modify compiler and compilation configuration in
         :meth:`setuptools.command.build_clib.build_clib.build_libraries`.
 
         """
-        OPTS_TO_REMOVE = ['-Wstrict-prototypes',]  # noqa: E231
+        OPTS_TO_REMOVE = ['-Wstrict-prototypes', '-Wl,-pie',]  # noqa: E231
         for opt in OPTS_TO_REMOVE:
             try:
                 self.compiler.compiler_so.remove(opt)
             except ValueError:
                 pass
 
         distutils_logger.info(
@@ -233,15 +233,16 @@
 
     """
     PY_ENV_VARS = [
         'PY_CXX',
         'PY_INCLUDES',  # typically included in 'CPPFLAGS'
         'PY_CXXFLAGS',  # untypically includes macros in 'CPPFLAGS'
         'PY_LDFLAGS',  # untypically includes 'LDLIBS'
-        'PY_NO_OMP',
+        'PY_NO_OMP',  # disable OpenMP explicitly
+        'PY_OMP',  # enable OpenMP explicitly unless overriden by `PY_NO_OMP`
         'PY_CXXFLAGS_OMP',
         'PY_LDFLAGS_OMP',
         'PY_BUILD_PARALLEL',
         'PY_SCM_VER_SCHEME',
         'PY_SCM_LOC_SCHEME',
     ]
     for env_var in PY_ENV_VARS:
@@ -590,23 +591,23 @@
     """
     # Check if OpenMP is explicitly disabled.
     if os.environ.get('PY_NO_OMP') is not None:
         prioprint("OpenMP is disabled explicitly.")
         return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
     # Check if OpenMP is unsupported.
-    if not check_openmp_support():
+    if os.environ.get('PY_OMP') is None and not check_openmp_support():
         prioprint(
             "OpenMP is disabled as "
             "it is not supported in this build enviromnent."
         )
         return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
     # Enable OpenMP by default otherwise.
-    prioprint("OpenMP is enabled by default.")
+    prioprint("OpenMP is enabled.")
 
     # Adapt `macros` and `cflags`.
     MACROS_OMP_RELATED = [
         ('TRV_USE_OMP', None),
         ('TRV_USE_FFTWOMP', None),
     ]
     for macro_ in MACROS_OMP_RELATED:
```

### Comparing `Triumvirate-0.2.1/src/Triumvirate.egg-info/PKG-INFO` & `Triumvirate-0.2.2/src/Triumvirate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.2.1
+Version: 0.2.2
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -753,19 +753,19 @@
 
 .. image:: https://img.shields.io/pypi/v/Triumvirate?logo=PyPI&color=informational
     :target: https://pypi.org/project/Triumvirate
     :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/msw/triumvirate?logo=Anaconda&color=informational
     :target: https://anaconda.org/msw/triumvirate
-    :alt: conda
+    :alt: Conda
 
 |Triumvirate| as a Python package is distributed through
 `PyPI <https://pypi.org/project/Triumvirate>`_ and
-`conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
+`Conda <https://anaconda.org/msw/triumvirate>`_. Instructions for installation
 can be found on the `Installation
 <https://triumvirate.readthedocs.io/en/latest/installation.html#python-package>`__
 page in the documentation.
 
 
 C++ library & program
 ---------------------
```

### Comparing `Triumvirate-0.2.1/src/Triumvirate.egg-info/SOURCES.txt` & `Triumvirate-0.2.2/src/Triumvirate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/__init__.py` & `Triumvirate-0.2.2/src/triumvirate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 __copyright__ = 'Copyright 2023, Mike S Wang & Naonori S Sugiyama'
 __date__ = '2023-05-31'
 __license__ = 'GPL-3.0'
 
 try:
     __version__ = version('triumvirate')
 except PackageNotFoundError:
-    __version__ = '0.2.0'  # fallback version number
+    __version__ = '0.2.1'  # fallback version number
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/_bihankel.py` & `Triumvirate-0.2.2/src/triumvirate/_bihankel.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_fftlog.pyx` & `Triumvirate-0.2.2/src/triumvirate/_fftlog.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_particles.pxd` & `Triumvirate-0.2.2/src/triumvirate/_particles.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_particles.pyx` & `Triumvirate-0.2.2/src/triumvirate/_particles.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_threept.pyx` & `Triumvirate-0.2.2/src/triumvirate/_threept.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_twopt.pyx` & `Triumvirate-0.2.2/src/triumvirate/_twopt.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_valid_install.py` & `Triumvirate-0.2.2/src/triumvirate/_valid_install.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/_winconv.py` & `Triumvirate-0.2.2/src/triumvirate/_winconv.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/catalogue.py` & `Triumvirate-0.2.2/src/triumvirate/catalogue.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
             The invocation of this method resets the particle data
             column ``'nz'``.
 
         """
         if np.isscalar(boxsize):
             boxsize = [boxsize, boxsize, boxsize]
 
-        volume = volume or np.product(boxsize)
+        volume = volume or np.prod(boxsize)
 
         self._pdata['nz'] = self.ntotal / volume
 
     def centre(self, boxsize, catalogue_ref=None):
         """Centre a (pair of) catalogue(s) in a box.
 
         Parameters
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/dataobjs.pxd` & `Triumvirate-0.2.2/src/triumvirate/dataobjs.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/dataobjs.pyx` & `Triumvirate-0.2.2/src/triumvirate/dataobjs.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/arrayops.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/arrayops.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/dataobjs.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/dataobjs.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/fftlog.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/fftlog.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/field.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/field.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/io.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/io.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/maths.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/maths.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/monitor.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/monitor.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/parameters.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/parameters.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/particles.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/particles.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/threept.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/threept.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/include/twopt.hpp` & `Triumvirate-0.2.2/src/triumvirate/include/twopt.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/logger.py` & `Triumvirate-0.2.2/src/triumvirate/logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/parameters.pxd` & `Triumvirate-0.2.2/src/triumvirate/parameters.pxd`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/parameters.pyx` & `Triumvirate-0.2.2/src/triumvirate/parameters.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/resources/params_template.ini` & `Triumvirate-0.2.2/src/triumvirate/resources/params_template.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/resources/params_template.yml` & `Triumvirate-0.2.2/src/triumvirate/resources/params_template.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/arrayops.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/arrayops.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ExtrapError::ExtrapError(const char* fmt_string, ...): std::runtime_error(
     "Extrapolation error."  // mandatory default error message
 ) {
   std::va_list args;
 
   char err_mesg_buf[4096];
   va_start(args, fmt_string);
-  std::vsprintf(err_mesg_buf, fmt_string, args);
+  std::vsnprintf(err_mesg_buf, sizeof(err_mesg_buf), fmt_string, args);
   va_end(args);
 
   this->err_mesg = std::string(err_mesg_buf);
 }
 
 const char* ExtrapError::what() const noexcept {return this->err_mesg.c_str();}
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/dataobjs.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/dataobjs.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/fftlog.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/fftlog.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/field.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/field.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/io.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/io.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -369,16 +369,19 @@
 // Three-point measurement data table
 // -----------------------------------------------------------------------
 
 void print_measurement_datatab_to_file(
   std::FILE* fileptr,
   trv::ParameterSet& params, trv::BispecMeasurements& meas_bispec
 ) {
-  char multipole_str[4];
-  std::sprintf(multipole_str, "%d%d%d", params.ell1, params.ell2, params.ELL);
+  char multipole_str[8];
+  std::snprintf(
+    multipole_str, sizeof(multipole_str), "%d%d%d",
+    params.ell1, params.ell2, params.ELL
+  );
 
   // Print data table columns.
   std::fprintf(
     fileptr,
     "%s "
     "[0] k1_cen, [1] k1_eff, [2] k2_cen, [3] k2_eff, [4] nmodes, "
     "[5] Re{bk%s_raw}, [6] Im{bk%s_raw}, "
@@ -401,16 +404,19 @@
   }
 }
 
 void print_measurement_datatab_to_file(
   std::FILE* fileptr,
   trv::ParameterSet& params, trv::ThreePCFMeasurements& meas_3pcf
 ) {
-  char multipole_str[4];
-  std::sprintf(multipole_str, "%d%d%d", params.ell1, params.ell2, params.ELL);
+  char multipole_str[8];
+  std::snprintf(
+    multipole_str, sizeof(multipole_str), "%d%d%d",
+    params.ell1, params.ell2, params.ELL
+  );
 
   // Print data table columns.
   std::fprintf(
     fileptr,
     "%s "
     "[0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, "
     "[5] Re{zeta%s_raw}, [6] Im{zeta%s_raw}, "
@@ -433,16 +439,19 @@
   }
 }
 
 void print_measurement_datatab_to_file(
   std::FILE* fileptr,
   trv::ParameterSet& params, trv::ThreePCFWindowMeasurements& meas_3pcf_win
 ) {
-  char multipole_str[4];
-  std::sprintf(multipole_str, "%d%d%d", params.ell1, params.ell2, params.ELL);
+  char multipole_str[8];
+  std::snprintf(
+    multipole_str, sizeof(multipole_str), "%d%d%d",
+    params.ell1, params.ell2, params.ELL
+  );
 
   // Print data table columns.
   std::fprintf(
     fileptr,
     "%s "
     "[0] r1_cen, [1] r1_eff, [2] r2_cen, [3] r2_eff, [4] npairs, "
     "[5] Re{zeta%s_raw}, [6] Im{zeta%s_raw}, "
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/maths.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/maths.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/monitor.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/monitor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
     std::chrono::duration_cast<std::chrono::seconds>(
       std::chrono::steady_clock::now() - clockStart
     ).count()
   );
 
   // Format the timestamp.
   char timestamp_[128];
-  std::sprintf(
-    timestamp_, "%s (+%s)",
+  std::snprintf(
+    timestamp_, sizeof(timestamp_), "%s (+%s)",
     show_current_datetime().c_str(), show_elapsed_time(elapsed_time).c_str()
   );
 
   std::string timestamp(timestamp_);
 
   return timestamp;
 }
@@ -136,15 +136,15 @@
   this->level_limit = level;
 }
 
 void Logger::emit(
   std::string log_type, const char* fmt_string, std::va_list args
 ) {
   char log_mesg_buf[4096];
-  std::vsprintf(log_mesg_buf, fmt_string, args);
+  std::vsnprintf(log_mesg_buf, sizeof(log_mesg_buf), fmt_string, args);
 
   std::printf(
     "[%s %s %s] %s\n",
     trv::sys::show_timestamp().c_str(), log_type.c_str(), SHOW_CPPSTATE,
     log_mesg_buf
   );
 }
@@ -254,15 +254,15 @@
   std::logic_error(
     "Unimplemented error."  // mandatory default error message
   ) {
   std::va_list args;
 
   char err_mesg_buf[4096];
   va_start(args, fmt_string);
-  std::vsprintf(err_mesg_buf, fmt_string, args);
+  std::vsnprintf(err_mesg_buf, sizeof(err_mesg_buf), fmt_string, args);
   va_end(args);
 
   this->err_mesg = std::string(err_mesg_buf);
 }
 
 const char* UnimplementedError::what() const noexcept {
   return this->err_mesg.c_str();
@@ -271,15 +271,15 @@
 IOError::IOError(const char* fmt_string, ...): std::runtime_error(
   "I/O error."  // mandatory default error message
 ) {
   std::va_list args;
 
   char err_mesg_buf[4096];
   va_start(args, fmt_string);
-  std::vsprintf(err_mesg_buf, fmt_string, args);
+  std::vsnprintf(err_mesg_buf, sizeof(err_mesg_buf), fmt_string, args);
   va_end(args);
 
   this->err_mesg = std::string(err_mesg_buf);
 }
 
 const char* IOError::what() const noexcept {return this->err_mesg.c_str();}
 
@@ -287,15 +287,15 @@
 std::invalid_argument(
   "Invalid parameter error."  // mandatory default error message
 ) {
   std::va_list args;
 
   char err_mesg_buf[4096];
   va_start(args, fmt_string);
-  std::vsprintf(err_mesg_buf, fmt_string, args);
+  std::vsnprintf(err_mesg_buf, sizeof(err_mesg_buf), fmt_string, args);
   va_end(args);
 
   this->err_mesg = std::string(err_mesg_buf);
 }
 
 const char* InvalidParameterError::what() const noexcept {
   return this->err_mesg.c_str();
@@ -305,15 +305,15 @@
 std::runtime_error(
   "Invalid data error."  // mandatory default error message
 ) {
   std::va_list args;
 
   char err_mesg_buf[4096];
   va_start(args, fmt_string);
-  std::vsprintf(err_mesg_buf, fmt_string, args);
+  std::vsnprintf(err_mesg_buf, sizeof(err_mesg_buf), fmt_string, args);
   va_end(args);
 
   this->err_mesg = std::string(err_mesg_buf);
 }
 
 const char* InvalidDataError::what() const noexcept {
   return this->err_mesg.c_str();
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/parameters.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/parameters.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -843,16 +843,16 @@
 
   return 0;
 }
 
 int ParameterSet::print_to_file() {
   // Set output file path to default.
   char ofilepath[1024];
-  std::sprintf(
-    ofilepath, "%s/parameters_used%s",
+  std::snprintf(
+    ofilepath, sizeof(ofilepath), "%s/parameters_used%s",
     this->measurement_dir.c_str(), this->output_tag.c_str()
   );
 
   return ParameterSet::print_to_file(ofilepath);
 }
 
 }  // namespace trv
```

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/particles.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/particles.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/threept.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/threept.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/src/twopt.cpp` & `Triumvirate-0.2.2/src/triumvirate/src/twopt.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/threept.py` & `Triumvirate-0.2.2/src/triumvirate/threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/src/triumvirate/twopt.py` & `Triumvirate-0.2.2/src/triumvirate/twopt.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/conftest.py` & `Triumvirate-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_catalogue.py` & `Triumvirate-0.2.2/tests/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_dataobjs.py` & `Triumvirate-0.2.2/tests/test_dataobjs.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.fits` & `Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.fits`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/ctlgs/sample_catalogue.h5` & `Triumvirate-0.2.2/tests/test_input/ctlgs/sample_catalogue.h5`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/ctlgs/test_rand_catalogue.txt` & `Triumvirate-0.2.2/tests/test_input/ctlgs/test_rand_catalogue.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/params/test_params.ini` & `Triumvirate-0.2.2/tests/test_input/params/test_params.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/params/test_params.yml` & `Triumvirate-0.2.2/tests/test_input/params/test_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/params/tmpl_params.yml` & `Triumvirate-0.2.2/tests/test_input/params/tmpl_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk000_bin0_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk000_diag_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/bk202_diag_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/bk202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/pk0_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/pk0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/pk0_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/pk0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/pk2_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/pk2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/pk2_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/pk2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xi0_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xi0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xi0_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xi0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xi2_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xi2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xi2_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xi2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xiw0.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xiw0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/xiw2.txt` & `Triumvirate-0.2.2/tests/test_input/stats/xiw2.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta000_bin0_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta000_diag_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_gpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zeta202_diag_lpp.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zeta202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zetaw000_bin0.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zetaw000_bin0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zetaw000_diag.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zetaw000_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_input/stats/zetaw202_diag.txt` & `Triumvirate-0.2.2/tests/test_input/stats/zetaw202_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_logger.py` & `Triumvirate-0.2.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_parameters.py` & `Triumvirate-0.2.2/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_threept.py` & `Triumvirate-0.2.2/tests/test_threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.2.1/tests/test_twopt.py` & `Triumvirate-0.2.2/tests/test_twopt.py`

 * *Files identical despite different names*

