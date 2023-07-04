# Comparing `tmp/EclipsingBinaries-3.1.8a5.tar.gz` & `tmp/EclipsingBinaries-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.1.8a5.tar", last modified: Sat Jul  1 20:36:14 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.1.9.tar", last modified: Tue Jul  4 00:06:25 2023, max compression
```

## Comparing `EclipsingBinaries-3.1.8a5.tar` & `EclipsingBinaries-3.1.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.747579 EclipsingBinaries-3.1.8a5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.719579 EclipsingBinaries-3.1.8a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.727579 EclipsingBinaries-3.1.8a5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.727579 EclipsingBinaries-3.1.8a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    91701 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.731579 EclipsingBinaries-3.1.8a5/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.743579 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/APASS_Catalog_ex.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/Gaia_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/O-C_paper_table.txt
--rw-r--r--   0 runner    (1001) docker     (123)    85904 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/OConnell_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/OConnell_table.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48237 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/O_C_ex.png
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:35:43.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.743579 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/calibration_images/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/calibration_images/purpose.txt
--rw-r--r--   0 runner    (1001) docker     (123)   135237 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/color_light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (123)    35357 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/example_OC_table.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/example_regression.txt
--rw-r--r--   0 runner    (1001) docker     (123)   118184 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/gui_color_light.png
--rw-r--r--   0 runner    (1001) docker     (123)   109712 2023-07-01 20:35:48.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (123)   136591 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/min_program_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)   131114 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/overlay_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tess_ccd_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.743579 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.735579 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-01 20:36:09.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-01 20:36:14.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:36:09.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-01 20:36:09.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:35:55.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-01 20:36:09.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 20:36:09.000000 EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-01 20:36:14.747579 EclipsingBinaries-3.1.8a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.743579 EclipsingBinaries-3.1.8a5/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)   222548 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/changelog/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/changelog/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.747579 EclipsingBinaries-3.1.8a5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/EB.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.719579 EclipsingBinaries-3.1.8a5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:36:14.747579 EclipsingBinaries-3.1.8a5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/docs/toolbox.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-01 20:36:14.747579 EclipsingBinaries-3.1.8a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:35:49.000000 EclipsingBinaries-3.1.8a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.552827 EclipsingBinaries-3.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.540828 EclipsingBinaries-3.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.544828 EclipsingBinaries-3.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.544828 EclipsingBinaries-3.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    91701 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.544828 EclipsingBinaries-3.1.9/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.548828 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/APASS_Catalog_ex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/Gaia_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/O-C_paper_table.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    85904 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/OConnell_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/OConnell_table.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48237 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/O_C_ex.png
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:05:52.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.548828 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/calibration_images/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-04 00:05:57.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/calibration_images/purpose.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   135237 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/color_light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35357 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/example_OC_table.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/example_regression.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   118184 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/gui_color_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109712 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136591 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/min_program_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   131114 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/overlay_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/tess_ccd_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.548828 EclipsingBinaries-3.1.9/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.544828 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-04 00:06:19.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-04 00:06:25.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:06:19.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-04 00:06:19.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:06:05.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 00:06:19.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 00:06:19.000000 EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-04 00:06:25.552827 EclipsingBinaries-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.548828 EclipsingBinaries-3.1.9/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)   222548 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/changelog/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/changelog/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.552827 EclipsingBinaries-3.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/EB.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.540828 EclipsingBinaries-3.1.9/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:06:25.552827 EclipsingBinaries-3.1.9/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/docs/toolbox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-04 00:06:25.552827 EclipsingBinaries-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:05:58.000000 EclipsingBinaries-3.1.9/setup.py
```

### Comparing `EclipsingBinaries-3.1.8a5/.github/ISSUE_TEMPLATE/bug_report.md` & `EclipsingBinaries-3.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/.github/ISSUE_TEMPLATE/feature_request.md` & `EclipsingBinaries-3.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/.github/workflows/ci_tests.yml` & `EclipsingBinaries-3.1.9/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/.github/workflows/codeql.yml` & `EclipsingBinaries-3.1.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/.github/workflows/python-publish.yml` & `EclipsingBinaries-3.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/CHANGELOG.md` & `EclipsingBinaries-3.1.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/CODE_OF_CONDUCT.md` & `EclipsingBinaries-3.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/APASS_Catalog_ex.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/APASS_Catalog_ex.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/O-C_paper_table.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/O-C_paper_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/OConnell_plot.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/OConnell_plot.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/OConnell_table.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/OConnell_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/O_C_ex.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/O_C_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/color_light_curve_ex.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/color_light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/example_OC_table.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/example_OC_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/example_regression.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/example_regression.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/gui_color_light.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/gui_color_light.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/light_curve_ex.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/min_program_demo.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/min_program_demo.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/overlay_example.png` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/overlay_example.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/pipeline.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/tess_ccd_info.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries/tess_ccd_info.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.1.9/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.8a5
+Version: 3.1.9
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `EclipsingBinaries-3.1.8a5/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.1.9/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/LICENSE` & `EclipsingBinaries-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/PKG-INFO` & `EclipsingBinaries-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.8a5
+Version: 3.1.9
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `EclipsingBinaries-3.1.8a5/README.md` & `EclipsingBinaries-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/changelog/package-lock.json` & `EclipsingBinaries-3.1.9/changelog/package-lock.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/changelog/package.json` & `EclipsingBinaries-3.1.9/changelog/package.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/conf.py` & `EclipsingBinaries-3.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/contributing.rst` & `EclipsingBinaries-3.1.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/index.rst` & `EclipsingBinaries-3.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/installation.rst` & `EclipsingBinaries-3.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/pipeline.rst` & `EclipsingBinaries-3.1.9/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/docs/toolbox.rst` & `EclipsingBinaries-3.1.9/docs/toolbox.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.8a5/setup.cfg` & `EclipsingBinaries-3.1.9/setup.cfg`

 * *Files identical despite different names*

