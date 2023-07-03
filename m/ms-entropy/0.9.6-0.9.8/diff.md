# Comparing `tmp/ms_entropy-0.9.6.tar.gz` & `tmp/ms_entropy-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.9.6.tar", last modified: Mon Jul  3 17:58:57 2023, max compression
+gzip compressed data, was "ms_entropy-0.9.8.tar", last modified: Mon Jul  3 22:10:20 2023, max compression
```

## Comparing `ms_entropy-0.9.6.tar` & `ms_entropy-0.9.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.478240 ms_entropy-0.9.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.482240 ms_entropy-0.9.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.482240 ms_entropy-0.9.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-multiple_cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_pickle_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions-low_memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example-with_individual_search_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/examples/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.486240 ms_entropy-0.9.6/ms_entropy/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/ms_entropy/entropy_search/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)   881493 2023-07-03 17:58:56.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    29246 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.486240 ms_entropy-0.9.6/ms_entropy/file_io/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/lbm2_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/mgf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/msp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/mzml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/file_io/spec_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/ms_entropy/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/df.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/pipe/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/ms_entropy/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.c
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.h
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.c
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.h
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)   344231 2023-07-03 17:58:56.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.c
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/entropy_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/spectra/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/ms_entropy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/ms_entropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:58:57.000000 ms_entropy-0.9.6/ms_entropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 17:58:57.494240 ms_entropy-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:58:57.490240 ms_entropy-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 17:58:48.000000 ms_entropy-0.9.6/tests/test_entropy_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.238684 ms_entropy-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 22:10:20.238684 ms_entropy-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.230684 ms_entropy-0.9.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.230684 ms_entropy-0.9.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.230684 ms_entropy-0.9.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-multiple_cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-search_mona-with_pickle_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-search_mona-with_read_write_functions-low_memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-search_mona-with_read_write_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example-with_individual_search_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/examples/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.230684 ms_entropy-0.9.8/ms_entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.234684 ms_entropy-0.9.8/ms_entropy/entropy_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)   881493 2023-07-03 22:10:19.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29246 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.234684 ms_entropy-0.9.8/ms_entropy/file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/lbm2_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/mgf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/msp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/mzml_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/file_io/spec_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.234684 ms_entropy-0.9.8/ms_entropy/pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/pipe/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.238684 ms_entropy-0.9.8/ms_entropy/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/CleanSpectrum.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/CleanSpectrum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/SpectralEntropy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/SpectralEntropy.h
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   344231 2023-07-03 22:10:19.000000 ms_entropy-0.9.8/ms_entropy/spectra/entropy_cython.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/entropy_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/entropy_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/spectra/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/ms_entropy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.234684 ms_entropy-0.9.8/ms_entropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-03 22:10:20.000000 ms_entropy-0.9.8/ms_entropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-03 22:10:20.000000 ms_entropy-0.9.8/ms_entropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:10:20.000000 ms_entropy-0.9.8/ms_entropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 22:10:20.000000 ms_entropy-0.9.8/ms_entropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 22:10:20.000000 ms_entropy-0.9.8/ms_entropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 22:10:20.238684 ms_entropy-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:10:20.234684 ms_entropy-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 22:10:09.000000 ms_entropy-0.9.8/tests/test_entropy_search.py
```

### Comparing `ms_entropy-0.9.6/LICENSE` & `ms_entropy-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/PKG-INFO` & `ms_entropy-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_entropy
-Version: 0.9.6
+Version: 0.9.8
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Author-email: Yuanyue Li <liyuanyue@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ms_entropy-0.9.6/README.md` & `ms_entropy-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/docs/source/conf.py` & `ms_entropy-0.9.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-2.py` & `ms_entropy-0.9.8/examples/example-2.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-multiple_cores.py` & `ms_entropy-0.9.8/examples/example-multiple_cores.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-search_mona-with_pickle_functions.py` & `ms_entropy-0.9.8/examples/example-search_mona-with_pickle_functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions-low_memory_usage.py` & `ms_entropy-0.9.8/examples/example-search_mona-with_read_write_functions-low_memory_usage.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-search_mona-with_read_write_functions.py` & `ms_entropy-0.9.8/examples/example-search_mona-with_read_write_functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example-with_individual_search_function.py` & `ms_entropy-0.9.8/examples/example-with_individual_search_function.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/examples/example.py` & `ms_entropy-0.9.8/examples/example.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search.py` & `ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c` & `ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx` & `ms_entropy-0.9.8/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.9.8/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.9.8/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.9.8/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.9.8/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.9.8/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/shared.py` & `ms_entropy-0.9.8/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.9.8/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/pipe/entropy.py` & `ms_entropy-0.9.8/ms_entropy/pipe/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/pipe/functions.py` & `ms_entropy-0.9.8/ms_entropy/pipe/functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/pipe/pipe.py` & `ms_entropy-0.9.8/ms_entropy/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.c` & `ms_entropy-0.9.8/ms_entropy/spectra/CleanSpectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/CleanSpectrum.h` & `ms_entropy-0.9.8/ms_entropy/spectra/CleanSpectrum.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.c` & `ms_entropy-0.9.8/ms_entropy/spectra/SpectralEntropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/SpectralEntropy.h` & `ms_entropy-0.9.8/ms_entropy/spectra/SpectralEntropy.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/entropy.py` & `ms_entropy-0.9.8/ms_entropy/spectra/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.c` & `ms_entropy-0.9.8/ms_entropy/spectra/entropy_cython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/entropy_cython.pyx` & `ms_entropy-0.9.8/ms_entropy/spectra/entropy_cython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/entropy_numba.py` & `ms_entropy-0.9.8/ms_entropy/spectra/entropy_numba.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy/spectra/tools.py` & `ms_entropy-0.9.8/ms_entropy/spectra/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/ms_entropy.egg-info/PKG-INFO` & `ms_entropy-0.9.8/ms_entropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-entropy
-Version: 0.9.6
+Version: 0.9.8
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Author-email: Yuanyue Li <liyuanyue@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ms_entropy-0.9.6/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.9.8/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/pyproject.toml` & `ms_entropy-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/setup.py` & `ms_entropy-0.9.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from setuptools import find_packages, setup, Extension
+from distutils.util import convert_path
 from Cython.Build import cythonize
 import numpy as np
 import os
 
 
 os.environ["CFLAGS"] = "-O3 -Wno-cpp -Wno-unused-function"
 
+# Read the version from the package file
+main_ns = {}
+ver_path = convert_path("ms_entropy/version.py")
+with open(ver_path) as ver_file:
+    exec(ver_file.read(), main_ns)
+
+
 setup(
     name="ms_entropy",
+    version=main_ns["__version__"],
     package_dir={"": "."},
     ext_modules=cythonize(
         [
             Extension(
                 "ms_entropy.spectra.entropy_cython",
                 [r"ms_entropy/spectra/entropy_cython.pyx", r"ms_entropy/spectra/CleanSpectrum.c", r"ms_entropy/spectra/SpectralEntropy.c"],
             ),
```

### Comparing `ms_entropy-0.9.6/tests/test_entropy.py` & `ms_entropy-0.9.8/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.9.6/tests/test_entropy_search.py` & `ms_entropy-0.9.8/tests/test_entropy_search.py`

 * *Files identical despite different names*

