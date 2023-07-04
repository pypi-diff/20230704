# Comparing `tmp/soapcw-0.1.6.tar.gz` & `tmp/soapcw-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.1.6.tar", last modified: Mon Jul  3 20:08:27 2023, max compression
+gzip compressed data, was "soapcw-0.1.7.tar", last modified: Tue Jul  4 07:46:36 2023, max compression
```

## Comparing `soapcw-0.1.6.tar` & `soapcw-0.1.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.890154 soapcw-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-03 20:06:51.000000 soapcw-0.1.6/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-03 20:06:51.000000 soapcw-0.1.6/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-03 20:06:51.000000 soapcw-0.1.6/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-03 20:06:51.000000 soapcw-0.1.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-03 20:06:51.000000 soapcw-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-07-03 20:08:27.890154 soapcw-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-03 20:06:51.000000 soapcw-0.1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/authors.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6317 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.882154 soapcw-0.1.6/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-03 20:06:51.000000 soapcw-0.1.6/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 20:06:52.000000 soapcw-0.1.6/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    37055 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.883154 soapcw-0.1.6/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-03 20:06:51.000000 soapcw-0.1.6/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-03 20:08:27.890154 soapcw-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-03 20:06:51.000000 soapcw-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.886154 soapcw-0.1.6/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.887154 soapcw-0.1.6/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17946 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.887154 soapcw-0.1.6/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3019 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/load_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.888154 soapcw-0.1.6/soapcw/cnn/pytorch/models/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/cnn.py
--rw-rw-rw-   0 root         (0) root         (0)     9628 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/pytorch/models/combined_cnn.py
--rw-rw-rw-   0 root         (0) root         (0)    11582 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.888154 soapcw-0.1.6/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42241 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.889154 soapcw-0.1.6/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/line_aware_stat/save_lookup.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2250446 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    63288 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.889154 soapcw-0.1.6/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 20:06:52.000000 soapcw-0.1.6/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-03 20:06:51.000000 soapcw-0.1.6/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.886154 soapcw-0.1.6/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1822 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-03 20:08:27.000000 soapcw-0.1.6/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:08:27.890154 soapcw-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-03 20:06:51.000000 soapcw-0.1.6/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.415026 soapcw-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-04 07:44:35.000000 soapcw-0.1.7/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-04 07:44:35.000000 soapcw-0.1.7/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-04 07:44:35.000000 soapcw-0.1.7/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-04 07:44:35.000000 soapcw-0.1.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-04 07:44:35.000000 soapcw-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-04 07:46:36.415026 soapcw-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-04 07:44:35.000000 soapcw-0.1.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.408026 soapcw-0.1.7/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/authors.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.408026 soapcw-0.1.7/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.408026 soapcw-0.1.7/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-04 07:44:35.000000 soapcw-0.1.7/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.409026 soapcw-0.1.7/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.409026 soapcw-0.1.7/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37055 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.409026 soapcw-0.1.7/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-04 07:44:35.000000 soapcw-0.1.7/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-07-04 07:46:36.416026 soapcw-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-04 07:44:35.000000 soapcw-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.411026 soapcw-0.1.7/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.412026 soapcw-0.1.7/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17946 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.413026 soapcw-0.1.7/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/pytorch/load_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.413026 soapcw-0.1.7/soapcw/cnn/pytorch/models/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/pytorch/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6596 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/pytorch/models/cnn.py
+-rw-rw-rw-   0 root         (0) root         (0)     9628 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/pytorch/models/combined_cnn.py
+-rw-rw-rw-   0 root         (0) root         (0)    11582 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.414026 soapcw-0.1.7/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42241 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.414026 soapcw-0.1.7/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/line_aware_stat/save_lookup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2250446 2023-07-04 07:46:35.000000 soapcw-0.1.7/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    63288 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.414026 soapcw-0.1.7/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-04 07:44:35.000000 soapcw-0.1.7/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.412026 soapcw-0.1.7/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-04 07:46:36.000000 soapcw-0.1.7/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:46:36.415026 soapcw-0.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-04 07:44:35.000000 soapcw-0.1.7/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-04 07:44:35.000000 soapcw-0.1.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-04 07:44:35.000000 soapcw-0.1.7/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-04 07:44:35.000000 soapcw-0.1.7/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-04 07:44:35.000000 soapcw-0.1.7/tests/test_soap.py
```

### Comparing `soapcw-0.1.6/CONTRIBUTING.rst` & `soapcw-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/LICENSE` & `soapcw-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/PKG-INFO` & `soapcw-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.6
+Version: 0.1.7
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.6/README.rst` & `soapcw-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/Makefile` & `soapcw-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/conf.py` & `soapcw-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/index.rst` & `soapcw-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/installation.rst` & `soapcw-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/make.bat` & `soapcw-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/docs/pipeline_usage/run_pipeline.rst` & `soapcw-0.1.7/docs/pipeline_usage/run_pipeline.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/css/general.css` & `soapcw-0.1.7/pipeline/css/general.css`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/make_dag_files_astro.py` & `soapcw-0.1.7/pipeline/make_dag_files_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/make_dag_files_lines.py` & `soapcw-0.1.7/pipeline/make_dag_files_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/make_html_page.py` & `soapcw-0.1.7/pipeline/make_html_page.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/run_full_soap_astro.py` & `soapcw-0.1.7/pipeline/run_full_soap_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/run_full_soap_lines.py` & `soapcw-0.1.7/pipeline/run_full_soap_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/scripts/table_scripts.js` & `soapcw-0.1.7/pipeline/scripts/table_scripts.js`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/pipeline/soap_config_parser.py` & `soapcw-0.1.7/pipeline/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/setup.cfg` & `soapcw-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.6
+current_version = 0.1.7
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -17,15 +17,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.1.6
+version = 0.1.7
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.1.6/setup.py` & `soapcw-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/__init__.py` & `soapcw-0.1.7/soapcw/__init__.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.1.7/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.1.7/soapcw/cnn/cnn_data_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.1.7/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/generate_test_data.py` & `soapcw-0.1.7/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/generate_train_data.py` & `soapcw-0.1.7/soapcw/cnn/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.1.7/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.1.7/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/pytorch/models/cnn.py` & `soapcw-0.1.7/soapcw/cnn/pytorch/models/cnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
     def conv_out_size(self, height_in, width_in, padding, dilation, kernel, stride, maxpool_size):
         height_out = int(((height_in + 2*padding[0] - dilation[0]*(kernel[0]-1)-1)/stride[0] + 1)/maxpool_size[0])
         width_out = int(((width_in + 2*padding[1] - dilation[1]*(kernel[1]-1)-1)/stride[1] + 1)/maxpool_size[1])
         return height_out, width_out
         
     def forward(self, y):
         """forward pass for training"""
-        y = torch.reshape(y, (-1, self.inchannels, self.input_dim[0], self.input_dim[1])) if self.num_conv > 0 else y
-        conv = self.conv_network(torch.reshape(y, (-1, self.inchannels, self.input_dim[0], self.input_dim[1]))) if self.num_conv > 0 else y
+        #y = y, (-1, self.inchannels, self.input_dim[0], self.input_dim[1])) if self.num_conv > 0 else y
+        conv = self.conv_network(y) if self.num_conv > 0 else y
         lin_in = torch.flatten(conv,start_dim=1) if self.num_conv > 0 else y   # flatten convolutional layers
         out = self.lin_network(lin_in) # run fully connected network
         return out
     
     def test(model, y):
         """generating samples when testing the network """
         num_data = y.size(0)
```

### Comparing `soapcw-0.1.6/soapcw/cnn/pytorch/models/combined_cnn.py` & `soapcw-0.1.7/soapcw/cnn/pytorch/models/combined_cnn.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cnn/train_model.py` & `soapcw-0.1.7/soapcw/cnn/train_model.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/generate_data.py` & `soapcw-0.1.7/soapcw/cw/generate_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/load_sfts.py` & `soapcw-0.1.7/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/make_sfts.py` & `soapcw-0.1.7/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/sft.py` & `soapcw-0.1.7/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/timeseries.py` & `soapcw-0.1.7/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/cw/tools.py` & `soapcw-0.1.7/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.1.7/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.1.7/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.1.7/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/soap_config_parser.py` & `soapcw-0.1.7/soapcw/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/soapcw.c` & `soapcw-0.1.7/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/soapcw.pyx` & `soapcw-0.1.7/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/tools/plots.py` & `soapcw-0.1.7/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw/tools/tools.py` & `soapcw-0.1.7/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/soapcw.egg-info/PKG-INFO` & `soapcw-0.1.7/soapcw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.1.6
+Version: 0.1.7
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.1.6/soapcw.egg-info/SOURCES.txt` & `soapcw-0.1.7/soapcw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/tests/SNR_injections.ipynb` & `soapcw-0.1.7/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/tests/test_cwload.py` & `soapcw-0.1.7/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/tests/test_line_aware_stat.py` & `soapcw-0.1.7/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.1.6/tests/test_soap.py` & `soapcw-0.1.7/tests/test_soap.py`

 * *Files identical despite different names*

